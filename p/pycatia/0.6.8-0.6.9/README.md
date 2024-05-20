# Comparing `tmp/pycatia-0.6.8.tar.gz` & `tmp/pycatia-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatia-0.6.8.tar", last modified: Mon Apr 22 07:59:03 2024, max compression
+gzip compressed data, was "pycatia-0.6.9.tar", last modified: Mon May 20 10:16:47 2024, max compression
```

## Comparing `pycatia-0.6.8.tar` & `pycatia-0.6.9.tar`

### file list

```diff
@@ -1,1337 +1,1336 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:03.045916 pycatia-0.6.8/
--rw-rw-rw-   0        0        0     1087 2022-04-12 12:15:17.000000 pycatia-0.6.8/LICENSE.txt
--rw-rw-rw-   0        0        0     5167 2024-04-22 07:59:03.043915 pycatia-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     4612 2024-03-17 16:28:56.000000 pycatia-0.6.8/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:00.890197 pycatia-0.6.8/pycatia/
--rw-rw-rw-   0        0        0      940 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.019522 pycatia-0.6.8/pycatia/abq_automation_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/__init__.py
--rw-rw-rw-   0        0        0     7247 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_analysis_case.py
--rw-rw-rw-   0        0        0     7127 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_analysis_cases.py
--rw-rw-rw-   0        0        0     3612 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_analysis_model.py
--rw-rw-rw-   0        0        0    10496 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_analytical_rigid_surface.py
--rw-rw-rw-   0        0        0    13529 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_boundary_condition.py
--rw-rw-rw-   0        0        0     6882 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_boundary_conditions.py
--rw-rw-rw-   0        0        0     1518 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_clamp_bc.py
--rw-rw-rw-   0        0        0    19646 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_concentrated_force.py
--rw-rw-rw-   0        0        0    16925 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_damper_connection_property.py
--rw-rw-rw-   0        0        0     4366 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_data_output_request.py
--rw-rw-rw-   0        0        0     6449 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_data_output_requests.py
--rw-rw-rw-   0        0        0    16748 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_displacement_bc.py
--rw-rw-rw-   0        0        0     1330 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_display_group.py
--rw-rw-rw-   0        0        0     2810 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_display_groups.py
--rw-rw-rw-   0        0        0    12560 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_explicit_dynamics_step.py
--rw-rw-rw-   0        0        0     8364 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_fastened_connection_enhancement.py
--rw-rw-rw-   0        0        0    12203 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_fastened_pair.py
--rw-rw-rw-   0        0        0     1699 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_field_output_request.py
--rw-rw-rw-   0        0        0     6530 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_field_output_requests.py
--rw-rw-rw-   0        0        0     6939 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_fields.py
--rw-rw-rw-   0        0        0    12762 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_film_condition.py
--rw-rw-rw-   0        0        0    16327 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_frequency_step.py
--rw-rw-rw-   0        0        0     6013 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_gasket_property.py
--rw-rw-rw-   0        0        0    14560 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_general_static_step.py
--rw-rw-rw-   0        0        0    11326 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_global_element_assignment.py
--rw-rw-rw-   0        0        0     9341 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_gravity.py
--rw-rw-rw-   0        0        0    12407 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_heat_transfer_step.py
--rw-rw-rw-   0        0        0     1713 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_history_output_request.py
--rw-rw-rw-   0        0        0     6702 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_history_output_requests.py
--rw-rw-rw-   0        0        0     8678 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_image_query.py
--rw-rw-rw-   0        0        0     3288 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_initial_step.py
--rw-rw-rw-   0        0        0     2098 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_initial_temperature.py
--rw-rw-rw-   0        0        0     1847 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_interaction.py
--rw-rw-rw-   0        0        0     6729 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_interactions.py
--rw-rw-rw-   0        0        0    34962 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_job.py
--rw-rw-rw-   0        0        0     5415 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_jobs.py
--rw-rw-rw-   0        0        0    13616 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_load.py
--rw-rw-rw-   0        0        0     6277 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_loads.py
--rw-rw-rw-   0        0        0    18643 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_mass_scaling.py
--rw-rw-rw-   0        0        0     4719 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_mass_scalings.py
--rw-rw-rw-   0        0        0    17803 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_mech_conn_behavior.py
--rw-rw-rw-   0        0        0    12140 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_output_request.py
--rw-rw-rw-   0        0        0     8229 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_output_requests.py
--rw-rw-rw-   0        0        0     2843 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_pressure.py
--rw-rw-rw-   0        0        0    10393 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_pretension_property.py
--rw-rw-rw-   0        0        0     6562 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_properties.py
--rw-rw-rw-   0        0        0     1828 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_property.py
--rw-rw-rw-   0        0        0    22478 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_rigid_body_constraint.py
--rw-rw-rw-   0        0        0    29395 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_rigid_coupling.py
--rw-rw-rw-   0        0        0    28094 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_smooth_coupling.py
--rw-rw-rw-   0        0        0     6737 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_smooth_step_amplitude.py
--rw-rw-rw-   0        0        0     8281 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_case.py
--rw-rw-rw-   0        0        0     4839 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_case_images.py
--rw-rw-rw-   0        0        0     6822 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_step.py
--rw-rw-rw-   0        0        0     4804 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_step_images.py
--rw-rw-rw-   0        0        0     2934 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_steps.py
--rw-rw-rw-   0        0        0    16760 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_spring_connection_property.py
--rw-rw-rw-   0        0        0     6200 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_step.py
--rw-rw-rw-   0        0        0     8887 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_steps.py
--rw-rw-rw-   0        0        0    19137 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_surface_to_surface_contact.py
--rw-rw-rw-   0        0        0     6712 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_tabular_amplitude.py
--rw-rw-rw-   0        0        0    10170 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_temperature.py
--rw-rw-rw-   0        0        0     3038 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_temperature_bc.py
--rw-rw-rw-   0        0        0     5524 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_temperature_history.py
--rw-rw-rw-   0        0        0     8478 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_thermal_conn_behavior.py
--rw-rw-rw-   0        0        0    10433 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abqfh_output_request.py
--rw-rw-rw-   0        0        0     8789 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_base_motion_vb.py
--rw-rw-rw-   0        0        0     4969 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_frequency_loading_vb.py
--rw-rw-rw-   0        0        0    10161 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_basic_vb.py
--rw-rw-rw-   0        0        0    17690 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_modal_vb.py
--rw-rw-rw-   0        0        0     7232 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_subspace_vb.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.129034 pycatia-0.6.8/pycatia/analysis_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/analysis_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1700 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_adaptivity_manager.py
--rw-rw-rw-   0        0        0     5350 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_case.py
--rw-rw-rw-   0        0        0     9409 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_cases.py
--rw-rw-rw-   0        0        0    16345 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_color_map.py
--rw-rw-rw-   0        0        0     2963 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_document.py
--rw-rw-rw-   0        0        0     6388 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_entities.py
--rw-rw-rw-   0        0        0    26162 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_entity.py
--rw-rw-rw-   0        0        0     3714 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_export.py
--rw-rw-rw-   0        0        0    33844 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_general_setting_att.py
--rw-rw-rw-   0        0        0     3468 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_global_sensor.py
--rw-rw-rw-   0        0        0    31399 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_image.py
--rw-rw-rw-   0        0        0     8192 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_images.py
--rw-rw-rw-   0        0        0     8323 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_import.py
--rw-rw-rw-   0        0        0     2717 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_linked_documents.py
--rw-rw-rw-   0        0        0     6589 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_local_entities.py
--rw-rw-rw-   0        0        0    23544 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_local_entity.py
--rw-rw-rw-   0        0        0     2602 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_local_sensor.py
--rw-rw-rw-   0        0        0    16431 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_manager.py
--rw-rw-rw-   0        0        0     1345 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_element.py
--rw-rw-rw-   0        0        0     8371 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_local_specification.py
--rw-rw-rw-   0        0        0     4662 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_local_specifications.py
--rw-rw-rw-   0        0        0     1947 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_manager.py
--rw-rw-rw-   0        0        0     1330 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_node.py
--rw-rw-rw-   0        0        0    17135 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_part.py
--rw-rw-rw-   0        0        0     5573 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_parts.py
--rw-rw-rw-   0        0        0     5999 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_model.py
--rw-rw-rw-   0        0        0     3652 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_models.py
--rw-rw-rw-   0        0        0     6430 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_output_entities.py
--rw-rw-rw-   0        0        0     7230 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_post_manager.py
--rw-rw-rw-   0        0        0    11583 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_post_pro_anr_setting_att.py
--rw-rw-rw-   0        0        0    24324 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_post_pro_setting_att.py
--rw-rw-rw-   0        0        0    32700 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_reporting_setting_att.py
--rw-rw-rw-   0        0        0     2931 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_sensor.py
--rw-rw-rw-   0        0        0     7724 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_set.py
--rw-rw-rw-   0        0        0    10862 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_sets.py
--rw-rw-rw-   0        0        0     2559 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_supports.py
--rw-rw-rw-   0        0        0     9210 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/analysis_interfaces/analysis_v4_services.py
--rw-rw-rw-   0        0        0    21400 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/basic_component.py
--rw-rw-rw-   0        0        0     2919 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/analysis_interfaces/basic_components.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.171033 pycatia-0.6.8/pycatia/arrangement_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/__init__.py
--rw-rw-rw-   0        0        0     6690 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arr_bendable_string.py
--rw-rw-rw-   0        0        0     2900 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arr_bom_report.py
--rw-rw-rw-   0        0        0     6767 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arr_nomenclature.py
--rw-rw-rw-   0        0        0     3112 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arr_nomenclature_tree.py
--rw-rw-rw-   0        0        0     3873 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arr_nomenclatures.py
--rw-rw-rw-   0        0        0     2578 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arr_system_line_product.py
--rw-rw-rw-   0        0        0     6450 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arr_workbench.py
--rw-rw-rw-   0        0        0     6369 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_area.py
--rw-rw-rw-   0        0        0     7221 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_areas.py
--rw-rw-rw-   0        0        0     6783 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_boundaries.py
--rw-rw-rw-   0        0        0     8719 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_boundary.py
--rw-rw-rw-   0        0        0     1315 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_contour.py
--rw-rw-rw-   0        0        0     6375 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_contours.py
--rw-rw-rw-   0        0        0    11749 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_item_reservation.py
--rw-rw-rw-   0        0        0     8569 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_item_reservations.py
--rw-rw-rw-   0        0        0     8138 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_node.py
--rw-rw-rw-   0        0        0     3017 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_nodes.py
--rw-rw-rw-   0        0        0     9493 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_pathway.py
--rw-rw-rw-   0        0        0     6801 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_pathways.py
--rw-rw-rw-   0        0        0    12330 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_product.py
--rw-rw-rw-   0        0        0     4712 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_rectangle.py
--rw-rw-rw-   0        0        0     6978 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_rectangles.py
--rw-rw-rw-   0        0        0     9245 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_run.py
--rw-rw-rw-   0        0        0     6653 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_runs.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.186063 pycatia-0.6.8/pycatia/assembly_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/assembly_interfaces/__init__.py
--rw-rw-rw-   0        0        0     3006 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/assembly_interfaces/assembly_boolean.py
--rw-rw-rw-   0        0        0    19642 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/assembly_interfaces/assembly_constraint_setting_att.py
--rw-rw-rw-   0        0        0     8437 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/assembly_interfaces/assembly_feature.py
--rw-rw-rw-   0        0        0    19318 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/assembly_interfaces/assembly_features.py
--rw-rw-rw-   0        0        0    18416 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/assembly_interfaces/assembly_general_setting_att.py
--rw-rw-rw-   0        0        0    18694 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/assembly_interfaces/assembly_hole.py
--rw-rw-rw-   0        0        0    13758 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/assembly_interfaces/assembly_pocket.py
--rw-rw-rw-   0        0        0     7002 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/assembly_interfaces/assembly_split.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.192060 pycatia-0.6.8/pycatia/base_interfaces/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/base_interfaces/__init__.py
--rw-rw-rw-   0        0        0      369 2024-04-22 07:21:05.000000 pycatia-0.6.8/pycatia/base_interfaces/base_application.py
--rw-rw-rw-   0        0        0     2683 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/base_interfaces/context.py
--rw-rw-rw-   0        0        0      414 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/base_interfaces/pycatia.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.199065 pycatia-0.6.8/pycatia/behavior_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/behavior_interfaces/__init__.py
--rw-rw-rw-   0        0        0     9017 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/behavior_interfaces/behavior.py
--rw-rw-rw-   0        0        0     3239 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/behavior_interfaces/behavior_extension.py
--rw-rw-rw-   0        0        0     6690 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/behavior_interfaces/behavior_vb_script.py
--rw-rw-rw-   0        0        0     3597 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/behavior_interfaces/behaviors.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.202093 pycatia-0.6.8/pycatia/bkt_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/bkt_interfaces/__init__.py
--rw-rw-rw-   0        0        0    15934 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/bkt_interfaces/behavior_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.206091 pycatia-0.6.8/pycatia/cat_dde_settings_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/cat_dde_settings_interfaces/__init__.py
--rw-rw-rw-   0        0        0   105295 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_dde_settings_interfaces/dxf_setting_att.py
--rw-rw-rw-   0        0        0    40793 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_dde_settings_interfaces/ig2_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.254579 pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/__init__.py
--rw-rw-rw-   0        0        0    10266 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/e5_property.py
--rw-rw-rw-   0        0        0     5407 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/ipd_template_property.py
--rw-rw-rw-   0        0        0   192369 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/mfg_hub_setting_att.py
--rw-rw-rw-   0        0        0     4424 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/mhi_relation_management.py
--rw-rw-rw-   0        0        0     1480 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/cat_logger.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.267579 pycatia-0.6.8/pycatia/cat_mat_interfaces/
--rw-rw-rw-   0        0        0        0 2022-08-18 11:15:13.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/__init__.py
--rw-rw-rw-   0        0        0     2842 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/analysis_material.py
--rw-rw-rw-   0        0        0     6087 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/material.py
--rw-rw-rw-   0        0        0     2019 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/material_document.py
--rw-rw-rw-   0        0        0     5351 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/material_families.py
--rw-rw-rw-   0        0        0     1801 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/material_family.py
--rw-rw-rw-   0        0        0    13313 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/material_manager.py
--rw-rw-rw-   0        0        0     4887 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/materials.py
--rw-rw-rw-   0        0        0     3489 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_mat_interfaces/positioned_material.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.319834 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/__init__.py
--rw-rw-rw-   0        0        0    19021 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_app_factory.py
--rw-rw-rw-   0        0        0     2624 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_application.py
--rw-rw-rw-   0        0        0    16917 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_attribute.py
--rw-rw-rw-   0        0        0     4167 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_attribute_report.py
--rw-rw-rw-   0        0        0     8152 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_build_part.py
--rw-rw-rw-   0        0        0     3691 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_class.py
--rw-rw-rw-   0        0        0     3221 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_cntr_flow.py
--rw-rw-rw-   0        0        0     8088 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_connectable.py
--rw-rw-rw-   0        0        0     8948 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_connector.py
--rw-rw-rw-   0        0        0    13776 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_functional.py
--rw-rw-rw-   0        0        0     5608 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_group.py
--rw-rw-rw-   0        0        0     2212 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_groupable.py
--rw-rw-rw-   0        0        0     7025 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_id.py
--rw-rw-rw-   0        0        0     3994 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_light_bend.py
--rw-rw-rw-   0        0        0    12225 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_light_connector.py
--rw-rw-rw-   0        0        0     5001 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_light_part.py
--rw-rw-rw-   0        0        0     5242 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_list_of_bstrs.py
--rw-rw-rw-   0        0        0     5225 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_list_of_doubles.py
--rw-rw-rw-   0        0        0     5244 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_list_of_longs.py
--rw-rw-rw-   0        0        0     5417 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_list_of_objects.py
--rw-rw-rw-   0        0        0     9084 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_logical_line.py
--rw-rw-rw-   0        0        0     3455 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_object.py
--rw-rw-rw-   0        0        0    22942 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_part_connector.py
--rw-rw-rw-   0        0        0     7613 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_phsyical_product.py
--rw-rw-rw-   0        0        0     3118 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_physical.py
--rw-rw-rw-   0        0        0    11743 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_place_part.py
--rw-rw-rw-   0        0        0     3429 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_resource.py
--rw-rw-rw-   0        0        0     4530 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_spatial.py
--rw-rw-rw-   0        0        0     3672 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_stretchable_data.py
--rw-rw-rw-   0        0        0     5597 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_temp_list_factory.py
--rw-rw-rw-   0        0        0     7631 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_workbench.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.322834 pycatia-0.6.8/pycatia/cat_rdg_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/cat_rdg_interfaces/__init__.py
--rw-rw-rw-   0        0        0    32293 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_rdg_interfaces/rendering_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.326834 pycatia-0.6.8/pycatia/cat_rma_interfaces/
--rw-rw-rw-   0        0        0        0 2022-08-18 11:15:13.000000 pycatia-0.6.8/pycatia/cat_rma_interfaces/__init__.py
--rw-rw-rw-   0        0        0    57980 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_rma_interfaces/rendering_material.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.339833 pycatia-0.6.8/pycatia/cat_rsc_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/cat_rsc_interfaces/__init__.py
--rw-rw-rw-   0        0        0    13301 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_environment.py
--rw-rw-rw-   0        0        0    11520 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_environment_wall.py
--rw-rw-rw-   0        0        0     5468 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_environments.py
--rw-rw-rw-   0        0        0    37352 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_light.py
--rw-rw-rw-   0        0        0     4708 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_lights.py
--rw-rw-rw-   0        0        0    41187 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_shooting.py
--rw-rw-rw-   0        0        0     4846 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_shootings.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.474127 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/__init__.py
--rw-rw-rw-   0        0        0     3804 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_annotation_break.py
--rw-rw-rw-   0        0        0     2378 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_2d_zone_from_3d_zone.py
--rw-rw-rw-   0        0        0     6652 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_class.py
--rw-rw-rw-   0        0        0     2356 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_colour.py
--rw-rw-rw-   0        0        0     7751 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_data.py
--rw-rw-rw-   0        0        0    17164 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_doc_link.py
--rw-rw-rw-   0        0        0     5691 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_flow.py
--rw-rw-rw-   0        0        0     4386 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_name.py
--rw-rw-rw-   0        0        0     3091 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_show.py
--rw-rw-rw-   0        0        0    10979 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_compatible.py
--rw-rw-rw-   0        0        0    32666 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_component.py
--rw-rw-rw-   0        0        0    14306 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_connectable.py
--rw-rw-rw-   0        0        0    10068 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_connection.py
--rw-rw-rw-   0        0        0    14039 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_connector.py
--rw-rw-rw-   0        0        0     4896 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_delete_check.py
--rw-rw-rw-   0        0        0     3028 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_delete_check2.py
--rw-rw-rw-   0        0        0     3395 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_environment.py
--rw-rw-rw-   0        0        0     3536 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_gap_priority.py
--rw-rw-rw-   0        0        0     3452 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_group.py
--rw-rw-rw-   0        0        0     3008 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_model_init.py
--rw-rw-rw-   0        0        0     8923 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_multi_image.py
--rw-rw-rw-   0        0        0     8943 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_multi_image_master.py
--rw-rw-rw-   0        0        0    11671 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_object_factory.py
--rw-rw-rw-   0        0        0    20901 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_object_factory2.py
--rw-rw-rw-   0        0        0     4679 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_replace.py
--rw-rw-rw-   0        0        0    15366 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_route.py
--rw-rw-rw-   0        0        0     3296 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_route2.py
--rw-rw-rw-   0        0        0     2474 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_scaling_rule.py
--rw-rw-rw-   0        0        0     6280 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_zone.py
--rw-rw-rw-   0        0        0     7615 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_arrow_display.py
--rw-rw-rw-   0        0        0    19219 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_base_factory.py
--rw-rw-rw-   0        0        0     6252 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_boundary_elem.py
--rw-rw-rw-   0        0        0     3944 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_catalog_component.py
--rw-rw-rw-   0        0        0     3781 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_catalog_route.py
--rw-rw-rw-   0        0        0     6030 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_cntr_connect.py
--rw-rw-rw-   0        0        0     5802 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_cntr_doc_link.py
--rw-rw-rw-   0        0        0     6684 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_cntr_graphic.py
--rw-rw-rw-   0        0        0    14915 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_cntr_location.py
--rw-rw-rw-   0        0        0     9752 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_comp_connector.py
--rw-rw-rw-   0        0        0     7819 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_comp_flow.py
--rw-rw-rw-   0        0        0    15238 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_comp_graphic.py
--rw-rw-rw-   0        0        0     5496 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_comp_group_ext.py
--rw-rw-rw-   0        0        0    25584 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_compatible.py
--rw-rw-rw-   0        0        0    52735 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_component.py
--rw-rw-rw-   0        0        0     8796 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_component2.py
--rw-rw-rw-   0        0        0     6070 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_component_group.py
--rw-rw-rw-   0        0        0     3190 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_connectable.py
--rw-rw-rw-   0        0        0     7407 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_drop_off_view.py
--rw-rw-rw-   0        0        0    11239 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_frame_info.py
--rw-rw-rw-   0        0        0     6920 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_gap_display.py
--rw-rw-rw-   0        0        0    11656 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr.py
--rw-rw-rw-   0        0        0     6463 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_cntr.py
--rw-rw-rw-   0        0        0    13900 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_comp.py
--rw-rw-rw-   0        0        0     9838 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_factory.py
--rw-rw-rw-   0        0        0    36789 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_route.py
--rw-rw-rw-   0        0        0     3795 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_route2.py
--rw-rw-rw-   0        0        0     2389 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_route_alternate.py
--rw-rw-rw-   0        0        0     6755 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_route_ellipse.py
--rw-rw-rw-   0        0        0     8151 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_zone.py
--rw-rw-rw-   0        0        0     5276 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_internal_flow.py
--rw-rw-rw-   0        0        0     5231 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_list_of_bst_rs.py
--rw-rw-rw-   0        0        0     5175 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_list_of_doubles.py
--rw-rw-rw-   0        0        0     5340 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_list_of_longs.py
--rw-rw-rw-   0        0        0     5429 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_list_of_objects.py
--rw-rw-rw-   0        0        0     8985 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_movable.py
--rw-rw-rw-   0        0        0     3431 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_movable2.py
--rw-rw-rw-   0        0        0     5306 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_network_analysis.py
--rw-rw-rw-   0        0        0     4210 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_obsolete_model.py
--rw-rw-rw-   0        0        0     2223 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_post_replace.py
--rw-rw-rw-   0        0        0     3207 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_replace.py
--rw-rw-rw-   0        0        0    41105 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_route.py
--rw-rw-rw-   0        0        0     9491 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_route_alternate_graphic.py
--rw-rw-rw-   0        0        0     7004 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_route_graphic.py
--rw-rw-rw-   0        0        0     7180 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_route_symbol.py
--rw-rw-rw-   0        0        0     9511 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_session.py
--rw-rw-rw-   0        0        0     5583 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_temp_list_factory.py
--rw-rw-rw-   0        0        0     5008 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_update_instances.py
--rw-rw-rw-   0        0        0     3192 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_workbench.py
--rw-rw-rw-   0        0        0     2034 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_zone.py
--rw-rw-rw-   0        0        0     6343 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_zone_graphic.py
--rw-rw-rw-   0        0        0     1920 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_zone_membership.py
--rw-rw-rw-   0        0        0     5343 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/schematic_extension.py
--rw-rw-rw-   0        0        0    20891 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/schematic_root.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.478126 pycatia-0.6.8/pycatia/cat_sde_setting_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/cat_sde_setting_interfaces/__init__.py
--rw-rw-rw-   0        0        0   129104 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sde_setting_interfaces/step_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.482127 pycatia-0.6.8/pycatia/cat_sm_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/cat_sm_interfaces/__init__.py
--rw-rw-rw-   0        0        0     5802 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sm_interfaces/catalog_shm_object_setting_att.py
--rw-rw-rw-   0        0        0   166298 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_sm_interfaces/view_characteristic_curves_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.489127 pycatia-0.6.8/pycatia/cat_smarteam_integ_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/cat_smarteam_integ_interfaces/__init__.py
--rw-rw-rw-   0        0        0    10819 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/cat_smarteam_integ_interfaces/sti_db_children.py
--rw-rw-rw-   0        0        0     8310 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/cat_smarteam_integ_interfaces/sti_db_item.py
--rw-rw-rw-   0        0        0    71028 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_smarteam_integ_interfaces/sti_engine.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.550200 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/__init__.py
--rw-rw-rw-   0        0        0    12014 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/end_cut_ess_object_setting_att.py
--rw-rw-rw-   0        0        0     3355 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sdd_product.py
--rw-rw-rw-   0        0        0     3390 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfd_product.py
--rw-rw-rw-   0        0        0     4898 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_connection_parameters.py
--rw-rw-rw-   0        0        0     7839 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_endcut.py
--rw-rw-rw-   0        0        0     8035 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_endcut_manager.py
--rw-rw-rw-   0        0        0    34661 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_factory.py
--rw-rw-rw-   0        0        0    13339 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_function_factory.py
--rw-rw-rw-   0        0        0    10680 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_manager.py
--rw-rw-rw-   0        0        0     4915 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member.py
--rw-rw-rw-   0        0        0    10463 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member2_points.py
--rw-rw-rw-   0        0        0     5462 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_curve.py
--rw-rw-rw-   0        0        0     6099 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_plane2_curves.py
--rw-rw-rw-   0        0        0     6674 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_point_length.py
--rw-rw-rw-   0        0        0     6376 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_point_up_to_limit.py
--rw-rw-rw-   0        0        0     8573 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_surf_surf.py
--rw-rw-rw-   0        0        0     3673 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_object.py
--rw-rw-rw-   0        0        0     1274 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_object_ext.py
--rw-rw-rw-   0        0        0    10868 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_opening.py
--rw-rw-rw-   0        0        0     8692 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_opening_contours_mgr.py
--rw-rw-rw-   0        0        0     8663 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_operation_factory.py
--rw-rw-rw-   0        0        0     7637 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_positioning_strategy_manager.py
--rw-rw-rw-   0        0        0    24387 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_profile.py
--rw-rw-rw-   0        0        0     5395 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_references.py
--rw-rw-rw-   0        0        0    13630 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_slot.py
--rw-rw-rw-   0        0        0     8434 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_slots.py
--rw-rw-rw-   0        0        0     2648 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_split_plate.py
--rw-rw-rw-   0        0        0     2916 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_split_plates.py
--rw-rw-rw-   0        0        0     4216 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_standard_contour_parameters.py
--rw-rw-rw-   0        0        0    16391 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_standard_opening.py
--rw-rw-rw-   0        0        0    16846 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_standard_pos_strategy_parameters.py
--rw-rw-rw-   0        0        0     9952 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_stiffener.py
--rw-rw-rw-   0        0        0    11176 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_stiffener_on_free_edge.py
--rw-rw-rw-   0        0        0    27220 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_super_plate.py
--rw-rw-rw-   0        0        0     5447 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_weld.py
--rw-rw-rw-   0        0        0     2809 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_welds.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.641344 pycatia-0.6.8/pycatia/cat_tps_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/__init__.py
--rw-rw-rw-   0        0        0    31138 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation.py
--rw-rw-rw-   0        0        0    19658 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_2.py
--rw-rw-rw-   0        0        0    20053 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_factory.py
--rw-rw-rw-   0        0        0    21864 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_factory_2.py
--rw-rw-rw-   0        0        0    14701 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_set.py
--rw-rw-rw-   0        0        0     2553 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_set_transform_into_assembly_set.py
--rw-rw-rw-   0        0        0     3630 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_sets.py
--rw-rw-rw-   0        0        0     4035 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/annotations.py
--rw-rw-rw-   0        0        0     2959 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/assembly_annotation_sets.py
--rw-rw-rw-   0        0        0     2674 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/associated_ref_frame.py
--rw-rw-rw-   0        0        0    11659 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/capture.py
--rw-rw-rw-   0        0        0     2041 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/capture_factory.py
--rw-rw-rw-   0        0        0     2140 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/captures.py
--rw-rw-rw-   0        0        0     2261 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/composite_tolerance.py
--rw-rw-rw-   0        0        0     1750 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/controlled_radius.py
--rw-rw-rw-   0        0        0     2509 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/datum_simple.py
--rw-rw-rw-   0        0        0    11536 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/datum_target.py
--rw-rw-rw-   0        0        0     3459 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/default_annotation.py
--rw-rw-rw-   0        0        0    10328 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/dimension_3d.py
--rw-rw-rw-   0        0        0     6204 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/dimension_limit.py
--rw-rw-rw-   0        0        0     1618 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/dimension_pattern.py
--rw-rw-rw-   0        0        0    19678 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/dmu_tol_setting_att.py
--rw-rw-rw-   0        0        0     1641 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/envelope_condition.py
--rw-rw-rw-   0        0        0     9245 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/flag_note.py
--rw-rw-rw-   0        0        0     1739 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/free_state.py
--rw-rw-rw-   0        0        0    69177 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/fta_infra_setting_att.py
--rw-rw-rw-   0        0        0   236553 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/fta_setting_att.py
--rw-rw-rw-   0        0        0     1649 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/material_condition.py
--rw-rw-rw-   0        0        0    11181 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/noa.py
--rw-rw-rw-   0        0        0     1745 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/non_semantic_datum.py
--rw-rw-rw-   0        0        0     3159 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/non_semantic_datum_target.py
--rw-rw-rw-   0        0        0     3293 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/non_semantic_dimension.py
--rw-rw-rw-   0        0        0     1702 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/non_semantic_gdt.py
--rw-rw-rw-   0        0        0     1919 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/particular_tol_elem.py
--rw-rw-rw-   0        0        0     5412 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/projected_tolerance_zone.py
--rw-rw-rw-   0        0        0    14500 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/reference_frame.py
--rw-rw-rw-   0        0        0     5978 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/roughness.py
--rw-rw-rw-   0        0        0    17825 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/semantic_gdt.py
--rw-rw-rw-   0        0        0     6829 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/shifted_profile_tolerance.py
--rw-rw-rw-   0        0        0     1763 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/tangent_plane.py
--rw-rw-rw-   0        0        0     2702 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/text.py
--rw-rw-rw-   0        0        0     2179 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/tolerance_per_unit_basis_restrictive_value.py
--rw-rw-rw-   0        0        0     3020 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/tolerance_unit_basis_value.py
--rw-rw-rw-   0        0        0     2303 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/tolerance_zone.py
--rw-rw-rw-   0        0        0     2507 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/tps_parallel_on_screen.py
--rw-rw-rw-   0        0        0     1221 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/tps_view.py
--rw-rw-rw-   0        0        0     2638 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/tps_view_factory.py
--rw-rw-rw-   0        0        0     2185 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/tps_views.py
--rw-rw-rw-   0        0        0     6229 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/user_surface.py
--rw-rw-rw-   0        0        0     7752 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/user_surfaces.py
--rw-rw-rw-   0        0        0     2137 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/cat_tps_interfaces/weld.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.645319 pycatia-0.6.8/pycatia/catia_de_settings_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/catia_de_settings_interfaces/__init__.py
--rw-rw-rw-   0        0        0    68427 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/catia_de_settings_interfaces/iges_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.655319 pycatia-0.6.8/pycatia/catia_v4_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/catia_v4_interfaces/__init__.py
--rw-rw-rw-   0        0        0    24031 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/catia_v4_interfaces/interop_setting_att.py
--rw-rw-rw-   0        0        0    34731 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/catia_v4_interfaces/migr_batch_setting_att.py
--rw-rw-rw-   0        0        0     8685 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/catia_v4_interfaces/spec_v4_setting_att.py
--rw-rw-rw-   0        0        0    33750 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/catia_v4_interfaces/v4_v5_space_setting_att.py
--rw-rw-rw-   0        0        0    38011 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/catia_v4_interfaces/v4_writing_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.659319 pycatia-0.6.8/pycatia/components_catalogs_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/components_catalogs_interfaces/__init__.py
--rw-rw-rw-   0        0        0     8304 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/components_catalogs_interfaces/catalog_document.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.661318 pycatia-0.6.8/pycatia/composites_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/composites_interfaces/__init__.py
--rw-rw-rw-   0        0        0     7398 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/composites_interfaces/composites_material.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.683344 pycatia-0.6.8/pycatia/dmaps_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/__init__.py
--rw-rw-rw-   0        0        0     5268 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/activities.py
--rw-rw-rw-   0        0        0    35559 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/activity.py
--rw-rw-rw-   0        0        0     1263 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/item.py
--rw-rw-rw-   0        0        0     7136 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/items.py
--rw-rw-rw-   0        0        0    19677 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/lib_tab_setting_att.py
--rw-rw-rw-   0        0        0     4257 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/outputs.py
--rw-rw-rw-   0        0        0     3389 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/process_document.py
--rw-rw-rw-   0        0        0     5641 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/resource.py
--rw-rw-rw-   0        0        0     2445 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/resource_collection.py
--rw-rw-rw-   0        0        0     5533 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/resources.py
--rw-rw-rw-   0        0        0    64615 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/tree_tab_setting_att.py
--rw-rw-rw-   0        0        0    14869 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dmaps_interfaces/verif_tab_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.685319 pycatia-0.6.8/pycatia/dnb_asy_activity_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_asy_activity_interfaces/__init__.py
--rw-rw-rw-   0        0        0     2006 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_asy_activity_interfaces/asy_sim_activity.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.688341 pycatia-0.6.8/pycatia/dnb_d5_iInterfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_d5_iInterfaces/__init__.py
--rw-rw-rw-   0        0        0    89435 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_d5_iInterfaces/import_d5_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.693345 pycatia-0.6.8/pycatia/dnb_device_activity_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_activity_interfaces/__init__.py
--rw-rw-rw-   0        0        0    10678 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_activity_interfaces/move_home_act.py
--rw-rw-rw-   0        0        0    10748 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_activity_interfaces/move_joints_act.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.708346 pycatia-0.6.8/pycatia/dnb_device_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_interfaces/__init__.py
--rw-rw-rw-   0        0        0     7327 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_interfaces/basic_device.py
--rw-rw-rw-   0        0        0     2590 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_interfaces/d5_device.py
--rw-rw-rw-   0        0        0    35302 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_interfaces/dev_analysis_setting_att.py
--rw-rw-rw-   0        0        0     6698 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_interfaces/device_joint_relations.py
--rw-rw-rw-   0        0        0     9840 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_interfaces/device_sim.py
--rw-rw-rw-   0        0        0     3876 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_interfaces/dof_state.py
--rw-rw-rw-   0        0        0    12950 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_device_interfaces/home_position.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.713566 pycatia-0.6.8/pycatia/dnb_dpm_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_dpm_interfaces/__init__.py
--rw-rw-rw-   0        0        0    12043 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_dpm_interfaces/mfg_assembly.py
--rw-rw-rw-   0        0        0    18123 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_dpm_interfaces/mfg_assembly_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.718567 pycatia-0.6.8/pycatia/dnb_ehm_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_ehm_interfaces/__init__.py
--rw-rw-rw-   0        0        0    30228 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_ehm_interfaces/ehm_insertion_act_plug_map_view_data.py
--rw-rw-rw-   0        0        0    13085 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_ehm_interfaces/plug_map_view_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.721566 pycatia-0.6.8/pycatia/dnb_ehs_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_ehs_interfaces/__init__.py
--rw-rw-rw-   0        0        0     2582 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_ehs_interfaces/ehs_update_smoothness_factor.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.724567 pycatia-0.6.8/pycatia/dnb_ekp_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_ekp_interfaces/__init__.py
--rw-rw-rw-   0        0        0    12898 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_ekp_interfaces/ekp_services.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.743568 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1657 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/curve_fastener.py
--rw-rw-rw-   0        0        0    16617 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/dnb_fastener_item_services.py
--rw-rw-rw-   0        0        0    16244 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/dnb_fastener_management.py
--rw-rw-rw-   0        0        0    10746 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/dnb_fastener_new_mfg_pos_services.py
--rw-rw-rw-   0        0        0    17815 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/fastener.py
--rw-rw-rw-   0        0        0    13251 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/fastener_group.py
--rw-rw-rw-   0        0        0     2482 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/fastener_set.py
--rw-rw-rw-   0        0        0     6392 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/fastener_work_bench.py
--rw-rw-rw-   0        0        0     5477 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_fastener_interfaces/point_fastener.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.747567 pycatia-0.6.8/pycatia/dnb_graph_editor/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_graph_editor/__init__.py
--rw-rw-rw-   0        0        0     3552 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_graph_editor/pert_node.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.794566 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/__init__.py
--rw-rw-rw-   0        0        0     9912 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_anthro.py
--rw-rw-rw-   0        0        0     9464 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_anthro_variable.py
--rw-rw-rw-   0        0        0    27658 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_body.py
--rw-rw-rw-   0        0        0     9382 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_body_element.py
--rw-rw-rw-   0        0        0     1368 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_center_of_gravity.py
--rw-rw-rw-   0        0        0     4220 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo.py
--rw-rw-rw-   0        0        0     4174 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo_carry.py
--rw-rw-rw-   0        0        0    28436 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo_lift_lower.py
--rw-rw-rw-   0        0        0     6665 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo_push_pull.py
--rw-rw-rw-   0        0        0     7278 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo_rula.py
--rw-rw-rw-   0        0        0     9276 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_hmi_workbench.py
--rw-rw-rw-   0        0        0     8074 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_human_catalog.py
--rw-rw-rw-   0        0        0     9888 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_line_of_sight.py
--rw-rw-rw-   0        0        0     4764 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_line_of_sight_node.py
--rw-rw-rw-   0        0        0     9321 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_manikin.py
--rw-rw-rw-   0        0        0     1820 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_manikin_part.py
--rw-rw-rw-   0        0        0     1298 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_node.py
--rw-rw-rw-   0        0        0    32651 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_segment.py
--rw-rw-rw-   0        0        0     5991 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_segment_node.py
--rw-rw-rw-   0        0        0    15408 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_vision.py
--rw-rw-rw-   0        0        0    15488 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swkdof.py
--rw-rw-rw-   0        0        0    31339 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swkik_constraint.py
--rw-rw-rw-   0        0        0     9021 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swkik_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.828082 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/__init__.py
--rw-rw-rw-   0        0        0     3775 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/auto_walk_activity.py
--rw-rw-rw-   0        0        0     3642 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/collision_free_walk.py
--rw-rw-rw-   0        0        0    22264 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/hts_ccp_setting_att.py
--rw-rw-rw-   0        0        0    41891 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/hts_general_setting_att.py
--rw-rw-rw-   0        0        0    10173 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/hts_joint_speed_settings_att.py
--rw-rw-rw-   0        0        0    36584 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/hts_task_display_setting_att.py
--rw-rw-rw-   0        0        0     4284 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_activity_group.py
--rw-rw-rw-   0        0        0    66950 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_activity_group_factory.py
--rw-rw-rw-   0        0        0    72493 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_acts_factory.py
--rw-rw-rw-   0        0        0     3969 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_call_task.py
--rw-rw-rw-   0        0        0     2392 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_program.py
--rw-rw-rw-   0        0        0     4355 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_task.py
--rw-rw-rw-   0        0        0     2473 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_task_list.py
--rw-rw-rw-   0        0        0    30215 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/move_to_posture_activity.py
--rw-rw-rw-   0        0        0    12771 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/pick_activity.py
--rw-rw-rw-   0        0        0    18095 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/place_activity.py
--rw-rw-rw-   0        0        0    10521 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/walk_activity.py
--rw-rw-rw-   0        0        0     3014 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/worker_activity.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.836085 pycatia-0.6.8/pycatia/dnb_igp_arc_commands/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_arc_commands/__init__.py
--rw-rw-rw-   0        0        0    14811 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_arc_commands/amp_path.py
--rw-rw-rw-   0        0        0    31990 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_arc_commands/amp_tag.py
--rw-rw-rw-   0        0        0    28761 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_arc_commands/arc_tag.py
--rw-rw-rw-   0        0        0    20357 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_arc_commands/arc_tag_group.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.841080 pycatia-0.6.8/pycatia/dnb_igp_olp_ui/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_olp_ui/__init__.py
--rw-rw-rw-   0        0        0    39040 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_olp_ui/igp_olp_setting_att.py
--rw-rw-rw-   0        0        0    23296 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_olp_ui/olp_translator.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.874080 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/__init__.py
--rw-rw-rw-   0        0        0     8818 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/call_robot_task_activity.py
--rw-rw-rw-   0        0        0    11994 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/device_task.py
--rw-rw-rw-   0        0        0     9247 2023-10-31 11:15:07.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/device_task_factory.py
--rw-rw-rw-   0        0        0     4209 2023-10-31 11:15:08.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/generic_action.py
--rw-rw-rw-   0        0        0     4906 2023-10-31 11:15:08.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/generic_action_factory.py
--rw-rw-rw-   0        0        0     4568 2023-10-31 11:15:08.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/mount_activity.py
--rw-rw-rw-   0        0        0    18460 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/mount_manager.py
--rw-rw-rw-   0        0        0     5692 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/move_action_activity.py
--rw-rw-rw-   0        0        0    12947 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/operation.py
--rw-rw-rw-   0        0        0     6927 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/operation_profile.py
--rw-rw-rw-   0        0        0    54586 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/robot_motion.py
--rw-rw-rw-   0        0        0    16852 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/robot_task.py
--rw-rw-rw-   0        0        0     9191 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/robot_task_clone_factory.py
--rw-rw-rw-   0        0        0     9169 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/robot_task_factory.py
--rw-rw-rw-   0        0        0    13836 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tag.py
--rw-rw-rw-   0        0        0     4475 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tag_factory.py
--rw-rw-rw-   0        0        0     9961 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tag_group.py
--rw-rw-rw-   0        0        0    15928 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tag_group_factory.py
--rw-rw-rw-   0        0        0     8202 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tcp_trace_activity.py
--rw-rw-rw-   0        0        0     4618 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/unmount_activity.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.880081 pycatia-0.6.8/pycatia/dnb_manufacturing_layout_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_manufacturing_layout_interfaces/__init__.py
--rw-rw-rw-   0        0        0     4104 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_manufacturing_layout_interfaces/attachment_cont.py
--rw-rw-rw-   0        0        0    10115 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_manufacturing_layout_interfaces/dnb_attachment.py
--rw-rw-rw-   0        0        0     3643 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_manufacturing_layout_interfaces/dnb_attachment_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.886080 pycatia-0.6.8/pycatia/dnb_mhi_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_mhi_interfaces/__init__.py
--rw-rw-rw-   0        0        0    28834 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_mhi_interfaces/mhi_load_parameters.py
--rw-rw-rw-   0        0        0     9326 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_mhi_interfaces/mhi_open_access.py
--rw-rw-rw-   0        0        0     6008 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_mhi_interfaces/mhi_save_access.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.889080 pycatia-0.6.8/pycatia/dnb_reporting_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_reporting_interfaces/__init__.py
--rw-rw-rw-   0        0        0    31159 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_reporting_interfaces/fas_reporting_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.896085 pycatia-0.6.8/pycatia/dnb_resource_program_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_resource_program_interfaces/__init__.py
--rw-rw-rw-   0        0        0     7106 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_resource_program_interfaces/active_task.py
--rw-rw-rw-   0        0        0     6817 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/dnb_resource_program_interfaces/resource_program_manager.py
--rw-rw-rw-   0        0        0     6540 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/dnb_resource_program_interfaces/task.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.924595 pycatia-0.6.8/pycatia/dnb_robot_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/__init__.py
--rw-rw-rw-   0        0        0     9640 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/aux_devices_mgt.py
--rw-rw-rw-   0        0        0    26028 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/calib_offsets.py
--rw-rw-rw-   0        0        0    12207 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/generic_accuracy_profile.py
--rw-rw-rw-   0        0        0    15337 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/generic_motion_profile.py
--rw-rw-rw-   0        0        0     8610 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/generic_obj_frame_profile.py
--rw-rw-rw-   0        0        0    19857 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/generic_tool_profile.py
--rw-rw-rw-   0        0        0     9779 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/parameter_profiles.py
--rw-rw-rw-   0        0        0    18481 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/parameter_profiles_factory.py
--rw-rw-rw-   0        0        0     6828 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/rob_analysis_heart_beat_usage_setting_att.py
--rw-rw-rw-   0        0        0    39452 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/rob_analysis_setting_att.py
--rw-rw-rw-   0        0        0     9653 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/rob_controller_factory.py
--rw-rw-rw-   0        0        0    50131 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/rob_generic_controller.py
--rw-rw-rw-   0        0        0    85179 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/rrs_setting_att.py
--rw-rw-rw-   0        0        0    25756 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/tcp_trace.py
--rw-rw-rw-   0        0        0    11973 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/tcp_trace_manager.py
--rw-rw-rw-   0        0        0     8388 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_robot_interfaces/tcp_trace_manager_graphics.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.931595 pycatia-0.6.8/pycatia/dnb_sim_activity_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_sim_activity_interfaces/__init__.py
--rw-rw-rw-   0        0        0     2779 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_sim_activity_interfaces/delay_act.py
--rw-rw-rw-   0        0        0     5693 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_sim_activity_interfaces/grab_act.py
--rw-rw-rw-   0        0        0     5750 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_sim_activity_interfaces/release_act.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.939594 pycatia-0.6.8/pycatia/dnb_simulation_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_simulation_interfaces/__init__.py
--rw-rw-rw-   0        0        0    87704 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_simulation_interfaces/analysis_setting_att.py
--rw-rw-rw-   0        0        0    51097 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_simulation_interfaces/sim_trace_setting_att.py
--rw-rw-rw-   0        0        0     8987 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_simulation_interfaces/simulation_init_state.py
--rw-rw-rw-   0        0        0   102279 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_simulation_interfaces/simulation_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.942594 pycatia-0.6.8/pycatia/dnb_sor_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_sor_interfaces/__init__.py
--rw-rw-rw-   0        0        0    46464 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/dnb_sor_interfaces/order_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.949595 pycatia-0.6.8/pycatia/dnb_state_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_state_interfaces/__init__.py
--rw-rw-rw-   0        0        0    27783 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_state_interfaces/dnb_3d_state.py
--rw-rw-rw-   0        0        0    17142 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_state_interfaces/dnb_3d_state_management.py
--rw-rw-rw-   0        0        0     3468 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_state_interfaces/dnb_3d_states.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.961594 pycatia-0.6.8/pycatia/dnb_work_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/dnb_work_interfaces/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_buy_off.py
--rw-rw-rw-   0        0        0     4046 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_change_notification.py
--rw-rw-rw-   0        0        0     4014 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_data_collection.py
--rw-rw-rw-   0        0        0     8948 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_text.py
--rw-rw-rw-   0        0        0     3239 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_text_access_ei.py
--rw-rw-rw-   0        0        0    31688 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/dnb_work_interfaces/work_general_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:01.976594 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/__init__.py
--rw-rw-rw-   0        0        0     3161 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_factory.py
--rw-rw-rw-   0        0        0    11778 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_root.py
--rw-rw-rw-   0        0        0   161905 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_setting_att.py
--rw-rw-rw-   0        0        0    19773 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_sheet.py
--rw-rw-rw-   0        0        0    10622 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_sheets.py
--rw-rw-rw-   0        0        0    31074 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_view.py
--rw-rw-rw-   0        0        0    22385 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_views.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.034109 pycatia-0.6.8/pycatia/drafting_interfaces/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/drafting_interfaces/__init__.py
--rw-rw-rw-   0        0        0    58714 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drafting_setting_att.py
--rw-rw-rw-   0        0        0    15442 2023-10-31 11:15:09.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_arrow.py
--rw-rw-rw-   0        0        0     6961 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_arrows.py
--rw-rw-rw-   0        0        0    19432 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_component.py
--rw-rw-rw-   0        0        0     8592 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_components.py
--rw-rw-rw-   0        0        0    19607 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dim_ext_line.py
--rw-rw-rw-   0        0        0    16275 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dim_line.py
--rw-rw-rw-   0        0        0    26915 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dim_value.py
--rw-rw-rw-   0        0        0    33304 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dimension.py
--rw-rw-rw-   0        0        0    13674 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dimensions.py
--rw-rw-rw-   0        0        0     7831 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_document.py
--rw-rw-rw-   0        0        0    16400 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_leader.py
--rw-rw-rw-   0        0        0     6746 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_leaders.py
--rw-rw-rw-   0        0        0     4506 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_page_setup.py
--rw-rw-rw-   0        0        0    13366 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_picture.py
--rw-rw-rw-   0        0        0     8215 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_pictures.py
--rw-rw-rw-   0        0        0     4043 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_root.py
--rw-rw-rw-   0        0        0    25212 2023-10-31 11:15:10.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_sheet.py
--rw-rw-rw-   0        0        0    10412 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_sheets.py
--rw-rw-rw-   0        0        0    42085 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_table.py
--rw-rw-rw-   0        0        0     7505 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_tables.py
--rw-rw-rw-   0        0        0    25355 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_text.py
--rw-rw-rw-   0        0        0    18904 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_text_properties.py
--rw-rw-rw-   0        0        0     9783 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_text_range.py
--rw-rw-rw-   0        0        0     6907 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_texts.py
--rw-rw-rw-   0        0        0     3890 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_thread.py
--rw-rw-rw-   0        0        0     6595 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_threads.py
--rw-rw-rw-   0        0        0    41664 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_view.py
--rw-rw-rw-   0        0        0    78715 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_view_generative_behavior.py
--rw-rw-rw-   0        0        0     6699 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_view_generative_links.py
--rw-rw-rw-   0        0        0     9466 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_views.py
--rw-rw-rw-   0        0        0    17595 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_welding.py
--rw-rw-rw-   0        0        0     7109 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/drafting_interfaces/drawing_weldings.py
--rw-rw-rw-   0        0        0    10022 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/drafting_interfaces/print_area.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.039111 pycatia-0.6.8/pycatia/electrical_schematic_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/electrical_schematic_interfaces/__init__.py
--rw-rw-rw-   0        0        0     5395 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/electrical_schematic_interfaces/electrical_schematic_object.py
--rw-rw-rw-   0        0        0     1584 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/electrical_schematic_interfaces/electrical_schematic_wire.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.063110 pycatia-0.6.8/pycatia/eno_cd5_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/__init__.py
--rw-rw-rw-   0        0        0    21333 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_engine.py
--rw-rw-rw-   0        0        0     6726 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_engine_v6_r2014x.py
--rw-rw-rw-   0        0        0    15184 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_engine_v6_r2015.py
--rw-rw-rw-   0        0        0     2551 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_id.py
--rw-rw-rw-   0        0        0     2636 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_ids.py
--rw-rw-rw-   0        0        0     3788 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_properties.py
--rw-rw-rw-   0        0        0     3880 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_property.py
--rw-rw-rw-   0        0        0    12261 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_save_item.py
--rw-rw-rw-   0        0        0     2963 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_save_items.py
--rw-rw-rw-   0        0        0     8166 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_save_operation.py
--rw-rw-rw-   0        0        0     5313 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_structure.py
--rw-rw-rw-   0        0        0     4823 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_template.py
--rw-rw-rw-   0        0        0     4175 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_template_type.py
--rw-rw-rw-   0        0        0     2789 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_template_types.py
--rw-rw-rw-   0        0        0     2555 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_templates.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.065110 pycatia-0.6.8/pycatia/enumeration/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.6.8/pycatia/enumeration/__init__.py
--rw-rw-rw-   0        0        0    54918 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/enumeration/enumeration_types.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.068110 pycatia-0.6.8/pycatia/exception_handling/
--rw-rw-rw-   0        0        0       76 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/exception_handling/__init__.py
--rw-rw-rw-   0        0        0      331 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/exception_handling/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.085110 pycatia-0.6.8/pycatia/fitting_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/fitting_interfaces/__init__.py
--rw-rw-rw-   0        0        0    31764 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/fitting_setting_att.py
--rw-rw-rw-   0        0        0    31745 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/manip_setting_att.py
--rw-rw-rw-   0        0        0    11585 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/sampled.py
--rw-rw-rw-   0        0        0     6392 2023-10-31 11:15:12.000000 pycatia-0.6.8/pycatia/fitting_interfaces/sampleds.py
--rw-rw-rw-   0        0        0     2587 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/sampleds_node.py
--rw-rw-rw-   0        0        0    18875 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/shot.py
--rw-rw-rw-   0        0        0     8890 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/shots.py
--rw-rw-rw-   0        0        0     8572 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/shuttle.py
--rw-rw-rw-   0        0        0     4528 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/shuttles.py
--rw-rw-rw-   0        0        0     8714 2023-10-31 11:15:11.000000 pycatia-0.6.8/pycatia/fitting_interfaces/track.py
--rw-rw-rw-   0        0        0     2253 2023-10-31 11:15:12.000000 pycatia-0.6.8/pycatia/fitting_interfaces/tracks.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.126628 pycatia-0.6.8/pycatia/funct_system_interfaces/
--rw-rw-rw-   0        0        0        0 2022-11-18 10:48:10.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/__init__.py
--rw-rw-rw-   0        0        0     9253 2023-10-31 11:15:12.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_actions_group.py
--rw-rw-rw-   0        0        0     5584 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_actions_groups.py
--rw-rw-rw-   0        0        0     3801 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_association.py
--rw-rw-rw-   0        0        0     5543 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_associations.py
--rw-rw-rw-   0        0        0     3332 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_facet_managers.py
--rw-rw-rw-   0        0        0     2458 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_gen_script_mgr.py
--rw-rw-rw-   0        0        0     2456 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_multi_rep_mgr.py
--rw-rw-rw-   0        0        0     2928 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_node_graph_layout.py
--rw-rw-rw-   0        0        0     1893 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_script.py
--rw-rw-rw-   0        0        0     5298 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/funct_scripts.py
--rw-rw-rw-   0        0        0     7114 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_action.py
--rw-rw-rw-   0        0        0     5292 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_actions.py
--rw-rw-rw-   0        0        0     7357 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_description.py
--rw-rw-rw-   0        0        0     2981 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_document.py
--rw-rw-rw-   0        0        0     2311 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_element.py
--rw-rw-rw-   0        0        0     2516 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_facet.py
--rw-rw-rw-   0        0        0     1337 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_facet_mgr.py
--rw-rw-rw-   0        0        0     3868 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_object.py
--rw-rw-rw-   0        0        0     3538 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_object_proxy.py
--rw-rw-rw-   0        0        0     5854 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_objects.py
--rw-rw-rw-   0        0        0     2796 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_position.py
--rw-rw-rw-   0        0        0    42528 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_system_setting_att.py
--rw-rw-rw-   0        0        0     2023 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_variant.py
--rw-rw-rw-   0        0        0     5009 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/funct_system_interfaces/functional_variants.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.151627 pycatia-0.6.8/pycatia/general_knowledge_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/__init__.py
--rw-rw-rw-   0        0        0     4605 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_check.py
--rw-rw-rw-   0        0        0    11432 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_check_runtime.py
--rw-rw-rw-   0        0        0     5669 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_report_object.py
--rw-rw-rw-   0        0        0     8170 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_report_objects.py
--rw-rw-rw-   0        0        0     4248 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule.py
--rw-rw-rw-   0        0        0     2237 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_base.py
--rw-rw-rw-   0        0        0     7428 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_base_component_runtime.py
--rw-rw-rw-   0        0        0    12861 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_base_component_runtimes.py
--rw-rw-rw-   0        0        0    25920 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_base_runtime.py
--rw-rw-rw-   0        0        0     3148 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_runtime.py
--rw-rw-rw-   0        0        0    11464 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_set.py
--rw-rw-rw-   0        0        0     4268 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_set_runtime.py
--rw-rw-rw-   0        0        0     4009 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/general_knowledge_interfaces/kwe_correct_function.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.348695 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/__init__.py
--rw-rw-rw-   0        0        0     5869 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_3d_curve_offset.py
--rw-rw-rw-   0        0        0    12406 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_affinity.py
--rw-rw-rw-   0        0        0    33611 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_assemble.py
--rw-rw-rw-   0        0        0     5961 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_line.py
--rw-rw-rw-   0        0        0     7527 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_to_axis.py
--rw-rw-rw-   0        0        0    55632 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_blend.py
--rw-rw-rw-   0        0        0     7640 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_boundary.py
--rw-rw-rw-   0        0        0     8127 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_bump.py
--rw-rw-rw-   0        0        0    13687 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle.py
--rw-rw-rw-   0        0        0    11751 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle2_points_rad.py
--rw-rw-rw-   0        0        0     6962 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle3_points.py
--rw-rw-rw-   0        0        0    16515 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_point.py
--rw-rw-rw-   0        0        0    17752 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_radius.py
--rw-rw-rw-   0        0        0     8549 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_axis.py
--rw-rw-rw-   0        0        0    16136 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_tangent.py
--rw-rw-rw-   0        0        0     7004 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_pt.py
--rw-rw-rw-   0        0        0    12421 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_rad.py
--rw-rw-rw-   0        0        0     1870 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_explicit.py
--rw-rw-rw-   0        0        0    19231 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_tritangent.py
--rw-rw-rw-   0        0        0     9967 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_combine.py
--rw-rw-rw-   0        0        0    52700 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_conic.py
--rw-rw-rw-   0        0        0    11890 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_connect.py
--rw-rw-rw-   0        0        0    22143 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_corner.py
--rw-rw-rw-   0        0        0     1522 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_explicit.py
--rw-rw-rw-   0        0        0    23254 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_par.py
--rw-rw-rw-   0        0        0    38073 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_smooth.py
--rw-rw-rw-   0        0        0    10014 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_cylinder.py
--rw-rw-rw-   0        0        0    15802 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_develop.py
--rw-rw-rw-   0        0        0    10462 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_direction.py
--rw-rw-rw-   0        0        0    11283 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extract.py
--rw-rw-rw-   0        0        0    47925 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extract_multi.py
--rw-rw-rw-   0        0        0    27662 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extrapol.py
--rw-rw-rw-   0        0        0     7103 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum.py
--rw-rw-rw-   0        0        0     6172 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum_polar.py
--rw-rw-rw-   0        0        0    14952 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extrude.py
--rw-rw-rw-   0        0        0   241892 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_factory.py
--rw-rw-rw-   0        0        0    37178 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fill.py
--rw-rw-rw-   0        0        0    20008 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_bi_tangent.py
--rw-rw-rw-   0        0        0    10397 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_tri_tangent.py
--rw-rw-rw-   0        0        0    33448 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_healing.py
--rw-rw-rw-   0        0        0    15240 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_helix.py
--rw-rw-rw-   0        0        0    17831 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_integrated_law.py
--rw-rw-rw-   0        0        0     9789 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_intersection.py
--rw-rw-rw-   0        0        0     3419 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_inverse.py
--rw-rw-rw-   0        0        0    12950 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_law_dist_proj.py
--rw-rw-rw-   0        0        0    11668 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_angle.py
--rw-rw-rw-   0        0        0    15163 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bi_tangent.py
--rw-rw-rw-   0        0        0    12124 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bisecting.py
--rw-rw-rw-   0        0        0     1563 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_explicit.py
--rw-rw-rw-   0        0        0    11145 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_normal.py
--rw-rw-rw-   0        0        0    12647 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_dir.py
--rw-rw-rw-   0        0        0    11500 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_pt.py
--rw-rw-rw-   0        0        0    12650 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_tangency.py
--rw-rw-rw-   0        0        0    66004 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_loft.py
--rw-rw-rw-   0        0        0     4732 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_mid_surface.py
--rw-rw-rw-   0        0        0     3966 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_near.py
--rw-rw-rw-   0        0        0     7666 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_offset.py
--rw-rw-rw-   0        0        0     2627 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_curve.py
--rw-rw-rw-   0        0        0     3464 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_line1_pt.py
--rw-rw-rw-   0        0        0     4556 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane2_lines.py
--rw-rw-rw-   0        0        0     5084 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane3_points.py
--rw-rw-rw-   0        0        0     5922 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_angle.py
--rw-rw-rw-   0        0        0     9143 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_equation.py
--rw-rw-rw-   0        0        0     1574 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_explicit.py
--rw-rw-rw-   0        0        0     9092 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_mean.py
--rw-rw-rw-   0        0        0     3780 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_normal.py
--rw-rw-rw-   0        0        0     3582 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset.py
--rw-rw-rw-   0        0        0     3828 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset_pt.py
--rw-rw-rw-   0        0        0     3820 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_tangent.py
--rw-rw-rw-   0        0        0     7334 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_between.py
--rw-rw-rw-   0        0        0     2910 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_center.py
--rw-rw-rw-   0        0        0     6861 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_coord.py
--rw-rw-rw-   0        0        0     1574 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_explicit.py
--rw-rw-rw-   0        0        0    13727 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_curve.py
--rw-rw-rw-   0        0        0    10203 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_plane.py
--rw-rw-rw-   0        0        0     6413 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_surface.py
--rw-rw-rw-   0        0        0     4257 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_tangent.py
--rw-rw-rw-   0        0        0    13045 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_polyline.py
--rw-rw-rw-   0        0        0    20768 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_position_transfo.py
--rw-rw-rw-   0        0        0    12602 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_project.py
--rw-rw-rw-   0        0        0    12198 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_reflect_line.py
--rw-rw-rw-   0        0        0    13300 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_revol.py
--rw-rw-rw-   0        0        0     9306 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_rolling_offset.py
--rw-rw-rw-   0        0        0    15353 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_rotate.py
--rw-rw-rw-   0        0        0     8015 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_scaling.py
--rw-rw-rw-   0        0        0     2752 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_section.py
--rw-rw-rw-   0        0        0    12625 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sphere.py
--rw-rw-rw-   0        0        0    18797 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spine.py
--rw-rw-rw-   0        0        0    11384 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spiral.py
--rw-rw-rw-   0        0        0    42885 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spline.py
--rw-rw-rw-   0        0        0    29811 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_split.py
--rw-rw-rw-   0        0        0     1536 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_surface_explicit.py
--rw-rw-rw-   0        0        0     8821 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep.py
--rw-rw-rw-   0        0        0    48206 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_circle.py
--rw-rw-rw-   0        0        0    36668 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_conic.py
--rw-rw-rw-   0        0        0    61549 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_explicit.py
--rw-rw-rw-   0        0        0    83811 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_line.py
--rw-rw-rw-   0        0        0     6611 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_symmetry.py
--rw-rw-rw-   0        0        0     6239 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_thickness.py
--rw-rw-rw-   0        0        0     5664 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_transfer.py
--rw-rw-rw-   0        0        0    15253 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_translate.py
--rw-rw-rw-   0        0        0    41726 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_trim.py
--rw-rw-rw-   0        0        0    18247 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_unfold.py
--rw-rw-rw-   0        0        0     1529 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_volume_explicit.py
--rw-rw-rw-   0        0        0    25152 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_curve.py
--rw-rw-rw-   0        0        0     6152 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_surface.py
--rw-rw-rw-   0        0        0     9447 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/line.py
--rw-rw-rw-   0        0        0    15721 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/plane.py
--rw-rw-rw-   0        0        0     4397 2024-04-22 07:18:08.000000 pycatia-0.6.8/pycatia/hybrid_shape_interfaces/point.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.427235 pycatia-0.6.8/pycatia/in_interfaces/
--rw-rw-rw-   0        0        0       21 2022-04-12 12:15:17.000000 pycatia-0.6.8/pycatia/in_interfaces/__init__.py
--rw-rw-rw-   0        0        0    44342 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/in_interfaces/application.py
--rw-rw-rw-   0        0        0     2526 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/camera.py
--rw-rw-rw-   0        0        0     2750 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/camera_2d.py
--rw-rw-rw-   0        0        0     2788 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/in_interfaces/camera_3d.py
--rw-rw-rw-   0        0        0     6518 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/cameras.py
--rw-rw-rw-   0        0        0    15339 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/cgr_adhesion_setting_att.py
--rw-rw-rw-   0        0        0    35762 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/in_interfaces/document.py
--rw-rw-rw-   0        0        0    18815 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/documentation_setting_att.py
--rw-rw-rw-   0        0        0    13040 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/documents.py
--rw-rw-rw-   0        0        0     4496 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/drafting_page_setup.py
--rw-rw-rw-   0        0        0     4029 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/file.py
--rw-rw-rw-   0        0        0     3238 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/file_component.py
--rw-rw-rw-   0        0        0    18372 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/file_system.py
--rw-rw-rw-   0        0        0     3353 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/files.py
--rw-rw-rw-   0        0        0     3070 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/folder.py
--rw-rw-rw-   0        0        0     3456 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/folders.py
--rw-rw-rw-   0        0        0    23020 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/general_session_setting_att.py
--rw-rw-rw-   0        0        0     4964 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/light_source.py
--rw-rw-rw-   0        0        0     5202 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/light_sources.py
--rw-rw-rw-   0        0        0    17013 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/macros_setting_att.py
--rw-rw-rw-   0        0        0     5189 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/move.py
--rw-rw-rw-   0        0        0     1524 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/in_interfaces/page_setup.py
--rw-rw-rw-   0        0        0     6667 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/position.py
--rw-rw-rw-   0        0        0     5030 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/printer.py
--rw-rw-rw-   0        0        0     3408 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/printers.py
--rw-rw-rw-   0        0        0    32920 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/printers_setting_att.py
--rw-rw-rw-   0        0        0     3855 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/reference.py
--rw-rw-rw-   0        0        0     3391 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/references.py
--rw-rw-rw-   0        0        0    21443 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/search_setting_att.py
--rw-rw-rw-   0        0        0    14907 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/selected_element.py
--rw-rw-rw-   0        0        0   120206 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/selection.py
--rw-rw-rw-   0        0        0     8395 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/selection_sets.py
--rw-rw-rw-   0        0        0    16122 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/send_to_service.py
--rw-rw-rw-   0        0        0     2870 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/setting_controllers.py
--rw-rw-rw-   0        0        0     3841 2023-10-31 11:15:13.000000 pycatia-0.6.8/pycatia/in_interfaces/specs_and_geom_window.py
--rw-rw-rw-   0        0        0     2617 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/specs_viewer.py
--rw-rw-rw-   0        0        0     7920 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/system_configuration.py
--rw-rw-rw-   0        0        0     6466 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/text_stream.py
--rw-rw-rw-   0        0        0    37903 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/tree_viz_manip_setting_att.py
--rw-rw-rw-   0        0        0    12781 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/in_interfaces/viewer.py
--rw-rw-rw-   0        0        0     2328 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/viewer_2d.py
--rw-rw-rw-   0        0        0    15660 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/in_interfaces/viewer_3d.py
--rw-rw-rw-   0        0        0     3400 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/viewers.py
--rw-rw-rw-   0        0        0     5770 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/viewpoint_2d.py
--rw-rw-rw-   0        0        0    15085 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/in_interfaces/viewpoint_3d.py
--rw-rw-rw-   0        0        0    45275 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/vis_property_set.py
--rw-rw-rw-   0        0        0   236225 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/visualization_setting_att.py
--rw-rw-rw-   0        0        0    31699 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/vrml_setting_att.py
--rw-rw-rw-   0        0        0    14902 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/in_interfaces/window.py
--rw-rw-rw-   0        0        0     4413 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/in_interfaces/windows.py
--rw-rw-rw-   0        0        0     1411 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/in_interfaces/workbench.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.442210 pycatia-0.6.8/pycatia/kinematics_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/__init__.py
--rw-rw-rw-   0        0        0     9162 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/dressup.py
--rw-rw-rw-   0        0        0     9843 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/dressups.py
--rw-rw-rw-   0        0        0     4495 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/joint.py
--rw-rw-rw-   0        0        0     5984 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/joints.py
--rw-rw-rw-   0        0        0     2407 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/kinematics_workbench.py
--rw-rw-rw-   0        0        0    18786 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/mechanism.py
--rw-rw-rw-   0        0        0     3544 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/mechanism_command.py
--rw-rw-rw-   0        0        0     6722 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/mechanism_commands.py
--rw-rw-rw-   0        0        0     6308 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/kinematics_interfaces/mechanisms.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.508217 pycatia-0.6.8/pycatia/knowledge_interfaces/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1927 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/angle.py
--rw-rw-rw-   0        0        0     2690 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/bool_param.py
--rw-rw-rw-   0        0        0     3421 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/check.py
--rw-rw-rw-   0        0        0     1953 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/constraint_satisfaction.py
--rw-rw-rw-   0        0        0     9573 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/design_table.py
--rw-rw-rw-   0        0        0     3498 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/dimension.py
--rw-rw-rw-   0        0        0     2343 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/enum_param.py
--rw-rw-rw-   0        0        0     4544 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/feature_generator.py
--rw-rw-rw-   0        0        0     2958 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/formula.py
--rw-rw-rw-   0        0        0     4000 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/free_parameter.py
--rw-rw-rw-   0        0        0     4638 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/free_parameters.py
--rw-rw-rw-   0        0        0    10652 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/int_param.py
--rw-rw-rw-   0        0        0     3767 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/knowledge_activate_object.py
--rw-rw-rw-   0        0        0     2397 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/knowledge_object.py
--rw-rw-rw-   0        0        0    39344 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/knowledge_sheet_setting_att.py
--rw-rw-rw-   0        0        0    14348 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/language_sheet_setting_att.py
--rw-rw-rw-   0        0        0     2853 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/law.py
--rw-rw-rw-   0        0        0     2040 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/length.py
--rw-rw-rw-   0        0        0     6890 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/list.py
--rw-rw-rw-   0        0        0     1743 2023-10-31 11:15:14.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/list_parameter.py
--rw-rw-rw-   0        0        0     1479 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/loop.py
--rw-rw-rw-   0        0        0    11560 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/optimization.py
--rw-rw-rw-   0        0        0     3504 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/optimization_constraint.py
--rw-rw-rw-   0        0        0     5210 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/optimization_constraints.py
--rw-rw-rw-   0        0        0     5475 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/optimizations.py
--rw-rw-rw-   0        0        0    12872 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/parameter.py
--rw-rw-rw-   0        0        0     3086 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/parameter_set.py
--rw-rw-rw-   0        0        0     4887 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/parameter_sets.py
--rw-rw-rw-   0        0        0    22463 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/parameters.py
--rw-rw-rw-   0        0        0    14637 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/real_param.py
--rw-rw-rw-   0        0        0     9594 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/relation.py
--rw-rw-rw-   0        0        0    26399 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/relations.py
--rw-rw-rw-   0        0        0    50792 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/report_generation_sheet_setting_att.py
--rw-rw-rw-   0        0        0     2647 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/rule.py
--rw-rw-rw-   0        0        0    10875 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/set_of_equation.py
--rw-rw-rw-   0        0        0     6820 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/str_param.py
--rw-rw-rw-   0        0        0    25272 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/tolerance_sheet_setting_att.py
--rw-rw-rw-   0        0        0     5525 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/unit.py
--rw-rw-rw-   0        0        0     3193 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/units.py
--rw-rw-rw-   0        0        0    32738 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/knowledge_interfaces/units_sheet_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.568729 pycatia-0.6.8/pycatia/manufacturing_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/__init__.py
--rw-rw-rw-   0        0        0    11810 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/machining_process.py
--rw-rw-rw-   0        0        0     5064 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_activities.py
--rw-rw-rw-   0        0        0    22355 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_activity.py
--rw-rw-rw-   0        0        0     2559 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_activity_syntax.py
--rw-rw-rw-   0        0        0     1780 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_activity_syntax2.py
--rw-rw-rw-   0        0        0     1501 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_apt_generator.py
--rw-rw-rw-   0        0        0    12195 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_copy_transformation.py
--rw-rw-rw-   0        0        0     2104 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_factories.py
--rw-rw-rw-   0        0        0     2501 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_feature.py
--rw-rw-rw-   0        0        0     3127 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_features.py
--rw-rw-rw-   0        0        0    16648 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_generator_data.py
--rw-rw-rw-   0        0        0     5055 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_hole.py
--rw-rw-rw-   0        0        0     8059 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_insert.py
--rw-rw-rw-   0        0        0    18105 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machinable_area.py
--rw-rw-rw-   0        0        0     4081 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machinable_feature.py
--rw-rw-rw-   0        0        0    36090 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machinable_geometry.py
--rw-rw-rw-   0        0        0    24584 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machine.py
--rw-rw-rw-   0        0        0    14731 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machining_axis.py
--rw-rw-rw-   0        0        0    79105 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_operation.py
--rw-rw-rw-   0        0        0     7207 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_output.py
--rw-rw-rw-   0        0        0    11452 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_output_generator.py
--rw-rw-rw-   0        0        0    21291 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_pattern.py
--rw-rw-rw-   0        0        0     2467 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_precedence.py
--rw-rw-rw-   0        0        0     4868 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_precedences.py
--rw-rw-rw-   0        0        0     2123 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_process.py
--rw-rw-rw-   0        0        0    25894 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_program.py
--rw-rw-rw-   0        0        0     2560 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_resource_factory.py
--rw-rw-rw-   0        0        0    50976 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_setup.py
--rw-rw-rw-   0        0        0     2508 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_setup2.py
--rw-rw-rw-   0        0        0     2631 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_setup3.py
--rw-rw-rw-   0        0        0    16460 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool.py
--rw-rw-rw-   0        0        0    13545 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_assembly.py
--rw-rw-rw-   0        0        0     2960 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_assembly2.py
--rw-rw-rw-   0        0        0     5907 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_corrector.py
--rw-rw-rw-   0        0        0    11361 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_motion.py
--rw-rw-rw-   0        0        0     4056 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_motions.py
--rw-rw-rw-   0        0        0     2146 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_user_representation.py
--rw-rw-rw-   0        0        0     5236 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_view.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.643284 pycatia-0.6.8/pycatia/mec_mod_interfaces/
--rw-rw-rw-   0        0        0       21 2022-04-12 12:15:17.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/__init__.py
--rw-rw-rw-   0        0        0    41134 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/axis_system.py
--rw-rw-rw-   0        0        0     4569 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/axis_systems.py
--rw-rw-rw-   0        0        0     3400 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/bi_dim_feat_edge.py
--rw-rw-rw-   0        0        0     4327 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/bodies.py
--rw-rw-rw-   0        0        0     9221 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/body.py
--rw-rw-rw-   0        0        0     5009 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/boundary.py
--rw-rw-rw-   0        0        0    25561 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/constraint.py
--rw-rw-rw-   0        0        0    12572 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/constraints.py
--rw-rw-rw-   0        0        0     6074 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/cylindrical_face.py
--rw-rw-rw-   0        0        0     3567 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/edge.py
--rw-rw-rw-   0        0        0     3144 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/face.py
--rw-rw-rw-   0        0        0     1206 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/factory.py
--rw-rw-rw-   0        0        0    12845 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/fix_together.py
--rw-rw-rw-   0        0        0     5880 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/fix_togethers.py
--rw-rw-rw-   0        0        0     3883 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/geometric_elements.py
--rw-rw-rw-   0        0        0     4868 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_bodies.py
--rw-rw-rw-   0        0        0     8830 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_body.py
--rw-rw-rw-   0        0        0     4473 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_shape.py
--rw-rw-rw-   0        0        0    15797 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_shape_instance.py
--rw-rw-rw-   0        0        0     4496 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_shapes.py
--rw-rw-rw-   0        0        0    16415 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/instance_factory.py
--rw-rw-rw-   0        0        0     2060 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/mono_dim_feat_edge.py
--rw-rw-rw-   0        0        0     2249 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/not_wire_boundary_mono_dim_feat_vertex.py
--rw-rw-rw-   0        0        0     7987 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/ordered_geometrical_set.py
--rw-rw-rw-   0        0        0     5249 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/ordered_geometrical_sets.py
--rw-rw-rw-   0        0        0     3835 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/origin_elements.py
--rw-rw-rw-   0        0        0    35366 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/part.py
--rw-rw-rw-   0        0        0     3350 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/part_document.py
--rw-rw-rw-   0        0        0   228006 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/part_infrastructure_setting_att.py
--rw-rw-rw-   0        0        0     9106 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/planar_face.py
--rw-rw-rw-   0        0        0     5802 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/rectilinear_bi_dim_feat_edge.py
--rw-rw-rw-   0        0        0     5880 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/rectilinear_mono_dim_feat_edge.py
--rw-rw-rw-   0        0        0     7577 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/rectilinear_tri_dim_feat_edge.py
--rw-rw-rw-   0        0        0     1455 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/shape.py
--rw-rw-rw-   0        0        0    15513 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/shape_instance.py
--rw-rw-rw-   0        0        0     4205 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/shapes.py
--rw-rw-rw-   0        0        0     5520 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/sketches.py
--rw-rw-rw-   0        0        0     4615 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/solid.py
--rw-rw-rw-   0        0        0     2895 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/tri_dim_feat_edge.py
--rw-rw-rw-   0        0        0     2121 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/tri_dim_feat_vertex_or_bi_dim_feat_vertex.py
--rw-rw-rw-   0        0        0     3661 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/vertex.py
--rw-rw-rw-   0        0        0     2201 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/mec_mod_interfaces/zero_dim_feat_vertex_or_wire_boundary_mono_dim_feat_vertex.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.646286 pycatia-0.6.8/pycatia/multi_cad_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/multi_cad_interfaces/__init__.py
--rw-rw-rw-   0        0        0    77496 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/multi_cad_interfaces/multi_cad_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.675284 pycatia-0.6.8/pycatia/navigator_interfaces/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.6.8/pycatia/navigator_interfaces/__init__.py
--rw-rw-rw-   0        0        0    16753 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/navigator_interfaces/annotated_view.py
--rw-rw-rw-   0        0        0     7991 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/navigator_interfaces/annotated_views.py
--rw-rw-rw-   0        0        0     5860 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/navigator_interfaces/dmu_data_flow.py
--rw-rw-rw-   0        0        0     3392 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/navigator_interfaces/dmu_review.py
--rw-rw-rw-   0        0        0     8226 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/navigator_interfaces/dmu_reviews.py
--rw-rw-rw-   0        0        0    15462 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/navigator_interfaces/group.py
--rw-rw-rw-   0        0        0     7702 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/navigator_interfaces/groups.py
--rw-rw-rw-   0        0        0     5397 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/navigator_interfaces/hyperlink.py
--rw-rw-rw-   0        0        0     7680 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/navigator_interfaces/hyperlinks.py
--rw-rw-rw-   0        0        0    16990 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/navigator_interfaces/marker_2D.py
--rw-rw-rw-   0        0        0    18553 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/navigator_interfaces/marker_2Ds.py
--rw-rw-rw-   0        0        0    21192 2023-10-31 11:15:15.000000 pycatia-0.6.8/pycatia/navigator_interfaces/marker_3D.py
--rw-rw-rw-   0        0        0     8999 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/navigator_interfaces/marker_3Ds.py
--rw-rw-rw-   0        0        0    70516 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/navigator_interfaces/marker_setting_att.py
--rw-rw-rw-   0        0        0   194067 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/navigator_interfaces/n_4D_navigator_setting_att.py
--rw-rw-rw-   0        0        0    15253 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/navigator_interfaces/navigator_workbench.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.686284 pycatia-0.6.8/pycatia/osm_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/osm_interfaces/__init__.py
--rw-rw-rw-   0        0        0     6467 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/osm_interfaces/product_scene.py
--rw-rw-rw-   0        0        0     8382 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/osm_interfaces/product_scenes.py
--rw-rw-rw-   0        0        0    15967 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/osm_interfaces/scene.py
--rw-rw-rw-   0        0        0    11312 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/osm_interfaces/scene_product_data.py
--rw-rw-rw-   0        0        0     2302 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/osm_interfaces/scene_workbench.py
--rw-rw-rw-   0        0        0     5879 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/osm_interfaces/scenes.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.806809 pycatia-0.6.8/pycatia/part_interfaces/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.6.8/pycatia/part_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/add.py
--rw-rw-rw-   0        0        0     3056 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/affinity.py
--rw-rw-rw-   0        0        0     3429 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/angular_repartition.py
--rw-rw-rw-   0        0        0     1542 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/assemble.py
--rw-rw-rw-   0        0        0     7032 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/part_interfaces/auto_draft.py
--rw-rw-rw-   0        0        0    11198 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/part_interfaces/auto_fillet.py
--rw-rw-rw-   0        0        0     3100 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/axis_to_axis.py
--rw-rw-rw-   0        0        0     4941 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/boolean_shape.py
--rw-rw-rw-   0        0        0    12608 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/chamfer.py
--rw-rw-rw-   0        0        0    20985 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/circ_pattern.py
--rw-rw-rw-   0        0        0    20843 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/close_surface.py
--rw-rw-rw-   0        0        0     7727 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/const_rad_edge_fillet.py
--rw-rw-rw-   0        0        0     2876 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/defeaturing.py
--rw-rw-rw-   0        0        0     1450 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/defeaturing_fillet_filter.py
--rw-rw-rw-   0        0        0     1220 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/defeaturing_filter.py
--rw-rw-rw-   0        0        0    16213 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/defeaturing_filter_with_range.py
--rw-rw-rw-   0        0        0     5861 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/part_interfaces/defeaturing_filters.py
--rw-rw-rw-   0        0        0     1440 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/defeaturing_hole_filter.py
--rw-rw-rw-   0        0        0     4428 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/draft.py
--rw-rw-rw-   0        0        0    17421 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/draft_domain.py
--rw-rw-rw-   0        0        0     3318 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/part_interfaces/draft_domains.py
--rw-rw-rw-   0        0        0     1559 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/dress_up_shape.py
--rw-rw-rw-   0        0        0     8016 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/edge_fillet.py
--rw-rw-rw-   0        0        0     4556 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/face_fillet.py
--rw-rw-rw-   0        0        0     4292 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/fillet.py
--rw-rw-rw-   0        0        0     1679 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/groove.py
--rw-rw-rw-   0        0        0    29826 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/hole.py
--rw-rw-rw-   0        0        0     2066 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/intersect.py
--rw-rw-rw-   0        0        0     3436 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/limit.py
--rw-rw-rw-   0        0        0     2599 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/linear_repartition.py
--rw-rw-rw-   0        0        0     2427 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/loft.py
--rw-rw-rw-   0        0        0     3339 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/mirror.py
--rw-rw-rw-   0        0        0     1565 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/pad.py
--rw-rw-rw-   0        0        0     5399 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/pattern.py
--rw-rw-rw-   0        0        0     1658 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/pocket.py
--rw-rw-rw-   0        0        0    15979 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/prism.py
--rw-rw-rw-   0        0        0    22607 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/rect_pattern.py
--rw-rw-rw-   0        0        0     1399 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/remove.py
--rw-rw-rw-   0        0        0     7521 2024-04-22 07:43:43.000000 pycatia-0.6.8/pycatia/part_interfaces/remove_face.py
--rw-rw-rw-   0        0        0     2246 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/repartition.py
--rw-rw-rw-   0        0        0     6879 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/replace_face.py
--rw-rw-rw-   0        0        0     8493 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/revolution.py
--rw-rw-rw-   0        0        0     1588 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/rib.py
--rw-rw-rw-   0        0        0     5134 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/rotate.py
--rw-rw-rw-   0        0        0     3573 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/scaling.py
--rw-rw-rw-   0        0        0     4394 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/scaling2.py
--rw-rw-rw-   0        0        0    10154 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/sew_surface.py
--rw-rw-rw-   0        0        0     1671 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/shaft.py
--rw-rw-rw-   0        0        0   160466 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/part_interfaces/shape_factory.py
--rw-rw-rw-   0        0        0    13547 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/shell.py
--rw-rw-rw-   0        0        0     3690 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/sketch_based_shape.py
--rw-rw-rw-   0        0        0     1677 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/slot.py
--rw-rw-rw-   0        0        0     6417 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/solid_combine.py
--rw-rw-rw-   0        0        0     2701 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/split.py
--rw-rw-rw-   0        0        0     7217 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/stiffener.py
--rw-rw-rw-   0        0        0     2155 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/surface_based_shape.py
--rw-rw-rw-   0        0        0    12355 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/sweep.py
--rw-rw-rw-   0        0        0     2746 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/symmetry.py
--rw-rw-rw-   0        0        0     4776 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/thick_surface.py
--rw-rw-rw-   0        0        0    12437 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/thickness.py
--rw-rw-rw-   0        0        0    12759 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/thread.py
--rw-rw-rw-   0        0        0     1609 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/part_interfaces/transformation_shape.py
--rw-rw-rw-   0        0        0     2817 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/translate.py
--rw-rw-rw-   0        0        0    18816 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/trim.py
--rw-rw-rw-   0        0        0     5254 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/tritangent_fillet.py
--rw-rw-rw-   0        0        0     4375 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/user_pattern.py
--rw-rw-rw-   0        0        0     3530 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/user_repartition.py
--rw-rw-rw-   0        0        0    16057 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/part_interfaces/var_rad_edge_fillet.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.819828 pycatia-0.6.8/pycatia/pcb_board_base/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/pcb_board_base/__init__.py
--rw-rw-rw-   0        0        0     6487 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/pcb_board_base/pcb_area.py
--rw-rw-rw-   0        0        0    12427 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/pcb_board_base/pcb_board.py
--rw-rw-rw-   0        0        0     8570 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/pcb_board_base/pcb_component.py
--rw-rw-rw-   0        0        0     5251 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/pcb_board_base/pcb_hole_and_pattern.py
--rw-rw-rw-   0        0        0     2786 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/pcb_board_base/pcb_object.py
--rw-rw-rw-   0        0        0     6278 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/pcb_board_base/pcb_workbench.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.828339 pycatia-0.6.8/pycatia/ppr_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/ppr_interfaces/__init__.py
--rw-rw-rw-   0        0        0     3301 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/ppr_interfaces/ppr_activity.py
--rw-rw-rw-   0        0        0     4201 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/ppr_interfaces/ppr_document.py
--rw-rw-rw-   0        0        0     2989 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/ppr_interfaces/ppr_products.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.832338 pycatia-0.6.8/pycatia/prismatic_machining_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/prismatic_machining_interfaces/__init__.py
--rw-rw-rw-   0        0        0    28065 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/prismatic_machining_interfaces/manufacturing_prismatic_machining_area.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.847340 pycatia-0.6.8/pycatia/product_structure_interfaces/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/product_structure_interfaces/__init__.py
--rw-rw-rw-   0        0        0     8618 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/product_structure_interfaces/analyze.py
--rw-rw-rw-   0        0        0     4851 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/product_structure_interfaces/assembly_convertor.py
--rw-rw-rw-   0        0        0    55459 2024-01-17 11:05:50.000000 pycatia-0.6.8/pycatia/product_structure_interfaces/product.py
--rw-rw-rw-   0        0        0     2726 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/product_structure_interfaces/product_document.py
--rw-rw-rw-   0        0        0    17080 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/product_structure_interfaces/products.py
--rw-rw-rw-   0        0        0     3536 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/product_structure_interfaces/publication.py
--rw-rw-rw-   0        0        0     9888 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/product_structure_interfaces/publications.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.850339 pycatia-0.6.8/pycatia/reporter_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/reporter_interfaces/__init__.py
--rw-rw-rw-   0        0        0     2913 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/reporter_interfaces/rpm_report.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.858338 pycatia-0.6.8/pycatia/scripts/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/scripts/__init__.py
--rw-rw-rw-   0        0        0      388 2022-04-12 12:15:17.000000 pycatia-0.6.8/pycatia/scripts/checking.py
--rw-rw-rw-   0        0        0     2916 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/scripts/csv_tools.py
--rw-rw-rw-   0        0        0      991 2023-05-01 08:46:40.000000 pycatia-0.6.8/pycatia/scripts/document_types.py
--rw-rw-rw-   0        0        0      289 2024-04-22 07:18:56.000000 pycatia-0.6.8/pycatia/scripts/vba.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.861338 pycatia-0.6.8/pycatia/simulation_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/simulation_interfaces/__init__.py
--rw-rw-rw-   0        0        0     9391 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/simulation_interfaces/replay.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.885339 pycatia-0.6.8/pycatia/sketcher_interfaces/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/__init__.py
--rw-rw-rw-   0        0        0     2778 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/axis_2D.py
--rw-rw-rw-   0        0        0     5198 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/circle_2D.py
--rw-rw-rw-   0        0        0     5365 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/control_point_2D.py
--rw-rw-rw-   0        0        0    17189 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/curve_2D.py
--rw-rw-rw-   0        0        0     8690 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/ellipse_2D.py
--rw-rw-rw-   0        0        0    20597 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/factory_2D.py
--rw-rw-rw-   0        0        0     1879 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/geometric_element.py
--rw-rw-rw-   0        0        0     2614 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/geometry_2D.py
--rw-rw-rw-   0        0        0     6669 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/hyperbola_2D.py
--rw-rw-rw-   0        0        0     5130 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/line_2D.py
--rw-rw-rw-   0        0        0     5831 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/parabola_2D.py
--rw-rw-rw-   0        0        0     3186 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/point_2D.py
--rw-rw-rw-   0        0        0    13438 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/sketch.py
--rw-rw-rw-   0        0        0     5320 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/sketcher_interfaces/spline_2D.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.917853 pycatia-0.6.8/pycatia/smt_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/smt_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1281 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/smt_interfaces/dmo_offset.py
--rw-rw-rw-   0        0        0    13612 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/dmo_offsets.py
--rw-rw-rw-   0        0        0     1296 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/smt_interfaces/dmo_thickness.py
--rw-rw-rw-   0        0        0    12803 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/dmo_thicknesses.py
--rw-rw-rw-   0        0        0     3051 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/free_space.py
--rw-rw-rw-   0        0        0     9863 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/free_spaces.py
--rw-rw-rw-   0        0        0     3901 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/merges.py
--rw-rw-rw-   0        0        0     6882 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/optimizer_work_bench.py
--rw-rw-rw-   0        0        0     1168 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/smt_interfaces/part_comp.py
--rw-rw-rw-   0        0        0     6318 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/part_comps.py
--rw-rw-rw-   0        0        0     1290 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/smt_interfaces/silhouette.py
--rw-rw-rw-   0        0        0     8446 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/silhouettes.py
--rw-rw-rw-   0        0        0     4739 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/simplifications.py
--rw-rw-rw-   0        0        0     1295 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/smt_interfaces/swept_volume.py
--rw-rw-rw-   0        0        0    25945 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/swept_volumes.py
--rw-rw-rw-   0        0        0    14549 2024-01-13 13:43:56.000000 pycatia-0.6.8/pycatia/smt_interfaces/three_d_cuts.py
--rw-rw-rw-   0        0        0    10615 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/vibration_volumes.py
--rw-rw-rw-   0        0        0     1282 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/smt_interfaces/wrapping.py
--rw-rw-rw-   0        0        0     8534 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/smt_interfaces/wrappings.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.947853 pycatia-0.6.8/pycatia/space_analyses_interfaces/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/__init__.py
--rw-rw-rw-   0        0        0    12149 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/clash.py
--rw-rw-rw-   0        0        0     3358 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/clash_result.py
--rw-rw-rw-   0        0        0     7004 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/clash_results.py
--rw-rw-rw-   0        0        0     6697 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/clashes.py
--rw-rw-rw-   0        0        0    11514 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/conflict.py
--rw-rw-rw-   0        0        0     3119 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/conflicts.py
--rw-rw-rw-   0        0        0    19991 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/distance.py
--rw-rw-rw-   0        0        0     7026 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/distances.py
--rw-rw-rw-   0        0        0      227 2022-04-12 12:15:17.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/general_functions.py
--rw-rw-rw-   0        0        0    14289 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/inertia.py
--rw-rw-rw-   0        0        0     6456 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/inertias.py
--rw-rw-rw-   0        0        0    25428 2024-02-22 13:04:44.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/measurable.py
--rw-rw-rw-   0        0        0    28190 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/measure_setting_att.py
--rw-rw-rw-   0        0        0    20050 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/section.py
--rw-rw-rw-   0        0        0    80468 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/sectioning_setting_att.py
--rw-rw-rw-   0        0        0     6942 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/sections.py
--rw-rw-rw-   0        0        0     7946 2023-11-08 17:25:46.000000 pycatia-0.6.8/pycatia/space_analyses_interfaces/spa_workbench.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.989853 pycatia-0.6.8/pycatia/structure_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/structure_interfaces/__init__.py
--rw-rw-rw-   0        0        0    11665 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/structure_interfaces/colour_ess_object_setting_att.py
--rw-rw-rw-   0        0        0    11489 2023-10-31 11:15:16.000000 pycatia-0.6.8/pycatia/structure_interfaces/colour_std_object_setting_att.py
--rw-rw-rw-   0        0        0    10128 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/material_ess_object_setting_att.py
--rw-rw-rw-   0        0        0    14843 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/path_ess_resources_setting_att.py
--rw-rw-rw-   0        0        0     7880 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/ppg_exec_log_setting_att.py
--rw-rw-rw-   0        0        0     3104 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_anchor_point.py
--rw-rw-rw-   0        0        0     2854 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_anchor_points.py
--rw-rw-rw-   0        0        0     7688 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_compute_services.py
--rw-rw-rw-   0        0        0     2582 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_cutback.py
--rw-rw-rw-   0        0        0     7760 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_cutout_feature.py
--rw-rw-rw-   0        0        0    19179 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_feature_factory.py
--rw-rw-rw-   0        0        0     1308 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_foundation.py
--rw-rw-rw-   0        0        0     4172 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_foundations.py
--rw-rw-rw-   0        0        0    11499 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_member.py
--rw-rw-rw-   0        0        0     8265 2023-10-31 11:15:17.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_member_extremity.py
--rw-rw-rw-   0        0        0     9768 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_members.py
--rw-rw-rw-   0        0        0     4980 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_nibbling_feature.py
--rw-rw-rw-   0        0        0     2036 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_object.py
--rw-rw-rw-   0        0        0     1261 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_object_ext.py
--rw-rw-rw-   0        0        0    72345 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_object_factory.py
--rw-rw-rw-   0        0        0     4672 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_plate.py
--rw-rw-rw-   0        0        0     9555 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_plates.py
--rw-rw-rw-   0        0        0     7056 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_section.py
--rw-rw-rw-   0        0        0     2206 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/str_workbench.py
--rw-rw-rw-   0        0        0     9938 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/structure_interfaces/type_ess_object_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:02.994853 pycatia-0.6.8/pycatia/surface_machining_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/surface_machining_interfaces/__init__.py
--rw-rw-rw-   0        0        0     3831 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/surface_machining_interfaces/manufacturing_surface_geom_area.py
--rw-rw-rw-   0        0        0     4841 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/surface_machining_interfaces/manufacturing_surface_machining_area.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:03.034916 pycatia-0.6.8/pycatia/system_interfaces/
--rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.8/pycatia/system_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1915 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/accesslog_statistics_setting_att.py
--rw-rw-rw-   0        0        0     7643 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/system_interfaces/any_object.py
--rw-rw-rw-   0        0        0    28964 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/cache_setting_att.py
--rw-rw-rw-   0        0        0     1666 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/cat_base_dispatch.py
--rw-rw-rw-   0        0        0     1530 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/cat_base_unknown.py
--rw-rw-rw-   0        0        0     8774 2024-03-17 16:28:56.000000 pycatia-0.6.8/pycatia/system_interfaces/collection.py
--rw-rw-rw-   0        0        0     1901 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/command_statistics_setting_att.py
--rw-rw-rw-   0        0        0     7521 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/disconnection_setting_att.py
--rw-rw-rw-   0        0        0    23652 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/dl_name_setting_att.py
--rw-rw-rw-   0        0        0    12275 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/dyn_license_setting_att.py
--rw-rw-rw-   0        0        0     9646 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/errorlog_statistics_setting_att.py
--rw-rw-rw-   0        0        0     1920 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/file_access_statistics_setting_att.py
--rw-rw-rw-   0        0        0    21080 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/general_statistics_setting_att.py
--rw-rw-rw-   0        0        0     7896 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/global_statistics_setting_att.py
--rw-rw-rw-   0        0        0     1257 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/i_dispatch.py
--rw-rw-rw-   0        0        0     1147 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/i_unknown.py
--rw-rw-rw-   0        0        0    29377 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/license_setting_att.py
--rw-rw-rw-   0        0        0    10573 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/memory_warning_setting_att.py
--rw-rw-rw-   0        0        0     2732 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/pcs_statistics_setting_att.py
--rw-rw-rw-   0        0        0     1895 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/server_statistics_setting_att.py
--rw-rw-rw-   0        0        0     1901 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/session_statistics_setting_att.py
--rw-rw-rw-   0        0        0    12823 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/setting_controller.py
--rw-rw-rw-   0        0        0    13615 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/setting_repository.py
--rw-rw-rw-   0        0        0    12861 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/system_interfaces/system_service.py
--rw-rw-rw-   0        0        0     1914 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/system_interfaces/workbench_statistics_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:03.036916 pycatia-0.6.8/pycatia/threed_xml_interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.8/pycatia/threed_xml_interfaces/__init__.py
--rw-rw-rw-   0        0        0    61791 2023-10-31 11:15:18.000000 pycatia-0.6.8/pycatia/threed_xml_interfaces/export_3d_xml_setting_att.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:03.041916 pycatia-0.6.8/pycatia/types/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.6.8/pycatia/types/__init__.py
--rw-rw-rw-   0        0        0      584 2022-11-18 10:48:10.000000 pycatia-0.6.8/pycatia/types/document_types.py
--rw-rw-rw-   0        0        0      566 2024-02-26 15:55:40.000000 pycatia-0.6.8/pycatia/types/general.py
--rw-rw-rw-   0        0        0       19 2024-04-22 07:25:19.000000 pycatia-0.6.8/pycatia/version.py
-drwxrwxrwx   0        0        0        0 2024-04-22 07:59:03.042916 pycatia-0.6.8/pycatia.egg-info/
--rw-rw-rw-   0        0        0     5167 2024-04-22 07:59:00.000000 pycatia-0.6.8/pycatia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    62668 2024-04-22 07:59:00.000000 pycatia-0.6.8/pycatia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 07:59:00.000000 pycatia-0.6.8/pycatia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-22 07:59:00.000000 pycatia-0.6.8/pycatia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 07:59:00.000000 pycatia-0.6.8/pycatia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 07:59:03.045916 pycatia-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-05-01 08:31:08.000000 pycatia-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.550163 pycatia-0.6.9/
+-rw-rw-rw-   0        0        0     1087 2022-04-12 12:15:17.000000 pycatia-0.6.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     5291 2024-05-20 10:16:47.549156 pycatia-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4736 2024-04-25 14:24:32.000000 pycatia-0.6.9/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.335749 pycatia-0.6.9/pycatia/
+-rw-rw-rw-   0        0        0      940 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.469234 pycatia-0.6.9/pycatia/abq_automation_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     7247 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_analysis_case.py
+-rw-rw-rw-   0        0        0     7127 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_analysis_cases.py
+-rw-rw-rw-   0        0        0     3612 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_analysis_model.py
+-rw-rw-rw-   0        0        0    10496 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_analytical_rigid_surface.py
+-rw-rw-rw-   0        0        0    13529 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_boundary_condition.py
+-rw-rw-rw-   0        0        0     6882 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_boundary_conditions.py
+-rw-rw-rw-   0        0        0     1518 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_clamp_bc.py
+-rw-rw-rw-   0        0        0    19646 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_concentrated_force.py
+-rw-rw-rw-   0        0        0    16925 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_damper_connection_property.py
+-rw-rw-rw-   0        0        0     4366 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_data_output_request.py
+-rw-rw-rw-   0        0        0     6449 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_data_output_requests.py
+-rw-rw-rw-   0        0        0    16748 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_displacement_bc.py
+-rw-rw-rw-   0        0        0     1330 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_display_group.py
+-rw-rw-rw-   0        0        0     2810 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_display_groups.py
+-rw-rw-rw-   0        0        0    12560 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_explicit_dynamics_step.py
+-rw-rw-rw-   0        0        0     8364 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_fastened_connection_enhancement.py
+-rw-rw-rw-   0        0        0    12203 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_fastened_pair.py
+-rw-rw-rw-   0        0        0     1699 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_field_output_request.py
+-rw-rw-rw-   0        0        0     6530 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_field_output_requests.py
+-rw-rw-rw-   0        0        0     6939 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_fields.py
+-rw-rw-rw-   0        0        0    12762 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_film_condition.py
+-rw-rw-rw-   0        0        0    16327 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_frequency_step.py
+-rw-rw-rw-   0        0        0     6013 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_gasket_property.py
+-rw-rw-rw-   0        0        0    14560 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_general_static_step.py
+-rw-rw-rw-   0        0        0    11326 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_global_element_assignment.py
+-rw-rw-rw-   0        0        0     9341 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_gravity.py
+-rw-rw-rw-   0        0        0    12407 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_heat_transfer_step.py
+-rw-rw-rw-   0        0        0     1713 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_history_output_request.py
+-rw-rw-rw-   0        0        0     6702 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_history_output_requests.py
+-rw-rw-rw-   0        0        0     8678 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_image_query.py
+-rw-rw-rw-   0        0        0     3288 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_initial_step.py
+-rw-rw-rw-   0        0        0     2098 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_initial_temperature.py
+-rw-rw-rw-   0        0        0     1847 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_interaction.py
+-rw-rw-rw-   0        0        0     6729 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_interactions.py
+-rw-rw-rw-   0        0        0    34962 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_job.py
+-rw-rw-rw-   0        0        0     5415 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_jobs.py
+-rw-rw-rw-   0        0        0    13616 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_load.py
+-rw-rw-rw-   0        0        0     6277 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_loads.py
+-rw-rw-rw-   0        0        0    18643 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_mass_scaling.py
+-rw-rw-rw-   0        0        0     4719 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_mass_scalings.py
+-rw-rw-rw-   0        0        0    17803 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_mech_conn_behavior.py
+-rw-rw-rw-   0        0        0    12140 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_output_request.py
+-rw-rw-rw-   0        0        0     8229 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_output_requests.py
+-rw-rw-rw-   0        0        0     2843 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_pressure.py
+-rw-rw-rw-   0        0        0    10393 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_pretension_property.py
+-rw-rw-rw-   0        0        0     6562 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_properties.py
+-rw-rw-rw-   0        0        0     1828 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_property.py
+-rw-rw-rw-   0        0        0    22478 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_rigid_body_constraint.py
+-rw-rw-rw-   0        0        0    29395 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_rigid_coupling.py
+-rw-rw-rw-   0        0        0    28094 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_smooth_coupling.py
+-rw-rw-rw-   0        0        0     6737 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_smooth_step_amplitude.py
+-rw-rw-rw-   0        0        0     8281 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_case.py
+-rw-rw-rw-   0        0        0     4839 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_case_images.py
+-rw-rw-rw-   0        0        0     6822 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_step.py
+-rw-rw-rw-   0        0        0     4804 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_step_images.py
+-rw-rw-rw-   0        0        0     2934 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_steps.py
+-rw-rw-rw-   0        0        0    16760 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_spring_connection_property.py
+-rw-rw-rw-   0        0        0     6200 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_step.py
+-rw-rw-rw-   0        0        0     8887 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_steps.py
+-rw-rw-rw-   0        0        0    19137 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_surface_to_surface_contact.py
+-rw-rw-rw-   0        0        0     6712 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_tabular_amplitude.py
+-rw-rw-rw-   0        0        0    10170 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_temperature.py
+-rw-rw-rw-   0        0        0     3038 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_temperature_bc.py
+-rw-rw-rw-   0        0        0     5524 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_temperature_history.py
+-rw-rw-rw-   0        0        0     8478 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_thermal_conn_behavior.py
+-rw-rw-rw-   0        0        0    10433 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abqfh_output_request.py
+-rw-rw-rw-   0        0        0     8789 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_base_motion_vb.py
+-rw-rw-rw-   0        0        0     4969 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_frequency_loading_vb.py
+-rw-rw-rw-   0        0        0    10161 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_basic_vb.py
+-rw-rw-rw-   0        0        0    17690 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_modal_vb.py
+-rw-rw-rw-   0        0        0     7232 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_subspace_vb.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.532139 pycatia-0.6.9/pycatia/analysis_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/analysis_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1700 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_adaptivity_manager.py
+-rw-rw-rw-   0        0        0     5350 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_case.py
+-rw-rw-rw-   0        0        0     9409 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_cases.py
+-rw-rw-rw-   0        0        0    16345 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_color_map.py
+-rw-rw-rw-   0        0        0     2963 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_document.py
+-rw-rw-rw-   0        0        0     6388 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_entities.py
+-rw-rw-rw-   0        0        0    26162 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_entity.py
+-rw-rw-rw-   0        0        0     3714 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_export.py
+-rw-rw-rw-   0        0        0    33844 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_general_setting_att.py
+-rw-rw-rw-   0        0        0     3468 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_global_sensor.py
+-rw-rw-rw-   0        0        0    31399 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_image.py
+-rw-rw-rw-   0        0        0     8192 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_images.py
+-rw-rw-rw-   0        0        0     8323 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_import.py
+-rw-rw-rw-   0        0        0     2717 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_linked_documents.py
+-rw-rw-rw-   0        0        0     6589 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_local_entities.py
+-rw-rw-rw-   0        0        0    23544 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_local_entity.py
+-rw-rw-rw-   0        0        0     2602 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_local_sensor.py
+-rw-rw-rw-   0        0        0    16431 2024-05-18 10:30:56.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_manager.py
+-rw-rw-rw-   0        0        0     1345 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_element.py
+-rw-rw-rw-   0        0        0     8371 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_local_specification.py
+-rw-rw-rw-   0        0        0     4662 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_local_specifications.py
+-rw-rw-rw-   0        0        0     1947 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_manager.py
+-rw-rw-rw-   0        0        0     1330 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_node.py
+-rw-rw-rw-   0        0        0    17135 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_part.py
+-rw-rw-rw-   0        0        0     5573 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_parts.py
+-rw-rw-rw-   0        0        0     5999 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_model.py
+-rw-rw-rw-   0        0        0     3652 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_models.py
+-rw-rw-rw-   0        0        0     6430 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_output_entities.py
+-rw-rw-rw-   0        0        0     7230 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_post_manager.py
+-rw-rw-rw-   0        0        0    11583 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_post_pro_anr_setting_att.py
+-rw-rw-rw-   0        0        0    24324 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_post_pro_setting_att.py
+-rw-rw-rw-   0        0        0    32700 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_reporting_setting_att.py
+-rw-rw-rw-   0        0        0     2931 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_sensor.py
+-rw-rw-rw-   0        0        0     7724 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_set.py
+-rw-rw-rw-   0        0        0    10862 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_sets.py
+-rw-rw-rw-   0        0        0     2559 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_supports.py
+-rw-rw-rw-   0        0        0     9210 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/analysis_interfaces/analysis_v4_services.py
+-rw-rw-rw-   0        0        0    21400 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/basic_component.py
+-rw-rw-rw-   0        0        0     2919 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/analysis_interfaces/basic_components.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.571833 pycatia-0.6.9/pycatia/arrangement_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     6690 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arr_bendable_string.py
+-rw-rw-rw-   0        0        0     2900 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arr_bom_report.py
+-rw-rw-rw-   0        0        0     6767 2024-01-13 13:43:56.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arr_nomenclature.py
+-rw-rw-rw-   0        0        0     3112 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arr_nomenclature_tree.py
+-rw-rw-rw-   0        0        0     3873 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arr_nomenclatures.py
+-rw-rw-rw-   0        0        0     2578 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arr_system_line_product.py
+-rw-rw-rw-   0        0        0     6450 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arr_workbench.py
+-rw-rw-rw-   0        0        0     6369 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_area.py
+-rw-rw-rw-   0        0        0     7221 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_areas.py
+-rw-rw-rw-   0        0        0     6783 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_boundaries.py
+-rw-rw-rw-   0        0        0     8719 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_boundary.py
+-rw-rw-rw-   0        0        0     1315 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_contour.py
+-rw-rw-rw-   0        0        0     6375 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_contours.py
+-rw-rw-rw-   0        0        0    11749 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_item_reservation.py
+-rw-rw-rw-   0        0        0     8569 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_item_reservations.py
+-rw-rw-rw-   0        0        0     8138 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_node.py
+-rw-rw-rw-   0        0        0     3017 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_nodes.py
+-rw-rw-rw-   0        0        0     9493 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_pathway.py
+-rw-rw-rw-   0        0        0     6801 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_pathways.py
+-rw-rw-rw-   0        0        0    12330 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_product.py
+-rw-rw-rw-   0        0        0     4712 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_rectangle.py
+-rw-rw-rw-   0        0        0     6978 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_rectangles.py
+-rw-rw-rw-   0        0        0     9245 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_run.py
+-rw-rw-rw-   0        0        0     6653 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_runs.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.585913 pycatia-0.6.9/pycatia/assembly_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/assembly_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3006 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/assembly_interfaces/assembly_boolean.py
+-rw-rw-rw-   0        0        0    19642 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/assembly_interfaces/assembly_constraint_setting_att.py
+-rw-rw-rw-   0        0        0     8437 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/assembly_interfaces/assembly_feature.py
+-rw-rw-rw-   0        0        0    19318 2024-01-13 13:43:56.000000 pycatia-0.6.9/pycatia/assembly_interfaces/assembly_features.py
+-rw-rw-rw-   0        0        0    18416 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/assembly_interfaces/assembly_general_setting_att.py
+-rw-rw-rw-   0        0        0    18694 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/assembly_interfaces/assembly_hole.py
+-rw-rw-rw-   0        0        0    13758 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/assembly_interfaces/assembly_pocket.py
+-rw-rw-rw-   0        0        0     7002 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/assembly_interfaces/assembly_split.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.593650 pycatia-0.6.9/pycatia/base_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/base_interfaces/__init__.py
+-rw-rw-rw-   0        0        0      369 2024-04-22 07:21:05.000000 pycatia-0.6.9/pycatia/base_interfaces/base_application.py
+-rw-rw-rw-   0        0        0     2683 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/base_interfaces/context.py
+-rw-rw-rw-   0        0        0      414 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/base_interfaces/pycatia.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.602181 pycatia-0.6.9/pycatia/behavior_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/behavior_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9017 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/behavior_interfaces/behavior.py
+-rw-rw-rw-   0        0        0     3239 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/behavior_interfaces/behavior_extension.py
+-rw-rw-rw-   0        0        0     6690 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/behavior_interfaces/behavior_vb_script.py
+-rw-rw-rw-   0        0        0     3597 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/behavior_interfaces/behaviors.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.605183 pycatia-0.6.9/pycatia/bkt_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/bkt_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    15934 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/bkt_interfaces/behavior_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.610278 pycatia-0.6.9/pycatia/cat_dde_settings_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/cat_dde_settings_interfaces/__init__.py
+-rw-rw-rw-   0        0        0   105295 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_dde_settings_interfaces/dxf_setting_att.py
+-rw-rw-rw-   0        0        0    40793 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_dde_settings_interfaces/ig2_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.618958 pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    10266 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/e5_property.py
+-rw-rw-rw-   0        0        0     5407 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/ipd_template_property.py
+-rw-rw-rw-   0        0        0   192369 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/mfg_hub_setting_att.py
+-rw-rw-rw-   0        0        0     4424 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/mhi_relation_management.py
+-rw-rw-rw-   0        0        0     1480 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/cat_logger.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.635456 pycatia-0.6.9/pycatia/cat_mat_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-08-18 11:15:13.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2842 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/analysis_material.py
+-rw-rw-rw-   0        0        0     6087 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/material.py
+-rw-rw-rw-   0        0        0     2019 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/material_document.py
+-rw-rw-rw-   0        0        0     5351 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/material_families.py
+-rw-rw-rw-   0        0        0     1801 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/material_family.py
+-rw-rw-rw-   0        0        0    13313 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/material_manager.py
+-rw-rw-rw-   0        0        0     4887 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/materials.py
+-rw-rw-rw-   0        0        0     3489 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_mat_interfaces/positioned_material.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.687036 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    19021 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_app_factory.py
+-rw-rw-rw-   0        0        0     2624 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_application.py
+-rw-rw-rw-   0        0        0    16917 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_attribute.py
+-rw-rw-rw-   0        0        0     4167 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_attribute_report.py
+-rw-rw-rw-   0        0        0     8152 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_build_part.py
+-rw-rw-rw-   0        0        0     3691 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_class.py
+-rw-rw-rw-   0        0        0     3221 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_cntr_flow.py
+-rw-rw-rw-   0        0        0     8088 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_connectable.py
+-rw-rw-rw-   0        0        0     8948 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_connector.py
+-rw-rw-rw-   0        0        0    13776 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_functional.py
+-rw-rw-rw-   0        0        0     5608 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_group.py
+-rw-rw-rw-   0        0        0     2212 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_groupable.py
+-rw-rw-rw-   0        0        0     7025 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_id.py
+-rw-rw-rw-   0        0        0     3994 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_light_bend.py
+-rw-rw-rw-   0        0        0    12225 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_light_connector.py
+-rw-rw-rw-   0        0        0     5001 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_light_part.py
+-rw-rw-rw-   0        0        0     5242 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_list_of_bstrs.py
+-rw-rw-rw-   0        0        0     5225 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_list_of_doubles.py
+-rw-rw-rw-   0        0        0     5244 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_list_of_longs.py
+-rw-rw-rw-   0        0        0     5417 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_list_of_objects.py
+-rw-rw-rw-   0        0        0     9084 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_logical_line.py
+-rw-rw-rw-   0        0        0     3455 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_object.py
+-rw-rw-rw-   0        0        0    22942 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_part_connector.py
+-rw-rw-rw-   0        0        0     7613 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_phsyical_product.py
+-rw-rw-rw-   0        0        0     3118 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_physical.py
+-rw-rw-rw-   0        0        0    11743 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_place_part.py
+-rw-rw-rw-   0        0        0     3429 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_resource.py
+-rw-rw-rw-   0        0        0     4530 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_spatial.py
+-rw-rw-rw-   0        0        0     3672 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_stretchable_data.py
+-rw-rw-rw-   0        0        0     5597 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_temp_list_factory.py
+-rw-rw-rw-   0        0        0     7631 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_workbench.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.690049 pycatia-0.6.9/pycatia/cat_rdg_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/cat_rdg_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    32293 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_rdg_interfaces/rendering_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.692605 pycatia-0.6.9/pycatia/cat_rma_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-08-18 11:15:13.000000 pycatia-0.6.9/pycatia/cat_rma_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    57980 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_rma_interfaces/rendering_material.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.705457 pycatia-0.6.9/pycatia/cat_rsc_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/cat_rsc_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    13301 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_environment.py
+-rw-rw-rw-   0        0        0    11520 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_environment_wall.py
+-rw-rw-rw-   0        0        0     5468 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_environments.py
+-rw-rw-rw-   0        0        0    37352 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_light.py
+-rw-rw-rw-   0        0        0     4708 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_lights.py
+-rw-rw-rw-   0        0        0    41187 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_shooting.py
+-rw-rw-rw-   0        0        0     4846 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_shootings.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.849317 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:06.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3804 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_annotation_break.py
+-rw-rw-rw-   0        0        0     2378 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_2d_zone_from_3d_zone.py
+-rw-rw-rw-   0        0        0     6652 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_class.py
+-rw-rw-rw-   0        0        0     2356 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_colour.py
+-rw-rw-rw-   0        0        0     7751 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_data.py
+-rw-rw-rw-   0        0        0    17164 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_doc_link.py
+-rw-rw-rw-   0        0        0     5691 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_flow.py
+-rw-rw-rw-   0        0        0     4386 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_name.py
+-rw-rw-rw-   0        0        0     3091 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_show.py
+-rw-rw-rw-   0        0        0    10979 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_compatible.py
+-rw-rw-rw-   0        0        0    32666 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_component.py
+-rw-rw-rw-   0        0        0    14306 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_connectable.py
+-rw-rw-rw-   0        0        0    10068 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_connection.py
+-rw-rw-rw-   0        0        0    14039 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_connector.py
+-rw-rw-rw-   0        0        0     4896 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_delete_check.py
+-rw-rw-rw-   0        0        0     3028 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_delete_check2.py
+-rw-rw-rw-   0        0        0     3395 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_environment.py
+-rw-rw-rw-   0        0        0     3536 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_gap_priority.py
+-rw-rw-rw-   0        0        0     3452 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_group.py
+-rw-rw-rw-   0        0        0     3008 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_model_init.py
+-rw-rw-rw-   0        0        0     8923 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_multi_image.py
+-rw-rw-rw-   0        0        0     8943 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_multi_image_master.py
+-rw-rw-rw-   0        0        0    11671 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_object_factory.py
+-rw-rw-rw-   0        0        0    20901 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_object_factory2.py
+-rw-rw-rw-   0        0        0     4679 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_replace.py
+-rw-rw-rw-   0        0        0    15366 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_route.py
+-rw-rw-rw-   0        0        0     3296 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_route2.py
+-rw-rw-rw-   0        0        0     2474 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_scaling_rule.py
+-rw-rw-rw-   0        0        0     6280 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_zone.py
+-rw-rw-rw-   0        0        0     7615 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_arrow_display.py
+-rw-rw-rw-   0        0        0    19219 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_base_factory.py
+-rw-rw-rw-   0        0        0     6252 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_boundary_elem.py
+-rw-rw-rw-   0        0        0     3944 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_catalog_component.py
+-rw-rw-rw-   0        0        0     3781 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_catalog_route.py
+-rw-rw-rw-   0        0        0     6030 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_cntr_connect.py
+-rw-rw-rw-   0        0        0     5802 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_cntr_doc_link.py
+-rw-rw-rw-   0        0        0     6684 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_cntr_graphic.py
+-rw-rw-rw-   0        0        0    14915 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_cntr_location.py
+-rw-rw-rw-   0        0        0     9752 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_comp_connector.py
+-rw-rw-rw-   0        0        0     7819 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_comp_flow.py
+-rw-rw-rw-   0        0        0    15238 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_comp_graphic.py
+-rw-rw-rw-   0        0        0     5496 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_comp_group_ext.py
+-rw-rw-rw-   0        0        0    25584 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_compatible.py
+-rw-rw-rw-   0        0        0    52735 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_component.py
+-rw-rw-rw-   0        0        0     8796 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_component2.py
+-rw-rw-rw-   0        0        0     6070 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_component_group.py
+-rw-rw-rw-   0        0        0     3190 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_connectable.py
+-rw-rw-rw-   0        0        0     7407 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_drop_off_view.py
+-rw-rw-rw-   0        0        0    11239 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_frame_info.py
+-rw-rw-rw-   0        0        0     6920 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_gap_display.py
+-rw-rw-rw-   0        0        0    11656 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr.py
+-rw-rw-rw-   0        0        0     6463 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_cntr.py
+-rw-rw-rw-   0        0        0    13900 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_comp.py
+-rw-rw-rw-   0        0        0     9838 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_factory.py
+-rw-rw-rw-   0        0        0    36789 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_route.py
+-rw-rw-rw-   0        0        0     3795 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_route2.py
+-rw-rw-rw-   0        0        0     2389 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_route_alternate.py
+-rw-rw-rw-   0        0        0     6755 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_route_ellipse.py
+-rw-rw-rw-   0        0        0     8151 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_zone.py
+-rw-rw-rw-   0        0        0     5276 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_internal_flow.py
+-rw-rw-rw-   0        0        0     5231 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_list_of_bst_rs.py
+-rw-rw-rw-   0        0        0     5175 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_list_of_doubles.py
+-rw-rw-rw-   0        0        0     5340 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_list_of_longs.py
+-rw-rw-rw-   0        0        0     5429 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_list_of_objects.py
+-rw-rw-rw-   0        0        0     8985 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_movable.py
+-rw-rw-rw-   0        0        0     3431 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_movable2.py
+-rw-rw-rw-   0        0        0     5306 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_network_analysis.py
+-rw-rw-rw-   0        0        0     4210 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_obsolete_model.py
+-rw-rw-rw-   0        0        0     2223 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_post_replace.py
+-rw-rw-rw-   0        0        0     3207 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_replace.py
+-rw-rw-rw-   0        0        0    41105 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_route.py
+-rw-rw-rw-   0        0        0     9491 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_route_alternate_graphic.py
+-rw-rw-rw-   0        0        0     7004 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_route_graphic.py
+-rw-rw-rw-   0        0        0     7180 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_route_symbol.py
+-rw-rw-rw-   0        0        0     9511 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_session.py
+-rw-rw-rw-   0        0        0     5583 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_temp_list_factory.py
+-rw-rw-rw-   0        0        0     5008 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_update_instances.py
+-rw-rw-rw-   0        0        0     3192 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_workbench.py
+-rw-rw-rw-   0        0        0     2034 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_zone.py
+-rw-rw-rw-   0        0        0     6343 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_zone_graphic.py
+-rw-rw-rw-   0        0        0     1920 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_zone_membership.py
+-rw-rw-rw-   0        0        0     5343 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/schematic_extension.py
+-rw-rw-rw-   0        0        0    20891 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/schematic_root.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.851979 pycatia-0.6.9/pycatia/cat_sde_setting_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/cat_sde_setting_interfaces/__init__.py
+-rw-rw-rw-   0        0        0   129104 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sde_setting_interfaces/step_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.856978 pycatia-0.6.9/pycatia/cat_sm_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/cat_sm_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     5802 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sm_interfaces/catalog_shm_object_setting_att.py
+-rw-rw-rw-   0        0        0   166298 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_sm_interfaces/view_characteristic_curves_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.863714 pycatia-0.6.9/pycatia/cat_smarteam_integ_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/cat_smarteam_integ_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    10819 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/cat_smarteam_integ_interfaces/sti_db_children.py
+-rw-rw-rw-   0        0        0     8310 2024-01-13 13:43:56.000000 pycatia-0.6.9/pycatia/cat_smarteam_integ_interfaces/sti_db_item.py
+-rw-rw-rw-   0        0        0    71028 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_smarteam_integ_interfaces/sti_engine.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:45.922193 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    12014 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/end_cut_ess_object_setting_att.py
+-rw-rw-rw-   0        0        0     3355 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sdd_product.py
+-rw-rw-rw-   0        0        0     3390 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfd_product.py
+-rw-rw-rw-   0        0        0     4898 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_connection_parameters.py
+-rw-rw-rw-   0        0        0     7839 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_endcut.py
+-rw-rw-rw-   0        0        0     8035 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_endcut_manager.py
+-rw-rw-rw-   0        0        0    34661 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_factory.py
+-rw-rw-rw-   0        0        0    13339 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_function_factory.py
+-rw-rw-rw-   0        0        0    10680 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_manager.py
+-rw-rw-rw-   0        0        0     4915 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member.py
+-rw-rw-rw-   0        0        0    10463 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member2_points.py
+-rw-rw-rw-   0        0        0     5462 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_curve.py
+-rw-rw-rw-   0        0        0     6099 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_plane2_curves.py
+-rw-rw-rw-   0        0        0     6674 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_point_length.py
+-rw-rw-rw-   0        0        0     6376 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_point_up_to_limit.py
+-rw-rw-rw-   0        0        0     8573 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_surf_surf.py
+-rw-rw-rw-   0        0        0     3673 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_object.py
+-rw-rw-rw-   0        0        0     1274 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_object_ext.py
+-rw-rw-rw-   0        0        0    10868 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_opening.py
+-rw-rw-rw-   0        0        0     8692 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_opening_contours_mgr.py
+-rw-rw-rw-   0        0        0     8663 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_operation_factory.py
+-rw-rw-rw-   0        0        0     7637 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_positioning_strategy_manager.py
+-rw-rw-rw-   0        0        0    24387 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_profile.py
+-rw-rw-rw-   0        0        0     5395 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_references.py
+-rw-rw-rw-   0        0        0    13630 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_slot.py
+-rw-rw-rw-   0        0        0     8434 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_slots.py
+-rw-rw-rw-   0        0        0     2648 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_split_plate.py
+-rw-rw-rw-   0        0        0     2916 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_split_plates.py
+-rw-rw-rw-   0        0        0     4216 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_standard_contour_parameters.py
+-rw-rw-rw-   0        0        0    16391 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_standard_opening.py
+-rw-rw-rw-   0        0        0    16846 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_standard_pos_strategy_parameters.py
+-rw-rw-rw-   0        0        0     9952 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_stiffener.py
+-rw-rw-rw-   0        0        0    11176 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_stiffener_on_free_edge.py
+-rw-rw-rw-   0        0        0    27220 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_super_plate.py
+-rw-rw-rw-   0        0        0     5447 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_weld.py
+-rw-rw-rw-   0        0        0     2809 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_welds.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.017864 pycatia-0.6.9/pycatia/cat_tps_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    31138 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation.py
+-rw-rw-rw-   0        0        0    19658 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_2.py
+-rw-rw-rw-   0        0        0    20053 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_factory.py
+-rw-rw-rw-   0        0        0    21864 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_factory_2.py
+-rw-rw-rw-   0        0        0    14701 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_set.py
+-rw-rw-rw-   0        0        0     2553 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_set_transform_into_assembly_set.py
+-rw-rw-rw-   0        0        0     3630 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_sets.py
+-rw-rw-rw-   0        0        0     4035 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/annotations.py
+-rw-rw-rw-   0        0        0     2959 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/assembly_annotation_sets.py
+-rw-rw-rw-   0        0        0     2674 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/associated_ref_frame.py
+-rw-rw-rw-   0        0        0    11659 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/capture.py
+-rw-rw-rw-   0        0        0     2041 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/capture_factory.py
+-rw-rw-rw-   0        0        0     2140 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/captures.py
+-rw-rw-rw-   0        0        0     2261 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/composite_tolerance.py
+-rw-rw-rw-   0        0        0     1750 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/controlled_radius.py
+-rw-rw-rw-   0        0        0     2509 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/datum_simple.py
+-rw-rw-rw-   0        0        0    11536 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/datum_target.py
+-rw-rw-rw-   0        0        0     3459 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/default_annotation.py
+-rw-rw-rw-   0        0        0    10328 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/dimension_3d.py
+-rw-rw-rw-   0        0        0     6204 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/dimension_limit.py
+-rw-rw-rw-   0        0        0     1618 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/dimension_pattern.py
+-rw-rw-rw-   0        0        0    19678 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/dmu_tol_setting_att.py
+-rw-rw-rw-   0        0        0     1641 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/envelope_condition.py
+-rw-rw-rw-   0        0        0     9245 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/flag_note.py
+-rw-rw-rw-   0        0        0     1739 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/free_state.py
+-rw-rw-rw-   0        0        0    69177 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/fta_infra_setting_att.py
+-rw-rw-rw-   0        0        0   236553 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/fta_setting_att.py
+-rw-rw-rw-   0        0        0     1649 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/material_condition.py
+-rw-rw-rw-   0        0        0    11181 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/noa.py
+-rw-rw-rw-   0        0        0     1745 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/non_semantic_datum.py
+-rw-rw-rw-   0        0        0     3159 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/non_semantic_datum_target.py
+-rw-rw-rw-   0        0        0     3293 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/non_semantic_dimension.py
+-rw-rw-rw-   0        0        0     1702 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/non_semantic_gdt.py
+-rw-rw-rw-   0        0        0     1919 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/particular_tol_elem.py
+-rw-rw-rw-   0        0        0     5412 2024-01-13 13:43:56.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/projected_tolerance_zone.py
+-rw-rw-rw-   0        0        0    14500 2024-01-13 13:43:56.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/reference_frame.py
+-rw-rw-rw-   0        0        0     5978 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/roughness.py
+-rw-rw-rw-   0        0        0    17825 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/semantic_gdt.py
+-rw-rw-rw-   0        0        0     6829 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/shifted_profile_tolerance.py
+-rw-rw-rw-   0        0        0     1763 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/tangent_plane.py
+-rw-rw-rw-   0        0        0     2702 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/text.py
+-rw-rw-rw-   0        0        0     2179 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/tolerance_per_unit_basis_restrictive_value.py
+-rw-rw-rw-   0        0        0     3020 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/tolerance_unit_basis_value.py
+-rw-rw-rw-   0        0        0     2303 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/tolerance_zone.py
+-rw-rw-rw-   0        0        0     2507 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/tps_parallel_on_screen.py
+-rw-rw-rw-   0        0        0     1221 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/tps_view.py
+-rw-rw-rw-   0        0        0     2638 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/tps_view_factory.py
+-rw-rw-rw-   0        0        0     2185 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/tps_views.py
+-rw-rw-rw-   0        0        0     6229 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/user_surface.py
+-rw-rw-rw-   0        0        0     7752 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/user_surfaces.py
+-rw-rw-rw-   0        0        0     2137 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/cat_tps_interfaces/weld.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.021885 pycatia-0.6.9/pycatia/catia_de_settings_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/catia_de_settings_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    68427 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/catia_de_settings_interfaces/iges_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.032008 pycatia-0.6.9/pycatia/catia_v4_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/catia_v4_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    24031 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/catia_v4_interfaces/interop_setting_att.py
+-rw-rw-rw-   0        0        0    34731 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/catia_v4_interfaces/migr_batch_setting_att.py
+-rw-rw-rw-   0        0        0     8685 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/catia_v4_interfaces/spec_v4_setting_att.py
+-rw-rw-rw-   0        0        0    33750 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/catia_v4_interfaces/v4_v5_space_setting_att.py
+-rw-rw-rw-   0        0        0    38011 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/catia_v4_interfaces/v4_writing_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.035330 pycatia-0.6.9/pycatia/components_catalogs_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/components_catalogs_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     8304 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/components_catalogs_interfaces/catalog_document.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.038329 pycatia-0.6.9/pycatia/composites_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/composites_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     7398 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/composites_interfaces/composites_material.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.059162 pycatia-0.6.9/pycatia/dmaps_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     5268 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/activities.py
+-rw-rw-rw-   0        0        0    35559 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/activity.py
+-rw-rw-rw-   0        0        0     1263 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/item.py
+-rw-rw-rw-   0        0        0     7136 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/items.py
+-rw-rw-rw-   0        0        0    19677 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/lib_tab_setting_att.py
+-rw-rw-rw-   0        0        0     4257 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/outputs.py
+-rw-rw-rw-   0        0        0     3389 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/process_document.py
+-rw-rw-rw-   0        0        0     5641 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/resource.py
+-rw-rw-rw-   0        0        0     2445 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/resource_collection.py
+-rw-rw-rw-   0        0        0     5533 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/resources.py
+-rw-rw-rw-   0        0        0    64615 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/tree_tab_setting_att.py
+-rw-rw-rw-   0        0        0    14869 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dmaps_interfaces/verif_tab_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.061778 pycatia-0.6.9/pycatia/dnb_asy_activity_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_asy_activity_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2006 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_asy_activity_interfaces/asy_sim_activity.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.064783 pycatia-0.6.9/pycatia/dnb_d5_iInterfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_d5_iInterfaces/__init__.py
+-rw-rw-rw-   0        0        0    89435 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_d5_iInterfaces/import_d5_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.069800 pycatia-0.6.9/pycatia/dnb_device_activity_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_activity_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    10678 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_activity_interfaces/move_home_act.py
+-rw-rw-rw-   0        0        0    10748 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_activity_interfaces/move_joints_act.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.083390 pycatia-0.6.9/pycatia/dnb_device_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     7327 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_interfaces/basic_device.py
+-rw-rw-rw-   0        0        0     2590 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_interfaces/d5_device.py
+-rw-rw-rw-   0        0        0    35302 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_interfaces/dev_analysis_setting_att.py
+-rw-rw-rw-   0        0        0     6698 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_interfaces/device_joint_relations.py
+-rw-rw-rw-   0        0        0     9840 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_interfaces/device_sim.py
+-rw-rw-rw-   0        0        0     3876 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_interfaces/dof_state.py
+-rw-rw-rw-   0        0        0    12950 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_device_interfaces/home_position.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.089899 pycatia-0.6.9/pycatia/dnb_dpm_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_dpm_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    12043 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_dpm_interfaces/mfg_assembly.py
+-rw-rw-rw-   0        0        0    18123 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_dpm_interfaces/mfg_assembly_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.094408 pycatia-0.6.9/pycatia/dnb_ehm_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_ehm_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    30228 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_ehm_interfaces/ehm_insertion_act_plug_map_view_data.py
+-rw-rw-rw-   0        0        0    13085 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_ehm_interfaces/plug_map_view_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.097408 pycatia-0.6.9/pycatia/dnb_ehs_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_ehs_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2582 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_ehs_interfaces/ehs_update_smoothness_factor.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.100977 pycatia-0.6.9/pycatia/dnb_ekp_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_ekp_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    12898 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_ekp_interfaces/ekp_services.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.119028 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1657 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/curve_fastener.py
+-rw-rw-rw-   0        0        0    16617 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/dnb_fastener_item_services.py
+-rw-rw-rw-   0        0        0    16244 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/dnb_fastener_management.py
+-rw-rw-rw-   0        0        0    10746 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/dnb_fastener_new_mfg_pos_services.py
+-rw-rw-rw-   0        0        0    17815 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/fastener.py
+-rw-rw-rw-   0        0        0    13251 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/fastener_group.py
+-rw-rw-rw-   0        0        0     2482 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/fastener_set.py
+-rw-rw-rw-   0        0        0     6392 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/fastener_work_bench.py
+-rw-rw-rw-   0        0        0     5477 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_fastener_interfaces/point_fastener.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.123129 pycatia-0.6.9/pycatia/dnb_graph_editor/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_graph_editor/__init__.py
+-rw-rw-rw-   0        0        0     3552 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_graph_editor/pert_node.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.167231 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9912 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_anthro.py
+-rw-rw-rw-   0        0        0     9464 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_anthro_variable.py
+-rw-rw-rw-   0        0        0    27658 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_body.py
+-rw-rw-rw-   0        0        0     9382 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_body_element.py
+-rw-rw-rw-   0        0        0     1368 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_center_of_gravity.py
+-rw-rw-rw-   0        0        0     4220 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo.py
+-rw-rw-rw-   0        0        0     4174 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo_carry.py
+-rw-rw-rw-   0        0        0    28436 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo_lift_lower.py
+-rw-rw-rw-   0        0        0     6665 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo_push_pull.py
+-rw-rw-rw-   0        0        0     7278 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo_rula.py
+-rw-rw-rw-   0        0        0     9274 2024-05-20 09:42:12.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_hmi_workbench.py
+-rw-rw-rw-   0        0        0     8074 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_human_catalog.py
+-rw-rw-rw-   0        0        0     9888 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_line_of_sight.py
+-rw-rw-rw-   0        0        0     4764 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_line_of_sight_node.py
+-rw-rw-rw-   0        0        0     9321 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_manikin.py
+-rw-rw-rw-   0        0        0     1820 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_manikin_part.py
+-rw-rw-rw-   0        0        0     1298 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_node.py
+-rw-rw-rw-   0        0        0    32651 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_segment.py
+-rw-rw-rw-   0        0        0     5991 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_segment_node.py
+-rw-rw-rw-   0        0        0    15408 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_vision.py
+-rw-rw-rw-   0        0        0    15488 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swkdof.py
+-rw-rw-rw-   0        0        0    31339 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swkik_constraint.py
+-rw-rw-rw-   0        0        0     9021 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swkik_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.209854 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/auto_walk_activity.py
+-rw-rw-rw-   0        0        0     3642 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/collision_free_walk.py
+-rw-rw-rw-   0        0        0    22264 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/hts_ccp_setting_att.py
+-rw-rw-rw-   0        0        0    41891 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/hts_general_setting_att.py
+-rw-rw-rw-   0        0        0    10173 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/hts_joint_speed_settings_att.py
+-rw-rw-rw-   0        0        0    36584 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/hts_task_display_setting_att.py
+-rw-rw-rw-   0        0        0     4284 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_activity_group.py
+-rw-rw-rw-   0        0        0    66950 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_activity_group_factory.py
+-rw-rw-rw-   0        0        0    72493 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_acts_factory.py
+-rw-rw-rw-   0        0        0     3969 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_call_task.py
+-rw-rw-rw-   0        0        0     2392 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_program.py
+-rw-rw-rw-   0        0        0     4355 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_task.py
+-rw-rw-rw-   0        0        0     2473 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_task_list.py
+-rw-rw-rw-   0        0        0    30215 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/move_to_posture_activity.py
+-rw-rw-rw-   0        0        0    12771 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/pick_activity.py
+-rw-rw-rw-   0        0        0    18095 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/place_activity.py
+-rw-rw-rw-   0        0        0    10521 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/walk_activity.py
+-rw-rw-rw-   0        0        0     3014 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/worker_activity.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.218864 pycatia-0.6.9/pycatia/dnb_igp_arc_commands/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_arc_commands/__init__.py
+-rw-rw-rw-   0        0        0    14811 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_arc_commands/amp_path.py
+-rw-rw-rw-   0        0        0    31990 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_arc_commands/amp_tag.py
+-rw-rw-rw-   0        0        0    28761 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_arc_commands/arc_tag.py
+-rw-rw-rw-   0        0        0    20357 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_arc_commands/arc_tag_group.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.223937 pycatia-0.6.9/pycatia/dnb_igp_olp_ui/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_olp_ui/__init__.py
+-rw-rw-rw-   0        0        0    39040 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_olp_ui/igp_olp_setting_att.py
+-rw-rw-rw-   0        0        0    23296 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_olp_ui/olp_translator.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.261418 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     8818 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/call_robot_task_activity.py
+-rw-rw-rw-   0        0        0    11994 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/device_task.py
+-rw-rw-rw-   0        0        0     9247 2023-10-31 11:15:07.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/device_task_factory.py
+-rw-rw-rw-   0        0        0     4209 2023-10-31 11:15:08.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/generic_action.py
+-rw-rw-rw-   0        0        0     4906 2023-10-31 11:15:08.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/generic_action_factory.py
+-rw-rw-rw-   0        0        0     4568 2023-10-31 11:15:08.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/mount_activity.py
+-rw-rw-rw-   0        0        0    18460 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/mount_manager.py
+-rw-rw-rw-   0        0        0     5692 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/move_action_activity.py
+-rw-rw-rw-   0        0        0    12947 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/operation.py
+-rw-rw-rw-   0        0        0     6927 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/operation_profile.py
+-rw-rw-rw-   0        0        0    54586 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/robot_motion.py
+-rw-rw-rw-   0        0        0    16852 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/robot_task.py
+-rw-rw-rw-   0        0        0     9191 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/robot_task_clone_factory.py
+-rw-rw-rw-   0        0        0     9169 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/robot_task_factory.py
+-rw-rw-rw-   0        0        0    13836 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tag.py
+-rw-rw-rw-   0        0        0     4475 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tag_factory.py
+-rw-rw-rw-   0        0        0     9961 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tag_group.py
+-rw-rw-rw-   0        0        0    15928 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tag_group_factory.py
+-rw-rw-rw-   0        0        0     8202 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tcp_trace_activity.py
+-rw-rw-rw-   0        0        0     4618 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/unmount_activity.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.267418 pycatia-0.6.9/pycatia/dnb_manufacturing_layout_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_manufacturing_layout_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     4104 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_manufacturing_layout_interfaces/attachment_cont.py
+-rw-rw-rw-   0        0        0    10115 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_manufacturing_layout_interfaces/dnb_attachment.py
+-rw-rw-rw-   0        0        0     3643 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_manufacturing_layout_interfaces/dnb_attachment_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.273213 pycatia-0.6.9/pycatia/dnb_mhi_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_mhi_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    28834 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_mhi_interfaces/mhi_load_parameters.py
+-rw-rw-rw-   0        0        0     9326 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_mhi_interfaces/mhi_open_access.py
+-rw-rw-rw-   0        0        0     6008 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_mhi_interfaces/mhi_save_access.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.276212 pycatia-0.6.9/pycatia/dnb_reporting_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_reporting_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    31159 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_reporting_interfaces/fas_reporting_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.283251 pycatia-0.6.9/pycatia/dnb_resource_program_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_resource_program_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     7106 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_resource_program_interfaces/active_task.py
+-rw-rw-rw-   0        0        0     6817 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/dnb_resource_program_interfaces/resource_program_manager.py
+-rw-rw-rw-   0        0        0     6540 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/dnb_resource_program_interfaces/task.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.309848 pycatia-0.6.9/pycatia/dnb_robot_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9640 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/aux_devices_mgt.py
+-rw-rw-rw-   0        0        0    26028 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/calib_offsets.py
+-rw-rw-rw-   0        0        0    12207 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/generic_accuracy_profile.py
+-rw-rw-rw-   0        0        0    15337 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/generic_motion_profile.py
+-rw-rw-rw-   0        0        0     8610 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/generic_obj_frame_profile.py
+-rw-rw-rw-   0        0        0    19857 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/generic_tool_profile.py
+-rw-rw-rw-   0        0        0     9779 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/parameter_profiles.py
+-rw-rw-rw-   0        0        0    18481 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/parameter_profiles_factory.py
+-rw-rw-rw-   0        0        0     6828 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/rob_analysis_heart_beat_usage_setting_att.py
+-rw-rw-rw-   0        0        0    39452 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/rob_analysis_setting_att.py
+-rw-rw-rw-   0        0        0     9653 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/rob_controller_factory.py
+-rw-rw-rw-   0        0        0    50131 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/rob_generic_controller.py
+-rw-rw-rw-   0        0        0    85179 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/rrs_setting_att.py
+-rw-rw-rw-   0        0        0    25756 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/tcp_trace.py
+-rw-rw-rw-   0        0        0    11973 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/tcp_trace_manager.py
+-rw-rw-rw-   0        0        0     8388 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_robot_interfaces/tcp_trace_manager_graphics.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.316855 pycatia-0.6.9/pycatia/dnb_sim_activity_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_sim_activity_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2779 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_sim_activity_interfaces/delay_act.py
+-rw-rw-rw-   0        0        0     5693 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_sim_activity_interfaces/grab_act.py
+-rw-rw-rw-   0        0        0     5750 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_sim_activity_interfaces/release_act.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.324992 pycatia-0.6.9/pycatia/dnb_simulation_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_simulation_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    87704 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_simulation_interfaces/analysis_setting_att.py
+-rw-rw-rw-   0        0        0    51097 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_simulation_interfaces/sim_trace_setting_att.py
+-rw-rw-rw-   0        0        0     8987 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_simulation_interfaces/simulation_init_state.py
+-rw-rw-rw-   0        0        0   102279 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_simulation_interfaces/simulation_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.327991 pycatia-0.6.9/pycatia/dnb_sor_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_sor_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    46464 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/dnb_sor_interfaces/order_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.334510 pycatia-0.6.9/pycatia/dnb_state_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_state_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    27783 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_state_interfaces/dnb_3d_state.py
+-rw-rw-rw-   0        0        0    17142 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_state_interfaces/dnb_3d_state_management.py
+-rw-rw-rw-   0        0        0     3468 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_state_interfaces/dnb_3d_states.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.346532 pycatia-0.6.9/pycatia/dnb_work_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/dnb_work_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3950 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_buy_off.py
+-rw-rw-rw-   0        0        0     4046 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_change_notification.py
+-rw-rw-rw-   0        0        0     4014 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_data_collection.py
+-rw-rw-rw-   0        0        0     8948 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_text.py
+-rw-rw-rw-   0        0        0     3239 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_text_access_ei.py
+-rw-rw-rw-   0        0        0    31688 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/dnb_work_interfaces/work_general_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.359236 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3161 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_factory.py
+-rw-rw-rw-   0        0        0    11778 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_root.py
+-rw-rw-rw-   0        0        0   161905 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_setting_att.py
+-rw-rw-rw-   0        0        0    19773 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_sheet.py
+-rw-rw-rw-   0        0        0    10622 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_sheets.py
+-rw-rw-rw-   0        0        0    31074 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_view.py
+-rw-rw-rw-   0        0        0    22385 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_views.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.420280 pycatia-0.6.9/pycatia/drafting_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/drafting_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    58714 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drafting_setting_att.py
+-rw-rw-rw-   0        0        0    15442 2023-10-31 11:15:09.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_arrow.py
+-rw-rw-rw-   0        0        0     6961 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_arrows.py
+-rw-rw-rw-   0        0        0    19432 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_component.py
+-rw-rw-rw-   0        0        0     8592 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_components.py
+-rw-rw-rw-   0        0        0    19607 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dim_ext_line.py
+-rw-rw-rw-   0        0        0    16275 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dim_line.py
+-rw-rw-rw-   0        0        0    26915 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dim_value.py
+-rw-rw-rw-   0        0        0    33304 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dimension.py
+-rw-rw-rw-   0        0        0    13674 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dimensions.py
+-rw-rw-rw-   0        0        0     7831 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_document.py
+-rw-rw-rw-   0        0        0    16400 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_leader.py
+-rw-rw-rw-   0        0        0     6746 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_leaders.py
+-rw-rw-rw-   0        0        0     4506 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_page_setup.py
+-rw-rw-rw-   0        0        0    13366 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_picture.py
+-rw-rw-rw-   0        0        0     8215 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_pictures.py
+-rw-rw-rw-   0        0        0     4043 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_root.py
+-rw-rw-rw-   0        0        0    25212 2023-10-31 11:15:10.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_sheet.py
+-rw-rw-rw-   0        0        0    10412 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_sheets.py
+-rw-rw-rw-   0        0        0    42085 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_table.py
+-rw-rw-rw-   0        0        0     7505 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_tables.py
+-rw-rw-rw-   0        0        0    25355 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_text.py
+-rw-rw-rw-   0        0        0    18904 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_text_properties.py
+-rw-rw-rw-   0        0        0     9783 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_text_range.py
+-rw-rw-rw-   0        0        0     6907 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_texts.py
+-rw-rw-rw-   0        0        0     3890 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_thread.py
+-rw-rw-rw-   0        0        0     6595 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_threads.py
+-rw-rw-rw-   0        0        0    41664 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_view.py
+-rw-rw-rw-   0        0        0    78715 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_view_generative_behavior.py
+-rw-rw-rw-   0        0        0     6699 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_view_generative_links.py
+-rw-rw-rw-   0        0        0     9466 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_views.py
+-rw-rw-rw-   0        0        0    17595 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_welding.py
+-rw-rw-rw-   0        0        0     7109 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/drafting_interfaces/drawing_weldings.py
+-rw-rw-rw-   0        0        0    10022 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/drafting_interfaces/print_area.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.427286 pycatia-0.6.9/pycatia/electrical_schematic_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/electrical_schematic_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     5395 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/electrical_schematic_interfaces/electrical_schematic_object.py
+-rw-rw-rw-   0        0        0     1584 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/electrical_schematic_interfaces/electrical_schematic_wire.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.452806 pycatia-0.6.9/pycatia/eno_cd5_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    21333 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_engine.py
+-rw-rw-rw-   0        0        0     6726 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_engine_v6_r2014x.py
+-rw-rw-rw-   0        0        0    15184 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_engine_v6_r2015.py
+-rw-rw-rw-   0        0        0     2551 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_id.py
+-rw-rw-rw-   0        0        0     2636 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_ids.py
+-rw-rw-rw-   0        0        0     3788 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_properties.py
+-rw-rw-rw-   0        0        0     3880 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_property.py
+-rw-rw-rw-   0        0        0    12261 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_save_item.py
+-rw-rw-rw-   0        0        0     2963 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_save_items.py
+-rw-rw-rw-   0        0        0     8166 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_save_operation.py
+-rw-rw-rw-   0        0        0     5313 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_structure.py
+-rw-rw-rw-   0        0        0     4823 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_template.py
+-rw-rw-rw-   0        0        0     4175 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_template_type.py
+-rw-rw-rw-   0        0        0     2789 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_template_types.py
+-rw-rw-rw-   0        0        0     2555 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_templates.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.455807 pycatia-0.6.9/pycatia/enumeration/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.6.9/pycatia/enumeration/__init__.py
+-rw-rw-rw-   0        0        0    54918 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/enumeration/enumeration_types.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.457805 pycatia-0.6.9/pycatia/exception_handling/
+-rw-rw-rw-   0        0        0       76 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/exception_handling/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/exception_handling/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.476891 pycatia-0.6.9/pycatia/fitting_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/fitting_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    31764 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/fitting_setting_att.py
+-rw-rw-rw-   0        0        0    31745 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/manip_setting_att.py
+-rw-rw-rw-   0        0        0    11585 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/sampled.py
+-rw-rw-rw-   0        0        0     6392 2023-10-31 11:15:12.000000 pycatia-0.6.9/pycatia/fitting_interfaces/sampleds.py
+-rw-rw-rw-   0        0        0     2587 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/sampleds_node.py
+-rw-rw-rw-   0        0        0    18875 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/shot.py
+-rw-rw-rw-   0        0        0     8890 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/shots.py
+-rw-rw-rw-   0        0        0     8572 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/shuttle.py
+-rw-rw-rw-   0        0        0     4528 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/shuttles.py
+-rw-rw-rw-   0        0        0     8714 2023-10-31 11:15:11.000000 pycatia-0.6.9/pycatia/fitting_interfaces/track.py
+-rw-rw-rw-   0        0        0     2253 2023-10-31 11:15:12.000000 pycatia-0.6.9/pycatia/fitting_interfaces/tracks.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.514762 pycatia-0.6.9/pycatia/funct_system_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-11-18 10:48:10.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9253 2023-10-31 11:15:12.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_actions_group.py
+-rw-rw-rw-   0        0        0     5584 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_actions_groups.py
+-rw-rw-rw-   0        0        0     3801 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_association.py
+-rw-rw-rw-   0        0        0     5543 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_associations.py
+-rw-rw-rw-   0        0        0     3332 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_facet_managers.py
+-rw-rw-rw-   0        0        0     2458 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_gen_script_mgr.py
+-rw-rw-rw-   0        0        0     2456 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_multi_rep_mgr.py
+-rw-rw-rw-   0        0        0     2928 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_node_graph_layout.py
+-rw-rw-rw-   0        0        0     1893 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_script.py
+-rw-rw-rw-   0        0        0     5298 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/funct_scripts.py
+-rw-rw-rw-   0        0        0     7114 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_action.py
+-rw-rw-rw-   0        0        0     5292 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_actions.py
+-rw-rw-rw-   0        0        0     7357 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_description.py
+-rw-rw-rw-   0        0        0     2981 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_document.py
+-rw-rw-rw-   0        0        0     2311 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_element.py
+-rw-rw-rw-   0        0        0     2516 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_facet.py
+-rw-rw-rw-   0        0        0     1337 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_facet_mgr.py
+-rw-rw-rw-   0        0        0     3868 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_object.py
+-rw-rw-rw-   0        0        0     3538 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_object_proxy.py
+-rw-rw-rw-   0        0        0     5854 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_objects.py
+-rw-rw-rw-   0        0        0     2796 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_position.py
+-rw-rw-rw-   0        0        0    42528 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_system_setting_att.py
+-rw-rw-rw-   0        0        0     2023 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_variant.py
+-rw-rw-rw-   0        0        0     5009 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/funct_system_interfaces/functional_variants.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.537080 pycatia-0.6.9/pycatia/general_knowledge_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     4605 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_check.py
+-rw-rw-rw-   0        0        0    11432 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_check_runtime.py
+-rw-rw-rw-   0        0        0     5669 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_report_object.py
+-rw-rw-rw-   0        0        0     8170 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_report_objects.py
+-rw-rw-rw-   0        0        0     4248 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule.py
+-rw-rw-rw-   0        0        0     2237 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_base.py
+-rw-rw-rw-   0        0        0     7428 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_base_component_runtime.py
+-rw-rw-rw-   0        0        0    12861 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_base_component_runtimes.py
+-rw-rw-rw-   0        0        0    25920 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_base_runtime.py
+-rw-rw-rw-   0        0        0     3148 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_runtime.py
+-rw-rw-rw-   0        0        0    11464 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_set.py
+-rw-rw-rw-   0        0        0     4268 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_set_runtime.py
+-rw-rw-rw-   0        0        0     4009 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/general_knowledge_interfaces/kwe_correct_function.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.738950 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     5869 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_3d_curve_offset.py
+-rw-rw-rw-   0        0        0    12406 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_affinity.py
+-rw-rw-rw-   0        0        0    33611 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_assemble.py
+-rw-rw-rw-   0        0        0     5972 2024-05-20 09:35:00.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_line.py
+-rw-rw-rw-   0        0        0     7527 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_to_axis.py
+-rw-rw-rw-   0        0        0    55632 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_blend.py
+-rw-rw-rw-   0        0        0     7640 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_boundary.py
+-rw-rw-rw-   0        0        0     8127 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_bump.py
+-rw-rw-rw-   0        0        0    13687 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle.py
+-rw-rw-rw-   0        0        0    11751 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle2_points_rad.py
+-rw-rw-rw-   0        0        0     6962 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle3_points.py
+-rw-rw-rw-   0        0        0    16515 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_point.py
+-rw-rw-rw-   0        0        0    17752 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_radius.py
+-rw-rw-rw-   0        0        0     8549 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_axis.py
+-rw-rw-rw-   0        0        0    16136 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_tangent.py
+-rw-rw-rw-   0        0        0     7004 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_pt.py
+-rw-rw-rw-   0        0        0    12421 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_rad.py
+-rw-rw-rw-   0        0        0     1870 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_explicit.py
+-rw-rw-rw-   0        0        0    19231 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_tritangent.py
+-rw-rw-rw-   0        0        0     9967 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_combine.py
+-rw-rw-rw-   0        0        0    52700 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_conic.py
+-rw-rw-rw-   0        0        0    11890 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_connect.py
+-rw-rw-rw-   0        0        0    22143 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_corner.py
+-rw-rw-rw-   0        0        0     1522 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_explicit.py
+-rw-rw-rw-   0        0        0    23254 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_par.py
+-rw-rw-rw-   0        0        0    38073 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_smooth.py
+-rw-rw-rw-   0        0        0    10014 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_cylinder.py
+-rw-rw-rw-   0        0        0    15802 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_develop.py
+-rw-rw-rw-   0        0        0    10462 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_direction.py
+-rw-rw-rw-   0        0        0    11283 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extract.py
+-rw-rw-rw-   0        0        0    47925 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extract_multi.py
+-rw-rw-rw-   0        0        0    27673 2024-05-20 09:34:59.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extrapol.py
+-rw-rw-rw-   0        0        0     7103 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum.py
+-rw-rw-rw-   0        0        0     6172 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum_polar.py
+-rw-rw-rw-   0        0        0    14952 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extrude.py
+-rw-rw-rw-   0        0        0   241892 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_factory.py
+-rw-rw-rw-   0        0        0    37178 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_fill.py
+-rw-rw-rw-   0        0        0    20008 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_bi_tangent.py
+-rw-rw-rw-   0        0        0    10397 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_tri_tangent.py
+-rw-rw-rw-   0        0        0    33448 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_healing.py
+-rw-rw-rw-   0        0        0    15240 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_helix.py
+-rw-rw-rw-   0        0        0    17831 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_integrated_law.py
+-rw-rw-rw-   0        0        0     9789 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_intersection.py
+-rw-rw-rw-   0        0        0     3419 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_inverse.py
+-rw-rw-rw-   0        0        0    12950 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_law_dist_proj.py
+-rw-rw-rw-   0        0        0    11668 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_angle.py
+-rw-rw-rw-   0        0        0    15163 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bi_tangent.py
+-rw-rw-rw-   0        0        0    12124 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bisecting.py
+-rw-rw-rw-   0        0        0     1563 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_explicit.py
+-rw-rw-rw-   0        0        0    11145 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_normal.py
+-rw-rw-rw-   0        0        0    12647 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_dir.py
+-rw-rw-rw-   0        0        0    11500 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_pt.py
+-rw-rw-rw-   0        0        0    12650 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_tangency.py
+-rw-rw-rw-   0        0        0    66004 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_loft.py
+-rw-rw-rw-   0        0        0     4732 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_mid_surface.py
+-rw-rw-rw-   0        0        0     3966 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_near.py
+-rw-rw-rw-   0        0        0     7666 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_offset.py
+-rw-rw-rw-   0        0        0     2627 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_curve.py
+-rw-rw-rw-   0        0        0     3464 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_line1_pt.py
+-rw-rw-rw-   0        0        0     4556 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane2_lines.py
+-rw-rw-rw-   0        0        0     5084 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane3_points.py
+-rw-rw-rw-   0        0        0     5922 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_angle.py
+-rw-rw-rw-   0        0        0     9143 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_equation.py
+-rw-rw-rw-   0        0        0     1574 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_explicit.py
+-rw-rw-rw-   0        0        0     9092 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_mean.py
+-rw-rw-rw-   0        0        0     3780 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_normal.py
+-rw-rw-rw-   0        0        0     3582 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset.py
+-rw-rw-rw-   0        0        0     3828 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset_pt.py
+-rw-rw-rw-   0        0        0     3820 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_tangent.py
+-rw-rw-rw-   0        0        0     7334 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_between.py
+-rw-rw-rw-   0        0        0     2910 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_center.py
+-rw-rw-rw-   0        0        0     6861 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_coord.py
+-rw-rw-rw-   0        0        0     1574 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_explicit.py
+-rw-rw-rw-   0        0        0    13727 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_curve.py
+-rw-rw-rw-   0        0        0    10203 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_plane.py
+-rw-rw-rw-   0        0        0     6413 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_surface.py
+-rw-rw-rw-   0        0        0     4257 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_tangent.py
+-rw-rw-rw-   0        0        0    13045 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_polyline.py
+-rw-rw-rw-   0        0        0    20768 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_position_transfo.py
+-rw-rw-rw-   0        0        0    12602 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_project.py
+-rw-rw-rw-   0        0        0    12198 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_reflect_line.py
+-rw-rw-rw-   0        0        0    13300 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_revol.py
+-rw-rw-rw-   0        0        0     9306 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_rolling_offset.py
+-rw-rw-rw-   0        0        0    15353 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_rotate.py
+-rw-rw-rw-   0        0        0     8015 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_scaling.py
+-rw-rw-rw-   0        0        0     2752 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_section.py
+-rw-rw-rw-   0        0        0    12625 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sphere.py
+-rw-rw-rw-   0        0        0    18797 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_spine.py
+-rw-rw-rw-   0        0        0    11384 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_spiral.py
+-rw-rw-rw-   0        0        0    42885 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_spline.py
+-rw-rw-rw-   0        0        0    29811 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_split.py
+-rw-rw-rw-   0        0        0     1536 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_surface_explicit.py
+-rw-rw-rw-   0        0        0     8821 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep.py
+-rw-rw-rw-   0        0        0    48206 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_circle.py
+-rw-rw-rw-   0        0        0    36668 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_conic.py
+-rw-rw-rw-   0        0        0    61549 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_explicit.py
+-rw-rw-rw-   0        0        0    83811 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_line.py
+-rw-rw-rw-   0        0        0     6611 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_symmetry.py
+-rw-rw-rw-   0        0        0     6239 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_thickness.py
+-rw-rw-rw-   0        0        0     5664 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_transfer.py
+-rw-rw-rw-   0        0        0    15253 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_translate.py
+-rw-rw-rw-   0        0        0    41726 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_trim.py
+-rw-rw-rw-   0        0        0    18247 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_unfold.py
+-rw-rw-rw-   0        0        0     1529 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_volume_explicit.py
+-rw-rw-rw-   0        0        0    25152 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_curve.py
+-rw-rw-rw-   0        0        0     6152 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_surface.py
+-rw-rw-rw-   0        0        0     9447 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/line.py
+-rw-rw-rw-   0        0        0    15721 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/plane.py
+-rw-rw-rw-   0        0        0     4397 2024-04-22 07:18:08.000000 pycatia-0.6.9/pycatia/hybrid_shape_interfaces/point.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.831768 pycatia-0.6.9/pycatia/in_interfaces/
+-rw-rw-rw-   0        0        0       21 2022-04-12 12:15:17.000000 pycatia-0.6.9/pycatia/in_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    44619 2024-05-20 09:23:48.000000 pycatia-0.6.9/pycatia/in_interfaces/application.py
+-rw-rw-rw-   0        0        0     2526 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/camera.py
+-rw-rw-rw-   0        0        0     2750 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/camera_2d.py
+-rw-rw-rw-   0        0        0     2788 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/in_interfaces/camera_3d.py
+-rw-rw-rw-   0        0        0     6518 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/cameras.py
+-rw-rw-rw-   0        0        0    15339 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/cgr_adhesion_setting_att.py
+-rw-rw-rw-   0        0        0    35762 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/in_interfaces/document.py
+-rw-rw-rw-   0        0        0    18815 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/documentation_setting_att.py
+-rw-rw-rw-   0        0        0    13068 2024-05-20 09:23:15.000000 pycatia-0.6.9/pycatia/in_interfaces/documents.py
+-rw-rw-rw-   0        0        0     4496 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/drafting_page_setup.py
+-rw-rw-rw-   0        0        0     4029 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/file.py
+-rw-rw-rw-   0        0        0     3238 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/file_component.py
+-rw-rw-rw-   0        0        0    18372 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/file_system.py
+-rw-rw-rw-   0        0        0     3353 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/files.py
+-rw-rw-rw-   0        0        0     3070 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/folder.py
+-rw-rw-rw-   0        0        0     3456 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/folders.py
+-rw-rw-rw-   0        0        0    23020 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/general_session_setting_att.py
+-rw-rw-rw-   0        0        0     4964 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/light_source.py
+-rw-rw-rw-   0        0        0     5202 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/light_sources.py
+-rw-rw-rw-   0        0        0    17013 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/macros_setting_att.py
+-rw-rw-rw-   0        0        0     5189 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/move.py
+-rw-rw-rw-   0        0        0     1524 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/in_interfaces/page_setup.py
+-rw-rw-rw-   0        0        0     6667 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/position.py
+-rw-rw-rw-   0        0        0     5030 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/printer.py
+-rw-rw-rw-   0        0        0     3408 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/printers.py
+-rw-rw-rw-   0        0        0    32920 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/printers_setting_att.py
+-rw-rw-rw-   0        0        0     3855 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/reference.py
+-rw-rw-rw-   0        0        0     3391 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/references.py
+-rw-rw-rw-   0        0        0    21443 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/search_setting_att.py
+-rw-rw-rw-   0        0        0    14907 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/selected_element.py
+-rw-rw-rw-   0        0        0   120206 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/selection.py
+-rw-rw-rw-   0        0        0     8395 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/selection_sets.py
+-rw-rw-rw-   0        0        0    16122 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/send_to_service.py
+-rw-rw-rw-   0        0        0     2870 2024-04-22 10:41:42.000000 pycatia-0.6.9/pycatia/in_interfaces/setting_controllers.py
+-rw-rw-rw-   0        0        0     3841 2023-10-31 11:15:13.000000 pycatia-0.6.9/pycatia/in_interfaces/specs_and_geom_window.py
+-rw-rw-rw-   0        0        0     2617 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/specs_viewer.py
+-rw-rw-rw-   0        0        0     7920 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/system_configuration.py
+-rw-rw-rw-   0        0        0     6466 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/text_stream.py
+-rw-rw-rw-   0        0        0    37903 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/tree_viz_manip_setting_att.py
+-rw-rw-rw-   0        0        0    12781 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/in_interfaces/viewer.py
+-rw-rw-rw-   0        0        0     2328 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/viewer_2d.py
+-rw-rw-rw-   0        0        0    15660 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/in_interfaces/viewer_3d.py
+-rw-rw-rw-   0        0        0     3400 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/viewers.py
+-rw-rw-rw-   0        0        0     5770 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/viewpoint_2d.py
+-rw-rw-rw-   0        0        0    15085 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/in_interfaces/viewpoint_3d.py
+-rw-rw-rw-   0        0        0    45275 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/vis_property_set.py
+-rw-rw-rw-   0        0        0   236225 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/visualization_setting_att.py
+-rw-rw-rw-   0        0        0    31699 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/vrml_setting_att.py
+-rw-rw-rw-   0        0        0    14902 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/in_interfaces/window.py
+-rw-rw-rw-   0        0        0     4413 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/in_interfaces/windows.py
+-rw-rw-rw-   0        0        0     1411 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/in_interfaces/workbench.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.847785 pycatia-0.6.9/pycatia/kinematics_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:07.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9162 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/dressup.py
+-rw-rw-rw-   0        0        0     9843 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/dressups.py
+-rw-rw-rw-   0        0        0     4495 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/joint.py
+-rw-rw-rw-   0        0        0     5984 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/joints.py
+-rw-rw-rw-   0        0        0     2407 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/kinematics_workbench.py
+-rw-rw-rw-   0        0        0    18786 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/mechanism.py
+-rw-rw-rw-   0        0        0     3544 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/mechanism_command.py
+-rw-rw-rw-   0        0        0     6722 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/mechanism_commands.py
+-rw-rw-rw-   0        0        0     6308 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/kinematics_interfaces/mechanisms.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.918056 pycatia-0.6.9/pycatia/knowledge_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1927 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/angle.py
+-rw-rw-rw-   0        0        0     2690 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/bool_param.py
+-rw-rw-rw-   0        0        0     3421 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/check.py
+-rw-rw-rw-   0        0        0     1953 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/constraint_satisfaction.py
+-rw-rw-rw-   0        0        0     9573 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/design_table.py
+-rw-rw-rw-   0        0        0     3498 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/dimension.py
+-rw-rw-rw-   0        0        0     2343 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/enum_param.py
+-rw-rw-rw-   0        0        0     4544 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/feature_generator.py
+-rw-rw-rw-   0        0        0     2958 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/formula.py
+-rw-rw-rw-   0        0        0     4000 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/free_parameter.py
+-rw-rw-rw-   0        0        0     4638 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/free_parameters.py
+-rw-rw-rw-   0        0        0    10652 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/int_param.py
+-rw-rw-rw-   0        0        0     3767 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/knowledge_activate_object.py
+-rw-rw-rw-   0        0        0     2397 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/knowledge_object.py
+-rw-rw-rw-   0        0        0    39344 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/knowledge_sheet_setting_att.py
+-rw-rw-rw-   0        0        0    14348 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/language_sheet_setting_att.py
+-rw-rw-rw-   0        0        0     2853 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/law.py
+-rw-rw-rw-   0        0        0     2040 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/length.py
+-rw-rw-rw-   0        0        0     6890 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/list.py
+-rw-rw-rw-   0        0        0     1743 2023-10-31 11:15:14.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/list_parameter.py
+-rw-rw-rw-   0        0        0     1479 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/loop.py
+-rw-rw-rw-   0        0        0    11560 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/optimization.py
+-rw-rw-rw-   0        0        0     3504 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/optimization_constraint.py
+-rw-rw-rw-   0        0        0     5210 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/optimization_constraints.py
+-rw-rw-rw-   0        0        0     5475 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/optimizations.py
+-rw-rw-rw-   0        0        0    12872 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/parameter.py
+-rw-rw-rw-   0        0        0     3086 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/parameter_set.py
+-rw-rw-rw-   0        0        0     4887 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/parameter_sets.py
+-rw-rw-rw-   0        0        0    22463 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/parameters.py
+-rw-rw-rw-   0        0        0    14637 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/real_param.py
+-rw-rw-rw-   0        0        0     9594 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/relation.py
+-rw-rw-rw-   0        0        0    26399 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/relations.py
+-rw-rw-rw-   0        0        0    50792 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/report_generation_sheet_setting_att.py
+-rw-rw-rw-   0        0        0     2647 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/rule.py
+-rw-rw-rw-   0        0        0    10875 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/set_of_equation.py
+-rw-rw-rw-   0        0        0     6820 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/str_param.py
+-rw-rw-rw-   0        0        0    25272 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/tolerance_sheet_setting_att.py
+-rw-rw-rw-   0        0        0     5525 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/unit.py
+-rw-rw-rw-   0        0        0     3193 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/units.py
+-rw-rw-rw-   0        0        0    32738 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/knowledge_interfaces/units_sheet_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:46.996419 pycatia-0.6.9/pycatia/manufacturing_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    11810 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/machining_process.py
+-rw-rw-rw-   0        0        0     5064 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_activities.py
+-rw-rw-rw-   0        0        0    22355 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_activity.py
+-rw-rw-rw-   0        0        0     2559 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_activity_syntax.py
+-rw-rw-rw-   0        0        0     1780 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_activity_syntax2.py
+-rw-rw-rw-   0        0        0     1501 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_apt_generator.py
+-rw-rw-rw-   0        0        0    12195 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_copy_transformation.py
+-rw-rw-rw-   0        0        0     2104 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_factories.py
+-rw-rw-rw-   0        0        0     2501 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_feature.py
+-rw-rw-rw-   0        0        0     3127 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_features.py
+-rw-rw-rw-   0        0        0    16648 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_generator_data.py
+-rw-rw-rw-   0        0        0     5055 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_hole.py
+-rw-rw-rw-   0        0        0     8059 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_insert.py
+-rw-rw-rw-   0        0        0    18105 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machinable_area.py
+-rw-rw-rw-   0        0        0     4081 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machinable_feature.py
+-rw-rw-rw-   0        0        0    36090 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machinable_geometry.py
+-rw-rw-rw-   0        0        0    24584 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machine.py
+-rw-rw-rw-   0        0        0    14731 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machining_axis.py
+-rw-rw-rw-   0        0        0    79105 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_operation.py
+-rw-rw-rw-   0        0        0     7207 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_output.py
+-rw-rw-rw-   0        0        0    11452 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_output_generator.py
+-rw-rw-rw-   0        0        0    21291 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_pattern.py
+-rw-rw-rw-   0        0        0     2467 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_precedence.py
+-rw-rw-rw-   0        0        0     4868 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_precedences.py
+-rw-rw-rw-   0        0        0     2123 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_process.py
+-rw-rw-rw-   0        0        0    25894 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_program.py
+-rw-rw-rw-   0        0        0     2560 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_resource_factory.py
+-rw-rw-rw-   0        0        0    50976 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_setup.py
+-rw-rw-rw-   0        0        0     2508 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_setup2.py
+-rw-rw-rw-   0        0        0     2631 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_setup3.py
+-rw-rw-rw-   0        0        0    16460 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool.py
+-rw-rw-rw-   0        0        0    13545 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_assembly.py
+-rw-rw-rw-   0        0        0     2960 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_assembly2.py
+-rw-rw-rw-   0        0        0     5907 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_corrector.py
+-rw-rw-rw-   0        0        0    11361 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_motion.py
+-rw-rw-rw-   0        0        0     4056 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_motions.py
+-rw-rw-rw-   0        0        0     2146 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_user_representation.py
+-rw-rw-rw-   0        0        0     5236 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_view.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.085991 pycatia-0.6.9/pycatia/mec_mod_interfaces/
+-rw-rw-rw-   0        0        0       21 2022-04-12 12:15:17.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    41134 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/axis_system.py
+-rw-rw-rw-   0        0        0     4569 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/axis_systems.py
+-rw-rw-rw-   0        0        0     3400 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/bi_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     4327 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/bodies.py
+-rw-rw-rw-   0        0        0     9221 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/body.py
+-rw-rw-rw-   0        0        0     5009 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/boundary.py
+-rw-rw-rw-   0        0        0    25561 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/constraint.py
+-rw-rw-rw-   0        0        0    12572 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/constraints.py
+-rw-rw-rw-   0        0        0     6074 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/cylindrical_face.py
+-rw-rw-rw-   0        0        0     3567 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/edge.py
+-rw-rw-rw-   0        0        0     3144 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/face.py
+-rw-rw-rw-   0        0        0     1206 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/factory.py
+-rw-rw-rw-   0        0        0    12845 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/fix_together.py
+-rw-rw-rw-   0        0        0     5880 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/fix_togethers.py
+-rw-rw-rw-   0        0        0     3883 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/geometric_elements.py
+-rw-rw-rw-   0        0        0     4868 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_bodies.py
+-rw-rw-rw-   0        0        0     8830 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_body.py
+-rw-rw-rw-   0        0        0     4473 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_shape.py
+-rw-rw-rw-   0        0        0    15797 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_shape_instance.py
+-rw-rw-rw-   0        0        0     4496 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_shapes.py
+-rw-rw-rw-   0        0        0    16415 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/instance_factory.py
+-rw-rw-rw-   0        0        0     2060 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/mono_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     2249 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/not_wire_boundary_mono_dim_feat_vertex.py
+-rw-rw-rw-   0        0        0     7987 2024-01-13 13:43:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/ordered_geometrical_set.py
+-rw-rw-rw-   0        0        0     5249 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/ordered_geometrical_sets.py
+-rw-rw-rw-   0        0        0     3835 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/origin_elements.py
+-rw-rw-rw-   0        0        0    35366 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/part.py
+-rw-rw-rw-   0        0        0     3350 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/part_document.py
+-rw-rw-rw-   0        0        0   228006 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/part_infrastructure_setting_att.py
+-rw-rw-rw-   0        0        0     9106 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/planar_face.py
+-rw-rw-rw-   0        0        0     5802 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/rectilinear_bi_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     5880 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/rectilinear_mono_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     7577 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/rectilinear_tri_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     1455 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/shape.py
+-rw-rw-rw-   0        0        0    15513 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/shape_instance.py
+-rw-rw-rw-   0        0        0     4205 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/shapes.py
+-rw-rw-rw-   0        0        0     5520 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/sketches.py
+-rw-rw-rw-   0        0        0     4615 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/solid.py
+-rw-rw-rw-   0        0        0     2895 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/tri_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     2121 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/tri_dim_feat_vertex_or_bi_dim_feat_vertex.py
+-rw-rw-rw-   0        0        0     3661 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/vertex.py
+-rw-rw-rw-   0        0        0     2201 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/mec_mod_interfaces/zero_dim_feat_vertex_or_wire_boundary_mono_dim_feat_vertex.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.089491 pycatia-0.6.9/pycatia/multi_cad_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/multi_cad_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    77496 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/multi_cad_interfaces/multi_cad_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.123627 pycatia-0.6.9/pycatia/navigator_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.6.9/pycatia/navigator_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    16753 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/navigator_interfaces/annotated_view.py
+-rw-rw-rw-   0        0        0     7991 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/navigator_interfaces/annotated_views.py
+-rw-rw-rw-   0        0        0     5860 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/navigator_interfaces/dmu_data_flow.py
+-rw-rw-rw-   0        0        0     3392 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/navigator_interfaces/dmu_review.py
+-rw-rw-rw-   0        0        0     8226 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/navigator_interfaces/dmu_reviews.py
+-rw-rw-rw-   0        0        0    15462 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/navigator_interfaces/group.py
+-rw-rw-rw-   0        0        0     7702 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/navigator_interfaces/groups.py
+-rw-rw-rw-   0        0        0     5397 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/navigator_interfaces/hyperlink.py
+-rw-rw-rw-   0        0        0     7680 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/navigator_interfaces/hyperlinks.py
+-rw-rw-rw-   0        0        0    16990 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/navigator_interfaces/marker_2D.py
+-rw-rw-rw-   0        0        0    18553 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/navigator_interfaces/marker_2Ds.py
+-rw-rw-rw-   0        0        0    21192 2023-10-31 11:15:15.000000 pycatia-0.6.9/pycatia/navigator_interfaces/marker_3D.py
+-rw-rw-rw-   0        0        0     8999 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/navigator_interfaces/marker_3Ds.py
+-rw-rw-rw-   0        0        0    70516 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/navigator_interfaces/marker_setting_att.py
+-rw-rw-rw-   0        0        0   194067 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/navigator_interfaces/n_4D_navigator_setting_att.py
+-rw-rw-rw-   0        0        0    15253 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/navigator_interfaces/navigator_workbench.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.138165 pycatia-0.6.9/pycatia/osm_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/osm_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     6467 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/osm_interfaces/product_scene.py
+-rw-rw-rw-   0        0        0     8382 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/osm_interfaces/product_scenes.py
+-rw-rw-rw-   0        0        0    15967 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/osm_interfaces/scene.py
+-rw-rw-rw-   0        0        0    11312 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/osm_interfaces/scene_product_data.py
+-rw-rw-rw-   0        0        0     2302 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/osm_interfaces/scene_workbench.py
+-rw-rw-rw-   0        0        0     5879 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/osm_interfaces/scenes.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.291321 pycatia-0.6.9/pycatia/part_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.6.9/pycatia/part_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/add.py
+-rw-rw-rw-   0        0        0     3056 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/affinity.py
+-rw-rw-rw-   0        0        0     3429 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/angular_repartition.py
+-rw-rw-rw-   0        0        0     1542 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/assemble.py
+-rw-rw-rw-   0        0        0     7032 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/part_interfaces/auto_draft.py
+-rw-rw-rw-   0        0        0    11198 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/part_interfaces/auto_fillet.py
+-rw-rw-rw-   0        0        0     3100 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/axis_to_axis.py
+-rw-rw-rw-   0        0        0     4941 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/boolean_shape.py
+-rw-rw-rw-   0        0        0    12608 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/chamfer.py
+-rw-rw-rw-   0        0        0    20985 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/circ_pattern.py
+-rw-rw-rw-   0        0        0    20843 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/close_surface.py
+-rw-rw-rw-   0        0        0     7727 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/const_rad_edge_fillet.py
+-rw-rw-rw-   0        0        0     2876 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/defeaturing.py
+-rw-rw-rw-   0        0        0     1450 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/defeaturing_fillet_filter.py
+-rw-rw-rw-   0        0        0     1220 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/defeaturing_filter.py
+-rw-rw-rw-   0        0        0    16213 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/defeaturing_filter_with_range.py
+-rw-rw-rw-   0        0        0     5861 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/part_interfaces/defeaturing_filters.py
+-rw-rw-rw-   0        0        0     1440 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/defeaturing_hole_filter.py
+-rw-rw-rw-   0        0        0     4428 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/draft.py
+-rw-rw-rw-   0        0        0    17421 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/draft_domain.py
+-rw-rw-rw-   0        0        0     3318 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/part_interfaces/draft_domains.py
+-rw-rw-rw-   0        0        0     1559 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/dress_up_shape.py
+-rw-rw-rw-   0        0        0     8016 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/edge_fillet.py
+-rw-rw-rw-   0        0        0     4556 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/face_fillet.py
+-rw-rw-rw-   0        0        0     4292 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/fillet.py
+-rw-rw-rw-   0        0        0     1679 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/groove.py
+-rw-rw-rw-   0        0        0    29826 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/hole.py
+-rw-rw-rw-   0        0        0     2066 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/intersect.py
+-rw-rw-rw-   0        0        0     3436 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/limit.py
+-rw-rw-rw-   0        0        0     2599 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/linear_repartition.py
+-rw-rw-rw-   0        0        0     2427 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/loft.py
+-rw-rw-rw-   0        0        0     3339 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/mirror.py
+-rw-rw-rw-   0        0        0     1565 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/pad.py
+-rw-rw-rw-   0        0        0     5399 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/pattern.py
+-rw-rw-rw-   0        0        0     1658 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/pocket.py
+-rw-rw-rw-   0        0        0    15979 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/prism.py
+-rw-rw-rw-   0        0        0    22607 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/rect_pattern.py
+-rw-rw-rw-   0        0        0     1399 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/remove.py
+-rw-rw-rw-   0        0        0     7521 2024-04-22 08:34:55.000000 pycatia-0.6.9/pycatia/part_interfaces/remove_face.py
+-rw-rw-rw-   0        0        0     2246 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/repartition.py
+-rw-rw-rw-   0        0        0     6879 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/replace_face.py
+-rw-rw-rw-   0        0        0     8493 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/revolution.py
+-rw-rw-rw-   0        0        0     1588 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/rib.py
+-rw-rw-rw-   0        0        0     5134 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/rotate.py
+-rw-rw-rw-   0        0        0     3573 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/scaling.py
+-rw-rw-rw-   0        0        0     4394 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/scaling2.py
+-rw-rw-rw-   0        0        0    10154 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/sew_surface.py
+-rw-rw-rw-   0        0        0     1671 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/shaft.py
+-rw-rw-rw-   0        0        0   160466 2024-04-22 10:42:29.000000 pycatia-0.6.9/pycatia/part_interfaces/shape_factory.py
+-rw-rw-rw-   0        0        0    13547 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/shell.py
+-rw-rw-rw-   0        0        0     3690 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/sketch_based_shape.py
+-rw-rw-rw-   0        0        0     1677 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/slot.py
+-rw-rw-rw-   0        0        0     6417 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/solid_combine.py
+-rw-rw-rw-   0        0        0     2701 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/split.py
+-rw-rw-rw-   0        0        0     7217 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/stiffener.py
+-rw-rw-rw-   0        0        0     2155 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/surface_based_shape.py
+-rw-rw-rw-   0        0        0    12355 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/sweep.py
+-rw-rw-rw-   0        0        0     2746 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/symmetry.py
+-rw-rw-rw-   0        0        0     4776 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/thick_surface.py
+-rw-rw-rw-   0        0        0    12437 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/thickness.py
+-rw-rw-rw-   0        0        0    12759 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/thread.py
+-rw-rw-rw-   0        0        0     1609 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/part_interfaces/transformation_shape.py
+-rw-rw-rw-   0        0        0     2817 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/translate.py
+-rw-rw-rw-   0        0        0    18816 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/trim.py
+-rw-rw-rw-   0        0        0     5254 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/tritangent_fillet.py
+-rw-rw-rw-   0        0        0     4375 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/user_pattern.py
+-rw-rw-rw-   0        0        0     3530 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/user_repartition.py
+-rw-rw-rw-   0        0        0    16057 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/part_interfaces/var_rad_edge_fillet.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.302852 pycatia-0.6.9/pycatia/pcb_board_base/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/pcb_board_base/__init__.py
+-rw-rw-rw-   0        0        0     6487 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/pcb_board_base/pcb_area.py
+-rw-rw-rw-   0        0        0    12427 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/pcb_board_base/pcb_board.py
+-rw-rw-rw-   0        0        0     8570 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/pcb_board_base/pcb_component.py
+-rw-rw-rw-   0        0        0     5251 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/pcb_board_base/pcb_hole_and_pattern.py
+-rw-rw-rw-   0        0        0     2786 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/pcb_board_base/pcb_object.py
+-rw-rw-rw-   0        0        0     6278 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/pcb_board_base/pcb_workbench.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.309865 pycatia-0.6.9/pycatia/ppr_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/ppr_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3301 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/ppr_interfaces/ppr_activity.py
+-rw-rw-rw-   0        0        0     4201 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/ppr_interfaces/ppr_document.py
+-rw-rw-rw-   0        0        0     2989 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/ppr_interfaces/ppr_products.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.312880 pycatia-0.6.9/pycatia/prismatic_machining_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/prismatic_machining_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    28065 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/prismatic_machining_interfaces/manufacturing_prismatic_machining_area.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.326902 pycatia-0.6.9/pycatia/product_structure_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/product_structure_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     8618 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/product_structure_interfaces/analyze.py
+-rw-rw-rw-   0        0        0     4851 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/product_structure_interfaces/assembly_convertor.py
+-rw-rw-rw-   0        0        0    55459 2024-01-17 11:05:50.000000 pycatia-0.6.9/pycatia/product_structure_interfaces/product.py
+-rw-rw-rw-   0        0        0     2726 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/product_structure_interfaces/product_document.py
+-rw-rw-rw-   0        0        0    17080 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/product_structure_interfaces/products.py
+-rw-rw-rw-   0        0        0     3536 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/product_structure_interfaces/publication.py
+-rw-rw-rw-   0        0        0     9888 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/product_structure_interfaces/publications.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.329913 pycatia-0.6.9/pycatia/reporter_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/reporter_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2913 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/reporter_interfaces/rpm_report.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.337434 pycatia-0.6.9/pycatia/scripts/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/scripts/__init__.py
+-rw-rw-rw-   0        0        0      388 2022-04-12 12:15:17.000000 pycatia-0.6.9/pycatia/scripts/checking.py
+-rw-rw-rw-   0        0        0     2916 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/scripts/csv_tools.py
+-rw-rw-rw-   0        0        0      289 2024-04-22 07:18:56.000000 pycatia-0.6.9/pycatia/scripts/vba.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.340454 pycatia-0.6.9/pycatia/simulation_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/simulation_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9391 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/simulation_interfaces/replay.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.367509 pycatia-0.6.9/pycatia/sketcher_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2778 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/axis_2D.py
+-rw-rw-rw-   0        0        0     5198 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/circle_2D.py
+-rw-rw-rw-   0        0        0     5365 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/control_point_2D.py
+-rw-rw-rw-   0        0        0    17189 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/curve_2D.py
+-rw-rw-rw-   0        0        0     8690 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/ellipse_2D.py
+-rw-rw-rw-   0        0        0    20597 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/factory_2D.py
+-rw-rw-rw-   0        0        0     1879 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/geometric_element.py
+-rw-rw-rw-   0        0        0     2614 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/geometry_2D.py
+-rw-rw-rw-   0        0        0     6669 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/hyperbola_2D.py
+-rw-rw-rw-   0        0        0     5130 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/line_2D.py
+-rw-rw-rw-   0        0        0     5831 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/parabola_2D.py
+-rw-rw-rw-   0        0        0     3186 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/point_2D.py
+-rw-rw-rw-   0        0        0    13438 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/sketch.py
+-rw-rw-rw-   0        0        0     5320 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/sketcher_interfaces/spline_2D.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.409122 pycatia-0.6.9/pycatia/smt_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/smt_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1281 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/smt_interfaces/dmo_offset.py
+-rw-rw-rw-   0        0        0    13612 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/dmo_offsets.py
+-rw-rw-rw-   0        0        0     1296 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/smt_interfaces/dmo_thickness.py
+-rw-rw-rw-   0        0        0    12803 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/dmo_thicknesses.py
+-rw-rw-rw-   0        0        0     3051 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/free_space.py
+-rw-rw-rw-   0        0        0     9863 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/free_spaces.py
+-rw-rw-rw-   0        0        0     3901 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/merges.py
+-rw-rw-rw-   0        0        0     6882 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/optimizer_work_bench.py
+-rw-rw-rw-   0        0        0     1168 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/smt_interfaces/part_comp.py
+-rw-rw-rw-   0        0        0     6318 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/part_comps.py
+-rw-rw-rw-   0        0        0     1290 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/smt_interfaces/silhouette.py
+-rw-rw-rw-   0        0        0     8446 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/silhouettes.py
+-rw-rw-rw-   0        0        0     4739 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/simplifications.py
+-rw-rw-rw-   0        0        0     1295 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/smt_interfaces/swept_volume.py
+-rw-rw-rw-   0        0        0    25945 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/swept_volumes.py
+-rw-rw-rw-   0        0        0    14549 2024-01-13 13:43:56.000000 pycatia-0.6.9/pycatia/smt_interfaces/three_d_cuts.py
+-rw-rw-rw-   0        0        0    10615 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/vibration_volumes.py
+-rw-rw-rw-   0        0        0     1282 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/smt_interfaces/wrapping.py
+-rw-rw-rw-   0        0        0     8534 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/smt_interfaces/wrappings.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.444510 pycatia-0.6.9/pycatia/space_analyses_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    12149 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/clash.py
+-rw-rw-rw-   0        0        0     3358 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/clash_result.py
+-rw-rw-rw-   0        0        0     7004 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/clash_results.py
+-rw-rw-rw-   0        0        0     6697 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/clashes.py
+-rw-rw-rw-   0        0        0    11514 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/conflict.py
+-rw-rw-rw-   0        0        0     3119 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/conflicts.py
+-rw-rw-rw-   0        0        0    19991 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/distance.py
+-rw-rw-rw-   0        0        0     7026 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/distances.py
+-rw-rw-rw-   0        0        0      227 2022-04-12 12:15:17.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/general_functions.py
+-rw-rw-rw-   0        0        0    14289 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/inertia.py
+-rw-rw-rw-   0        0        0     6456 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/inertias.py
+-rw-rw-rw-   0        0        0    25428 2024-02-22 13:04:44.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/measurable.py
+-rw-rw-rw-   0        0        0    28190 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/measure_setting_att.py
+-rw-rw-rw-   0        0        0    20050 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/section.py
+-rw-rw-rw-   0        0        0    80468 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/sectioning_setting_att.py
+-rw-rw-rw-   0        0        0     6942 2024-03-17 16:28:56.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/sections.py
+-rw-rw-rw-   0        0        0     7946 2023-11-08 17:25:46.000000 pycatia-0.6.9/pycatia/space_analyses_interfaces/spa_workbench.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.487809 pycatia-0.6.9/pycatia/structure_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/structure_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    11665 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/structure_interfaces/colour_ess_object_setting_att.py
+-rw-rw-rw-   0        0        0    11489 2023-10-31 11:15:16.000000 pycatia-0.6.9/pycatia/structure_interfaces/colour_std_object_setting_att.py
+-rw-rw-rw-   0        0        0    10128 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/material_ess_object_setting_att.py
+-rw-rw-rw-   0        0        0    14843 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/path_ess_resources_setting_att.py
+-rw-rw-rw-   0        0        0     7880 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/ppg_exec_log_setting_att.py
+-rw-rw-rw-   0        0        0     3104 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_anchor_point.py
+-rw-rw-rw-   0        0        0     2854 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_anchor_points.py
+-rw-rw-rw-   0        0        0     7688 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_compute_services.py
+-rw-rw-rw-   0        0        0     2582 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_cutback.py
+-rw-rw-rw-   0        0        0     7760 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_cutout_feature.py
+-rw-rw-rw-   0        0        0    19179 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_feature_factory.py
+-rw-rw-rw-   0        0        0     1308 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_foundation.py
+-rw-rw-rw-   0        0        0     4172 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_foundations.py
+-rw-rw-rw-   0        0        0    11499 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_member.py
+-rw-rw-rw-   0        0        0     8265 2023-10-31 11:15:17.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_member_extremity.py
+-rw-rw-rw-   0        0        0     9768 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_members.py
+-rw-rw-rw-   0        0        0     4980 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_nibbling_feature.py
+-rw-rw-rw-   0        0        0     2036 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_object.py
+-rw-rw-rw-   0        0        0     1261 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_object_ext.py
+-rw-rw-rw-   0        0        0    72345 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_object_factory.py
+-rw-rw-rw-   0        0        0     4672 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_plate.py
+-rw-rw-rw-   0        0        0     9555 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_plates.py
+-rw-rw-rw-   0        0        0     7056 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_section.py
+-rw-rw-rw-   0        0        0     2206 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/str_workbench.py
+-rw-rw-rw-   0        0        0     9938 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/structure_interfaces/type_ess_object_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.492834 pycatia-0.6.9/pycatia/surface_machining_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/surface_machining_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3831 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/surface_machining_interfaces/manufacturing_surface_geom_area.py
+-rw-rw-rw-   0        0        0     4841 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/surface_machining_interfaces/manufacturing_surface_machining_area.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.537629 pycatia-0.6.9/pycatia/system_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.6.9/pycatia/system_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/accesslog_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     7643 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/system_interfaces/any_object.py
+-rw-rw-rw-   0        0        0    28964 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/cache_setting_att.py
+-rw-rw-rw-   0        0        0     1666 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/cat_base_dispatch.py
+-rw-rw-rw-   0        0        0     1530 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/cat_base_unknown.py
+-rw-rw-rw-   0        0        0     8774 2024-05-20 08:53:48.000000 pycatia-0.6.9/pycatia/system_interfaces/collection.py
+-rw-rw-rw-   0        0        0     1901 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/command_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     7521 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/disconnection_setting_att.py
+-rw-rw-rw-   0        0        0    23652 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/dl_name_setting_att.py
+-rw-rw-rw-   0        0        0    12275 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/dyn_license_setting_att.py
+-rw-rw-rw-   0        0        0     9646 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/errorlog_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     1920 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/file_access_statistics_setting_att.py
+-rw-rw-rw-   0        0        0    21080 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/general_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     7896 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/global_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     1257 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/i_dispatch.py
+-rw-rw-rw-   0        0        0     1147 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/i_unknown.py
+-rw-rw-rw-   0        0        0    29377 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/license_setting_att.py
+-rw-rw-rw-   0        0        0    10573 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/memory_warning_setting_att.py
+-rw-rw-rw-   0        0        0     2732 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/pcs_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     1895 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/server_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     1901 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/session_statistics_setting_att.py
+-rw-rw-rw-   0        0        0    12823 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/setting_controller.py
+-rw-rw-rw-   0        0        0    13615 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/setting_repository.py
+-rw-rw-rw-   0        0        0    12861 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/system_interfaces/system_service.py
+-rw-rw-rw-   0        0        0     1914 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/system_interfaces/workbench_statistics_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.540644 pycatia-0.6.9/pycatia/threed_xml_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-05 09:15:08.000000 pycatia-0.6.9/pycatia/threed_xml_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    61791 2023-10-31 11:15:18.000000 pycatia-0.6.9/pycatia/threed_xml_interfaces/export_3d_xml_setting_att.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.545651 pycatia-0.6.9/pycatia/types/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.6.9/pycatia/types/__init__.py
+-rw-rw-rw-   0        0        0     1981 2024-05-20 09:10:03.000000 pycatia-0.6.9/pycatia/types/document.py
+-rw-rw-rw-   0        0        0      566 2024-02-26 15:55:40.000000 pycatia-0.6.9/pycatia/types/general.py
+-rw-rw-rw-   0        0        0       19 2024-05-10 08:01:01.000000 pycatia-0.6.9/pycatia/version.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:16:47.547650 pycatia-0.6.9/pycatia.egg-info/
+-rw-rw-rw-   0        0        0     5291 2024-05-20 10:16:44.000000 pycatia-0.6.9/pycatia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    62628 2024-05-20 10:16:45.000000 pycatia-0.6.9/pycatia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 10:16:44.000000 pycatia-0.6.9/pycatia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 10:16:44.000000 pycatia-0.6.9/pycatia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 10:16:44.000000 pycatia-0.6.9/pycatia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 10:16:47.550163 pycatia-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-05-01 08:31:08.000000 pycatia-0.6.9/setup.py
```

### Comparing `pycatia-0.6.8/LICENSE.txt` & `pycatia-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/PKG-INFO` & `pycatia-0.6.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatia
-Version: 0.6.8
+Version: 0.6.9
 Summary: A python module to interface with the CATIA V5 COM object.
 Home-page: https://github.com/evereux/pycatia
 Author: Paul Bourne
 Author-email: evereux@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,15 @@
 
 .. _pycatia.readthedocs.io: https://pycatia.readthedocs.io
 .. _installation: https://pycatia.readthedocs.io/en/latest/installation.html
 .. _introduction: https://pycatia.readthedocs.io/en/latest/introduction.html
 .. _examples: https://pycatia.readthedocs.io/en/latest/examples.html
 .. _user_scripts: https://pycatia.readthedocs.io/en/latest/user_scripts.html
 .. _pypi.org: https://pypi.org/project/pycatia/
