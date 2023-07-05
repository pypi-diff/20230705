# Comparing `tmp/resqpy-4.8.9.tar.gz` & `tmp/resqpy-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resqpy-4.8.9.tar", max compression
+gzip compressed data, was "resqpy-4.9.0.tar", max compression
```

## Comparing `resqpy-4.8.9.tar` & `resqpy-4.9.0.tar`

### file list

```diff
@@ -1,198 +1,198 @@
--rw-r--r--   0        0        0     1059 2023-06-01 10:28:07.054076 resqpy-4.8.9/LICENSE
--rw-r--r--   0        0        0     2893 2023-06-01 10:28:07.054076 resqpy-4.8.9/README.md
--rw-r--r--   0        0        0     3354 2023-06-01 10:28:23.206389 resqpy-4.8.9/pyproject.toml
--rw-r--r--   0        0        0      555 2023-06-01 10:28:23.206389 resqpy-4.8.9/resqpy/__init__.py
--rw-r--r--   0        0        0    24782 2023-06-01 10:28:07.066076 resqpy-4.8.9/resqpy/crs.py
--rw-r--r--   0        0        0     1982 2023-06-01 10:28:07.066076 resqpy-4.8.9/resqpy/derived_model/__init__.py
--rw-r--r--   0        0        0     6410 2023-06-01 10:28:07.066076 resqpy-4.8.9/resqpy/derived_model/_add_edges_per_column_property_array.py
--rw-r--r--   0        0        0    21022 2023-06-01 10:28:07.066076 resqpy-4.8.9/resqpy/derived_model/_add_faults.py
--rw-r--r--   0        0        0     6417 2023-06-01 10:28:07.066076 resqpy-4.8.9/resqpy/derived_model/_add_one_blocked_well_property.py
--rw-r--r--   0        0        0     8657 2023-06-01 10:28:07.066076 resqpy-4.8.9/resqpy/derived_model/_add_one_grid_property_array.py
--rw-r--r--   0        0        0     2431 2023-06-01 10:28:07.066076 resqpy-4.8.9/resqpy/derived_model/_add_single_cell_grid.py
--rw-r--r--   0        0        0     5495 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_add_wells_from_ascii_file.py
--rw-r--r--   0        0        0     6037 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_add_zone_by_layer_property.py
--rw-r--r--   0        0        0    11586 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_coarsened_grid.py
--rw-r--r--   0        0        0    10520 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_common.py
--rw-r--r--   0        0        0     3730 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_copy_grid.py
--rw-r--r--   0        0        0    11731 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_drape_to_surface.py
--rw-r--r--   0        0        0    16391 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_extract_box.py
--rw-r--r--   0        0        0    22969 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_extract_box_for_well.py
--rw-r--r--   0        0        0    20325 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_fault_throw_scaling.py
--rw-r--r--   0        0        0     7157 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_gather_ensemble.py
--rw-r--r--   0        0        0    17929 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_interpolated_grid.py
--rw-r--r--   0        0        0     9876 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_local_depth_adjustment.py
--rw-r--r--   0        0        0    20513 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_refined_grid.py
--rw-r--r--   0        0        0     5166 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_tilted_grid.py
--rw-r--r--   0        0        0     4792 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_unsplit_grid.py
--rw-r--r--   0        0        0    18825 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_zonal_grid.py
--rw-r--r--   0        0        0     4358 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/derived_model/_zone_layer_ranges_from_array.py
--rw-r--r--   0        0        0      996 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/fault/__init__.py
--rw-r--r--   0        0        0    29402 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/fault/_gcs_functions.py
--rw-r--r--   0        0        0   109110 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/fault/_grid_connection_set.py
--rw-r--r--   0        0        0      692 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/grid/__init__.py
--rw-r--r--   0        0        0    20689 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/grid/_cell_properties.py
--rw-r--r--   0        0        0    10120 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/grid/_connection_sets.py
--rw-r--r--   0        0        0    19936 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/grid/_create_grid_xml.py
--rw-r--r--   0        0        0    32064 2023-06-01 10:28:07.070076 resqpy-4.8.9/resqpy/grid/_defined_geometry.py
--rw-r--r--   0        0        0    28203 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_extract_functions.py
--rw-r--r--   0        0        0    16516 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_face_functions.py
--rw-r--r--   0        0        0    12236 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_faults.py
--rw-r--r--   0        0        0   127766 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_grid.py
--rw-r--r--   0        0        0     3544 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_grid_types.py
--rw-r--r--   0        0        0      338 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_intervals_info.py
--rw-r--r--   0        0        0      604 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_moved_functions.py
--rw-r--r--   0        0        0     7243 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_pillars.py
--rw-r--r--   0        0        0     5386 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_pixel_maps.py
--rw-r--r--   0        0        0    65440 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_points_functions.py
--rw-r--r--   0        0        0    45761 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_regular_grid.py
--rw-r--r--   0        0        0    19413 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_transmissibility.py
--rw-r--r--   0        0        0     7944 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_write_hdf5_from_caches.py
--rw-r--r--   0        0        0     6147 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_write_nexus_corp.py
--rw-r--r--   0        0        0    13087 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid/_xyz.py
--rw-r--r--   0        0        0     2593 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid_surface/__init__.py
--rw-r--r--   0        0        0    35739 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid_surface/_blocked_well_populate.py
--rw-r--r--   0        0        0    64016 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid_surface/_find_faces.py
--rw-r--r--   0        0        0    26056 2023-06-01 10:28:07.074077 resqpy-4.8.9/resqpy/grid_surface/_grid_skin.py
--rw-r--r--   0        0        0    14379 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/grid_surface/_grid_surface.py
--rw-r--r--   0        0        0    22498 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/grid_surface/_trajectory_intersects.py
--rw-r--r--   0        0        0    39760 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/grid_surface/grid_surface_cuda.py
--rw-r--r--   0        0        0      539 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/lines/__init__.py
--rw-r--r--   0        0        0    11960 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/lines/_common.py
--rw-r--r--   0        0        0    41425 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/lines/_polyline.py
--rw-r--r--   0        0        0    26366 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/lines/_polyline_set.py
--rw-r--r--   0        0        0      378 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/model/__init__.py
--rw-r--r--   0        0        0    30205 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/model/_catalogue.py
--rw-r--r--   0        0        0     2840 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/model/_context.py
--rw-r--r--   0        0        0    34552 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/model/_forestry.py
--rw-r--r--   0        0        0     3371 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/model/_grids.py
--rw-r--r--   0        0        0    14238 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/model/_hdf5.py
--rw-r--r--   0        0        0   103055 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/model/_model.py
--rw-r--r--   0        0        0    23589 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/model/_xml.py
--rw-r--r--   0        0        0      909 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/multi_processing/__init__.py
--rw-r--r--   0        0        0     7301 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/multi_processing/_multiprocessing.py
--rw-r--r--   0        0        0       72 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/multi_processing/wrappers/__init__.py
--rw-r--r--   0        0        0     5952 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/multi_processing/wrappers/blocked_well_mp.py
--rw-r--r--   0        0        0    21156 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/multi_processing/wrappers/grid_surface_mp.py
--rw-r--r--   0        0        0     5793 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/multi_processing/wrappers/mesh_mp.py
--rw-r--r--   0        0        0       84 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/olio/__init__.py
--rw-r--r--   0        0        0     2147 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/olio/ab_toolbox.py
--rw-r--r--   0        0        0     7521 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/olio/base.py
--rw-r--r--   0        0        0    20925 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/olio/box_utilities.py
--rw-r--r--   0        0        0     5935 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/olio/class_dict.py
--rw-r--r--   0        0        0     9489 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/olio/consolidation.py
--rw-r--r--   0        0        0     5177 2023-06-01 10:28:07.078076 resqpy-4.8.9/resqpy/olio/data/build.py
--rw-r--r--   0        0        0   498136 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/data/properties.json
--rw-r--r--   0        0        0    19836 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/dataframe.py
--rw-r--r--   0        0        0      307 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/exceptions.py
--rw-r--r--   0        0        0     1313 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/factors.py
--rw-r--r--   0        0        0    24541 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/fine_coarse.py
--rw-r--r--   0        0        0    27669 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/grid_functions.py
--rw-r--r--   0        0        0    20158 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/intersection.py
--rw-r--r--   0        0        0     8408 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/keyword_files.py
--rw-r--r--   0        0        0    19210 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/load_data.py
--rw-r--r--   0        0        0     6628 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/point_inclusion.py
--rw-r--r--   0        0        0     1103 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/random_seed.py
--rw-r--r--   0        0        0     5441 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/read_nexus_fault.py
--rw-r--r--   0        0        0    17083 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/relperm.py
--rw-r--r--   0        0        0    12189 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/simple_lines.py
--rw-r--r--   0        0        0      760 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/time.py
--rw-r--r--   0        0        0      822 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/trademark.py
--rw-r--r--   0        0        0    61869 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/transmission.py
--rw-r--r--   0        0        0    44768 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/triangulation.py
--rw-r--r--   0        0        0     7324 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/uuid.py
--rw-r--r--   0        0        0    45231 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/vdb.py
--rw-r--r--   0        0        0    46253 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/vector_utilities.py
--rw-r--r--   0        0        0     6185 2023-06-01 10:28:07.082077 resqpy-4.8.9/resqpy/olio/volume.py
--rw-r--r--   0        0        0    26220 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/olio/wellspec_keywords.py
--rw-r--r--   0        0        0     5142 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/olio/write_data.py
--rw-r--r--   0        0        0    19055 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/olio/write_hdf5.py
--rw-r--r--   0        0        0    24925 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/olio/xml_et.py
--rw-r--r--   0        0        0     1824 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/olio/xml_namespaces.py
--rw-r--r--   0        0        0     5709 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/olio/zmap_reader.py
--rw-r--r--   0        0        0     2206 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/__init__.py
--rw-r--r--   0        0        0     2937 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/_utils.py
--rw-r--r--   0        0        0     1685 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/boundary_feature.py
--rw-r--r--   0        0        0     5190 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/boundary_feature_interpretation.py
--rw-r--r--   0        0        0     6186 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/earth_model_interpretation.py
--rw-r--r--   0        0        0    12457 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/fault_interpretation.py
--rw-r--r--   0        0        0     2757 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/fluid_boundary_feature.py
--rw-r--r--   0        0        0     1702 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/frontier_feature.py
--rw-r--r--   0        0        0     4498 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/generic_interpretation.py
--rw-r--r--   0        0        0     3771 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/genetic_boundary_feature.py
--rw-r--r--   0        0        0     8605 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/geobody_boundary_interpretation.py
--rw-r--r--   0        0        0     1836 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/geobody_feature.py
--rw-r--r--   0        0        0     8052 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/geobody_interpretation.py
--rw-r--r--   0        0        0     1739 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/geologic_unit_feature.py
--rw-r--r--   0        0        0     8346 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/horizon_interpretation.py
--rw-r--r--   0        0        0     2697 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/organization_feature.py
--rw-r--r--   0        0        0     5565 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/rock_fluid_unit_feature.py
--rw-r--r--   0        0        0     1802 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/structural_organization_interpretation.py
--rw-r--r--   0        0        0     2675 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/tectonic_boundary_feature.py
--rw-r--r--   0        0        0     1843 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/wellbore_feature.py
--rw-r--r--   0        0        0     6973 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/organize/wellbore_interpretation.py
--rw-r--r--   0        0        0     2155 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/property/__init__.py
--rw-r--r--   0        0        0    16697 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/property/_collection_add_part.py
--rw-r--r--   0        0        0    12926 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/property/_collection_create_xml.py
--rw-r--r--   0        0        0    30090 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/property/_collection_get_attributes.py
--rw-r--r--   0        0        0     5368 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/property/_collection_support.py
--rw-r--r--   0        0        0    24426 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/property/_property.py
--rw-r--r--   0        0        0    66946 2023-06-01 10:28:07.086077 resqpy-4.8.9/resqpy/property/grid_property_collection.py
--rw-r--r--   0        0        0   143306 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/property/property_collection.py
--rw-r--r--   0        0        0    36127 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/property/property_common.py
--rw-r--r--   0        0        0     5557 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/property/property_kind.py
--rw-r--r--   0        0        0     7737 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/property/string_lookup.py
--rw-r--r--   0        0        0     1077 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/property/well_interval_property.py
--rw-r--r--   0        0        0     1577 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/property/well_interval_property_collection.py
--rw-r--r--   0        0        0     1205 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/property/well_log.py
--rw-r--r--   0        0        0     7633 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/property/well_log_collection.py
--rw-r--r--   0        0        0      713 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/rq_import/__init__.py
--rw-r--r--   0        0        0     4493 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/rq_import/_add_ab_properties.py
--rw-r--r--   0        0        0     6067 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/rq_import/_add_surfaces.py
--rw-r--r--   0        0        0    32019 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/rq_import/_grid_from_cp.py
--rw-r--r--   0        0        0    34317 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/rq_import/_import_nexus.py
--rw-r--r--   0        0        0     6306 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/rq_import/_import_vdb_all_grids.py
--rw-r--r--   0        0        0    21372 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/rq_import/_import_vdb_ensemble.py
--rw-r--r--   0        0        0     1311 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/strata/__init__.py
--rw-r--r--   0        0        0     8861 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/strata/_binary_contact_interpretation.py
--rw-r--r--   0        0        0    10381 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/strata/_geologic_unit_interpretation.py
--rw-r--r--   0        0        0     1772 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/strata/_strata_common.py
--rw-r--r--   0        0        0     6797 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/strata/_stratigraphic_column.py
--rw-r--r--   0        0        0    13322 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/strata/_stratigraphic_column_rank.py
--rw-r--r--   0        0        0     7432 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/strata/_stratigraphic_unit_feature.py
--rw-r--r--   0        0        0    10167 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/strata/_stratigraphic_unit_interpretation.py
--rw-r--r--   0        0        0      696 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/surface/__init__.py
--rw-r--r--   0        0        0     2331 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/surface/_base_surface.py
--rw-r--r--   0        0        0     3082 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/surface/_combined_surface.py
--rw-r--r--   0        0        0    42192 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/surface/_mesh.py
--rw-r--r--   0        0        0    26120 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/surface/_pointset.py
--rw-r--r--   0        0        0    56386 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/surface/_surface.py
--rw-r--r--   0        0        0    24315 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/surface/_tri_mesh.py
--rw-r--r--   0        0        0    25907 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/surface/_triangulated_patch.py
--rw-r--r--   0        0        0     1074 2023-06-01 10:28:07.090077 resqpy-4.8.9/resqpy/time_series/__init__.py
--rw-r--r--   0        0        0     8595 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/time_series/_any_time_series.py
--rw-r--r--   0        0        0     6617 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/time_series/_from_nexus_summary.py
--rw-r--r--   0        0        0     6366 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/time_series/_functions.py
--rw-r--r--   0        0        0     3311 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/time_series/_geologic_time_series.py
--rw-r--r--   0        0        0     2759 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/time_series/_time_duration.py
--rw-r--r--   0        0        0    10818 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/time_series/_time_series.py
--rw-r--r--   0        0        0      603 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/unstructured/__init__.py
--rw-r--r--   0        0        0    15328 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/unstructured/_hexa_grid.py
--rw-r--r--   0        0        0    35856 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/unstructured/_prism_grid.py
--rw-r--r--   0        0        0     7862 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/unstructured/_pyramid_grid.py
--rw-r--r--   0        0        0    10208 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/unstructured/_tetra_grid.py
--rw-r--r--   0        0        0    51550 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/unstructured/_unstructured_grid.py
--rw-r--r--   0        0        0     1135 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/weights_and_measures/__init__.py
--rw-r--r--   0        0        0     5434 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/weights_and_measures/nexus_units.py
--rw-r--r--   0        0        0    16186 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/weights_and_measures/weights_and_measures.py
--rw-r--r--   0        0        0      990 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/__init__.py
--rw-r--r--   0        0        0   188806 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/_blocked_well.py
--rw-r--r--   0        0        0    22138 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/_deviation_survey.py
--rw-r--r--   0        0        0     7154 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/_md_datum.py
--rw-r--r--   0        0        0    50015 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/_trajectory.py
--rw-r--r--   0        0        0    15192 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/_wellbore_frame.py
--rw-r--r--   0        0        0     8403 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/_wellbore_marker.py
--rw-r--r--   0        0        0    20933 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/_wellbore_marker_frame.py
--rw-r--r--   0        0        0    22555 2023-06-01 10:28:07.094077 resqpy-4.8.9/resqpy/well/blocked_well_frame.py
--rw-r--r--   0        0        0    24703 2023-06-01 10:28:07.098077 resqpy-4.8.9/resqpy/well/well_object_funcs.py
--rw-r--r--   0        0        0     5969 2023-06-01 10:28:07.098077 resqpy-4.8.9/resqpy/well/well_utils.py
--rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 resqpy-4.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-28 14:27:39.060922 resqpy-4.9.0/LICENSE
+-rw-r--r--   0        0        0     2893 2023-06-28 14:27:39.060922 resqpy-4.9.0/README.md
+-rw-r--r--   0        0        0     3354 2023-06-28 14:27:59.280961 resqpy-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-06-28 14:27:59.280961 resqpy-4.9.0/resqpy/__init__.py
+-rw-r--r--   0        0        0    24782 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/crs.py
+-rw-r--r--   0        0        0     1982 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/__init__.py
+-rw-r--r--   0        0        0     6410 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/_add_edges_per_column_property_array.py
+-rw-r--r--   0        0        0    21022 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/_add_faults.py
+-rw-r--r--   0        0        0     6417 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/_add_one_blocked_well_property.py
+-rw-r--r--   0        0        0     8657 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/_add_one_grid_property_array.py
+-rw-r--r--   0        0        0     2431 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/_add_single_cell_grid.py
+-rw-r--r--   0        0        0     5495 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/_add_wells_from_ascii_file.py
+-rw-r--r--   0        0        0     6037 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/_add_zone_by_layer_property.py
+-rw-r--r--   0        0        0    11586 2023-06-28 14:27:39.072922 resqpy-4.9.0/resqpy/derived_model/_coarsened_grid.py
+-rw-r--r--   0        0        0    10520 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_common.py
+-rw-r--r--   0        0        0     3730 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_copy_grid.py
+-rw-r--r--   0        0        0    11731 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_drape_to_surface.py
+-rw-r--r--   0        0        0    16391 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_extract_box.py
+-rw-r--r--   0        0        0    22969 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_extract_box_for_well.py
+-rw-r--r--   0        0        0    20325 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_fault_throw_scaling.py
+-rw-r--r--   0        0        0     7157 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_gather_ensemble.py
+-rw-r--r--   0        0        0    17929 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_interpolated_grid.py
+-rw-r--r--   0        0        0     9876 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_local_depth_adjustment.py
+-rw-r--r--   0        0        0    20513 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_refined_grid.py
+-rw-r--r--   0        0        0     5166 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_tilted_grid.py
+-rw-r--r--   0        0        0     4792 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_unsplit_grid.py
+-rw-r--r--   0        0        0    18825 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_zonal_grid.py
+-rw-r--r--   0        0        0     4358 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/derived_model/_zone_layer_ranges_from_array.py
+-rw-r--r--   0        0        0      996 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/fault/__init__.py
+-rw-r--r--   0        0        0    29402 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/fault/_gcs_functions.py
+-rw-r--r--   0        0        0   109110 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/fault/_grid_connection_set.py
+-rw-r--r--   0        0        0      692 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/__init__.py
+-rw-r--r--   0        0        0    20689 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/_cell_properties.py
+-rw-r--r--   0        0        0    10120 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/_connection_sets.py
+-rw-r--r--   0        0        0    19936 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/_create_grid_xml.py
+-rw-r--r--   0        0        0    32064 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/_defined_geometry.py
+-rw-r--r--   0        0        0    28203 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/_extract_functions.py
+-rw-r--r--   0        0        0    16516 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/_face_functions.py
+-rw-r--r--   0        0        0    12236 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/_faults.py
+-rw-r--r--   0        0        0   127766 2023-06-28 14:27:39.076922 resqpy-4.9.0/resqpy/grid/_grid.py
+-rw-r--r--   0        0        0     3544 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_grid_types.py
+-rw-r--r--   0        0        0      338 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_intervals_info.py
+-rw-r--r--   0        0        0      604 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_moved_functions.py
+-rw-r--r--   0        0        0     7243 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_pillars.py
+-rw-r--r--   0        0        0     5386 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_pixel_maps.py
+-rw-r--r--   0        0        0    65440 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_points_functions.py
+-rw-r--r--   0        0        0    45761 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_regular_grid.py
+-rw-r--r--   0        0        0    19413 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_transmissibility.py
+-rw-r--r--   0        0        0     7944 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_write_hdf5_from_caches.py
+-rw-r--r--   0        0        0     6147 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_write_nexus_corp.py
+-rw-r--r--   0        0        0    13087 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid/_xyz.py
+-rw-r--r--   0        0        0     2593 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid_surface/__init__.py
+-rw-r--r--   0        0        0    35739 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid_surface/_blocked_well_populate.py
+-rw-r--r--   0        0        0    64016 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid_surface/_find_faces.py
+-rw-r--r--   0        0        0    26056 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid_surface/_grid_skin.py
+-rw-r--r--   0        0        0    14379 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid_surface/_grid_surface.py
+-rw-r--r--   0        0        0    22498 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid_surface/_trajectory_intersects.py
+-rw-r--r--   0        0        0    39760 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/grid_surface/grid_surface_cuda.py
+-rw-r--r--   0        0        0      539 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/lines/__init__.py
+-rw-r--r--   0        0        0    11960 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/lines/_common.py
+-rw-r--r--   0        0        0    42464 2023-06-28 14:27:39.080922 resqpy-4.9.0/resqpy/lines/_polyline.py
+-rw-r--r--   0        0        0    27721 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/lines/_polyline_set.py
+-rw-r--r--   0        0        0      378 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/model/__init__.py
+-rw-r--r--   0        0        0    30205 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/model/_catalogue.py
+-rw-r--r--   0        0        0     2840 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/model/_context.py
+-rw-r--r--   0        0        0    34552 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/model/_forestry.py
+-rw-r--r--   0        0        0     3371 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/model/_grids.py
+-rw-r--r--   0        0        0    14238 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/model/_hdf5.py
+-rw-r--r--   0        0        0   103055 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/model/_model.py
+-rw-r--r--   0        0        0    23589 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/model/_xml.py
+-rw-r--r--   0        0        0      909 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/multi_processing/__init__.py
+-rw-r--r--   0        0        0     7301 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/multi_processing/_multiprocessing.py
+-rw-r--r--   0        0        0       72 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/multi_processing/wrappers/__init__.py
+-rw-r--r--   0        0        0     5952 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/multi_processing/wrappers/blocked_well_mp.py
+-rw-r--r--   0        0        0    21156 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/multi_processing/wrappers/grid_surface_mp.py
+-rw-r--r--   0        0        0     5793 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/multi_processing/wrappers/mesh_mp.py
+-rw-r--r--   0        0        0       84 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/olio/__init__.py
+-rw-r--r--   0        0        0     2147 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/olio/ab_toolbox.py
+-rw-r--r--   0        0        0     7521 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/olio/base.py
+-rw-r--r--   0        0        0    20925 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/olio/box_utilities.py
+-rw-r--r--   0        0        0     5935 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/olio/class_dict.py
+-rw-r--r--   0        0        0     9489 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/olio/consolidation.py
+-rw-r--r--   0        0        0     5177 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/olio/data/build.py
+-rw-r--r--   0        0        0   498136 2023-06-28 14:27:39.084922 resqpy-4.9.0/resqpy/olio/data/properties.json
+-rw-r--r--   0        0        0    19836 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/dataframe.py
+-rw-r--r--   0        0        0      307 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/exceptions.py
+-rw-r--r--   0        0        0     1313 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/factors.py
+-rw-r--r--   0        0        0    24541 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/fine_coarse.py
+-rw-r--r--   0        0        0    27669 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/grid_functions.py
+-rw-r--r--   0        0        0    20158 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/intersection.py
+-rw-r--r--   0        0        0     8408 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/keyword_files.py
+-rw-r--r--   0        0        0    19210 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/load_data.py
+-rw-r--r--   0        0        0     6628 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/point_inclusion.py
+-rw-r--r--   0        0        0     1103 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/random_seed.py
+-rw-r--r--   0        0        0     5441 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/read_nexus_fault.py
+-rw-r--r--   0        0        0    17083 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/relperm.py
+-rw-r--r--   0        0        0    12189 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/simple_lines.py
+-rw-r--r--   0        0        0      760 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/time.py
+-rw-r--r--   0        0        0      822 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/trademark.py
+-rw-r--r--   0        0        0    61869 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/transmission.py
+-rw-r--r--   0        0        0    44768 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/triangulation.py
+-rw-r--r--   0        0        0     7324 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/uuid.py
+-rw-r--r--   0        0        0    45231 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/vdb.py
+-rw-r--r--   0        0        0    46253 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/vector_utilities.py
+-rw-r--r--   0        0        0     6185 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/volume.py
+-rw-r--r--   0        0        0    26220 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/wellspec_keywords.py
+-rw-r--r--   0        0        0     5142 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/write_data.py
+-rw-r--r--   0        0        0    19055 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/write_hdf5.py
+-rw-r--r--   0        0        0    24925 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/xml_et.py
+-rw-r--r--   0        0        0     1824 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/xml_namespaces.py
+-rw-r--r--   0        0        0     5709 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/olio/zmap_reader.py
+-rw-r--r--   0        0        0     2206 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/organize/__init__.py
+-rw-r--r--   0        0        0     2937 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/organize/_utils.py
+-rw-r--r--   0        0        0     1685 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/organize/boundary_feature.py
+-rw-r--r--   0        0        0     5190 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/organize/boundary_feature_interpretation.py
+-rw-r--r--   0        0        0     6186 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/organize/earth_model_interpretation.py
+-rw-r--r--   0        0        0    12457 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/organize/fault_interpretation.py
+-rw-r--r--   0        0        0     2757 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/organize/fluid_boundary_feature.py
+-rw-r--r--   0        0        0     1702 2023-06-28 14:27:39.088922 resqpy-4.9.0/resqpy/organize/frontier_feature.py
+-rw-r--r--   0        0        0     4498 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/generic_interpretation.py
+-rw-r--r--   0        0        0     3771 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/genetic_boundary_feature.py
+-rw-r--r--   0        0        0     8605 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/geobody_boundary_interpretation.py
+-rw-r--r--   0        0        0     1836 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/geobody_feature.py
+-rw-r--r--   0        0        0     8052 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/geobody_interpretation.py
+-rw-r--r--   0        0        0     1739 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/geologic_unit_feature.py
+-rw-r--r--   0        0        0     8346 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/horizon_interpretation.py
+-rw-r--r--   0        0        0     2697 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/organization_feature.py
+-rw-r--r--   0        0        0     5565 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/rock_fluid_unit_feature.py
+-rw-r--r--   0        0        0     1802 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/structural_organization_interpretation.py
+-rw-r--r--   0        0        0     2675 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/tectonic_boundary_feature.py
+-rw-r--r--   0        0        0     1843 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/wellbore_feature.py
+-rw-r--r--   0        0        0     6973 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/organize/wellbore_interpretation.py
+-rw-r--r--   0        0        0     2155 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/__init__.py
+-rw-r--r--   0        0        0    16961 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/_collection_add_part.py
+-rw-r--r--   0        0        0    12926 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/_collection_create_xml.py
+-rw-r--r--   0        0        0    31893 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/_collection_get_attributes.py
+-rw-r--r--   0        0        0     5889 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/_collection_support.py
+-rw-r--r--   0        0        0    24426 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/_property.py
+-rw-r--r--   0        0        0    66946 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/grid_property_collection.py
+-rw-r--r--   0        0        0   143771 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/property_collection.py
+-rw-r--r--   0        0        0    36370 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/property_common.py
+-rw-r--r--   0        0        0     5557 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/property_kind.py
+-rw-r--r--   0        0        0     7737 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/string_lookup.py
+-rw-r--r--   0        0        0     1077 2023-06-28 14:27:39.092923 resqpy-4.9.0/resqpy/property/well_interval_property.py
+-rw-r--r--   0        0        0     1610 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/property/well_interval_property_collection.py
+-rw-r--r--   0        0        0     1205 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/property/well_log.py
+-rw-r--r--   0        0        0     7633 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/property/well_log_collection.py
+-rw-r--r--   0        0        0      713 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/rq_import/__init__.py
+-rw-r--r--   0        0        0     4493 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/rq_import/_add_ab_properties.py
+-rw-r--r--   0        0        0     6067 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/rq_import/_add_surfaces.py
+-rw-r--r--   0        0        0    32019 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/rq_import/_grid_from_cp.py
+-rw-r--r--   0        0        0    34317 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/rq_import/_import_nexus.py
+-rw-r--r--   0        0        0     6306 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/rq_import/_import_vdb_all_grids.py
+-rw-r--r--   0        0        0    21372 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/rq_import/_import_vdb_ensemble.py
+-rw-r--r--   0        0        0     1311 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/strata/__init__.py
+-rw-r--r--   0        0        0     8861 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/strata/_binary_contact_interpretation.py
+-rw-r--r--   0        0        0    10381 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/strata/_geologic_unit_interpretation.py
+-rw-r--r--   0        0        0     1772 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/strata/_strata_common.py
+-rw-r--r--   0        0        0     6797 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/strata/_stratigraphic_column.py
+-rw-r--r--   0        0        0    13322 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/strata/_stratigraphic_column_rank.py
+-rw-r--r--   0        0        0     7432 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/strata/_stratigraphic_unit_feature.py
+-rw-r--r--   0        0        0    10167 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/strata/_stratigraphic_unit_interpretation.py
+-rw-r--r--   0        0        0      696 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/surface/__init__.py
+-rw-r--r--   0        0        0     2331 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/surface/_base_surface.py
+-rw-r--r--   0        0        0     3082 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/surface/_combined_surface.py
+-rw-r--r--   0        0        0    42192 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/surface/_mesh.py
+-rw-r--r--   0        0        0    27024 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/surface/_pointset.py
+-rw-r--r--   0        0        0    58417 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/surface/_surface.py
+-rw-r--r--   0        0        0    24315 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/surface/_tri_mesh.py
+-rw-r--r--   0        0        0    25907 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/surface/_triangulated_patch.py
+-rw-r--r--   0        0        0     1074 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/time_series/__init__.py
+-rw-r--r--   0        0        0     8595 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/time_series/_any_time_series.py
+-rw-r--r--   0        0        0     6617 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/time_series/_from_nexus_summary.py
+-rw-r--r--   0        0        0     6366 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/time_series/_functions.py
+-rw-r--r--   0        0        0     3311 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/time_series/_geologic_time_series.py
+-rw-r--r--   0        0        0     2759 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/time_series/_time_duration.py
+-rw-r--r--   0        0        0    10818 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/time_series/_time_series.py
+-rw-r--r--   0        0        0      603 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/unstructured/__init__.py
+-rw-r--r--   0        0        0    15328 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/unstructured/_hexa_grid.py
+-rw-r--r--   0        0        0    35856 2023-06-28 14:27:39.096923 resqpy-4.9.0/resqpy/unstructured/_prism_grid.py
+-rw-r--r--   0        0        0     7862 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/unstructured/_pyramid_grid.py
+-rw-r--r--   0        0        0    10208 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/unstructured/_tetra_grid.py
+-rw-r--r--   0        0        0    51550 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/unstructured/_unstructured_grid.py
+-rw-r--r--   0        0        0     1135 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/weights_and_measures/__init__.py
+-rw-r--r--   0        0        0     5434 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/weights_and_measures/nexus_units.py
+-rw-r--r--   0        0        0    16186 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/weights_and_measures/weights_and_measures.py
+-rw-r--r--   0        0        0      990 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/__init__.py
+-rw-r--r--   0        0        0   188822 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/_blocked_well.py
+-rw-r--r--   0        0        0    22138 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/_deviation_survey.py
+-rw-r--r--   0        0        0     7154 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/_md_datum.py
+-rw-r--r--   0        0        0    50015 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/_trajectory.py
+-rw-r--r--   0        0        0    15192 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/_wellbore_frame.py
+-rw-r--r--   0        0        0     8403 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/_wellbore_marker.py
+-rw-r--r--   0        0        0    20933 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/_wellbore_marker_frame.py
+-rw-r--r--   0        0        0    22555 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/blocked_well_frame.py
+-rw-r--r--   0        0        0    24703 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/well_object_funcs.py
+-rw-r--r--   0        0        0     5969 2023-06-28 14:27:39.100923 resqpy-4.9.0/resqpy/well/well_utils.py
+-rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 resqpy-4.9.0/PKG-INFO
```

### Comparing `resqpy-4.8.9/LICENSE` & `resqpy-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/README.md` & `resqpy-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/pyproject.toml` & `resqpy-4.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["poetry>=1.0.2", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "resqpy"
-version = "4.8.9" # Set at build time
+version = "4.9.0" # Set at build time
 description = "Python API for working with RESQML models"
 authors = ["BP"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bp/resqpy"
 documentation = "https://resqpy.readthedocs.io/en/latest/"
 keywords = ["RESQML"]
```

### Comparing `resqpy-4.8.9/resqpy/__init__.py` & `resqpy-4.9.0/resqpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,10 @@
     weights_and_measures
     well
     olio
 """
 
 import logging
 
-__version__ = "4.8.9"  # Set at build time
+__version__ = "4.9.0"  # Set at build time
 log = logging.getLogger(__name__)
 log.info(f"Imported resqpy version {__version__}")
```

### Comparing `resqpy-4.8.9/resqpy/crs.py` & `resqpy-4.9.0/resqpy/crs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/__init__.py` & `resqpy-4.9.0/resqpy/derived_model/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_add_edges_per_column_property_array.py` & `resqpy-4.9.0/resqpy/derived_model/_add_edges_per_column_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_add_faults.py` & `resqpy-4.9.0/resqpy/derived_model/_add_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_add_one_blocked_well_property.py` & `resqpy-4.9.0/resqpy/derived_model/_add_one_blocked_well_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_add_one_grid_property_array.py` & `resqpy-4.9.0/resqpy/derived_model/_add_one_grid_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_add_single_cell_grid.py` & `resqpy-4.9.0/resqpy/derived_model/_add_single_cell_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_add_wells_from_ascii_file.py` & `resqpy-4.9.0/resqpy/derived_model/_add_wells_from_ascii_file.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_add_zone_by_layer_property.py` & `resqpy-4.9.0/resqpy/derived_model/_add_zone_by_layer_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_coarsened_grid.py` & `resqpy-4.9.0/resqpy/derived_model/_coarsened_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_common.py` & `resqpy-4.9.0/resqpy/derived_model/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_copy_grid.py` & `resqpy-4.9.0/resqpy/derived_model/_copy_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_drape_to_surface.py` & `resqpy-4.9.0/resqpy/derived_model/_drape_to_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_extract_box.py` & `resqpy-4.9.0/resqpy/derived_model/_extract_box.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_extract_box_for_well.py` & `resqpy-4.9.0/resqpy/derived_model/_extract_box_for_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_fault_throw_scaling.py` & `resqpy-4.9.0/resqpy/derived_model/_fault_throw_scaling.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_gather_ensemble.py` & `resqpy-4.9.0/resqpy/derived_model/_gather_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_interpolated_grid.py` & `resqpy-4.9.0/resqpy/derived_model/_interpolated_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_local_depth_adjustment.py` & `resqpy-4.9.0/resqpy/derived_model/_local_depth_adjustment.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_refined_grid.py` & `resqpy-4.9.0/resqpy/derived_model/_refined_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_tilted_grid.py` & `resqpy-4.9.0/resqpy/derived_model/_tilted_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_unsplit_grid.py` & `resqpy-4.9.0/resqpy/derived_model/_unsplit_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_zonal_grid.py` & `resqpy-4.9.0/resqpy/derived_model/_zonal_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/derived_model/_zone_layer_ranges_from_array.py` & `resqpy-4.9.0/resqpy/derived_model/_zone_layer_ranges_from_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/fault/__init__.py` & `resqpy-4.9.0/resqpy/fault/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/fault/_gcs_functions.py` & `resqpy-4.9.0/resqpy/fault/_gcs_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/fault/_grid_connection_set.py` & `resqpy-4.9.0/resqpy/fault/_grid_connection_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/__init__.py` & `resqpy-4.9.0/resqpy/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_cell_properties.py` & `resqpy-4.9.0/resqpy/grid/_cell_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_connection_sets.py` & `resqpy-4.9.0/resqpy/grid/_connection_sets.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_create_grid_xml.py` & `resqpy-4.9.0/resqpy/grid/_create_grid_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_defined_geometry.py` & `resqpy-4.9.0/resqpy/grid/_defined_geometry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_extract_functions.py` & `resqpy-4.9.0/resqpy/grid/_extract_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_face_functions.py` & `resqpy-4.9.0/resqpy/grid/_face_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_faults.py` & `resqpy-4.9.0/resqpy/grid/_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_grid.py` & `resqpy-4.9.0/resqpy/grid/_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_grid_types.py` & `resqpy-4.9.0/resqpy/grid/_grid_types.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_moved_functions.py` & `resqpy-4.9.0/resqpy/grid/_moved_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_pillars.py` & `resqpy-4.9.0/resqpy/grid/_pillars.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_pixel_maps.py` & `resqpy-4.9.0/resqpy/grid/_pixel_maps.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_points_functions.py` & `resqpy-4.9.0/resqpy/grid/_points_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_regular_grid.py` & `resqpy-4.9.0/resqpy/grid/_regular_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_transmissibility.py` & `resqpy-4.9.0/resqpy/grid/_transmissibility.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_write_hdf5_from_caches.py` & `resqpy-4.9.0/resqpy/grid/_write_hdf5_from_caches.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_write_nexus_corp.py` & `resqpy-4.9.0/resqpy/grid/_write_nexus_corp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid/_xyz.py` & `resqpy-4.9.0/resqpy/grid/_xyz.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid_surface/__init__.py` & `resqpy-4.9.0/resqpy/grid_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid_surface/_blocked_well_populate.py` & `resqpy-4.9.0/resqpy/grid_surface/_blocked_well_populate.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid_surface/_find_faces.py` & `resqpy-4.9.0/resqpy/grid_surface/_find_faces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid_surface/_grid_skin.py` & `resqpy-4.9.0/resqpy/grid_surface/_grid_skin.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid_surface/_grid_surface.py` & `resqpy-4.9.0/resqpy/grid_surface/_grid_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid_surface/_trajectory_intersects.py` & `resqpy-4.9.0/resqpy/grid_surface/_trajectory_intersects.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/grid_surface/grid_surface_cuda.py` & `resqpy-4.9.0/resqpy/grid_surface/grid_surface_cuda.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/lines/__init__.py` & `resqpy-4.9.0/resqpy/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/lines/_common.py` & `resqpy-4.9.0/resqpy/lines/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/lines/_polyline.py` & `resqpy-4.9.0/resqpy/lines/_polyline.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import math as maths
 import numpy as np
 import warnings
 
 import resqpy.olio.intersection as meet
 import resqpy.lines
+import resqpy.property as rqp
 import resqpy.olio.point_inclusion as pip
 import resqpy.olio.uuid as bu
 import resqpy.olio.vector_utilities as vu
 import resqpy.olio.write_hdf5 as rwh5
 import resqpy.olio.xml_et as rqet
 import resqpy.lines._common as rql_c
 from resqpy.olio.xml_namespaces import curly_namespace as ns
@@ -70,14 +71,15 @@
                 is_closed = set_bool
         self.isclosed = is_closed
         self.nodepatch = None
         self.crs_uuid = set_crs
         self.coordinates = None
         self.centre = None
         self.rep_int_root = rep_int_root  # Optional represented interpretation xml root node
+        self.property_collection = None
         super().__init__(model = parent_model,
                          uuid = uuid,
                          title = title,
                          originator = originator,
                          extra_metadata = extra_metadata)
 
         if self.root is None and all(i is not None for i in [is_closed, set_coord, set_crs, title]):
@@ -813,14 +815,35 @@
             xy = np.stack(np.meshgrid(x, y), axis = -1).reshape((-1, 2))
             inside = pip.pip_array_cn(xy, self.coordinates)
             nf_xy = n_xy.astype(float)
             d_xy *= (nf_xy + 1.0) / nf_xy
             a = d_xy[0] * d_xy[1] * float(np.count_nonzero(inside)) / float(inside.size)
         return a
 
+    def extract_property_collection(self, refresh = False):
+        """Returns a property collection for the polyline.
+
+        arguments:
+            refresh (bool, default False): if True, the property collection is refreshed
+                from the current state of the model; if False and the property collection
+                has already been cached for the polyline, then the cached copy is used
+
+        returns:
+            a PropertyCollection holding those properties in the model where this polyline
+            is the supporting representation
+
+        notes:
+            polyline properties may have indexable element of 'nodes' or 'intervals';
+            for interval properties, the number of elements depends on whether the
+            polyline is closed or not
+        """
+        if self.property_collection is None or refresh:
+            self.property_collection = rqp.PropertyCollection(support = self)
+        return self.property_collection
+
     def create_xml(self,
                    ext_uuid = None,
                    add_as_part = True,
                    add_relationships = True,
                    title = None,
                    originator = None):
         """Create xml for polyline and optionally adds as part to model.
```

### Comparing `resqpy-4.8.9/resqpy/lines/_polyline_set.py` & `resqpy-4.9.0/resqpy/lines/_polyline_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 log = logging.getLogger(__name__)
 
 import os
 import numpy as np
 
 import resqpy.crs as rcrs
 import resqpy.lines
+import resqpy.property as rqp
 import resqpy.olio.simple_lines as rsl
 import resqpy.olio.uuid as bu
 import resqpy.olio.vector_utilities as vu
 import resqpy.olio.write_hdf5 as rwh5
 import resqpy.olio.xml_et as rqet
 import resqpy.lines._common as rql_c
 from resqpy.olio.xml_namespaces import curly_namespace as ns
@@ -67,14 +68,15 @@
         self.rep_int_root = None
         self.save_polys = False
         self.boolnotconstant = None
         self.boolvalue = None
         self.closed_array = None
         self.crs_uuid = crs_uuid
         self.indices = None
+        self.property_collection = None
 
         super().__init__(model = parent_model,
                          uuid = uuid,
                          title = title,
                          originator = originator,
                          extra_metadata = extra_metadata)
 
@@ -95,15 +97,15 @@
             self.polys = polylines
             # Setting the title of the first polyline given as the PolylineSet title
             if not self.title:
                 if len(polylines) > 1:
                     self.title = f"{polylines[0].title} + {len(polylines)-1} polylines"
                 else:
                     self.title = polylines[0].title
-
+            self.combine_polylines(polylines)
         elif irap_file is not None:  # Create from an input IRAP file
             if crs_uuid is None:
                 log.warning(f'applying generic model CRS when loading polylines from IRAP file: {irap_file}')
             self._set_from_irap(irap_file)
 
         elif charisma_file is not None:
             if crs_uuid is None:
@@ -599,7 +601,31 @@
         lines = []
         for i, poly in enumerate(self.polys):
             for point in poly.coordinates:
                 lines.append(f"INLINE-\t0\t0\t{point[0]}\t{point[1]}\t{point[2]}\t{faultname}\t{i+1}\n")
         with open(file_name, 'w') as f:
             for item in lines:
                 f.write(item)
+
+    def extract_property_collection(self, refresh = False):
+        """Returns a property collection for the polyline set.
+
+        arguments:
+            refresh (bool, default False): if True, the property collection is refreshed
+                from the current state of the model; if False and the property collection
+                has already been cached for the polyline set, then the cached copy is used
+
+        returns:
+            a PropertyCollection holding those properties in the model where this polyline set
+            is the supporting representation
+
+        notes:
+            polyline set properties may have indexable element of 'nodes' or 'intervals';
+            for interval properties, the number of elements per polyline depends on whether the
+            polyline is closed or not;
+            it is currently left to calling code build the composite property array from data
+            for individual polylines, or to find the subset of the combined property data that
+            is applicable to an individual polyline
+        """
+        if self.property_collection is None or refresh:
+            self.property_collection = rqp.PropertyCollection(support = self)
+        return self.property_collection
```

### Comparing `resqpy-4.8.9/resqpy/model/_catalogue.py` & `resqpy-4.9.0/resqpy/model/_catalogue.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/model/_context.py` & `resqpy-4.9.0/resqpy/model/_context.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/model/_forestry.py` & `resqpy-4.9.0/resqpy/model/_forestry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/model/_grids.py` & `resqpy-4.9.0/resqpy/model/_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/model/_hdf5.py` & `resqpy-4.9.0/resqpy/model/_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/model/_model.py` & `resqpy-4.9.0/resqpy/model/_model.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/model/_xml.py` & `resqpy-4.9.0/resqpy/model/_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/multi_processing/__init__.py` & `resqpy-4.9.0/resqpy/multi_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/multi_processing/_multiprocessing.py` & `resqpy-4.9.0/resqpy/multi_processing/_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/multi_processing/wrappers/blocked_well_mp.py` & `resqpy-4.9.0/resqpy/multi_processing/wrappers/blocked_well_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/multi_processing/wrappers/grid_surface_mp.py` & `resqpy-4.9.0/resqpy/multi_processing/wrappers/grid_surface_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/multi_processing/wrappers/mesh_mp.py` & `resqpy-4.9.0/resqpy/multi_processing/wrappers/mesh_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/ab_toolbox.py` & `resqpy-4.9.0/resqpy/olio/ab_toolbox.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/base.py` & `resqpy-4.9.0/resqpy/olio/base.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/box_utilities.py` & `resqpy-4.9.0/resqpy/olio/box_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/class_dict.py` & `resqpy-4.9.0/resqpy/olio/class_dict.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/consolidation.py` & `resqpy-4.9.0/resqpy/olio/consolidation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/data/build.py` & `resqpy-4.9.0/resqpy/olio/data/build.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/data/properties.json` & `resqpy-4.9.0/resqpy/olio/data/properties.json`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/dataframe.py` & `resqpy-4.9.0/resqpy/olio/dataframe.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/factors.py` & `resqpy-4.9.0/resqpy/olio/factors.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/fine_coarse.py` & `resqpy-4.9.0/resqpy/olio/fine_coarse.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/grid_functions.py` & `resqpy-4.9.0/resqpy/olio/grid_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/intersection.py` & `resqpy-4.9.0/resqpy/olio/intersection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/keyword_files.py` & `resqpy-4.9.0/resqpy/olio/keyword_files.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/load_data.py` & `resqpy-4.9.0/resqpy/olio/load_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/point_inclusion.py` & `resqpy-4.9.0/resqpy/olio/point_inclusion.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/random_seed.py` & `resqpy-4.9.0/resqpy/olio/random_seed.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/read_nexus_fault.py` & `resqpy-4.9.0/resqpy/olio/read_nexus_fault.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/relperm.py` & `resqpy-4.9.0/resqpy/olio/relperm.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/simple_lines.py` & `resqpy-4.9.0/resqpy/olio/simple_lines.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/time.py` & `resqpy-4.9.0/resqpy/olio/time.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/trademark.py` & `resqpy-4.9.0/resqpy/olio/trademark.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/transmission.py` & `resqpy-4.9.0/resqpy/olio/transmission.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/triangulation.py` & `resqpy-4.9.0/resqpy/olio/triangulation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/uuid.py` & `resqpy-4.9.0/resqpy/olio/uuid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/vdb.py` & `resqpy-4.9.0/resqpy/olio/vdb.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/vector_utilities.py` & `resqpy-4.9.0/resqpy/olio/vector_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/volume.py` & `resqpy-4.9.0/resqpy/olio/volume.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/wellspec_keywords.py` & `resqpy-4.9.0/resqpy/olio/wellspec_keywords.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/write_data.py` & `resqpy-4.9.0/resqpy/olio/write_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/write_hdf5.py` & `resqpy-4.9.0/resqpy/olio/write_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/xml_et.py` & `resqpy-4.9.0/resqpy/olio/xml_et.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/xml_namespaces.py` & `resqpy-4.9.0/resqpy/olio/xml_namespaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/olio/zmap_reader.py` & `resqpy-4.9.0/resqpy/olio/zmap_reader.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/__init__.py` & `resqpy-4.9.0/resqpy/organize/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/_utils.py` & `resqpy-4.9.0/resqpy/organize/_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/boundary_feature.py` & `resqpy-4.9.0/resqpy/organize/boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/boundary_feature_interpretation.py` & `resqpy-4.9.0/resqpy/organize/boundary_feature_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/earth_model_interpretation.py` & `resqpy-4.9.0/resqpy/organize/earth_model_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/fault_interpretation.py` & `resqpy-4.9.0/resqpy/organize/fault_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/fluid_boundary_feature.py` & `resqpy-4.9.0/resqpy/organize/fluid_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/frontier_feature.py` & `resqpy-4.9.0/resqpy/organize/frontier_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/generic_interpretation.py` & `resqpy-4.9.0/resqpy/organize/generic_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/genetic_boundary_feature.py` & `resqpy-4.9.0/resqpy/organize/genetic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/geobody_boundary_interpretation.py` & `resqpy-4.9.0/resqpy/organize/geobody_boundary_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/geobody_feature.py` & `resqpy-4.9.0/resqpy/organize/geobody_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/geobody_interpretation.py` & `resqpy-4.9.0/resqpy/organize/geobody_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/geologic_unit_feature.py` & `resqpy-4.9.0/resqpy/organize/geologic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/horizon_interpretation.py` & `resqpy-4.9.0/resqpy/organize/horizon_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/organization_feature.py` & `resqpy-4.9.0/resqpy/organize/organization_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/rock_fluid_unit_feature.py` & `resqpy-4.9.0/resqpy/organize/rock_fluid_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/structural_organization_interpretation.py` & `resqpy-4.9.0/resqpy/organize/structural_organization_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/tectonic_boundary_feature.py` & `resqpy-4.9.0/resqpy/organize/tectonic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/wellbore_feature.py` & `resqpy-4.9.0/resqpy/organize/wellbore_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/organize/wellbore_interpretation.py` & `resqpy-4.9.0/resqpy/organize/wellbore_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/__init__.py` & `resqpy-4.9.0/resqpy/property/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/_collection_add_part.py` & `resqpy-4.9.0/resqpy/property/_collection_add_part.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import resqpy.property.property_common as rqp_c
 import resqpy.property._collection_get_attributes as pcga
 
 
 def _add_selected_part_from_other_dict(collection, part, other, realization, support_uuid, uuid, continuous,
                                        categorical, count, points, indexable, property_kind, facet_type, facet,
                                        citation_title, citation_title_match_mode, time_series_uuid, time_index,
-                                       string_lookup_uuid, related_uuid, const_value, ignore_clashes):
+                                       string_lookup_uuid, related_uuid, const_value, extra, ignore_clashes):
     if _check_not_none_and_not_equals(realization, other.realization_for_part, part):
         return
     if _check_not_none_and_not_uuid_match(support_uuid, other.support_uuid_for_part, part):
         return
     if _check_not_none_and_not_uuid_match(uuid, other.uuid_for_part, part):
         return
     if _check_not_none_and_not_equals(continuous, other.continuous_for_part, part):
@@ -51,14 +51,21 @@
         return
     if _check_not_none_and_not_equals(const_value, other.constant_value_for_part, part):
         return
     if related_uuid is not None:
         assert other.model is not None
         if other.model.part(parts_list = [part], related_uuid = related_uuid) is None:
             return
+    if extra is not None and len(extra):
+        em = other.extra_metadata_for_part(part)
+        if em is None or len(em) < len(extra):
+            return
+        for key, value in extra.items():
+            if em.get(key) != value:
+                return
     if part in collection.dict.keys():
         if ignore_clashes:
             return
         assert (False)
     collection.dict[part] = other.dict[part]
```

### Comparing `resqpy-4.8.9/resqpy/property/_collection_create_xml.py` & `resqpy-4.9.0/resqpy/property/_collection_create_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/_collection_get_attributes.py` & `resqpy-4.9.0/resqpy/property/_collection_get_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -399,14 +399,15 @@
         else:
             max_value = lower_scaling * (1.0 - fix_zero_at)
             n_prop[:] = np.where(n_prop > max_value, max_value, n_prop)
     return min_value, max_value, n_prop
 
 
 def _supporting_shape_grid(support, indexable_element, direction):
+    shape_list = None
     if indexable_element is None or indexable_element == 'cells':
         shape_list = [support.nk, support.nj, support.ni]
     elif indexable_element == 'columns':
         shape_list = [support.nj, support.ni]
     elif indexable_element == 'layers':
         shape_list = [support.nk]
     elif indexable_element == 'faces':
@@ -438,74 +439,112 @@
     axis = 'KJI'.index(direction.upper())
     shape_list = [support.nk, support.nj, support.ni]
     shape_list[axis] += 1  # note: properties for grid faces include outer faces
     return shape_list
 
 
 def _supporting_shape_grid_nodes(support):
+    shape_list = None
     assert not support.k_gaps, 'indexable element of nodes not currently supported for grids with K gaps'
     if support.has_split_coordinate_lines:
         pillar_count = (support.nj + 1) * (support.ni + 1) + support.split_pillars_count
         shape_list = [support.nk + 1, pillar_count]
     else:
         shape_list = [support.nk + 1, support.nj + 1, support.ni + 1]
     return shape_list
 
 
 def _supporting_shape_wellboreframe(support, indexable_element):
+    shape_list = None
     if indexable_element is None or indexable_element == 'nodes':
         shape_list = [support.node_count]
     elif indexable_element == 'intervals':
         shape_list = [support.node_count - 1]
     return shape_list
 
 
 def _supporting_shape_wellboremarkerframe(support, indexable_element):
+    shape_list = None
     if indexable_element is None or indexable_element == 'nodes':
         shape_list = [support.node_count]
     elif indexable_element == 'intervals':
         shape_list = [support.node_count - 1]
     return shape_list
 
 
 def _supporting_shape_blockedwell(support, indexable_element):
+    shape_list = None
     if indexable_element is None or indexable_element == 'intervals':
         shape_list = [support.node_count - 1]  # all intervals, including unblocked
     elif indexable_element == 'nodes':
         shape_list = [support.node_count]
     elif indexable_element == 'cells':
         shape_list = [support.cell_count]  # ie. blocked intervals only
     return shape_list
 
 
 def _supporting_shape_mesh(support, indexable_element):
+    shape_list = None
     if indexable_element is None or indexable_element == 'cells' or indexable_element == 'columns':
         shape_list = [support.nj - 1, support.ni - 1]
     elif indexable_element == 'nodes':
         shape_list = [support.nj, support.ni]
     return shape_list
 
 
 def _supporting_shape_surface(support, indexable_element):
-    if indexable_element is None or indexable_element == 'faces':
+    shape_list = None
+    if indexable_element is None or indexable_element in ['triangles', 'faces']:
         shape_list = [support.triangle_count()]
     elif indexable_element == 'nodes':
         shape_list = [support.node_count()]
     return shape_list
 
 
 def _supporting_shape_gridconnectionset(support, indexable_element):
+    shape_list = None
     if indexable_element is None or indexable_element == 'faces':
         shape_list = [support.count]
     return shape_list
 
 
+def _supporting_shape_polyline(support, indexable_element):
+    shape_list = None
+    if indexable_element is None or indexable_element == 'intervals':
+        shape_list = [len(support.coordinates) - (0 if support.isclosed else 1)]
+    elif indexable_element == 'nodes':
+        shape_list = [len(support.coordinates)]
+    return shape_list
+
+
+def _supporting_shape_polylineset(support, indexable_element):
+    shape_list = None
+    if indexable_element is None or indexable_element == 'intervals':
+        if support.boolnotconstant:
+            reduction = len(support.closed_array) - np.count_nonzero(support.closed_array)
+        else:
+            reduction = 0 if support.boolvalue else len(support.closed_array)
+        shape_list = [len(support.coordinates) - reduction]
+    elif indexable_element == 'nodes':
+        shape_list = [len(support.coordinates)]
+    return shape_list
+
+
+def _supporting_shape_pointset(support, indexable_element):
+    shape_list = None
+    if indexable_element is None or indexable_element == 'nodes':
+        shape_list = [len(support.full_array_ref())]
+    return shape_list
+
+
 def _supporting_shape_other(support, indexable_element):
     if indexable_element is None or indexable_element == 'cells':
         shape_list = [support.cell_count]
+    elif indexable_element == 'nodes':
+        shape_list = [support.node_count]
     elif indexable_element == 'faces per cell':
         support.cache_all_geometry_arrays()
         shape_list = [len(support.faces_per_cell)]
     return shape_list, support
 
 
 def _realizations_array_ref_get_r_extent(fill_missing, r_list):
@@ -513,24 +552,31 @@
         r_extent = r_list[-1] + 1
     else:
         r_extent = len(r_list)
     return r_extent
 
 
 def _get_indexable_element(indexable_element, support_type):
+    # returns a default indexable element depending on the type of supporting representation
     if indexable_element is None:
         if support_type in [
                 'obj_IjkGridRepresentation', 'obj_BlockedWellboreRepresentation', 'obj_Grid2dRepresentation',
                 'obj_UnstructuredGridRepresentation'
         ]:
             indexable_element = 'cells'
-        elif support_type in ['obj_WellboreFrameRepresentation', 'obj_WellboreMarkerFrameRepresentation']:
-            indexable_element = 'nodes'  # note: could be 'intervals'
-        elif support_type in ['obj_GridConnectionSetRepresentation', 'obj_TriangulatedSetRepresentation']:
+        elif support_type in [
+                'obj_WellboreFrameRepresentation', 'obj_WellboreMarkerFrameRepresentation', 'obj_PointSetRepresentation'
+        ]:
+            indexable_element = 'nodes'  # note: could be 'intervals' (except for PointSet properties)
+        elif support_type == 'obj_GridConnectionSetRepresentation':
             indexable_element = 'faces'
+        elif support_type == 'obj_TriangulatedSetRepresentation':
+            indexable_element = 'triangles'
+        elif support_type in ['obj_PolylineRepresentation', 'obj_PolylineSetRepresentation']:
+            indexable_element = 'intervals'  # could also be 'nodes'
         else:
             raise Exception('indexable element unknown for unsupported supporting representation object')
     return indexable_element
 
 
 def _cached_part_array_ref_get_array(collection, part, dtype, model, cached_array_name, use_pack):
     const_value = collection.constant_value_for_part(part)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `resqpy-4.8.9/resqpy/property/_collection_support.py` & `resqpy-4.9.0/resqpy/property/_collection_support.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,27 +30,28 @@
 def _set_support_uuid_notnone(collection, support, support_uuid, model, modify_parts):
     # when at global level was causing circular reference loading issues as grid imports this module
     import resqpy.fault as rqf
     import resqpy.grid as grr
     import resqpy.surface as rqs
     import resqpy.unstructured as rug
     import resqpy.well as rqw
+    import resqpy.lines as rql
 
     assert model is not None, 'model not established when setting support for property collection'
     if collection.support_uuid is not None and not bu.matching_uuids(support_uuid, collection.support_uuid):
         log.warning('changing supporting representation for property collection')
     collection.support_uuid = support_uuid
     collection.support = support
     if collection.support is None:
         _set_support_uuid_notnone_supportnone(collection, support_uuid, model)
     else:
         if type(collection.support) in [
                 grr.Grid, grr.RegularGrid, rqw.WellboreFrame, rqw.BlockedWell, rqs.Mesh, rqf.GridConnectionSet,
                 rug.UnstructuredGrid, rug.HexaGrid, rug.TetraGrid, rug.PrismGrid, rug.VerticalPrismGrid,
-                rug.PyramidGrid, rqw.WellboreMarkerFrame, rqs.Surface
+                rug.PyramidGrid, rqw.WellboreMarkerFrame, rqs.Surface, rql.Polyline, rql.PolylineSet, rqs.PointSet
         ]:
             collection.support_root = collection.support.root
         else:
             raise TypeError('unsupported property supporting representation class: ' + str(type(collection.support)))
     if modify_parts:
         for (part, info) in collection.dict.items():
             if info[1] is not None:
@@ -61,14 +62,15 @@
 
 def _set_support_uuid_notnone_supportnone(collection, support_uuid, model):
     import resqpy.fault as rqf
     import resqpy.grid as grr
     import resqpy.surface as rqs
     import resqpy.unstructured as rug
     import resqpy.well as rqw
+    import resqpy.lines as rql
 
     support_part = model.part_for_uuid(support_uuid)
     assert support_part is not None, 'supporting representation part missing in model'
     collection.support_root = model.root_for_part(support_part)
     support_type = model.type_of_part(support_part)
     assert support_type is not None
     if support_type == 'obj_IjkGridRepresentation':
@@ -86,14 +88,20 @@
     elif support_type == 'obj_UnstructuredGridRepresentation':
         collection.support = rug.UnstructuredGrid(model,
                                                   uuid = collection.support_uuid,
                                                   geometry_required = False,
                                                   find_properties = False)
     elif support_type == 'obj_WellboreMarkerFrameRepresentation':
         collection.support = rqw.WellboreMarkerFrame(model, uuid = collection.support_uuid)
+    elif support_type == 'obj_PolylineRepresentation':
+        collection.support = rql.Polyline(model, uuid = collection.support_uuid)
+    elif support_type == 'obj_PolylineSetRepresentation':
+        collection.support = rql.PolylineSet(model, uuid = collection.support_uuid)
+    elif support_type == 'obj_PointSetRepresentation':
+        collection.support = rqs.PointSet(model, uuid = collection.support_uuid)
     else:
         raise TypeError('unsupported property supporting representation class: ' + str(support_type))
 
 
 def _set_support_and_model_from_collection(collection, other, support_uuid, grid):
     _confirm_support_and_model_from_collection(collection, support_uuid, grid, other)
```

### Comparing `resqpy-4.8.9/resqpy/property/_property.py` & `resqpy-4.9.0/resqpy/property/_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/grid_property_collection.py` & `resqpy-4.9.0/resqpy/property/grid_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/property_collection.py` & `resqpy-4.9.0/resqpy/property/property_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
 
         # when at global level was causing circular reference loading issues as grid imports this module
         import resqpy.fault as rqf
         import resqpy.grid as grr
         import resqpy.surface as rqs
         import resqpy.unstructured as rug
         import resqpy.well as rqw
+        import resqpy.lines as rql
 
         support = self.support
 
         if isinstance(support, grr.Grid):
             shape_list = pcga._supporting_shape_grid(support, indexable_element, direction)
 
         elif isinstance(support, rqw.WellboreFrame):
@@ -180,22 +181,30 @@
 
         elif isinstance(support, rqf.GridConnectionSet):
             shape_list = pcga._supporting_shape_gridconnectionset(support, indexable_element)
 
         elif isinstance(support, rqs.Surface):
             shape_list = pcga._supporting_shape_surface(support, indexable_element)
 
-        elif type(support) in [
-                rug.UnstructuredGrid, rug.HexaGrid, rug.TetraGrid, rug.PrismGrid, rug.VerticalPrismGrid, rug.PyramidGrid
-        ]:
+        elif type(support) in  \
+            [rug.UnstructuredGrid, rug.HexaGrid, rug.TetraGrid, rug.PrismGrid, rug.VerticalPrismGrid, rug.PyramidGrid]:
             shape_list, support = pcga._supporting_shape_other(support, indexable_element)
 
         elif isinstance(support, rqw.WellboreMarkerFrame):
             shape_list = pcga._supporting_shape_wellboremarkerframe(support, indexable_element)
 
+        elif isinstance(support, rql.Polyline):
+            shape_list = pcga._supporting_shape_polyline(support, indexable_element)
+
+        elif isinstance(support, rql.PolylineSet):
+            shape_list = pcga._supporting_shape_polylineset(support, indexable_element)
+
+        elif isinstance(support, rqs.PointSet):
+            shape_list = pcga._supporting_shape_pointset(support, indexable_element)
+
         else:
             raise Exception(f'unsupported support class {type(support)} for property')
 
         return shape_list
 
     def populate_from_property_set(self, property_set_root):
         """Populates this (newly created) collection based on xml members of property set."""
@@ -443,14 +452,15 @@
             time_series_uuid = None,
             time_index = None,
             uom = None,
             string_lookup_uuid = None,
             categorical = None,
             related_uuid = None,
             const_value = None,
+            extra = None,
             ignore_clashes = False):
         """Adds those parts from the other PropertyCollection which match all arguments that are not None.
 
         arguments:
            other: another PropertyCollection object related to the same support as this collection
            citation_title_match_mode (str, optional): if present, one of 'is', 'starts', 'ends', 'contains', 'is not',
               'does not start', 'does not end', 'does not contain'; None is the same as 'is'
@@ -481,15 +491,15 @@
         if time_index is not None:
             assert time_index >= 0
 
         for (part, info) in other.dict.items():
             pcap._add_selected_part_from_other_dict(self, part, other, realization, support_uuid, uuid, continuous,
                                                     categorical, count, points, indexable, property_kind, facet_type,
                                                     facet, citation_title, citation_title_match_mode, time_series_uuid,
-                                                    time_index, string_lookup_uuid, related_uuid, const_value,
+                                                    time_index, string_lookup_uuid, related_uuid, const_value, extra,
                                                     ignore_clashes)
 
     def inherit_similar_parts_for_time_series_from_other_collection(self,
                                                                     other,
                                                                     example_part,
                                                                     citation_title_match_mode = None,
                                                                     ignore_clashes = False):
```

### Comparing `resqpy-4.8.9/resqpy/property/property_common.py` & `resqpy-4.9.0/resqpy/property/property_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,16 @@
                                     time_index = None,
                                     uom = None,
                                     string_lookup_uuid = None,
                                     categorical = None,
                                     title = None,
                                     title_mode = None,
                                     related_uuid = None,
-                                    const_value = None):
+                                    const_value = None,
+                                    extra = None):
     """Returns a new PropertyCollection with those parts which match all arguments that are not None.
 
     arguments:
        collection (PropertyCollection): an existing collection from which a subset will be returned as a new object
        realization (int, optional): realization number to filter on
        support_uuid (UUID or str, optional): UUID of supporting representation, to filter on
        uuid (UUID or str, optional): a property uuid to select a singleton property from the collection
@@ -545,14 +546,15 @@
        categorical (bool, optional): if True, only categorical properties are selected; if False they are excluded
        title (str, optional): synonymous with citation_title argument
        title_mode (str, optional): if present, one of 'is', 'starts', 'ends', 'contains', 'is not',
            'does not start', 'does not end', 'does not contain'; None is the same as 'is'; will default to 'is'
            if not specified and title or citation_title argument is present
        related_uuid (UUID or str, optional): only properties with direct relationship to this uuid are selected
        const_value (float or int, optional): only properties flagged as constant, with given value, are selected
+       extra (dict, optional): only properties where the extra metadata includes all the items of this dict are selected
 
     returns:
        a new PropertyCollection containing those properties which match the filter parameters that are not None
 
     notes:
        the existing collection might often be the 'main' collection holding all the properties
        for a supporting representation (eg. grid, blocked well or wellbore frame);
@@ -590,15 +592,16 @@
                                                          citation_title_match_mode = title_mode,
                                                          time_series_uuid = time_series_uuid,
                                                          time_index = time_index,
                                                          uom = uom,
                                                          string_lookup_uuid = string_lookup_uuid,
                                                          categorical = categorical,
                                                          related_uuid = related_uuid,
-                                                         const_value = const_value)
+                                                         const_value = const_value,
+                                                         extra = extra)
     return view
 
 
 def property_over_time_series_from_collection(collection, example_part):
     """Returns a new PropertyCollection with parts like the example part, over all indices in its time series.
 
     arguments:
```

### Comparing `resqpy-4.8.9/resqpy/property/property_kind.py` & `resqpy-4.9.0/resqpy/property/property_kind.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/string_lookup.py` & `resqpy-4.9.0/resqpy/property/string_lookup.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/well_interval_property.py` & `resqpy-4.9.0/resqpy/property/well_interval_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/well_interval_property_collection.py` & `resqpy-4.9.0/resqpy/property/well_interval_property_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,17 @@
         """Generator that yields component Interval log or Blocked well log objects."""
 
         return (rqp_wip.WellIntervalProperty(collection = self, part = part) for part in self.parts())
 
     def to_pandas(self, include_units = False):
         """Returns a dataframe with a column for each well log included in the collection."""
 
-        cell_indices = [rqp_c.return_cell_indices(i, self.support.cell_indices) for i in self.support.cell_grid_link]
+        cell_indices = [
+            rqp_c.return_cell_indices(i, self.support.cell_indices) for i in self.support.cell_grid_link if i != -1
+        ]
         data = {}
         for log in self.logs():
             col_name = log.name
             values = log.values()
             data[col_name] = values
         df = pd.DataFrame(data = data, index = cell_indices)
         return df
```

### Comparing `resqpy-4.8.9/resqpy/property/well_log.py` & `resqpy-4.9.0/resqpy/property/well_log.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/property/well_log_collection.py` & `resqpy-4.9.0/resqpy/property/well_log_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/rq_import/__init__.py` & `resqpy-4.9.0/resqpy/rq_import/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/rq_import/_add_ab_properties.py` & `resqpy-4.9.0/resqpy/rq_import/_add_ab_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/rq_import/_add_surfaces.py` & `resqpy-4.9.0/resqpy/rq_import/_add_surfaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/rq_import/_grid_from_cp.py` & `resqpy-4.9.0/resqpy/rq_import/_grid_from_cp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/rq_import/_import_nexus.py` & `resqpy-4.9.0/resqpy/rq_import/_import_nexus.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/rq_import/_import_vdb_all_grids.py` & `resqpy-4.9.0/resqpy/rq_import/_import_vdb_all_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/rq_import/_import_vdb_ensemble.py` & `resqpy-4.9.0/resqpy/rq_import/_import_vdb_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/strata/__init__.py` & `resqpy-4.9.0/resqpy/strata/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/strata/_binary_contact_interpretation.py` & `resqpy-4.9.0/resqpy/strata/_binary_contact_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/strata/_geologic_unit_interpretation.py` & `resqpy-4.9.0/resqpy/strata/_geologic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/strata/_strata_common.py` & `resqpy-4.9.0/resqpy/strata/_strata_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/strata/_stratigraphic_column.py` & `resqpy-4.9.0/resqpy/strata/_stratigraphic_column.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/strata/_stratigraphic_column_rank.py` & `resqpy-4.9.0/resqpy/strata/_stratigraphic_column_rank.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/strata/_stratigraphic_unit_feature.py` & `resqpy-4.9.0/resqpy/strata/_stratigraphic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/strata/_stratigraphic_unit_interpretation.py` & `resqpy-4.9.0/resqpy/strata/_stratigraphic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/surface/__init__.py` & `resqpy-4.9.0/resqpy/surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/surface/_base_surface.py` & `resqpy-4.9.0/resqpy/surface/_base_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/surface/_combined_surface.py` & `resqpy-4.9.0/resqpy/surface/_combined_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/surface/_mesh.py` & `resqpy-4.9.0/resqpy/surface/_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/surface/_pointset.py` & `resqpy-4.9.0/resqpy/surface/_pointset.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy as np
 
 import resqpy.crs as rcrs
 import resqpy.olio.uuid as bu
 import resqpy.olio.vector_utilities as vec
 import resqpy.olio.write_hdf5 as rwh5
 import resqpy.olio.xml_et as rqet
+import resqpy.property as rqp
 import resqpy.surface
 import resqpy.surface._base_surface as rqsb
 from resqpy.olio.xml_namespaces import curly_namespace as ns
 
 
 class PointSet(rqsb.BaseSurface):
     """Class for RESQML Point Set Representation within resqpy model object."""  # TODO: Work in Progress
@@ -74,14 +75,15 @@
 
         self.crs_uuid = crs_uuid
         self.patch_count = None
         self.patch_ref_list = []  # ordered list of (patch hdf5 ext uuid, path in hdf5, point count)
         self.patch_array_list = []  # ordered list of numpy float arrays (or None before loading), each of shape (N, 3)
         self.full_array = None  # composite points (all patches)
         self.represented_interpretation_root = None
+        self.property_collection = None
         super().__init__(model = parent_model,
                          uuid = uuid,
                          title = title,
                          originator = originator,
                          extra_metadata = extra_metadata)
 
         if self.root is not None:
@@ -247,16 +249,16 @@
             self.model.h5_array_element(h5_key_pair,
                                         cache_array = True,
                                         object = self,
                                         array_attribute = 'temp_points',
                                         dtype = 'float')
         except Exception:
             log.exception('hdf5 points failure for point set patch ' + str(patch_index))
-        assert self.temp_points.ndim == 2 and self.temp_points.shape[
-            1] == 3, 'unsupported dimensionality to points array'
+        assert self.temp_points.ndim == 2 and self.temp_points.shape[1] == 3,  \
+            'unsupported dimensionality to points array'
         self.patch_array_list[patch_index] = self.temp_points.copy()
         delattr(self, 'temp_points')
         return self.patch_array_list[patch_index]
 
     def load_all_patches(self):
         """Load hdf5 data for all patches and cache as separate numpy arrays; not usually called directly."""
 
@@ -392,20 +394,39 @@
         if points_array.shape[-1] == 2:
             shape = list(points_array.shape)
             shape[-1] = 3
             p = np.zeros(shape)
             p[..., :2] = points_array
             points_array = p
         self.patch_array_list.append(points_array.reshape(-1, 3).copy())
-        self.patch_ref_list.append((None, None, points_array.shape[0]))
+        self.patch_ref_list.append((None, None, points_array.size // 3))
         self.full_array = None
         if self.patch_count is None:
             self.patch_count = 0
         self.patch_count += 1
 
+    def extract_property_collection(self, refresh = False):
+        """Returns a property collection for the point set.
+
+        arguments:
+            refresh (bool, default False): if True, the property collection is refreshed
+                from the current state of the model; if False and the property collection
+                has already been cached for the point set, then the cached copy is used
+
+        returns:
+            a PropertyCollection holding those properties in the model where this point set
+            is the supporting representation
+
+        note:
+            point set properties have indexable element of 'nodes'
+        """
+        if self.property_collection is None or refresh:
+            self.property_collection = rqp.PropertyCollection(support = self)
+        return self.property_collection
+
     def write_hdf5(self, file_name = None, mode = 'a'):
         """Create or append to an hdf5 file, writing datasets for the point set patches after caching arrays.
 
         :meta common:
         """
 
         if not file_name:
```

### Comparing `resqpy-4.8.9/resqpy/surface/_surface.py` & `resqpy-4.9.0/resqpy/surface/_surface.py`

 * *Files 3% similar despite different names*

```diff
@@ -914,14 +914,54 @@
         s = abs_zero[ec[:, 0]] + abs_zero[ec[:, 1]]
         # TODO: ignore divide by zero
         ep = (p[ec[:, 0]] * abs_zero[ec[:, 1]] + p[ec[:, 1]] * abs_zero[ec[:, 0]]) / s
         # TODO: unignore, and use midpoint of those edges?
 
         return ep
 
+    def resampled_surface(self, title = None):
+        """Creates a new triangulated set which is a resampled version of the current triangulated set. Each existing triangle in the tset is divided equally into 4 new triangles.
+           
+        arguments:
+            title (str): a new title for the output triangulated set, if None the title will have the same title as the input triangulated set
+        
+        returns:
+            resqpy.surface.Surface object, with extra_metadata ('resampled from surface': <uuid>), where uuid is the origin surface uuid
+        """
+        rt, rp = self.triangles_and_points()
+        edge1 = np.mean(rp[rt[:]][:, ::2, :], axis = 1)
+        edge2 = np.mean(rp[rt[:]][:, 1:, :], axis = 1)
+        edge3 = np.mean(rp[rt[:]][:, :2, :], axis = 1)
+        allpoints = np.concatenate((rp, edge1, edge2, edge3), axis = 0)
+        count1 = len(rp)
+        count2 = count1 + len(edge1)
+        count3 = count2 + len(edge2)
+        tris = []
+        for i in range(len(rt)):
+            tris.extend([[rt[i][0], count1 + i, count3 + i], [rt[i][1], count2 + i, count3 + i],
+                         [rt[i][2], count1 + i, count2 + i], [count1 + i, count2 + i, count3 + i]])
+
+        # TODO: implement alternate solution using edge functions in olio triangulation to optimise
+        points_unique, inverse = np.unique(allpoints, axis = 0, return_inverse = True)
+        tris = np.array(tris)
+        tris_unique = np.empty(shape = tris.shape)
+        tris_unique[:, 0] = inverse[tris[:, 0]]
+        tris_unique[:, 1] = inverse[tris[:, 1]]
+        tris_unique[:, 2] = inverse[tris[:, 2]]
+
+        if title is None:
+            title = self.citation_title
+        resampled = rqs.Surface(self.model,
+                                title = title,
+                                crs_uuid = self.crs_uuid,
+                                extra_metadata = {'resampled from surface': str(self.uuid)})
+        resampled.set_from_triangles_and_points(tris_unique, points_unique)
+
+        return resampled
+
     def write_hdf5(self, file_name = None, mode = 'a'):
         """Create or append to an hdf5 file, writing datasets for the triangulated patches after caching arrays.
 
         :meta common:
         """
 
         if self.uuid is None:
```

### Comparing `resqpy-4.8.9/resqpy/surface/_tri_mesh.py` & `resqpy-4.9.0/resqpy/surface/_tri_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/surface/_triangulated_patch.py` & `resqpy-4.9.0/resqpy/surface/_triangulated_patch.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/time_series/__init__.py` & `resqpy-4.9.0/resqpy/time_series/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/time_series/_any_time_series.py` & `resqpy-4.9.0/resqpy/time_series/_any_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/time_series/_from_nexus_summary.py` & `resqpy-4.9.0/resqpy/time_series/_from_nexus_summary.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/time_series/_functions.py` & `resqpy-4.9.0/resqpy/time_series/_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/time_series/_geologic_time_series.py` & `resqpy-4.9.0/resqpy/time_series/_geologic_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/time_series/_time_duration.py` & `resqpy-4.9.0/resqpy/time_series/_time_duration.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/time_series/_time_series.py` & `resqpy-4.9.0/resqpy/time_series/_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/unstructured/__init__.py` & `resqpy-4.9.0/resqpy/unstructured/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/unstructured/_hexa_grid.py` & `resqpy-4.9.0/resqpy/unstructured/_hexa_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/unstructured/_prism_grid.py` & `resqpy-4.9.0/resqpy/unstructured/_prism_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/unstructured/_pyramid_grid.py` & `resqpy-4.9.0/resqpy/unstructured/_pyramid_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/unstructured/_tetra_grid.py` & `resqpy-4.9.0/resqpy/unstructured/_tetra_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/unstructured/_unstructured_grid.py` & `resqpy-4.9.0/resqpy/unstructured/_unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/weights_and_measures/__init__.py` & `resqpy-4.9.0/resqpy/weights_and_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/weights_and_measures/nexus_units.py` & `resqpy-4.9.0/resqpy/weights_and_measures/nexus_units.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/weights_and_measures/weights_and_measures.py` & `resqpy-4.9.0/resqpy/weights_and_measures/weights_and_measures.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/__init__.py` & `resqpy-4.9.0/resqpy/well/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/_blocked_well.py` & `resqpy-4.9.0/resqpy/well/_blocked_well.py`

 * *Files 0% similar despite different names*

```diff
@@ -3444,35 +3444,35 @@
                         sl_dict[gridpc.string_lookup_uuid_for_part(part)] = [part]
             else:
                 sl_dict = {None: cell_parts}
 
             sl_ts_dict = {}
             for sl_uuid in sl_dict.keys():
                 if len(gridpc.time_series_uuid_list()) > 0:
-                    # dictionary with keys for time_series uuids and None for static properties
-                    # values for each key are a list of property parts associated with that time_series_uuid, or None
+                    # dictionary with keys for string_lookup uuids and None where missing
+                    # values for each key are a list of property parts associated with that lookup uuid, or None
                     time_dict = {}
                     for part in sl_dict[sl_uuid]:
                         if gridpc.time_series_uuid_for_part(part) in time_dict.keys():
                             time_dict[gridpc.time_series_uuid_for_part(part)] =  \
                                 time_dict[gridpc.time_series_uuid_for_part(part)] + [part]
                         else:
                             time_dict[gridpc.time_series_uuid_for_part(part)] = [part]
                 else:
-                    time_dict = {None: cell_parts}
+                    time_dict = {None: sl_dict[sl_uuid]}
                 sl_ts_dict[sl_uuid] = time_dict
 
             for sl_uuid in sl_ts_dict.keys():
                 time_dict = sl_ts_dict[sl_uuid]
                 for time_uuid in time_dict.keys():
                     parts = time_dict[time_uuid]
                     for part in parts:
                         array = gridpc.cached_part_array_ref(part)
                         indices = self.cell_indices_for_grid_uuid(grid.uuid)
-                        bwarray = np.empty(shape = (indices.shape[0],))
+                        bwarray = np.empty(shape = (indices.shape[0],), dtype = array.dtype)
                         for i, ind in enumerate(indices):
                             bwarray[i] = array[tuple(ind)]
                         bwpc.add_cached_array_to_imported_list(
                             bwarray,
                             source_info = f'property from grid {grid.title}',
                             keyword = gridpc.citation_title_for_part(part),
                             discrete = (not gridpc.continuous_for_part(part)),
```

### Comparing `resqpy-4.8.9/resqpy/well/_deviation_survey.py` & `resqpy-4.9.0/resqpy/well/_deviation_survey.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/_md_datum.py` & `resqpy-4.9.0/resqpy/well/_md_datum.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/_trajectory.py` & `resqpy-4.9.0/resqpy/well/_trajectory.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/_wellbore_frame.py` & `resqpy-4.9.0/resqpy/well/_wellbore_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/_wellbore_marker.py` & `resqpy-4.9.0/resqpy/well/_wellbore_marker.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/_wellbore_marker_frame.py` & `resqpy-4.9.0/resqpy/well/_wellbore_marker_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/blocked_well_frame.py` & `resqpy-4.9.0/resqpy/well/blocked_well_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/well_object_funcs.py` & `resqpy-4.9.0/resqpy/well/well_object_funcs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/resqpy/well/well_utils.py` & `resqpy-4.9.0/resqpy/well/well_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.9/PKG-INFO` & `resqpy-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resqpy
-Version: 4.8.9
+Version: 4.9.0
 Summary: Python API for working with RESQML models
 Home-page: https://github.com/bp/resqpy
 License: MIT
 Keywords: RESQML
 Author: BP
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 5 - Production/Stable
```