+.. _pycatia-tools: https://github.com/evereux/pycatia-tools
 
 pycatia
 =======
 
 alpha software
 --------------
 
@@ -93,14 +94,16 @@
 
 
 Examples And Scripts
 --------------------
 
 See the documentation @ examples_ and user_scripts_.
 
+A GUI based application that uses pycatia - pycatia-tools_.
+
 
 Asking Questions
 ----------------
 
 Please read the following with regards to raising questions: https://github.com/evereux/pycatia/issues/28
```

### Comparing `pycatia-0.6.8/README.rst` & `pycatia-0.6.9/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .. _pycatia.readthedocs.io: https://pycatia.readthedocs.io
 .. _installation: https://pycatia.readthedocs.io/en/latest/installation.html
 .. _introduction: https://pycatia.readthedocs.io/en/latest/introduction.html
 .. _examples: https://pycatia.readthedocs.io/en/latest/examples.html
 .. _user_scripts: https://pycatia.readthedocs.io/en/latest/user_scripts.html
 .. _pypi.org: https://pypi.org/project/pycatia/
+.. _pycatia-tools: https://github.com/evereux/pycatia-tools
 
 pycatia
 =======
 
 alpha software
 --------------
 
@@ -77,14 +78,16 @@
 
 
 Examples And Scripts
 --------------------
 
 See the documentation @ examples_ and user_scripts_.
 
+A GUI based application that uses pycatia - pycatia-tools_.
+
 
 Asking Questions
 ----------------
 
 Please read the following with regards to raising questions: https://github.com/evereux/pycatia/issues/28
```

### Comparing `pycatia-0.6.8/pycatia/__init__.py` & `pycatia-0.6.9/pycatia/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_analysis_case.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_analysis_case.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_analysis_cases.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_analysis_cases.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_analysis_model.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_analysis_model.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_analytical_rigid_surface.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_analytical_rigid_surface.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_boundary_condition.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_boundary_condition.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_boundary_conditions.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_clamp_bc.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_clamp_bc.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_concentrated_force.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_concentrated_force.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_damper_connection_property.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_damper_connection_property.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_data_output_request.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_data_output_request.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_data_output_requests.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_data_output_requests.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_displacement_bc.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_displacement_bc.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_display_group.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_display_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_display_groups.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_display_groups.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_explicit_dynamics_step.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_explicit_dynamics_step.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_fastened_connection_enhancement.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_fastened_connection_enhancement.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_fastened_pair.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_fastened_pair.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_field_output_request.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_field_output_request.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_field_output_requests.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_field_output_requests.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_fields.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_fields.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_film_condition.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_film_condition.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_frequency_step.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_frequency_step.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_gasket_property.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_gasket_property.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_general_static_step.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_general_static_step.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_global_element_assignment.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_global_element_assignment.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_gravity.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_gravity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_heat_transfer_step.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_heat_transfer_step.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_history_output_request.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_history_output_request.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_history_output_requests.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_history_output_requests.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_image_query.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_image_query.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_initial_step.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_initial_step.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_initial_temperature.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_initial_temperature.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_interaction.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_interaction.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_interactions.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_interactions.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_job.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_job.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_jobs.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_jobs.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_load.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_load.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_loads.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_loads.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_mass_scaling.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_mass_scaling.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_mass_scalings.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_mass_scalings.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_mech_conn_behavior.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_mech_conn_behavior.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_output_request.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_output_request.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_output_requests.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_output_requests.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_pressure.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_pressure.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_pretension_property.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_pretension_property.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_properties.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_properties.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_property.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_property.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_rigid_body_constraint.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_rigid_body_constraint.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_rigid_coupling.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_rigid_coupling.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_smooth_coupling.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_smooth_coupling.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_smooth_step_amplitude.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_smooth_step_amplitude.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_case.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_case.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_case_images.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_case_images.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_step.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_step.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_step_images.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_step_images.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_solution_steps.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_solution_steps.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_spring_connection_property.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_spring_connection_property.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_step.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_step.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_steps.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_steps.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_surface_to_surface_contact.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_surface_to_surface_contact.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_tabular_amplitude.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_tabular_amplitude.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_temperature.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_temperature.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_temperature_bc.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_temperature_bc.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_temperature_history.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_temperature_history.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abq_thermal_conn_behavior.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abq_thermal_conn_behavior.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abqfh_output_request.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abqfh_output_request.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_base_motion_vb.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_base_motion_vb.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_frequency_loading_vb.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_frequency_loading_vb.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_basic_vb.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_basic_vb.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_modal_vb.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_modal_vb.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_subspace_vb.py` & `pycatia-0.6.9/pycatia/abq_automation_interfaces/abqiaabq_steady_state_lin_dyn_step_subspace_vb.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_adaptivity_manager.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_adaptivity_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_case.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_case.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_cases.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_cases.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_color_map.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_color_map.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_document.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_entities.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_entities.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_entity.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_entity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_export.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_export.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_general_setting_att.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_general_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_global_sensor.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_global_sensor.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_image.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_image.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_images.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_images.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_import.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_import.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_linked_documents.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_linked_documents.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_local_entities.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_local_entities.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_local_entity.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_local_entity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_local_sensor.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_local_sensor.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_manager.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_element.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_element.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_local_specification.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_local_specification.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_local_specifications.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_local_specifications.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_manager.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_node.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_node.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_part.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_part.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_mesh_parts.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_mesh_parts.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_model.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_model.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_models.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_models.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_output_entities.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_output_entities.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_post_manager.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_post_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_post_pro_anr_setting_att.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_post_pro_anr_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_post_pro_setting_att.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_post_pro_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_reporting_setting_att.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_reporting_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_sensor.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_sensor.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_set.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_set.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_sets.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_sets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_supports.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_supports.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/analysis_v4_services.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/analysis_v4_services.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/basic_component.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/basic_component.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/analysis_interfaces/basic_components.py` & `pycatia-0.6.9/pycatia/analysis_interfaces/basic_components.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arr_bendable_string.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arr_bendable_string.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arr_bom_report.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arr_bom_report.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arr_nomenclature.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arr_nomenclature.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arr_nomenclature_tree.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arr_nomenclature_tree.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arr_nomenclatures.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arr_nomenclatures.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arr_system_line_product.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arr_system_line_product.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arr_workbench.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arr_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_area.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_area.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_areas.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_areas.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_boundaries.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_boundaries.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_boundary.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_boundary.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_contour.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_contour.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_contours.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_contours.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_item_reservation.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_item_reservation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_item_reservations.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_item_reservations.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_node.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_node.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_nodes.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_nodes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_pathway.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_pathway.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_pathways.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_pathways.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_product.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_product.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_rectangle.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_rectangle.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_rectangles.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_rectangles.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_run.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_run.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/arrangement_interfaces/arrangement_runs.py` & `pycatia-0.6.9/pycatia/arrangement_interfaces/arrangement_runs.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/assembly_interfaces/assembly_boolean.py` & `pycatia-0.6.9/pycatia/assembly_interfaces/assembly_boolean.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/assembly_interfaces/assembly_constraint_setting_att.py` & `pycatia-0.6.9/pycatia/assembly_interfaces/assembly_constraint_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/assembly_interfaces/assembly_feature.py` & `pycatia-0.6.9/pycatia/assembly_interfaces/assembly_feature.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/assembly_interfaces/assembly_features.py` & `pycatia-0.6.9/pycatia/assembly_interfaces/assembly_features.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/assembly_interfaces/assembly_general_setting_att.py` & `pycatia-0.6.9/pycatia/assembly_interfaces/assembly_general_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/assembly_interfaces/assembly_hole.py` & `pycatia-0.6.9/pycatia/assembly_interfaces/assembly_hole.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/assembly_interfaces/assembly_pocket.py` & `pycatia-0.6.9/pycatia/assembly_interfaces/assembly_pocket.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/assembly_interfaces/assembly_split.py` & `pycatia-0.6.9/pycatia/assembly_interfaces/assembly_split.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/base_interfaces/context.py` & `pycatia-0.6.9/pycatia/base_interfaces/context.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/behavior_interfaces/behavior.py` & `pycatia-0.6.9/pycatia/behavior_interfaces/behavior.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/behavior_interfaces/behavior_extension.py` & `pycatia-0.6.9/pycatia/behavior_interfaces/behavior_extension.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/behavior_interfaces/behavior_vb_script.py` & `pycatia-0.6.9/pycatia/behavior_interfaces/behavior_vb_script.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/behavior_interfaces/behaviors.py` & `pycatia-0.6.9/pycatia/behavior_interfaces/behaviors.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/bkt_interfaces/behavior_setting_att.py` & `pycatia-0.6.9/pycatia/bkt_interfaces/behavior_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_dde_settings_interfaces/dxf_setting_att.py` & `pycatia-0.6.9/pycatia/cat_dde_settings_interfaces/dxf_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_dde_settings_interfaces/ig2_setting_att.py` & `pycatia-0.6.9/pycatia/cat_dde_settings_interfaces/ig2_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/e5_property.py` & `pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/e5_property.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/ipd_template_property.py` & `pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/ipd_template_property.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/mfg_hub_setting_att.py` & `pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/mfg_hub_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_ipd_adapter_interfaces/mhi_relation_management.py` & `pycatia-0.6.9/pycatia/cat_ipd_adapter_interfaces/mhi_relation_management.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_logger.py` & `pycatia-0.6.9/pycatia/cat_logger.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_mat_interfaces/analysis_material.py` & `pycatia-0.6.9/pycatia/cat_mat_interfaces/analysis_material.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_mat_interfaces/material.py` & `pycatia-0.6.9/pycatia/cat_mat_interfaces/material.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_mat_interfaces/material_document.py` & `pycatia-0.6.9/pycatia/cat_mat_interfaces/material_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_mat_interfaces/material_families.py` & `pycatia-0.6.9/pycatia/cat_mat_interfaces/material_families.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_mat_interfaces/material_family.py` & `pycatia-0.6.9/pycatia/cat_mat_interfaces/material_family.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_mat_interfaces/material_manager.py` & `pycatia-0.6.9/pycatia/cat_mat_interfaces/material_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_mat_interfaces/materials.py` & `pycatia-0.6.9/pycatia/cat_mat_interfaces/materials.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_mat_interfaces/positioned_material.py` & `pycatia-0.6.9/pycatia/cat_mat_interfaces/positioned_material.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_app_factory.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_app_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_application.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_application.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_attribute.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_attribute.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_attribute_report.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_attribute_report.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_build_part.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_build_part.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_class.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_class.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_cntr_flow.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_cntr_flow.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_connectable.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_connectable.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_connector.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_connector.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_functional.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_functional.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_group.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_groupable.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_groupable.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_id.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_id.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_light_bend.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_light_bend.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_light_connector.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_light_connector.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_light_part.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_light_part.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_list_of_bstrs.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_list_of_bstrs.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_list_of_doubles.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_list_of_doubles.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_list_of_longs.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_list_of_longs.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_list_of_objects.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_list_of_objects.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_logical_line.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_logical_line.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_object.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_part_connector.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_part_connector.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_phsyical_product.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_phsyical_product.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_physical.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_physical.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_place_part.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_place_part.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_resource.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_resource.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_spatial.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_spatial.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_stretchable_data.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_stretchable_data.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_temp_list_factory.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_temp_list_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_plant_ship_interfaces/psp_workbench.py` & `pycatia-0.6.9/pycatia/cat_plant_ship_interfaces/psp_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rdg_interfaces/rendering_setting_att.py` & `pycatia-0.6.9/pycatia/cat_rdg_interfaces/rendering_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rma_interfaces/rendering_material.py` & `pycatia-0.6.9/pycatia/cat_rma_interfaces/rendering_material.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_environment.py` & `pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_environment.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_environment_wall.py` & `pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_environment_wall.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_environments.py` & `pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_environments.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_light.py` & `pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_light.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_lights.py` & `pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_lights.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_shooting.py` & `pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_shooting.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_rsc_interfaces/rendering_shootings.py` & `pycatia-0.6.9/pycatia/cat_rsc_interfaces/rendering_shootings.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_annotation_break.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_annotation_break.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_2d_zone_from_3d_zone.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_2d_zone_from_3d_zone.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_class.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_class.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_colour.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_colour.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_data.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_data.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_doc_link.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_doc_link.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_flow.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_flow.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_name.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_name.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_cntr_show.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_cntr_show.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_compatible.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_compatible.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_component.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_component.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_connectable.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_connectable.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_connection.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_connection.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_connector.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_connector.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_delete_check.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_delete_check.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_delete_check2.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_delete_check2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_environment.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_environment.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_gap_priority.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_gap_priority.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_group.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_model_init.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_model_init.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_multi_image.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_multi_image.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_multi_image_master.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_multi_image_master.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_object_factory.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_object_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_object_factory2.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_object_factory2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_replace.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_replace.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_route.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_route.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_route2.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_route2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_scaling_rule.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_scaling_rule.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_app_zone.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_app_zone.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_arrow_display.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_arrow_display.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_base_factory.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_base_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_boundary_elem.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_boundary_elem.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_catalog_component.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_catalog_component.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_catalog_route.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_catalog_route.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_cntr_connect.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_cntr_connect.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_cntr_doc_link.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_cntr_doc_link.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_cntr_graphic.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_cntr_graphic.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_cntr_location.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_cntr_location.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_comp_connector.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_comp_connector.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_comp_flow.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_comp_flow.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_comp_graphic.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_comp_graphic.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_comp_group_ext.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_comp_group_ext.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_compatible.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_compatible.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_component.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_component.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_component2.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_component2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_component_group.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_component_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_connectable.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_connectable.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_drop_off_view.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_drop_off_view.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_frame_info.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_frame_info.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_gap_display.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_gap_display.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_cntr.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_cntr.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_comp.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_comp.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_factory.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_route.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_route.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_route2.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_route2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_route_alternate.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_route_alternate.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_route_ellipse.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_route_ellipse.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_grr_zone.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_grr_zone.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_internal_flow.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_internal_flow.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_list_of_bst_rs.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_list_of_bst_rs.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_list_of_doubles.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_list_of_doubles.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_list_of_longs.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_list_of_longs.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_list_of_objects.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_list_of_objects.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_movable.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_movable.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_movable2.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_movable2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_network_analysis.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_network_analysis.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_obsolete_model.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_obsolete_model.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_post_replace.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_post_replace.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_replace.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_replace.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_route.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_route.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_route_alternate_graphic.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_route_alternate_graphic.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_route_graphic.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_route_graphic.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_route_symbol.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_route_symbol.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_session.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_session.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_temp_list_factory.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_temp_list_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_update_instances.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_update_instances.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_workbench.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_zone.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_zone.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_zone_graphic.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_zone_graphic.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/sch_zone_membership.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/sch_zone_membership.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/schematic_extension.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/schematic_extension.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sch_platform_interfaces/schematic_root.py` & `pycatia-0.6.9/pycatia/cat_sch_platform_interfaces/schematic_root.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sde_setting_interfaces/step_setting_att.py` & `pycatia-0.6.9/pycatia/cat_sde_setting_interfaces/step_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sm_interfaces/catalog_shm_object_setting_att.py` & `pycatia-0.6.9/pycatia/cat_sm_interfaces/catalog_shm_object_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_sm_interfaces/view_characteristic_curves_setting_att.py` & `pycatia-0.6.9/pycatia/cat_sm_interfaces/view_characteristic_curves_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_smarteam_integ_interfaces/sti_db_children.py` & `pycatia-0.6.9/pycatia/cat_smarteam_integ_interfaces/sti_db_children.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_smarteam_integ_interfaces/sti_db_item.py` & `pycatia-0.6.9/pycatia/cat_smarteam_integ_interfaces/sti_db_item.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_smarteam_integ_interfaces/sti_engine.py` & `pycatia-0.6.9/pycatia/cat_smarteam_integ_interfaces/sti_engine.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/end_cut_ess_object_setting_att.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/end_cut_ess_object_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sdd_product.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sdd_product.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfd_product.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfd_product.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_connection_parameters.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_connection_parameters.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_endcut.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_endcut.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_endcut_manager.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_endcut_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_factory.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_function_factory.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_function_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_manager.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member2_points.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member2_points.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_curve.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_curve.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_plane2_curves.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_plane2_curves.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_point_length.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_point_length.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_point_up_to_limit.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_point_up_to_limit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_member_surf_surf.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_member_surf_surf.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_object.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_object_ext.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_object_ext.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_opening.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_opening.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_opening_contours_mgr.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_opening_contours_mgr.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_operation_factory.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_operation_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_positioning_strategy_manager.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_positioning_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_profile.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_profile.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_references.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_references.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_slot.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_slot.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_slots.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_slots.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_split_plate.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_split_plate.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_split_plates.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_split_plates.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_standard_contour_parameters.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_standard_contour_parameters.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_standard_opening.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_standard_opening.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_standard_pos_strategy_parameters.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_standard_pos_strategy_parameters.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_stiffener.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_stiffener.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_stiffener_on_free_edge.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_stiffener_on_free_edge.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_super_plate.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_super_plate.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_weld.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_weld.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_str_functional_interfaces/sfm_welds.py` & `pycatia-0.6.9/pycatia/cat_str_functional_interfaces/sfm_welds.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_2.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_factory.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_factory_2.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_factory_2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_set.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_set.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_set_transform_into_assembly_set.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_set_transform_into_assembly_set.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/annotation_sets.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/annotation_sets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/annotations.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/annotations.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/assembly_annotation_sets.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/assembly_annotation_sets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/associated_ref_frame.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/associated_ref_frame.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/capture.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/capture.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/capture_factory.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/capture_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/captures.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/captures.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/composite_tolerance.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/composite_tolerance.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/controlled_radius.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/controlled_radius.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/datum_simple.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/datum_simple.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/datum_target.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/datum_target.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/default_annotation.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/default_annotation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/dimension_3d.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/dimension_3d.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/dimension_limit.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/dimension_limit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/dimension_pattern.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/dimension_pattern.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/dmu_tol_setting_att.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/dmu_tol_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/envelope_condition.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/envelope_condition.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/flag_note.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/flag_note.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/free_state.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/free_state.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/fta_infra_setting_att.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/fta_infra_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/fta_setting_att.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/fta_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/material_condition.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/material_condition.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/noa.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/noa.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/non_semantic_datum.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/non_semantic_datum.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/non_semantic_datum_target.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/non_semantic_datum_target.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/non_semantic_dimension.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/non_semantic_dimension.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/non_semantic_gdt.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/non_semantic_gdt.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/particular_tol_elem.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/particular_tol_elem.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/projected_tolerance_zone.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/projected_tolerance_zone.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/reference_frame.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/reference_frame.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/roughness.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/roughness.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/semantic_gdt.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/semantic_gdt.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/shifted_profile_tolerance.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/shifted_profile_tolerance.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/tangent_plane.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/tangent_plane.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/text.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/text.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/tolerance_per_unit_basis_restrictive_value.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/tolerance_per_unit_basis_restrictive_value.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/tolerance_unit_basis_value.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/tolerance_unit_basis_value.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/tolerance_zone.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/tolerance_zone.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/tps_parallel_on_screen.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/tps_parallel_on_screen.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/tps_view.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/tps_view.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/tps_view_factory.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/tps_view_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/tps_views.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/tps_views.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/user_surface.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/user_surface.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/user_surfaces.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/user_surfaces.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/cat_tps_interfaces/weld.py` & `pycatia-0.6.9/pycatia/cat_tps_interfaces/weld.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/catia_de_settings_interfaces/iges_setting_att.py` & `pycatia-0.6.9/pycatia/catia_de_settings_interfaces/iges_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/catia_v4_interfaces/interop_setting_att.py` & `pycatia-0.6.9/pycatia/catia_v4_interfaces/interop_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/catia_v4_interfaces/migr_batch_setting_att.py` & `pycatia-0.6.9/pycatia/catia_v4_interfaces/migr_batch_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/catia_v4_interfaces/spec_v4_setting_att.py` & `pycatia-0.6.9/pycatia/catia_v4_interfaces/spec_v4_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/catia_v4_interfaces/v4_v5_space_setting_att.py` & `pycatia-0.6.9/pycatia/catia_v4_interfaces/v4_v5_space_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/catia_v4_interfaces/v4_writing_setting_att.py` & `pycatia-0.6.9/pycatia/catia_v4_interfaces/v4_writing_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/components_catalogs_interfaces/catalog_document.py` & `pycatia-0.6.9/pycatia/components_catalogs_interfaces/catalog_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/composites_interfaces/composites_material.py` & `pycatia-0.6.9/pycatia/composites_interfaces/composites_material.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/activities.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/activities.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/activity.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/item.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/item.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/items.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/items.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/lib_tab_setting_att.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/lib_tab_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/outputs.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/outputs.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/process_document.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/process_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/resource.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/resource.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/resource_collection.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/resource_collection.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/resources.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/resources.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/tree_tab_setting_att.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/tree_tab_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dmaps_interfaces/verif_tab_setting_att.py` & `pycatia-0.6.9/pycatia/dmaps_interfaces/verif_tab_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_asy_activity_interfaces/asy_sim_activity.py` & `pycatia-0.6.9/pycatia/dnb_asy_activity_interfaces/asy_sim_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_d5_iInterfaces/import_d5_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_d5_iInterfaces/import_d5_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_activity_interfaces/move_home_act.py` & `pycatia-0.6.9/pycatia/dnb_device_activity_interfaces/move_home_act.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_activity_interfaces/move_joints_act.py` & `pycatia-0.6.9/pycatia/dnb_device_activity_interfaces/move_joints_act.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_interfaces/basic_device.py` & `pycatia-0.6.9/pycatia/dnb_device_interfaces/basic_device.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_interfaces/d5_device.py` & `pycatia-0.6.9/pycatia/dnb_device_interfaces/d5_device.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_interfaces/dev_analysis_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_device_interfaces/dev_analysis_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_interfaces/device_joint_relations.py` & `pycatia-0.6.9/pycatia/dnb_device_interfaces/device_joint_relations.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_interfaces/device_sim.py` & `pycatia-0.6.9/pycatia/dnb_device_interfaces/device_sim.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_interfaces/dof_state.py` & `pycatia-0.6.9/pycatia/dnb_device_interfaces/dof_state.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_device_interfaces/home_position.py` & `pycatia-0.6.9/pycatia/dnb_device_interfaces/home_position.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_dpm_interfaces/mfg_assembly.py` & `pycatia-0.6.9/pycatia/dnb_dpm_interfaces/mfg_assembly.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_dpm_interfaces/mfg_assembly_factory.py` & `pycatia-0.6.9/pycatia/dnb_dpm_interfaces/mfg_assembly_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_ehm_interfaces/ehm_insertion_act_plug_map_view_data.py` & `pycatia-0.6.9/pycatia/dnb_ehm_interfaces/ehm_insertion_act_plug_map_view_data.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_ehm_interfaces/plug_map_view_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_ehm_interfaces/plug_map_view_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_ehs_interfaces/ehs_update_smoothness_factor.py` & `pycatia-0.6.9/pycatia/dnb_ehs_interfaces/ehs_update_smoothness_factor.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_ekp_interfaces/ekp_services.py` & `pycatia-0.6.9/pycatia/dnb_ekp_interfaces/ekp_services.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/curve_fastener.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/curve_fastener.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/dnb_fastener_item_services.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/dnb_fastener_item_services.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/dnb_fastener_management.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/dnb_fastener_management.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/dnb_fastener_new_mfg_pos_services.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/dnb_fastener_new_mfg_pos_services.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/fastener.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/fastener.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/fastener_group.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/fastener_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/fastener_set.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/fastener_set.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/fastener_work_bench.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/fastener_work_bench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_fastener_interfaces/point_fastener.py` & `pycatia-0.6.9/pycatia/dnb_fastener_interfaces/point_fastener.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_graph_editor/pert_node.py` & `pycatia-0.6.9/pycatia/dnb_graph_editor/pert_node.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_anthro.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_anthro.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_anthro_variable.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_anthro_variable.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_body.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_body.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_body_element.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_body_element.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_center_of_gravity.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_center_of_gravity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo_carry.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo_carry.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo_lift_lower.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo_lift_lower.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo_push_pull.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo_push_pull.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_ergo_rula.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_ergo_rula.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_hmi_workbench.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_hmi_workbench.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,16 @@
         :rtype: SWKHumanCatalog
         """
 
         return SWKManikin(self.com_object.CreateRightForearm(pi_manikin_name, pi_sex, pi_percentile, pi_population))
 
     def new_human_catalog(self) -> SWKHumanCatalog:
         """
-            .. note::
+
+        .. note::
             :class: toggle
 
             Microsoft Visual Basic Object Browser
                 | Function NewHumanCatalog(piPathFile As String) As SWKHumanCatalog
                 |     Member of SWKHumanModelingItf.SWKHmiWorkbench
 
         :rtype: SWKHumanCatalog
```

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_human_catalog.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_human_catalog.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_line_of_sight.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_line_of_sight.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_line_of_sight_node.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_line_of_sight_node.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_manikin.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_manikin.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_manikin_part.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_manikin_part.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_node.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_node.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_segment.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_segment.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_segment_node.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_segment_node.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swk_vision.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swk_vision.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swkdof.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swkdof.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swkik_constraint.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swkik_constraint.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_modeling_interfaces/swkik_manager.py` & `pycatia-0.6.9/pycatia/dnb_human_modeling_interfaces/swkik_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/auto_walk_activity.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/auto_walk_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/collision_free_walk.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/collision_free_walk.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/hts_ccp_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/hts_ccp_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/hts_general_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/hts_general_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/hts_joint_speed_settings_att.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/hts_joint_speed_settings_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/hts_task_display_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/hts_task_display_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_activity_group.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_activity_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_activity_group_factory.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_activity_group_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_acts_factory.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_acts_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_call_task.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_call_task.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_program.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_program.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_task.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_task.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/human_task_list.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/human_task_list.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/move_to_posture_activity.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/move_to_posture_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/pick_activity.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/pick_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/place_activity.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/place_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/walk_activity.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/walk_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_human_sim_interfaces/worker_activity.py` & `pycatia-0.6.9/pycatia/dnb_human_sim_interfaces/worker_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_arc_commands/amp_path.py` & `pycatia-0.6.9/pycatia/dnb_igp_arc_commands/amp_path.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_arc_commands/amp_tag.py` & `pycatia-0.6.9/pycatia/dnb_igp_arc_commands/amp_tag.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_arc_commands/arc_tag.py` & `pycatia-0.6.9/pycatia/dnb_igp_arc_commands/arc_tag.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_arc_commands/arc_tag_group.py` & `pycatia-0.6.9/pycatia/dnb_igp_arc_commands/arc_tag_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_olp_ui/igp_olp_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_igp_olp_ui/igp_olp_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_olp_ui/olp_translator.py` & `pycatia-0.6.9/pycatia/dnb_igp_olp_ui/olp_translator.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/call_robot_task_activity.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/call_robot_task_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/device_task.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/device_task.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/device_task_factory.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/device_task_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/generic_action.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/generic_action.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/generic_action_factory.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/generic_action_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/mount_activity.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/mount_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/mount_manager.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/mount_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/move_action_activity.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/move_action_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/operation.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/operation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/operation_profile.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/operation_profile.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/robot_motion.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/robot_motion.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/robot_task.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/robot_task.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/robot_task_clone_factory.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/robot_task_clone_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/robot_task_factory.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/robot_task_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tag.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tag.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tag_factory.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tag_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tag_group.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tag_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tag_group_factory.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tag_group_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/tcp_trace_activity.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/tcp_trace_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_igp_setup_interfaces/unmount_activity.py` & `pycatia-0.6.9/pycatia/dnb_igp_setup_interfaces/unmount_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_manufacturing_layout_interfaces/attachment_cont.py` & `pycatia-0.6.9/pycatia/dnb_manufacturing_layout_interfaces/attachment_cont.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_manufacturing_layout_interfaces/dnb_attachment.py` & `pycatia-0.6.9/pycatia/dnb_manufacturing_layout_interfaces/dnb_attachment.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_manufacturing_layout_interfaces/dnb_attachment_factory.py` & `pycatia-0.6.9/pycatia/dnb_manufacturing_layout_interfaces/dnb_attachment_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_mhi_interfaces/mhi_load_parameters.py` & `pycatia-0.6.9/pycatia/dnb_mhi_interfaces/mhi_load_parameters.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_mhi_interfaces/mhi_open_access.py` & `pycatia-0.6.9/pycatia/dnb_mhi_interfaces/mhi_open_access.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_mhi_interfaces/mhi_save_access.py` & `pycatia-0.6.9/pycatia/dnb_mhi_interfaces/mhi_save_access.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_reporting_interfaces/fas_reporting_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_reporting_interfaces/fas_reporting_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_resource_program_interfaces/active_task.py` & `pycatia-0.6.9/pycatia/dnb_resource_program_interfaces/active_task.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_resource_program_interfaces/resource_program_manager.py` & `pycatia-0.6.9/pycatia/dnb_resource_program_interfaces/resource_program_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_resource_program_interfaces/task.py` & `pycatia-0.6.9/pycatia/dnb_resource_program_interfaces/task.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/aux_devices_mgt.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/aux_devices_mgt.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/calib_offsets.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/calib_offsets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/generic_accuracy_profile.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/generic_accuracy_profile.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/generic_motion_profile.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/generic_motion_profile.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/generic_obj_frame_profile.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/generic_obj_frame_profile.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/generic_tool_profile.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/generic_tool_profile.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/parameter_profiles.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/parameter_profiles.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/parameter_profiles_factory.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/parameter_profiles_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/rob_analysis_heart_beat_usage_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/rob_analysis_heart_beat_usage_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/rob_analysis_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/rob_analysis_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/rob_controller_factory.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/rob_controller_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/rob_generic_controller.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/rob_generic_controller.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/rrs_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/rrs_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/tcp_trace.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/tcp_trace.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/tcp_trace_manager.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/tcp_trace_manager.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_robot_interfaces/tcp_trace_manager_graphics.py` & `pycatia-0.6.9/pycatia/dnb_robot_interfaces/tcp_trace_manager_graphics.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_sim_activity_interfaces/delay_act.py` & `pycatia-0.6.9/pycatia/dnb_sim_activity_interfaces/delay_act.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_sim_activity_interfaces/grab_act.py` & `pycatia-0.6.9/pycatia/dnb_sim_activity_interfaces/grab_act.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_sim_activity_interfaces/release_act.py` & `pycatia-0.6.9/pycatia/dnb_sim_activity_interfaces/release_act.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_simulation_interfaces/analysis_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_simulation_interfaces/analysis_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_simulation_interfaces/sim_trace_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_simulation_interfaces/sim_trace_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_simulation_interfaces/simulation_init_state.py` & `pycatia-0.6.9/pycatia/dnb_simulation_interfaces/simulation_init_state.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_simulation_interfaces/simulation_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_simulation_interfaces/simulation_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_sor_interfaces/order_generator.py` & `pycatia-0.6.9/pycatia/dnb_sor_interfaces/order_generator.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_state_interfaces/dnb_3d_state.py` & `pycatia-0.6.9/pycatia/dnb_state_interfaces/dnb_3d_state.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_state_interfaces/dnb_3d_state_management.py` & `pycatia-0.6.9/pycatia/dnb_state_interfaces/dnb_3d_state_management.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_state_interfaces/dnb_3d_states.py` & `pycatia-0.6.9/pycatia/dnb_state_interfaces/dnb_3d_states.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_buy_off.py` & `pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_buy_off.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_change_notification.py` & `pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_change_notification.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_data_collection.py` & `pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_data_collection.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_text.py` & `pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_text.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_work_interfaces/wi_text_access_ei.py` & `pycatia-0.6.9/pycatia/dnb_work_interfaces/wi_text_access_ei.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/dnb_work_interfaces/work_general_setting_att.py` & `pycatia-0.6.9/pycatia/dnb_work_interfaces/work_general_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_factory.py` & `pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_root.py` & `pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_root.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_setting_att.py` & `pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_sheet.py` & `pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_sheet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_sheets.py` & `pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_sheets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_view.py` & `pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_view.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_2dL_interfaces/layout_2d_views.py` & `pycatia-0.6.9/pycatia/drafting_2dL_interfaces/layout_2d_views.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drafting_setting_att.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drafting_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_arrow.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_arrow.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_arrows.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_arrows.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_component.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_component.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_components.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_components.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dim_ext_line.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dim_ext_line.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dim_line.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dim_line.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dim_value.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dim_value.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dimension.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dimension.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_dimensions.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_dimensions.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_document.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_leader.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_leader.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_leaders.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_leaders.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_page_setup.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_page_setup.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_picture.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_picture.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_pictures.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_pictures.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_root.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_root.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_sheet.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_sheet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_sheets.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_sheets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_table.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_table.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_tables.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_tables.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_text.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_text.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_text_properties.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_text_properties.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_text_range.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_text_range.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_texts.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_texts.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_thread.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_thread.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_threads.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_threads.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_view.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_view.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_view_generative_behavior.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_view_generative_behavior.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_view_generative_links.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_view_generative_links.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_views.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_views.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_welding.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_welding.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/drawing_weldings.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/drawing_weldings.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/drafting_interfaces/print_area.py` & `pycatia-0.6.9/pycatia/drafting_interfaces/print_area.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/electrical_schematic_interfaces/electrical_schematic_object.py` & `pycatia-0.6.9/pycatia/electrical_schematic_interfaces/electrical_schematic_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/electrical_schematic_interfaces/electrical_schematic_wire.py` & `pycatia-0.6.9/pycatia/electrical_schematic_interfaces/electrical_schematic_wire.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_engine.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_engine.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_engine_v6_r2014x.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_engine_v6_r2014x.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_engine_v6_r2015.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_engine_v6_r2015.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_id.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_id.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_ids.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_ids.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_properties.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_properties.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_property.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_property.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_save_item.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_save_item.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_save_items.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_save_items.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_save_operation.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_save_operation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_structure.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_structure.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_template.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_template.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_template_type.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_template_type.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_template_types.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_template_types.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/eno_cd5_interfaces/cd5_templates.py` & `pycatia-0.6.9/pycatia/eno_cd5_interfaces/cd5_templates.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/enumeration/enumeration_types.py` & `pycatia-0.6.9/pycatia/enumeration/enumeration_types.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/fitting_setting_att.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/fitting_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/manip_setting_att.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/manip_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/sampled.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/sampled.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/sampleds.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/sampleds.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/sampleds_node.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/sampleds_node.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/shot.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/shot.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/shots.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/shots.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/shuttle.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/shuttle.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/shuttles.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/shuttles.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/track.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/track.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/fitting_interfaces/tracks.py` & `pycatia-0.6.9/pycatia/fitting_interfaces/tracks.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_actions_group.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_actions_group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_actions_groups.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_actions_groups.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_association.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_association.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_associations.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_associations.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_facet_managers.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_facet_managers.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_gen_script_mgr.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_gen_script_mgr.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_multi_rep_mgr.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_multi_rep_mgr.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_node_graph_layout.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_node_graph_layout.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_script.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_script.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/funct_scripts.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/funct_scripts.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_action.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_action.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_actions.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_actions.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_description.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_description.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_document.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_element.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_element.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_facet.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_facet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_facet_mgr.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_facet_mgr.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_object.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_object_proxy.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_object_proxy.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_objects.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_objects.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_position.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_position.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_system_setting_att.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_system_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_variant.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_variant.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/funct_system_interfaces/functional_variants.py` & `pycatia-0.6.9/pycatia/funct_system_interfaces/functional_variants.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_check.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_check.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_check_runtime.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_check_runtime.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_report_object.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_report_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_report_objects.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_report_objects.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_base.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_base.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_base_component_runtime.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_base_component_runtime.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_base_component_runtimes.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_base_component_runtimes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_base_runtime.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_base_runtime.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_runtime.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_runtime.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_set.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_set.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/expert_rule_set_runtime.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/expert_rule_set_runtime.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/general_knowledge_interfaces/kwe_correct_function.py` & `pycatia-0.6.9/pycatia/general_knowledge_interfaces/kwe_correct_function.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_3d_curve_offset.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_3d_curve_offset.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_affinity.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_affinity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_assemble.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_assemble.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_line.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,11 +154,11 @@
 
     @element.setter
     def element(self, value: Reference):
         """
         :param Reference value:
         """
 
-        self.hybrid_shape_axis_line.Element = value
+        self.hybrid_shape_axis_line.Element = value.com_object
 
     def __repr__(self):
         return f'HybridShapeAxisLine(name="{ self.name }")'
```

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_to_axis.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_to_axis.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_blend.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_blend.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_boundary.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_boundary.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_bump.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_bump.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle2_points_rad.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle2_points_rad.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle3_points.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle3_points.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_point.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_point.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_radius.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_radius.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_axis.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_axis.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_tangent.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_tangent.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_pt.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_pt.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_rad.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_rad.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_explicit.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_explicit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_tritangent.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_tritangent.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_combine.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_combine.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_conic.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_conic.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_connect.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_connect.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_corner.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_corner.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_explicit.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_explicit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_par.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_par.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_smooth.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_smooth.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_cylinder.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_cylinder.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_develop.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_develop.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_direction.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_direction.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extract.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extract.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extract_multi.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extract_multi.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extrapol.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extrapol.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 
     @support.setter
     def support(self, value: Reference):
         """
         :param Reference value:
         """
 
-        self.hybrid_shape_extrapol.Support = value
+        self.hybrid_shape_extrapol.Support = value.com_object
 
     def get_boundary(self, i_pos: int) -> Reference:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
```

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum_polar.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum_polar.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extrude.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_extrude.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_factory.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fill.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_fill.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_bi_tangent.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_bi_tangent.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_tri_tangent.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_tri_tangent.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_healing.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_healing.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_helix.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_helix.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_integrated_law.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_integrated_law.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_intersection.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_intersection.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_inverse.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_inverse.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_law_dist_proj.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_law_dist_proj.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_angle.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_angle.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bi_tangent.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bi_tangent.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bisecting.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bisecting.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_explicit.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_explicit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_normal.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_normal.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_dir.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_dir.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_pt.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_pt.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_tangency.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_line_tangency.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_loft.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_loft.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_mid_surface.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_mid_surface.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_near.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_near.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_offset.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_offset.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_curve.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_curve.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_line1_pt.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_line1_pt.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane2_lines.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane2_lines.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane3_points.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane3_points.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_angle.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_angle.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_equation.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_equation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_explicit.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_explicit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_mean.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_mean.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_normal.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_normal.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset_pt.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset_pt.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_tangent.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_tangent.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_between.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_between.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_center.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_center.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_coord.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_coord.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_explicit.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_explicit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_curve.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_curve.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_plane.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_plane.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_surface.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_surface.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_tangent.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_point_tangent.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_polyline.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_polyline.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_position_transfo.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_position_transfo.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_project.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_project.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_reflect_line.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_reflect_line.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_revol.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_revol.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_rolling_offset.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_rolling_offset.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_rotate.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_rotate.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_scaling.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_scaling.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_section.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_section.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sphere.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sphere.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spine.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_spine.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spiral.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_spiral.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spline.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_spline.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_split.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_split.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_surface_explicit.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_surface_explicit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_circle.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_circle.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_conic.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_conic.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_explicit.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_explicit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_line.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_line.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_symmetry.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_symmetry.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_thickness.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_thickness.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_transfer.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_transfer.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_translate.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_translate.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_trim.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_trim.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_unfold.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_unfold.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_volume_explicit.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_volume_explicit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_curve.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_curve.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_surface.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_surface.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/line.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/line.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/plane.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/plane.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/hybrid_shape_interfaces/point.py` & `pycatia-0.6.9/pycatia/hybrid_shape_interfaces/point.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/application.py` & `pycatia-0.6.9/pycatia/in_interfaces/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pycatia.in_interfaces.send_to_service import SendToService
 from pycatia.in_interfaces.system_configuration import SystemConfiguration
 from pycatia.in_interfaces.window import Window
 from pycatia.in_interfaces.windows import Windows
 from pycatia.system_interfaces.any_object import AnyObject
 from pycatia.system_interfaces.system_service import SystemService
 from pycatia.in_interfaces.setting_controllers import SettingControllers
-from pycatia.types.document_types import document_type
+from pycatia.types.document import document_types
 
 
 class Application(AnyObject):
     """
 
     .. note::
         :class: toggle
@@ -88,16 +88,20 @@
             |          Dim ActiveDoc As Document
             |          Set ActiveDoc = CATIA.ActiveDocument
 
         :rtype: Document
         """
         try:
             active_doc_com = self.com_object.ActiveDocument
-            doc_suffix = active_doc_com.Name.split('.')[-1]
-            return document_type[doc_suffix](active_doc_com)
+            extension = active_doc_com.Name.split('.')[-1]
+            types = [document_types[k]['type'] for k in (document_types) if document_types[k]['extension'] == extension]
+            if len(types) > 1:
+                raise CATIAApplicationException('There was a problem determining the document type.')
+            document_type = types[0]
+            return document_type(active_doc_com)
         except com_error:
             raise CATIAApplicationException('Is there an active document?')
 
     @property
     def active_printer(self) -> Printer:
         """
         .. note::
```

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/camera.py` & `pycatia-0.6.9/pycatia/in_interfaces/camera.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/camera_2d.py` & `pycatia-0.6.9/pycatia/in_interfaces/camera_2d.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/camera_3d.py` & `pycatia-0.6.9/pycatia/in_interfaces/camera_3d.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/cameras.py` & `pycatia-0.6.9/pycatia/in_interfaces/cameras.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/cgr_adhesion_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/cgr_adhesion_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/document.py` & `pycatia-0.6.9/pycatia/in_interfaces/document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/documentation_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/documentation_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/documents.py` & `pycatia-0.6.9/pycatia/in_interfaces/documents.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import warnings
 
 from pywintypes import com_error
 
 from pycatia.exception_handling import CATIAApplicationException
 from pycatia.in_interfaces.document import Document
 from pycatia.system_interfaces.collection import Collection
-from pycatia.types.document_types import document_type
+from pycatia.types.document import document_types
 from pycatia.types.general import cat_variant, list_str
-from pycatia.scripts.document_types import get_document_type
 
 
 class Documents(Collection):
     """
     The Documents object is used to access multiple open documents in the catia session.
 
     Usage::
@@ -83,22 +82,22 @@
                 |          Dim PartDoc As Document
                 |          Set PartDoc = Documents.Add("Part")
 
         :param str document_type:
         :rtype: Document
         """
 
-        # document_types string must be one of these types:
-        # 'Part', 'Product', 'Drawing', 'FunctionalSystem', 'CATMaterial', 'CatalogDocument'
+        # see pycatia.types.docs for supported Documents.
 
-        dt = get_document_type(document_type)
+        if document_type.lower() not in [t.lower() for t in document_types]:
+            raise CATIAApplicationException(f'Document type {document_type} not supported. Allowed types are {[t for t in document_types]}.')
 
-        self.logger.info(f'Creating a new "{dt}".')
+        document = document_types[document_type]['type']
 
-        return Document(self.documents.Add(dt))
+        return document(self.documents.Add(document_type))
 
     def count_types(self, file_type_list: list_str) -> int:
         """
         Returns the number of documents which presents special file extensions like:
             'catpart', 'catdrawing', 'catproduct', 'catmaterial', 'catalog', 'catfct'
 
 
@@ -303,15 +302,15 @@
         :param str file_name:
         :rtype: Document
         """
         # return Document(self.documents.Read(file_name))
 
         read_doc_com = self.documents.Read(file_name)
         doc_suffix = file_name.split('.')[-1]
-        return document_type[doc_suffix](read_doc_com)
+        return document_types[doc_suffix](read_doc_com)
 
     def __getitem__(self, n: int) -> Document:
         if (n + 1) > self.count:
             raise StopIteration
 
         return Document(self.documents.Item(n + 1))
```

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/drafting_page_setup.py` & `pycatia-0.6.9/pycatia/in_interfaces/drafting_page_setup.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/file.py` & `pycatia-0.6.9/pycatia/in_interfaces/file.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/file_component.py` & `pycatia-0.6.9/pycatia/in_interfaces/file_component.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/file_system.py` & `pycatia-0.6.9/pycatia/in_interfaces/file_system.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/files.py` & `pycatia-0.6.9/pycatia/in_interfaces/files.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/folder.py` & `pycatia-0.6.9/pycatia/in_interfaces/folder.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/folders.py` & `pycatia-0.6.9/pycatia/in_interfaces/folders.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/general_session_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/general_session_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/light_source.py` & `pycatia-0.6.9/pycatia/in_interfaces/light_source.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/light_sources.py` & `pycatia-0.6.9/pycatia/in_interfaces/light_sources.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/macros_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/macros_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/move.py` & `pycatia-0.6.9/pycatia/in_interfaces/move.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/page_setup.py` & `pycatia-0.6.9/pycatia/in_interfaces/page_setup.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/position.py` & `pycatia-0.6.9/pycatia/in_interfaces/position.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/printer.py` & `pycatia-0.6.9/pycatia/in_interfaces/printer.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/printers.py` & `pycatia-0.6.9/pycatia/in_interfaces/printers.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/printers_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/printers_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/reference.py` & `pycatia-0.6.9/pycatia/in_interfaces/reference.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/references.py` & `pycatia-0.6.9/pycatia/in_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/search_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/search_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/selected_element.py` & `pycatia-0.6.9/pycatia/in_interfaces/selected_element.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/selection.py` & `pycatia-0.6.9/pycatia/in_interfaces/selection.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/selection_sets.py` & `pycatia-0.6.9/pycatia/in_interfaces/selection_sets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/send_to_service.py` & `pycatia-0.6.9/pycatia/in_interfaces/send_to_service.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/setting_controllers.py` & `pycatia-0.6.9/pycatia/in_interfaces/setting_controllers.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/specs_and_geom_window.py` & `pycatia-0.6.9/pycatia/in_interfaces/specs_and_geom_window.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/specs_viewer.py` & `pycatia-0.6.9/pycatia/in_interfaces/specs_viewer.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/system_configuration.py` & `pycatia-0.6.9/pycatia/in_interfaces/system_configuration.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/text_stream.py` & `pycatia-0.6.9/pycatia/in_interfaces/text_stream.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/tree_viz_manip_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/tree_viz_manip_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/viewer.py` & `pycatia-0.6.9/pycatia/in_interfaces/viewer.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/viewer_2d.py` & `pycatia-0.6.9/pycatia/in_interfaces/viewer_2d.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/viewer_3d.py` & `pycatia-0.6.9/pycatia/in_interfaces/viewer_3d.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/viewers.py` & `pycatia-0.6.9/pycatia/in_interfaces/viewers.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/viewpoint_2d.py` & `pycatia-0.6.9/pycatia/in_interfaces/viewpoint_2d.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/viewpoint_3d.py` & `pycatia-0.6.9/pycatia/in_interfaces/viewpoint_3d.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/vis_property_set.py` & `pycatia-0.6.9/pycatia/in_interfaces/vis_property_set.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/visualization_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/visualization_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/vrml_setting_att.py` & `pycatia-0.6.9/pycatia/in_interfaces/vrml_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/window.py` & `pycatia-0.6.9/pycatia/in_interfaces/window.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/windows.py` & `pycatia-0.6.9/pycatia/in_interfaces/windows.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/in_interfaces/workbench.py` & `pycatia-0.6.9/pycatia/in_interfaces/workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/dressup.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/dressup.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/dressups.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/dressups.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/joint.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/joint.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/joints.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/joints.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/kinematics_workbench.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/kinematics_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/mechanism.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/mechanism.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/mechanism_command.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/mechanism_command.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/mechanism_commands.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/mechanism_commands.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/kinematics_interfaces/mechanisms.py` & `pycatia-0.6.9/pycatia/kinematics_interfaces/mechanisms.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/angle.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/angle.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/bool_param.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/bool_param.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/check.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/check.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/constraint_satisfaction.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/constraint_satisfaction.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/design_table.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/design_table.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/dimension.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/dimension.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/enum_param.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/enum_param.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/feature_generator.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/feature_generator.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/formula.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/formula.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/free_parameter.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/free_parameter.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/free_parameters.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/free_parameters.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/int_param.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/int_param.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/knowledge_activate_object.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/knowledge_activate_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/knowledge_object.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/knowledge_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/knowledge_sheet_setting_att.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/knowledge_sheet_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/language_sheet_setting_att.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/language_sheet_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/law.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/law.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/length.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/length.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/list.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/list.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/list_parameter.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/list_parameter.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/loop.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/loop.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/optimization.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/optimization.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/optimization_constraint.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/optimization_constraint.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/optimization_constraints.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/optimization_constraints.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/optimizations.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/optimizations.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/parameter.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/parameter.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/parameter_set.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/parameter_set.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/parameter_sets.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/parameter_sets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/parameters.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/parameters.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/real_param.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/real_param.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/relation.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/relation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/relations.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/relations.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/report_generation_sheet_setting_att.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/report_generation_sheet_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/rule.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/rule.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/set_of_equation.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/set_of_equation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/str_param.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/str_param.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/tolerance_sheet_setting_att.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/tolerance_sheet_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/unit.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/unit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/units.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/units.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/knowledge_interfaces/units_sheet_setting_att.py` & `pycatia-0.6.9/pycatia/knowledge_interfaces/units_sheet_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/machining_process.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/machining_process.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_activities.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_activities.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_activity.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_activity_syntax.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_activity_syntax.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_activity_syntax2.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_activity_syntax2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_apt_generator.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_apt_generator.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_copy_transformation.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_copy_transformation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_factories.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_factories.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_feature.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_feature.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_features.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_features.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_generator_data.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_generator_data.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_hole.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_hole.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_insert.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_insert.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machinable_area.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machinable_area.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machinable_feature.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machinable_feature.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machinable_geometry.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machinable_geometry.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machine.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machine.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_machining_axis.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_machining_axis.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_operation.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_operation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_output.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_output.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_output_generator.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_output_generator.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_pattern.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_pattern.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_precedence.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_precedence.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_precedences.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_precedences.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_process.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_process.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_program.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_program.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_resource_factory.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_resource_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_setup.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_setup.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_setup2.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_setup2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_setup3.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_setup3.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_assembly.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_assembly.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_assembly2.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_assembly2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_corrector.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_corrector.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_motion.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_motion.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_tool_motions.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_tool_motions.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_user_representation.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_user_representation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/manufacturing_interfaces/manufacturing_view.py` & `pycatia-0.6.9/pycatia/manufacturing_interfaces/manufacturing_view.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/axis_system.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/axis_system.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/axis_systems.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/axis_systems.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/bi_dim_feat_edge.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/bi_dim_feat_edge.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/bodies.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/bodies.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/body.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/body.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/boundary.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/boundary.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/constraint.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/constraint.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/constraints.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/constraints.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/cylindrical_face.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/cylindrical_face.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/edge.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/edge.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/face.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/face.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/factory.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/fix_together.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/fix_together.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/fix_togethers.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/fix_togethers.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/geometric_elements.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/geometric_elements.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_bodies.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_bodies.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_body.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_body.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_shape.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_shape.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_shape_instance.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_shape_instance.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/hybrid_shapes.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/hybrid_shapes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/instance_factory.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/instance_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/mono_dim_feat_edge.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/mono_dim_feat_edge.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/not_wire_boundary_mono_dim_feat_vertex.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/not_wire_boundary_mono_dim_feat_vertex.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/ordered_geometrical_set.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/ordered_geometrical_set.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/ordered_geometrical_sets.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/ordered_geometrical_sets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/origin_elements.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/origin_elements.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/part.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/part.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/part_document.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/part_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/part_infrastructure_setting_att.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/part_infrastructure_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/planar_face.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/planar_face.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/rectilinear_bi_dim_feat_edge.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/rectilinear_bi_dim_feat_edge.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/rectilinear_mono_dim_feat_edge.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/rectilinear_mono_dim_feat_edge.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/rectilinear_tri_dim_feat_edge.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/rectilinear_tri_dim_feat_edge.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/shape.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/shape.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/shape_instance.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/shape_instance.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/shapes.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/shapes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/sketches.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/sketches.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/solid.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/solid.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/tri_dim_feat_edge.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/tri_dim_feat_edge.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/tri_dim_feat_vertex_or_bi_dim_feat_vertex.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/tri_dim_feat_vertex_or_bi_dim_feat_vertex.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/vertex.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/vertex.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/mec_mod_interfaces/zero_dim_feat_vertex_or_wire_boundary_mono_dim_feat_vertex.py` & `pycatia-0.6.9/pycatia/mec_mod_interfaces/zero_dim_feat_vertex_or_wire_boundary_mono_dim_feat_vertex.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/multi_cad_interfaces/multi_cad_setting_att.py` & `pycatia-0.6.9/pycatia/multi_cad_interfaces/multi_cad_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/annotated_view.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/annotated_view.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/annotated_views.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/annotated_views.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/dmu_data_flow.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/dmu_data_flow.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/dmu_review.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/dmu_review.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/dmu_reviews.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/dmu_reviews.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/group.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/group.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/groups.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/groups.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/hyperlink.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/hyperlink.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/hyperlinks.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/marker_2D.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/marker_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/marker_2Ds.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/marker_2Ds.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/marker_3D.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/marker_3D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/marker_3Ds.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/marker_3Ds.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/marker_setting_att.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/marker_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/n_4D_navigator_setting_att.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/n_4D_navigator_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/navigator_interfaces/navigator_workbench.py` & `pycatia-0.6.9/pycatia/navigator_interfaces/navigator_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/osm_interfaces/product_scene.py` & `pycatia-0.6.9/pycatia/osm_interfaces/product_scene.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/osm_interfaces/product_scenes.py` & `pycatia-0.6.9/pycatia/osm_interfaces/product_scenes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/osm_interfaces/scene.py` & `pycatia-0.6.9/pycatia/osm_interfaces/scene.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/osm_interfaces/scene_product_data.py` & `pycatia-0.6.9/pycatia/osm_interfaces/scene_product_data.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/osm_interfaces/scene_workbench.py` & `pycatia-0.6.9/pycatia/osm_interfaces/scene_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/osm_interfaces/scenes.py` & `pycatia-0.6.9/pycatia/osm_interfaces/scenes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/add.py` & `pycatia-0.6.9/pycatia/part_interfaces/add.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/affinity.py` & `pycatia-0.6.9/pycatia/part_interfaces/affinity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/angular_repartition.py` & `pycatia-0.6.9/pycatia/part_interfaces/angular_repartition.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/assemble.py` & `pycatia-0.6.9/pycatia/part_interfaces/assemble.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/auto_draft.py` & `pycatia-0.6.9/pycatia/part_interfaces/auto_draft.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/auto_fillet.py` & `pycatia-0.6.9/pycatia/part_interfaces/auto_fillet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/axis_to_axis.py` & `pycatia-0.6.9/pycatia/part_interfaces/axis_to_axis.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/boolean_shape.py` & `pycatia-0.6.9/pycatia/part_interfaces/boolean_shape.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/chamfer.py` & `pycatia-0.6.9/pycatia/part_interfaces/chamfer.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/circ_pattern.py` & `pycatia-0.6.9/pycatia/part_interfaces/circ_pattern.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/close_surface.py` & `pycatia-0.6.9/pycatia/part_interfaces/close_surface.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/const_rad_edge_fillet.py` & `pycatia-0.6.9/pycatia/part_interfaces/const_rad_edge_fillet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/defeaturing.py` & `pycatia-0.6.9/pycatia/part_interfaces/defeaturing.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/defeaturing_fillet_filter.py` & `pycatia-0.6.9/pycatia/part_interfaces/defeaturing_fillet_filter.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/defeaturing_filter.py` & `pycatia-0.6.9/pycatia/part_interfaces/defeaturing_filter.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/defeaturing_filter_with_range.py` & `pycatia-0.6.9/pycatia/part_interfaces/defeaturing_filter_with_range.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/defeaturing_filters.py` & `pycatia-0.6.9/pycatia/part_interfaces/defeaturing_filters.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/defeaturing_hole_filter.py` & `pycatia-0.6.9/pycatia/part_interfaces/defeaturing_hole_filter.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/draft.py` & `pycatia-0.6.9/pycatia/part_interfaces/draft.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/draft_domain.py` & `pycatia-0.6.9/pycatia/part_interfaces/draft_domain.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/draft_domains.py` & `pycatia-0.6.9/pycatia/part_interfaces/draft_domains.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/dress_up_shape.py` & `pycatia-0.6.9/pycatia/part_interfaces/dress_up_shape.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/edge_fillet.py` & `pycatia-0.6.9/pycatia/part_interfaces/edge_fillet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/face_fillet.py` & `pycatia-0.6.9/pycatia/part_interfaces/face_fillet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/fillet.py` & `pycatia-0.6.9/pycatia/part_interfaces/fillet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/groove.py` & `pycatia-0.6.9/pycatia/part_interfaces/groove.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/hole.py` & `pycatia-0.6.9/pycatia/part_interfaces/hole.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/intersect.py` & `pycatia-0.6.9/pycatia/part_interfaces/intersect.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/limit.py` & `pycatia-0.6.9/pycatia/part_interfaces/limit.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/linear_repartition.py` & `pycatia-0.6.9/pycatia/part_interfaces/linear_repartition.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/loft.py` & `pycatia-0.6.9/pycatia/part_interfaces/loft.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/mirror.py` & `pycatia-0.6.9/pycatia/part_interfaces/mirror.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/pad.py` & `pycatia-0.6.9/pycatia/part_interfaces/pad.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/pattern.py` & `pycatia-0.6.9/pycatia/part_interfaces/pattern.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/pocket.py` & `pycatia-0.6.9/pycatia/part_interfaces/pocket.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/prism.py` & `pycatia-0.6.9/pycatia/part_interfaces/prism.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/rect_pattern.py` & `pycatia-0.6.9/pycatia/part_interfaces/rect_pattern.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/remove.py` & `pycatia-0.6.9/pycatia/part_interfaces/remove.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/remove_face.py` & `pycatia-0.6.9/pycatia/part_interfaces/remove_face.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/repartition.py` & `pycatia-0.6.9/pycatia/part_interfaces/repartition.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/replace_face.py` & `pycatia-0.6.9/pycatia/part_interfaces/replace_face.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/revolution.py` & `pycatia-0.6.9/pycatia/part_interfaces/revolution.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/rib.py` & `pycatia-0.6.9/pycatia/part_interfaces/rib.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/rotate.py` & `pycatia-0.6.9/pycatia/part_interfaces/rotate.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/scaling.py` & `pycatia-0.6.9/pycatia/part_interfaces/scaling.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/scaling2.py` & `pycatia-0.6.9/pycatia/part_interfaces/scaling2.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/sew_surface.py` & `pycatia-0.6.9/pycatia/part_interfaces/sew_surface.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/shaft.py` & `pycatia-0.6.9/pycatia/part_interfaces/shaft.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/shape_factory.py` & `pycatia-0.6.9/pycatia/part_interfaces/shape_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/shell.py` & `pycatia-0.6.9/pycatia/part_interfaces/shell.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/sketch_based_shape.py` & `pycatia-0.6.9/pycatia/part_interfaces/sketch_based_shape.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/slot.py` & `pycatia-0.6.9/pycatia/part_interfaces/slot.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/solid_combine.py` & `pycatia-0.6.9/pycatia/part_interfaces/solid_combine.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/split.py` & `pycatia-0.6.9/pycatia/part_interfaces/split.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/stiffener.py` & `pycatia-0.6.9/pycatia/part_interfaces/stiffener.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/surface_based_shape.py` & `pycatia-0.6.9/pycatia/part_interfaces/surface_based_shape.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/sweep.py` & `pycatia-0.6.9/pycatia/part_interfaces/sweep.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/symmetry.py` & `pycatia-0.6.9/pycatia/part_interfaces/symmetry.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/thick_surface.py` & `pycatia-0.6.9/pycatia/part_interfaces/thick_surface.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/thickness.py` & `pycatia-0.6.9/pycatia/part_interfaces/thickness.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/thread.py` & `pycatia-0.6.9/pycatia/part_interfaces/thread.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/transformation_shape.py` & `pycatia-0.6.9/pycatia/part_interfaces/transformation_shape.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/translate.py` & `pycatia-0.6.9/pycatia/part_interfaces/translate.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/trim.py` & `pycatia-0.6.9/pycatia/part_interfaces/trim.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/tritangent_fillet.py` & `pycatia-0.6.9/pycatia/part_interfaces/tritangent_fillet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/user_pattern.py` & `pycatia-0.6.9/pycatia/part_interfaces/user_pattern.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/user_repartition.py` & `pycatia-0.6.9/pycatia/part_interfaces/user_repartition.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/part_interfaces/var_rad_edge_fillet.py` & `pycatia-0.6.9/pycatia/part_interfaces/var_rad_edge_fillet.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/pcb_board_base/pcb_area.py` & `pycatia-0.6.9/pycatia/pcb_board_base/pcb_area.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/pcb_board_base/pcb_board.py` & `pycatia-0.6.9/pycatia/pcb_board_base/pcb_board.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/pcb_board_base/pcb_component.py` & `pycatia-0.6.9/pycatia/pcb_board_base/pcb_component.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/pcb_board_base/pcb_hole_and_pattern.py` & `pycatia-0.6.9/pycatia/pcb_board_base/pcb_hole_and_pattern.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/pcb_board_base/pcb_object.py` & `pycatia-0.6.9/pycatia/pcb_board_base/pcb_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/pcb_board_base/pcb_workbench.py` & `pycatia-0.6.9/pycatia/pcb_board_base/pcb_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/ppr_interfaces/ppr_activity.py` & `pycatia-0.6.9/pycatia/ppr_interfaces/ppr_activity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/ppr_interfaces/ppr_document.py` & `pycatia-0.6.9/pycatia/ppr_interfaces/ppr_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/ppr_interfaces/ppr_products.py` & `pycatia-0.6.9/pycatia/ppr_interfaces/ppr_products.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/prismatic_machining_interfaces/manufacturing_prismatic_machining_area.py` & `pycatia-0.6.9/pycatia/prismatic_machining_interfaces/manufacturing_prismatic_machining_area.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/product_structure_interfaces/analyze.py` & `pycatia-0.6.9/pycatia/product_structure_interfaces/analyze.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/product_structure_interfaces/assembly_convertor.py` & `pycatia-0.6.9/pycatia/product_structure_interfaces/assembly_convertor.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/product_structure_interfaces/product.py` & `pycatia-0.6.9/pycatia/product_structure_interfaces/product.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/product_structure_interfaces/product_document.py` & `pycatia-0.6.9/pycatia/product_structure_interfaces/product_document.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/product_structure_interfaces/products.py` & `pycatia-0.6.9/pycatia/product_structure_interfaces/products.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/product_structure_interfaces/publication.py` & `pycatia-0.6.9/pycatia/product_structure_interfaces/publication.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/product_structure_interfaces/publications.py` & `pycatia-0.6.9/pycatia/product_structure_interfaces/publications.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/reporter_interfaces/rpm_report.py` & `pycatia-0.6.9/pycatia/reporter_interfaces/rpm_report.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/scripts/csv_tools.py` & `pycatia-0.6.9/pycatia/scripts/csv_tools.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/simulation_interfaces/replay.py` & `pycatia-0.6.9/pycatia/simulation_interfaces/replay.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/axis_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/axis_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/circle_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/circle_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/control_point_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/control_point_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/curve_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/curve_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/ellipse_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/ellipse_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/factory_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/factory_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/geometric_element.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/geometric_element.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/geometry_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/geometry_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/hyperbola_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/hyperbola_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/line_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/line_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/parabola_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/parabola_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/point_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/point_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/sketch.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/sketch.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/sketcher_interfaces/spline_2D.py` & `pycatia-0.6.9/pycatia/sketcher_interfaces/spline_2D.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/dmo_offset.py` & `pycatia-0.6.9/pycatia/smt_interfaces/dmo_offset.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/dmo_offsets.py` & `pycatia-0.6.9/pycatia/smt_interfaces/dmo_offsets.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/dmo_thickness.py` & `pycatia-0.6.9/pycatia/smt_interfaces/dmo_thickness.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/dmo_thicknesses.py` & `pycatia-0.6.9/pycatia/smt_interfaces/dmo_thicknesses.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/free_space.py` & `pycatia-0.6.9/pycatia/smt_interfaces/free_space.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/free_spaces.py` & `pycatia-0.6.9/pycatia/smt_interfaces/free_spaces.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/merges.py` & `pycatia-0.6.9/pycatia/smt_interfaces/merges.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/optimizer_work_bench.py` & `pycatia-0.6.9/pycatia/smt_interfaces/optimizer_work_bench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/part_comp.py` & `pycatia-0.6.9/pycatia/smt_interfaces/part_comp.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/part_comps.py` & `pycatia-0.6.9/pycatia/smt_interfaces/part_comps.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/silhouette.py` & `pycatia-0.6.9/pycatia/smt_interfaces/silhouette.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/silhouettes.py` & `pycatia-0.6.9/pycatia/smt_interfaces/silhouettes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/simplifications.py` & `pycatia-0.6.9/pycatia/smt_interfaces/simplifications.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/swept_volume.py` & `pycatia-0.6.9/pycatia/smt_interfaces/swept_volume.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/swept_volumes.py` & `pycatia-0.6.9/pycatia/smt_interfaces/swept_volumes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/three_d_cuts.py` & `pycatia-0.6.9/pycatia/smt_interfaces/three_d_cuts.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/vibration_volumes.py` & `pycatia-0.6.9/pycatia/smt_interfaces/vibration_volumes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/wrapping.py` & `pycatia-0.6.9/pycatia/smt_interfaces/wrapping.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/smt_interfaces/wrappings.py` & `pycatia-0.6.9/pycatia/smt_interfaces/wrappings.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/clash.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/clash.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/clash_result.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/clash_result.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/clash_results.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/clash_results.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/clashes.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/clashes.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/conflict.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/conflict.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/conflicts.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/conflicts.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/distance.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/distance.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/distances.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/distances.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/inertia.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/inertia.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/inertias.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/inertias.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/measurable.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/measurable.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/measure_setting_att.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/measure_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/section.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/section.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/sectioning_setting_att.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/sectioning_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/sections.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/sections.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/space_analyses_interfaces/spa_workbench.py` & `pycatia-0.6.9/pycatia/space_analyses_interfaces/spa_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/colour_ess_object_setting_att.py` & `pycatia-0.6.9/pycatia/structure_interfaces/colour_ess_object_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/colour_std_object_setting_att.py` & `pycatia-0.6.9/pycatia/structure_interfaces/colour_std_object_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/material_ess_object_setting_att.py` & `pycatia-0.6.9/pycatia/structure_interfaces/material_ess_object_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/path_ess_resources_setting_att.py` & `pycatia-0.6.9/pycatia/structure_interfaces/path_ess_resources_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/ppg_exec_log_setting_att.py` & `pycatia-0.6.9/pycatia/structure_interfaces/ppg_exec_log_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_anchor_point.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_anchor_point.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_anchor_points.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_anchor_points.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_compute_services.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_compute_services.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_cutback.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_cutback.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_cutout_feature.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_cutout_feature.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_feature_factory.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_feature_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_foundation.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_foundation.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_foundations.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_foundations.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_member.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_member.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_member_extremity.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_member_extremity.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_members.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_members.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_nibbling_feature.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_nibbling_feature.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_object.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_object_ext.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_object_ext.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_object_factory.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_object_factory.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_plate.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_plate.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_plates.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_plates.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_section.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_section.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/str_workbench.py` & `pycatia-0.6.9/pycatia/structure_interfaces/str_workbench.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/structure_interfaces/type_ess_object_setting_att.py` & `pycatia-0.6.9/pycatia/structure_interfaces/type_ess_object_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/surface_machining_interfaces/manufacturing_surface_geom_area.py` & `pycatia-0.6.9/pycatia/surface_machining_interfaces/manufacturing_surface_geom_area.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/surface_machining_interfaces/manufacturing_surface_machining_area.py` & `pycatia-0.6.9/pycatia/surface_machining_interfaces/manufacturing_surface_machining_area.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/accesslog_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/accesslog_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/any_object.py` & `pycatia-0.6.9/pycatia/system_interfaces/any_object.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/cache_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/cache_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/cat_base_dispatch.py` & `pycatia-0.6.9/pycatia/system_interfaces/cat_base_dispatch.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/cat_base_unknown.py` & `pycatia-0.6.9/pycatia/system_interfaces/cat_base_unknown.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/collection.py` & `pycatia-0.6.9/pycatia/system_interfaces/collection.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/command_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/command_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/disconnection_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/disconnection_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/dl_name_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/dl_name_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/dyn_license_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/dyn_license_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/errorlog_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/errorlog_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/file_access_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/file_access_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/general_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/general_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/global_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/global_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/i_dispatch.py` & `pycatia-0.6.9/pycatia/system_interfaces/i_dispatch.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/i_unknown.py` & `pycatia-0.6.9/pycatia/system_interfaces/i_unknown.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/license_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/license_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/memory_warning_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/memory_warning_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/pcs_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/pcs_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/server_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/server_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/session_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/session_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/setting_controller.py` & `pycatia-0.6.9/pycatia/system_interfaces/setting_controller.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/setting_repository.py` & `pycatia-0.6.9/pycatia/system_interfaces/setting_repository.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/system_service.py` & `pycatia-0.6.9/pycatia/system_interfaces/system_service.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/system_interfaces/workbench_statistics_setting_att.py` & `pycatia-0.6.9/pycatia/system_interfaces/workbench_statistics_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/threed_xml_interfaces/export_3d_xml_setting_att.py` & `pycatia-0.6.9/pycatia/threed_xml_interfaces/export_3d_xml_setting_att.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia/types/general.py` & `pycatia-0.6.9/pycatia/types/general.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.6.8/pycatia.egg-info/PKG-INFO` & `pycatia-0.6.9/pycatia.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatia
-Version: 0.6.8
+Version: 0.6.9
 Summary: A python module to interface with the CATIA V5 COM object.
 Home-page: https://github.com/evereux/pycatia
 Author: Paul Bourne
 Author-email: evereux@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,15 @@
 
 .. _pycatia.readthedocs.io: https://pycatia.readthedocs.io
 .. _installation: https://pycatia.readthedocs.io/en/latest/installation.html
 .. _introduction: https://pycatia.readthedocs.io/en/latest/introduction.html
 .. _examples: https://pycatia.readthedocs.io/en/latest/examples.html
 .. _user_scripts: https://pycatia.readthedocs.io/en/latest/user_scripts.html
 .. _pypi.org: https://pypi.org/project/pycatia/
+.. _pycatia-tools: https://github.com/evereux/pycatia-tools
 
 pycatia
 =======
 
 alpha software
 --------------
 
@@ -93,14 +94,16 @@
 
 
 Examples And Scripts
 --------------------
 
 See the documentation @ examples_ and user_scripts_.
 
+A GUI based application that uses pycatia - pycatia-tools_.
+
 
 Asking Questions
 ----------------
 
 Please read the following with regards to raising questions: https://github.com/evereux/pycatia/issues/28
```

### Comparing `pycatia-0.6.8/pycatia.egg-info/SOURCES.txt` & `pycatia-0.6.9/pycatia.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1125,15 +1125,14 @@
 pycatia/product_structure_interfaces/publication.py
 pycatia/product_structure_interfaces/publications.py
 pycatia/reporter_interfaces/__init__.py
 pycatia/reporter_interfaces/rpm_report.py
 pycatia/scripts/__init__.py
 pycatia/scripts/checking.py
 pycatia/scripts/csv_tools.py
-pycatia/scripts/document_types.py
 pycatia/scripts/vba.py
 pycatia/simulation_interfaces/__init__.py
 pycatia/simulation_interfaces/replay.py
 pycatia/sketcher_interfaces/__init__.py
 pycatia/sketcher_interfaces/axis_2D.py
 pycatia/sketcher_interfaces/circle_2D.py
 pycatia/sketcher_interfaces/control_point_2D.py
@@ -1240,9 +1239,9 @@
 pycatia/system_interfaces/setting_controller.py
 pycatia/system_interfaces/setting_repository.py
 pycatia/system_interfaces/system_service.py
 pycatia/system_interfaces/workbench_statistics_setting_att.py
 pycatia/threed_xml_interfaces/__init__.py
 pycatia/threed_xml_interfaces/export_3d_xml_setting_att.py
 pycatia/types/__init__.py
-pycatia/types/document_types.py
+pycatia/types/document.py
 pycatia/types/general.py
```

### Comparing `pycatia-0.6.8/setup.py` & `pycatia-0.6.9/setup.py`

 * *Files identical despite different names*

