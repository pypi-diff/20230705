# Comparing `tmp/srai-0.1.4.tar.gz` & `tmp/srai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.1.4.tar", last modified: Thu Jun 22 17:29:50 2023, max compression
+gzip compressed data, was "srai-0.2.0.tar", last modified: Wed Jul  5 10:29:09 2023, max compression
```

## Comparing `srai-0.1.4.tar` & `srai-0.2.0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0    10760 2023-06-22 17:29:25.324639 srai-0.1.4/LICENSE.md
--rw-r--r--   0        0        0    16318 2023-06-22 17:29:25.324639 srai-0.1.4/README.md
--rw-r--r--   0        0        0     4602 2023-06-22 17:29:50.605131 srai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      404 2023-06-22 17:29:25.336639 srai-0.1.4/srai/__init__.py
--rw-r--r--   0        0        0      155 2023-06-22 17:29:25.336639 srai-0.1.4/srai/constants.py
--rw-r--r--   0        0        0      755 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/__init__.py
--rw-r--r--   0        0        0     2722 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/_base.py
--rw-r--r--   0        0        0     8327 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/contextual_count_embedder.py
--rw-r--r--   0        0        0     4840 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/count_embedder.py
--rw-r--r--   0        0        0      136 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/gtfs2vec/__init__.py
--rw-r--r--   0        0        0     9413 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/gtfs2vec/embedder.py
--rw-r--r--   0        0        0     2369 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/gtfs2vec/model.py
--rw-r--r--   0        0        0      247 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/hex2vec/__init__.py
--rw-r--r--   0        0        0     8553 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/hex2vec/embedder.py
--rw-r--r--   0        0        0     6932 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/hex2vec/model.py
--rw-r--r--   0        0        0     6319 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/hex2vec/neighbour_dataset.py
--rw-r--r--   0        0        0      153 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/highway2vec/__init__.py
--rw-r--r--   0        0        0     6148 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/highway2vec/embedder.py
--rw-r--r--   0        0        0     2908 2023-06-22 17:29:25.336639 srai-0.1.4/srai/embedders/highway2vec/model.py
--rw-r--r--   0        0        0      580 2023-06-22 17:29:25.336639 srai-0.1.4/srai/exceptions.py
--rw-r--r--   0        0        0      531 2023-06-22 17:29:25.336639 srai-0.1.4/srai/joiners/__init__.py
--rw-r--r--   0        0        0      731 2023-06-22 17:29:25.336639 srai-0.1.4/srai/joiners/_base.py
--rw-r--r--   0        0        0     3836 2023-06-22 17:29:25.336639 srai-0.1.4/srai/joiners/intersection_joiner.py
--rw-r--r--   0        0        0      725 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/__init__.py
--rw-r--r--   0        0        0      591 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/_base.py
--rw-r--r--   0        0        0     2195 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/geoparquet_loader.py
--rw-r--r--   0        0        0     5371 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/gtfs_loader.py
--rw-r--r--   0        0        0      257 2023-06-22 17:29:25.336639 srai-0.1.4/srai/loaders/osm_loaders/__init__.py
--rw-r--r--   0        0        0     6424 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/_base.py
--rw-r--r--   0        0        0      469 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/__init__.py
--rw-r--r--   0        0        0     2011 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/_typing.py
--rw-r--r--   0        0        0     5324 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/base_osm_groups.py
--rw-r--r--   0        0        0     8849 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/geofabrik.py
--rw-r--r--   0        0        0    15758 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/hex2vec.py
--rw-r--r--   0        0        0     2438 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/filters/popular.py
--rw-r--r--   0        0        0     5536 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/osm_online_loader.py
--rw-r--r--   0        0        0     5772 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/osm_pbf_loader.py
--rw-r--r--   0        0        0     2777 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/osm_tile_data_collector.py
--rw-r--r--   0        0        0     4703 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/osm_tile_loader.py
--rw-r--r--   0        0        0    10106 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/pbf_file_downloader.py
--rw-r--r--   0        0        0    11124 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_loaders/pbf_file_handler.py
--rw-r--r--   0        0        0      118 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_way_loader/__init__.py
--rw-r--r--   0        0        0     7587 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_way_loader/constants.py
--rw-r--r--   0        0        0    13854 2023-06-22 17:29:25.340639 srai-0.1.4/srai/loaders/osm_way_loader/osm_way_loader.py
--rw-r--r--   0        0        0      467 2023-06-22 17:29:25.340639 srai-0.1.4/srai/neighbourhoods/__init__.py
--rw-r--r--   0        0        0     3679 2023-06-22 17:29:25.340639 srai-0.1.4/srai/neighbourhoods/_base.py
--rw-r--r--   0        0        0     2887 2023-06-22 17:29:25.340639 srai-0.1.4/srai/neighbourhoods/adjacency_neighbourhood.py
--rw-r--r--   0        0        0     3221 2023-06-22 17:29:25.340639 srai-0.1.4/srai/neighbourhoods/h3_neighbourhood.py
--rw-r--r--   0        0        0      496 2023-06-22 17:29:25.340639 srai-0.1.4/srai/plotting/__init__.py
--rw-r--r--   0        0        0    11189 2023-06-22 17:29:25.340639 srai-0.1.4/srai/plotting/folium_wrapper.py
--rw-r--r--   0        0        0    14174 2023-06-22 17:29:25.340639 srai-0.1.4/srai/plotting/plotly_wrapper.py
--rw-r--r--   0        0        0      934 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/__init__.py
--rw-r--r--   0        0        0      957 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/_base.py
--rw-r--r--   0        0        0    11462 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/_spherical_voronoi.py
--rw-r--r--   0        0        0    15475 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     6651 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/h3_regionalizer.py
--rw-r--r--   0        0        0     3142 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/s2_regionalizer.py
--rw-r--r--   0        0        0     4163 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/slippy_map_regionalizer.py
--rw-r--r--   0        0        0     5940 2023-06-22 17:29:25.340639 srai-0.1.4/srai/regionalizers/voronoi_regionalizer.py
--rw-r--r--   0        0        0      654 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/__init__.py
--rw-r--r--   0        0        0     2910 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/_optional.py
--rw-r--r--   0        0        0      239 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/_pytorch_stubs.py
--rw-r--r--   0        0        0      999 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/download.py
--rw-r--r--   0        0        0      944 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/geocode.py
--rw-r--r--   0        0        0     2521 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/geometry.py
--rw-r--r--   0        0        0     1153 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/merge.py
--rw-r--r--   0        0        0      717 2023-06-22 17:29:25.340639 srai-0.1.4/srai/utils/typing.py
--rw-r--r--   0        0        0       29 2023-06-22 17:29:25.340639 srai-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     7806 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/conftest.py
--rw-r--r--   0        0        0      534 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/constants.py
--rw-r--r--   0        0        0     2600 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/generation.py
--rw-r--r--   0        0        0     2716 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_embedder.py
--rw-r--r--   0        0        0    97383 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_features.parquet
--rw-r--r--   0        0        0   111218 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
--rw-r--r--   0        0        0    14226 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
--rw-r--r--   0        0        0    14498 2023-06-22 17:29:25.340639 srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_result.parquet
--rw-r--r--   0        0        0    89227 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0    86944 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0    16794 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    15781 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     1061 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_model.py
--rw-r--r--   0        0        0     3037 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/hex2vec/test_neighbour_dataset.py
--rw-r--r--   0        0        0    24053 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/test_contextual_count_embedder.py
--rw-r--r--   0        0        0     8273 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/test_count_embedder.py
--rw-r--r--   0        0        0     7091 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/test_gtfs2vec_embedder.py
--rw-r--r--   0        0        0     3630 2023-06-22 17:29:25.344639 srai-0.1.4/tests/embedders/test_highway2vec_embedder.py
--rw-r--r--   0        0        0     1765 2023-06-22 17:29:25.344639 srai-0.1.4/tests/joiners/conftest.py
--rw-r--r--   0        0        0     2529 2023-06-22 17:29:25.344639 srai-0.1.4/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0        0        0     3001 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/conftest.py
--rw-r--r--   0        0        0     4284 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/conftest.py
--rw-r--r--   0        0        0     4824 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/filters/popular_filter_example.json
--rw-r--r--   0        0        0     3413 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
--rw-r--r--   0        0        0     3276 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
--rw-r--r--   0        0        0      342 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   111539 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/poland.geojson
--rw-r--r--   0        0        0   252620 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
--rw-r--r--   0        0        0     2811 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_osm_online_loader.py
--rw-r--r--   0        0        0     8690 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_osm_pbf_loader.py
--rw-r--r--   0        0        0     3156 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
--rw-r--r--   0        0        0     3165 2023-06-22 17:29:25.344639 srai-0.1.4/tests/loaders/osm_loaders/test_osm_tile_loader.py
--rw-r--r--   0        0        0     3353 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl
--rw-r--r--   0        0        0     2804 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl
--rw-r--r--   0        0        0     3822 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl
--rw-r--r--   0        0        0     5109 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl
--rw-r--r--   0        0        0     3822 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl
--rw-r--r--   0        0        0      629 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl
--rw-r--r--   0        0        0    10789 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/osm_way_loader/test_osm_way_loader.py
--rw-r--r--   0        0        0    27801 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/test_files/example.parquet
--rw-r--r--   0        0        0     2181 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0        0        0     3176 2023-06-22 17:29:25.348639 srai-0.1.4/tests/loaders/test_gtfs_loader.py
--rw-r--r--   0        0        0     4755 2023-06-22 17:29:25.348639 srai-0.1.4/tests/miscellaneous/test_optional_dependencies.py
--rw-r--r--   0        0        0     4028 2023-06-22 17:29:25.348639 srai-0.1.4/tests/neighbourhoods/h3/test_no_regions.py
--rw-r--r--   0        0        0     5668 2023-06-22 17:29:25.348639 srai-0.1.4/tests/neighbourhoods/h3/test_with_regions.py
--rw-r--r--   0        0        0     8063 2023-06-22 17:29:25.348639 srai-0.1.4/tests/neighbourhoods/test_adjacency_neighbourhood.py
--rw-r--r--   0        0        0     5586 2023-06-22 17:29:25.348639 srai-0.1.4/tests/neighbourhoods/test_neighbourhood.py
--rw-r--r--   0        0        0     3667 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/conftest.py
--rw-r--r--   0        0        0     6505 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2208 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_h3_regionalizer.py
--rw-r--r--   0        0        0     1841 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_s2_regionalizer.py
--rw-r--r--   0        0        0     2689 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_slippy_map_regionalizer.py
--rw-r--r--   0        0        0     4983 2023-06-22 17:29:25.348639 srai-0.1.4/tests/regionalizers/test_voronoi_regionalizer.py
--rw-r--r--   0        0        0    18478 1970-01-01 00:00:00.000000 srai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10760 2023-07-05 10:28:47.765951 srai-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0    16727 2023-07-05 10:28:47.765951 srai-0.2.0/README.md
+-rw-r--r--   0        0        0     4627 2023-07-05 10:29:09.566147 srai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-07-05 10:28:47.777951 srai-0.2.0/srai/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-05 10:28:47.777951 srai-0.2.0/srai/constants.py
+-rw-r--r--   0        0        0      798 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     4848 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/_base.py
+-rw-r--r--   0        0        0     8327 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     4857 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      136 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0    11278 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2283 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0    10683 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6822 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6319 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     7935 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2860 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2023-07-05 10:28:47.781951 srai-0.2.0/srai/exceptions.py
+-rw-r--r--   0        0        0      531 2023-07-05 10:28:47.781951 srai-0.2.0/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2023-07-05 10:28:47.781951 srai-0.2.0/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2023-07-05 10:28:47.781951 srai-0.2.0/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      725 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/_base.py
+-rw-r--r--   0        0        0     2195 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5371 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     6424 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      469 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     2011 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5324 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0     8849 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15758 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2438 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5536 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     5772 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2777 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     4703 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0    10106 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/pbf_file_downloader.py
+-rw-r--r--   0        0        0    11124 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/pbf_file_handler.py
+-rw-r--r--   0        0        0      118 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7587 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    13854 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      467 2023-07-05 10:28:47.781951 srai-0.2.0/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     3679 2023-07-05 10:28:47.781951 srai-0.2.0/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     2887 2023-07-05 10:28:47.781951 srai-0.2.0/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     3221 2023-07-05 10:28:47.781951 srai-0.2.0/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      496 2023-07-05 10:28:47.781951 srai-0.2.0/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11189 2023-07-05 10:28:47.781951 srai-0.2.0/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14174 2023-07-05 10:28:47.781951 srai-0.2.0/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0      934 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/__init__.py
+-rw-r--r--   0        0        0      957 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/_base.py
+-rw-r--r--   0        0        0    11462 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15475 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     6651 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/h3_regionalizer.py
+-rw-r--r--   0        0        0     3142 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/s2_regionalizer.py
+-rw-r--r--   0        0        0     4163 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     5940 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/voronoi_regionalizer.py
+-rw-r--r--   0        0        0      654 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/__init__.py
+-rw-r--r--   0        0        0     2910 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/_optional.py
+-rw-r--r--   0        0        0      239 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/_pytorch_stubs.py
+-rw-r--r--   0        0        0      999 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/download.py
+-rw-r--r--   0        0        0      944 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/geocode.py
+-rw-r--r--   0        0        0     2521 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/geometry.py
+-rw-r--r--   0        0        0     1153 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/merge.py
+-rw-r--r--   0        0        0      717 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/typing.py
+-rw-r--r--   0        0        0       29 2023-07-05 10:28:47.781951 srai-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/conftest.py
+-rw-r--r--   0        0        0      534 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2600 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     2716 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1061 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3037 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    24053 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0     8273 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3630 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     1765 2023-07-05 10:28:47.785951 srai-0.2.0/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2529 2023-07-05 10:28:47.785951 srai-0.2.0/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     3001 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4284 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     3413 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3276 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   111539 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     2811 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     8690 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3156 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3165 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3353 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl
+-rw-r--r--   0        0        0     2804 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl
+-rw-r--r--   0        0        0     3822 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl
+-rw-r--r--   0        0        0     5109 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl
+-rw-r--r--   0        0        0     3822 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl
+-rw-r--r--   0        0        0      629 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl
+-rw-r--r--   0        0        0    10789 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2181 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3176 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4755 2023-07-05 10:28:47.789951 srai-0.2.0/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     4028 2023-07-05 10:28:47.789951 srai-0.2.0/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     5668 2023-07-05 10:28:47.789951 srai-0.2.0/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0     8063 2023-07-05 10:28:47.789951 srai-0.2.0/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     5586 2023-07-05 10:28:47.789951 srai-0.2.0/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0     3667 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/conftest.py
+-rw-r--r--   0        0        0     6505 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2208 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_h3_regionalizer.py
+-rw-r--r--   0        0        0     1841 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_s2_regionalizer.py
+-rw-r--r--   0        0        0     2689 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     4983 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_voronoi_regionalizer.py
+-rw-r--r--   0        0        0    18930 1970-01-01 00:00:00.000000 srai-0.2.0/PKG-INFO
```

### Comparing `srai-0.1.4/LICENSE.md` & `srai-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/README.md` & `srai-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -268,14 +268,25 @@
 plot_numeric_data(regions, embeddings, 0, map=folium_map)
 ```
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/embedding_hex2vec_embedder.jpg" style="max-width:600px;width:100%"/>
 </p>
 
+### Pre-trained models usage
+
+We provide pre-trained models for some of the embedding methods. To use them, simply download them from [here](https://drive.google.com/drive/folders/14sH33-kNxA0q1O1abPWTpuix8raR_XbD?usp=drive_link) and load them using `load` method:
+
+```python
+from srai.embedders import Hex2VecEmbedder
+
+model_path = "path/to/model"
+embedder = Hex2VecEmbedder.load(model_path)
+```
+
 ### Plotting, utilities and more
 
 We also provide utilities for different spatial operations and plotting functions adopted to data formats used in `srai` For a full list of available methods, please refer to the [documentation](https://srai-lab.github.io/srai).
 
 ## Contributing
 
 If you are willing to contribute to `srai`, feel free to do so! Visit [our contributing guide](./CONTRIBUTING.md) for more details.
```

#### html2text {}

```diff
@@ -144,47 +144,52 @@
 (regions, features, joint) # Option 2: fit_transform embeddings =
 embedder.fit_transform(regions, features, joint, neighbourhood, batch_size=128)
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
 tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings, 0,
 map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                         embedding_hex2vec_embedder.jpg]
-### Plotting, utilities and more We also provide utilities for different
-spatial operations and plotting functions adopted to data formats used in
-`srai` For a full list of available methods, please refer to the
-[documentation](https://srai-lab.github.io/srai). ## Contributing If you are
-willing to contribute to `srai`, feel free to do so! Visit [our contributing
-guide](./CONTRIBUTING.md) for more details. ## Publications Some of the methods
-implemented in `srai` have been published in scientific journals and
-conferences. 1. Szymon WoÅºniak and Piotr SzymaÅski. 2021. Hex2vec: Context-
-Aware Embedding H3 Hexagons with OpenStreetMap Tags. In Proceedings of the 4th
-ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge Discovery
-(GEOAI '21). Association for Computing Machinery, New York, NY, USA, 61â71.
-[paper](https://doi.org/10.1145/3486635.3491076), [arXiv](https://arxiv.org/
-abs/2111.00970) 2. Piotr Gramacki, Szymon WoÅºniak, and Piotr SzymaÅski. 2021.
-Gtfs2vec: Learning GTFS Embeddings for comparing Public Transport Offer in
-Microregions. In Proceedings of the 1st ACM SIGSPATIAL International Workshop
-on Searching and Mining Large Collections of Geospatial Data (GeoSearch'21).
-Association for Computing Machinery, New York, NY, USA, 5â12. [paper](https:/
-/doi.org/10.1145/3486640.3491392), [arXiv](https://arxiv.org/abs/2111.00960) 3.
-Kamil Raczycki and Piotr SzymaÅski. 2021. Transfer learning approach to
-bicycle-sharing systems' station location planning using OpenStreetMap data. In
-Proceedings of the 4th ACM SIGSPATIAL International Workshop on Advances in
-Resilient and Intelligent Cities (ARIC '21). Association for Computing
-Machinery, New York, NY, USA, 1â12. [paper](https://doi.org/10.1145/
-3486626.3493434), [arXiv](https://arxiv.org/abs/2111.00990) 4. Kacper LeÅniara
-and Piotr SzymaÅski. 2022. Highway2vec: representing OpenStreetMap
-microregions with respect to their road network characteristics. In Proceedings
-of the 5th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge
-Discovery (GeoAI '22). Association for Computing Machinery, New York, NY, USA,
-18â29. [paper](https://doi.org/10.1145/3557918.3565865), [arXiv](https://
-arxiv.org/abs/2304.13865) ## Acknowledgements We would like to thank Piotr
-SzymaÅski PhD \([@niedakh](https://twitter.com/niedakh)\) for his invaluable
-guidance and support in the development of this library. His expertise and
-mentorship have been instrumental in shaping the library's design and
-functionality, and we are very grateful for his input. ## Citation TBD ##
-License This library is licensed under the [Apache License 2.0](https://
-github.com/srai-lab/srai/blob/main/LICENSE.md). The free [OpenStreetMap](https:
-//www.openstreetmap.org/) data, which is used for the development of SRAI, is
-licensed under the [Open Data Commons Open Database License](https://
-opendatacommons.org/licenses/odbl/) (ODbL) by the [OpenStreetMap Foundation]
-(https://osmfoundation.org/) (OSMF).
+### Pre-trained models usage We provide pre-trained models for some of the
+embedding methods. To use them, simply download them from [here](https://
+drive.google.com/drive/folders/14sH33-
+kNxA0q1O1abPWTpuix8raR_XbD?usp=drive_link) and load them using `load` method:
+```python from srai.embedders import Hex2VecEmbedder model_path = "path/to/
+model" embedder = Hex2VecEmbedder.load(model_path) ``` ### Plotting, utilities
+and more We also provide utilities for different spatial operations and
+plotting functions adopted to data formats used in `srai` For a full list of
+available methods, please refer to the [documentation](https://srai-
+lab.github.io/srai). ## Contributing If you are willing to contribute to
+`srai`, feel free to do so! Visit [our contributing guide](./CONTRIBUTING.md)
+for more details. ## Publications Some of the methods implemented in `srai`
+have been published in scientific journals and conferences. 1. Szymon WoÅºniak
+and Piotr SzymaÅski. 2021. Hex2vec: Context-Aware Embedding H3 Hexagons with
+OpenStreetMap Tags. In Proceedings of the 4th ACM SIGSPATIAL International
+Workshop on AI for Geographic Knowledge Discovery (GEOAI '21). Association for
+Computing Machinery, New York, NY, USA, 61â71. [paper](https://doi.org/
+10.1145/3486635.3491076), [arXiv](https://arxiv.org/abs/2111.00970) 2. Piotr
+Gramacki, Szymon WoÅºniak, and Piotr SzymaÅski. 2021. Gtfs2vec: Learning GTFS
+Embeddings for comparing Public Transport Offer in Microregions. In Proceedings
+of the 1st ACM SIGSPATIAL International Workshop on Searching and Mining Large
+Collections of Geospatial Data (GeoSearch'21). Association for Computing
+Machinery, New York, NY, USA, 5â12. [paper](https://doi.org/10.1145/
+3486640.3491392), [arXiv](https://arxiv.org/abs/2111.00960) 3. Kamil Raczycki
+and Piotr SzymaÅski. 2021. Transfer learning approach to bicycle-sharing
+systems' station location planning using OpenStreetMap data. In Proceedings of
+the 4th ACM SIGSPATIAL International Workshop on Advances in Resilient and
+Intelligent Cities (ARIC '21). Association for Computing Machinery, New York,
+NY, USA, 1â12. [paper](https://doi.org/10.1145/3486626.3493434), [arXiv]
+(https://arxiv.org/abs/2111.00990) 4. Kacper LeÅniara and Piotr SzymaÅski.
+2022. Highway2vec: representing OpenStreetMap microregions with respect to
+their road network characteristics. In Proceedings of the 5th ACM SIGSPATIAL
+International Workshop on AI for Geographic Knowledge Discovery (GeoAI '22).
+Association for Computing Machinery, New York, NY, USA, 18â29. [paper](https:
+//doi.org/10.1145/3557918.3565865), [arXiv](https://arxiv.org/abs/2304.13865)
+## Acknowledgements We would like to thank Piotr SzymaÅski PhD \([@niedakh]
+(https://twitter.com/niedakh)\) for his invaluable guidance and support in the
+development of this library. His expertise and mentorship have been
+instrumental in shaping the library's design and functionality, and we are very
+grateful for his input. ## Citation TBD ## License This library is licensed
+under the [Apache License 2.0](https://github.com/srai-lab/srai/blob/main/
+LICENSE.md). The free [OpenStreetMap](https://www.openstreetmap.org/) data,
+which is used for the development of SRAI, is licensed under the [Open Data
+Commons Open Database License](https://opendatacommons.org/licenses/odbl/)
+(ODbL) by the [OpenStreetMap Foundation](https://osmfoundation.org/) (OSMF).
```

### Comparing `srai-0.1.4/pyproject.toml` & `srai-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "srai"
-version = "0.1.4"
+version = "0.2.0"
 description = "A set of python modules for geospatial machine learning and data mining"
 authors = [
     { name = "SRAI Lab", email = "spatialrepresentationsforai@gmail.com" },
     { name = "Piotr Gramacki" },
     { name = "Kacper Leśniara" },
     { name = "Kamil Raczycki" },
     { name = "Szymon Woźniak" },
@@ -53,29 +53,30 @@
 Repository = "https://github.com/srai-lab/srai"
 Documentation = "https://srai-lab.github.io/srai"
 Changelog = "https://github.com/srai-lab/srai/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 osm = [
     "osmium",
-    "osmnx",
+    "osmnx<=1.4.0",
     "overpass",
     "pillow",
 ]
 voronoi = [
     "pymap3d",
     "haversine",
     "spherical-geometry",
 ]
 gtfs = [
     "gtfs-kit",
 ]
 plotting = [
     "folium",
     "mapclassify",
+    "matplotlib",
     "plotly",
     "kaleido<=0.2.1",
 ]
 torch = [
     "pytorch-lightning",
     "torch",
 ]
@@ -195,15 +196,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.1.4"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore: bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `srai-0.1.4/srai/embedders/__init__.py` & `srai-0.2.0/srai/embedders/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 This module contains embedders, used to convert spatial data to their vector representations.
 
 Embedders are designed to unify different types of spatial data embedding methods, such as hex2vec
 or gtfs2vec into a single interface. This allows to easily switch between different embedding
 methods without changing the rest of the code.
 """
 
-from ._base import Embedder
+
+from ._base import Embedder, Model, ModelT
 from .contextual_count_embedder import ContextualCountEmbedder
 from .count_embedder import CountEmbedder
 from .gtfs2vec import GTFS2VecEmbedder
 from .hex2vec import Hex2VecEmbedder
 from .highway2vec import Highway2VecEmbedder
 
 __all__ = [
     "Embedder",
     "CountEmbedder",
     "ContextualCountEmbedder",
     "GTFS2VecEmbedder",
     "Hex2VecEmbedder",
     "Highway2VecEmbedder",
+    "Model",
+    "ModelT",
 ]
```

### Comparing `srai-0.1.4/srai/embedders/contextual_count_embedder.py` & `srai-0.2.0/srai/embedders/contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/embedders/count_embedder.py` & `srai-0.2.0/srai/embedders/count_embedder.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,18 +25,17 @@
                 to be found in the resulting embedding. If not None, the missing features are added
                 and filled with 0. The unexpected features are removed.
                 The resulting columns are sorted accordingly. Defaults to None.
             count_subcategories (bool, optional): Whether to count all subcategories individually
                 or count features only on the highest level based on features column name.
                 Defaults to True.
         """
-        if expected_output_features is not None:
-            self.expected_output_features = pd.Series(expected_output_features)
-        else:
-            self.expected_output_features = None
+        self.expected_output_features: Optional[pd.Series] = (
+            None if expected_output_features is None else pd.Series(expected_output_features)
+        )
 
         self.count_subcategories = count_subcategories
 
     def transform(
         self,
         regions_gdf: gpd.GeoDataFrame,
         features_gdf: gpd.GeoDataFrame,
@@ -85,30 +84,32 @@
         if self.count_subcategories:
             feature_encodings = pd.get_dummies(features_df)
         else:
             feature_encodings = features_df.notna().astype(int)
         joint_with_encodings = joint_df.join(feature_encodings)
         region_embeddings = joint_with_encodings.groupby(level=0).sum()
 
-        if self.expected_output_features is not None:
-            region_embeddings = self._filter_to_expected_features(region_embeddings)
+        region_embeddings = self._maybe_filter_to_expected_features(region_embeddings)
         region_embedding_df = regions_df.join(region_embeddings, how="left").fillna(0).astype(int)
 
         return region_embedding_df
 
-    def _filter_to_expected_features(self, region_embeddings: pd.DataFrame) -> pd.DataFrame:
+    def _maybe_filter_to_expected_features(self, region_embeddings: pd.DataFrame) -> pd.DataFrame:
         """
         Add missing and remove excessive columns from embeddings.
 
         Args:
             region_embeddings (pd.DataFrame): Counted frequencies of each feature value.
 
         Returns:
             pd.DataFrame: Embeddings with expected columns only.
         """
+        if self.expected_output_features is None:
+            return region_embeddings
+
         missing_features = self.expected_output_features[
             ~self.expected_output_features.isin(region_embeddings.columns)
         ]
         missing_features_df = pd.DataFrame(
             0, index=region_embeddings.index, columns=missing_features
         )
         region_embeddings = pd.concat([region_embeddings, missing_features_df], axis=1)
```

### Comparing `srai-0.1.4/srai/embedders/gtfs2vec/embedder.py` & `srai-0.2.0/srai/embedders/gtfs2vec/embedder.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 This module contains embedder from gtfs2vec paper [1].
 
 References:
     1. https://doi.org/10.1145/3486640.3491392
 """
 
 
+import json
 from functools import reduce
-from typing import Any, Dict, List, Optional
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Type, Union
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 
-from srai.embedders import Embedder
+from srai.embedders import Embedder, ModelT
 from srai.embedders.gtfs2vec.model import GTFS2VecModel
 from srai.exceptions import ModelNotFitException
 from srai.loaders.gtfs_loader import GTFS2VEC_DIRECTIONS_PREFIX, GTFS2VEC_TRIPS_PREFIX
 from srai.utils._optional import import_optional_dependencies
 
 
 class GTFS2VecEmbedder(Embedder):
@@ -40,14 +42,15 @@
         import_optional_dependencies(
             dependency_group="torch", modules=["torch", "pytorch_lightning"]
         )
         self._model: Optional[GTFS2VecModel] = None
         self._hidden_size = hidden_size
         self._embedding_size = embedding_size
         self._skip_autoencoder = skip_autoencoder
+        self._is_fitted = False
 
     def transform(
         self,
         regions_gdf: gpd.GeoDataFrame,
         features_gdf: gpd.GeoDataFrame,
         joint_gdf: gpd.GeoDataFrame,
     ) -> pd.DataFrame:
@@ -267,7 +270,65 @@
 
         embeddings = model(torch.Tensor(features.to_numpy().astype(np.float32))).detach().numpy()
 
         return pd.DataFrame(
             data=embeddings,
             index=features.index,
         )
+
+    def _save(self, path: Union[Path, str], embedder_config: Dict[str, Any]) -> None:
+        if isinstance(path, str):
+            path = Path(path)
+
+        model = self._maybe_get_model()
+
+        path.mkdir(parents=True, exist_ok=True)
+
+        model.save(path / "model.pt")
+
+        config = {
+            "model_config": model.get_config(),
+            "embedder_config": embedder_config,
+        }
+        with open(path / "config.json", "w") as f:
+            json.dump(config, f, ensure_ascii=False, indent=4)
+
+    def save(self, path: Union[Path, str]) -> None:
+        """
+        Save the model to a directory.
+
+        Args:
+            path (Path): Path to the directory.
+        """
+        embedder_config = {
+            "hidden_size": self._hidden_size,
+            "embedding_size": self._embedding_size,
+            "skip_autoencoder": self._skip_autoencoder,
+        }
+        self._save(path, embedder_config)
+
+    @classmethod
+    def _load(cls, path: Union[Path, str], model_module: Type[ModelT]) -> "GTFS2VecEmbedder":
+        if isinstance(path, str):
+            path = Path(path)
+
+        with (path / "config.json").open("r") as f:
+            config = json.load(f)
+        embedder = cls(**config["embedder_config"])
+        model_path = path / "model.pt"
+        model = model_module.load(model_path, **config["model_config"])
+        embedder._model = model
+        embedder._is_fitted = True
+        return embedder
+
+    @classmethod
+    def load(cls, path: Union[Path, str]) -> "GTFS2VecEmbedder":
+        """
+        Load the model from a directory.
+
+        Args:
+            path (Path): Path to the directory.
+
+        Returns:
+            Hex2VecEmbedder: The loaded embedder.
+        """
+        return cls._load(path, GTFS2VecModel)
```

### Comparing `srai-0.1.4/srai/embedders/gtfs2vec/model.py` & `srai-0.2.0/srai/embedders/gtfs2vec/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,22 @@
 This module contains embedding model from gtfs2vec paper [1].
 
 References:
     1. https://doi.org/10.1145/3486640.3491392
 """
 from typing import TYPE_CHECKING, Any
 
+from srai.embedders import Model
 from srai.utils._optional import import_optional_dependencies
 
 if TYPE_CHECKING:  # pragma: no cover
     import torch
 
 
-try:  # pragma: no cover
-    from pytorch_lightning import LightningModule
-
-except ImportError:
-    from srai.utils._pytorch_stubs import LightningModule
-
-
-class GTFS2VecModel(LightningModule):  # type: ignore
+class GTFS2VecModel(Model):
     """Autoencoder based embedding model for gtfs2vec."""
 
     def __init__(
         self,
         n_features: int,
         n_hidden: int = 48,
         n_embed: int = 64,
@@ -41,15 +35,16 @@
         super().__init__()
         import_optional_dependencies(
             dependency_group="torch", modules=["torch", "pytorch_lightning"]
         )
         from torch import nn
 
         self.n_features = n_features
-
+        self.n_hidden = n_hidden
+        self.n_embed = n_embed
         self.encoder = nn.Sequential(
             nn.Linear(n_features, n_hidden), nn.ReLU(), nn.Linear(n_hidden, n_embed)
         )
         self.decoder = nn.Sequential(
             nn.Linear(n_embed, n_hidden), nn.ReLU(), nn.Linear(n_hidden, n_features)
         )
```

### Comparing `srai-0.1.4/srai/embedders/hex2vec/embedder.py` & `srai-0.2.0/srai/embedders/hex2vec/embedder.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 Hex2Vec Embedder.
 
 This module contains embedder from Hex2Vec paper[1].
 
 References:
     [1] https://dl.acm.org/doi/10.1145/3486635.3491076
 """
-from typing import Any, Dict, List, Optional, TypeVar
+import json
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 
-from srai.embedders import CountEmbedder
+from srai.embedders import CountEmbedder, ModelT
 from srai.embedders.hex2vec.model import Hex2VecModel
 from srai.embedders.hex2vec.neighbour_dataset import NeighbourDataset
 from srai.exceptions import ModelNotFitException
 from srai.neighbourhoods import Neighbourhood
 from srai.utils._optional import import_optional_dependencies
 
 T = TypeVar("T")
@@ -119,15 +121,19 @@
         """
         import pytorch_lightning as pl
         from torch.utils.data import DataLoader
 
         trainer_kwargs = self._prepare_trainer_kwargs(trainer_kwargs)
 
         counts_df = self._get_raw_counts(regions_gdf, features_gdf, joint_gdf)
-        num_features = len(counts_df.columns)
+
+        if self.expected_output_features is None:  # type: ignore
+            self.expected_output_features = pd.Series(counts_df.columns)
+
+        num_features = len(self.expected_output_features)  # type: ignore
         self._model = Hex2VecModel(
             layer_sizes=[num_features, *self._encoder_sizes], learning_rate=learning_rate
         )
         dataset = NeighbourDataset(counts_df, neighbourhood, negative_sample_k_distance)
         dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True)
 
         trainer = pl.Trainer(**trainer_kwargs)
@@ -199,7 +205,68 @@
             raise ModelNotFitException("Model not fitted. Call fit() or fit_transform() first.")
 
     def _assert_encoder_sizes_correct(self, encoder_sizes: List[int]) -> None:
         if len(encoder_sizes) < 1:
             raise ValueError("Encoder sizes must have at least one element - embedding size.")
         if any(size <= 0 for size in encoder_sizes):
             raise ValueError("Encoder sizes must be positive integers.")
+
+    def _save(self, path: Union[Path, str], embedder_config: Dict[str, Any]) -> None:
+        if isinstance(path, str):
+            path = Path(path)
+
+        self._check_is_fitted()
+
+        path.mkdir(parents=True, exist_ok=True)
+
+        self._model.save(path / "model.pt")  # type: ignore
+
+        config = {
+            "model_config": self._model.get_config(),  # type: ignore
+            "embedder_config": embedder_config,
+        }
+        with open(path / "config.json", "w") as f:
+            json.dump(config, f, ensure_ascii=False, indent=4)
+
+    def save(self, path: Union[Path, str]) -> None:
+        """
+        Save the model to a directory.
+
+        Args:
+            path (Path): Path to the directory.
+        """
+        embedder_config = {
+            "encoder_sizes": self._encoder_sizes,
+            "expected_output_features": (
+                self.expected_output_features.tolist()
+                if self.expected_output_features is not None
+                else None
+            ),
+        }
+        self._save(path, embedder_config)
+
+    @classmethod
+    def _load(cls, path: Union[Path, str], model_module: Type[ModelT]) -> "Hex2VecEmbedder":
+        if isinstance(path, str):
+            path = Path(path)
+
+        with (path / "config.json").open("r") as f:
+            config = json.load(f)
+        embedder = cls(**config["embedder_config"])
+        model_path = path / "model.pt"
+        model = model_module.load(model_path, **config["model_config"])
+        embedder._model = model
+        embedder._is_fitted = True
+        return embedder
+
+    @classmethod
+    def load(cls, path: Union[Path, str]) -> "Hex2VecEmbedder":
+        """
+        Load the model from a directory.
+
+        Args:
+            path (Path): Path to the directory.
+
+        Returns:
+            Hex2VecEmbedder: The loaded embedder.
+        """
+        return cls._load(path, Hex2VecModel)
```

### Comparing `srai-0.1.4/srai/embedders/hex2vec/model.py` & `srai-0.2.0/srai/embedders/hex2vec/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,22 @@
 This module contains the embedding model from Hex2Vec paper[1].
 
 References:
     [1] https://dl.acm.org/doi/10.1145/3486635.3491076
 """
 from typing import TYPE_CHECKING, List, Tuple
 
+from srai.embedders import Model
 from srai.utils._optional import import_optional_dependencies
 
 if TYPE_CHECKING:  # pragma: no cover
     import torch
 
 
-try:  # pragma: no cover
-    from pytorch_lightning import LightningModule
-
-except ImportError:
-    from srai.utils._pytorch_stubs import LightningModule
-
-
-class Hex2VecModel(LightningModule):  # type: ignore
+class Hex2VecModel(Model):
     """
     Hex2Vec embedding model.
 
     This class implements the embedding model from Hex2Vec paper. It is based on a skip-gram model
     with negative sampling and triplet-loss. The model takes vectors of numbers as input (raw counts
     of features) per region and outputs dense embeddings.
     """
@@ -46,14 +40,15 @@
         """
         import_optional_dependencies(
             dependency_group="torch", modules=["torch", "pytorch_lightning"]
         )
         from torch import nn
 
         super().__init__()
+        self.layer_sizes = layer_sizes
         self.learning_rate = learning_rate
 
         if len(layer_sizes) < 2:
             raise ValueError("layer_sizes must contain at least 2 elements")
 
         def create_layers(sizes: List[Tuple[int, int]]) -> nn.Sequential:
             layers = []
```

### Comparing `srai-0.1.4/srai/embedders/hex2vec/neighbour_dataset.py` & `srai-0.2.0/srai/embedders/hex2vec/neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/embedders/highway2vec/model.py` & `srai-0.2.0/srai/embedders/highway2vec/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,22 @@
 This module contains the embedding model from the `highway2vec` paper [1].
 
 References:
     1. https://doi.org/10.1145/3557918.3565865
 """
 from typing import TYPE_CHECKING
 
+from srai.embedders import Model
 from srai.utils._optional import import_optional_dependencies
 
 if TYPE_CHECKING:  # pragma: no cover
     import torch
 
 
-try:  # pragma: no cover
-    from pytorch_lightning import LightningModule
-
-except ImportError:
-    from srai.utils._pytorch_stubs import LightningModule
-
-
-class Highway2VecModel(LightningModule):  # type: ignore
+class Highway2VecModel(Model):
     """Autoencoder based embedding model for highway2vec."""
 
     def __init__(self, n_features: int, n_hidden: int = 64, n_embed: int = 30, lr: float = 1e-3):
         """
         Init Highway2VecModel.
 
         Args:
@@ -49,14 +43,17 @@
             nn.Linear(n_hidden, n_embed),
         )
         self.decoder = nn.Sequential(
             nn.Linear(n_embed, n_hidden),
             nn.ReLU(),
             nn.Linear(n_hidden, n_features),
         )
+        self.n_features = n_features
+        self.n_hidden = n_hidden
+        self.n_embed = n_embed
         self.lr = lr
 
     def forward(self, x: "torch.Tensor") -> "torch.Tensor":
         """
         Forward pass.
 
         Args:
```

### Comparing `srai-0.1.4/srai/exceptions.py` & `srai-0.2.0/srai/exceptions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/joiners/__init__.py` & `srai-0.2.0/srai/joiners/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/joiners/_base.py` & `srai-0.2.0/srai/joiners/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/joiners/intersection_joiner.py` & `srai-0.2.0/srai/joiners/intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/__init__.py` & `srai-0.2.0/srai/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/_base.py` & `srai-0.2.0/srai/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/geoparquet_loader.py` & `srai-0.2.0/srai/loaders/geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/gtfs_loader.py` & `srai-0.2.0/srai/loaders/gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/_base.py` & `srai-0.2.0/srai/loaders/osm_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/filters/_typing.py` & `srai-0.2.0/srai/loaders/osm_loaders/filters/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/filters/base_osm_groups.py` & `srai-0.2.0/srai/loaders/osm_loaders/filters/base_osm_groups.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/filters/geofabrik.py` & `srai-0.2.0/srai/loaders/osm_loaders/filters/geofabrik.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/filters/hex2vec.py` & `srai-0.2.0/srai/loaders/osm_loaders/filters/hex2vec.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/filters/popular.py` & `srai-0.2.0/srai/loaders/osm_loaders/filters/popular.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/osm_online_loader.py` & `srai-0.2.0/srai/loaders/osm_loaders/osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/osm_pbf_loader.py` & `srai-0.2.0/srai/loaders/osm_loaders/osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/osm_tile_data_collector.py` & `srai-0.2.0/srai/loaders/osm_loaders/osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/osm_tile_loader.py` & `srai-0.2.0/srai/loaders/osm_loaders/osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/pbf_file_downloader.py` & `srai-0.2.0/srai/loaders/osm_loaders/pbf_file_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_loaders/pbf_file_handler.py` & `srai-0.2.0/srai/loaders/osm_loaders/pbf_file_handler.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_way_loader/constants.py` & `srai-0.2.0/srai/loaders/osm_way_loader/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/loaders/osm_way_loader/osm_way_loader.py` & `srai-0.2.0/srai/loaders/osm_way_loader/osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/neighbourhoods/_base.py` & `srai-0.2.0/srai/neighbourhoods/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/neighbourhoods/adjacency_neighbourhood.py` & `srai-0.2.0/srai/neighbourhoods/adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/neighbourhoods/h3_neighbourhood.py` & `srai-0.2.0/srai/neighbourhoods/h3_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/plotting/folium_wrapper.py` & `srai-0.2.0/srai/plotting/folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/plotting/plotly_wrapper.py` & `srai-0.2.0/srai/plotting/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/regionalizers/__init__.py` & `srai-0.2.0/srai/regionalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/regionalizers/_base.py` & `srai-0.2.0/srai/regionalizers/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/regionalizers/_spherical_voronoi.py` & `srai-0.2.0/srai/regionalizers/_spherical_voronoi.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/regionalizers/administrative_boundary_regionalizer.py` & `srai-0.2.0/srai/regionalizers/administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/regionalizers/h3_regionalizer.py` & `srai-0.2.0/srai/regionalizers/h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/regionalizers/s2_regionalizer.py` & `srai-0.2.0/srai/regionalizers/s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/regionalizers/slippy_map_regionalizer.py` & `srai-0.2.0/srai/regionalizers/slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/regionalizers/voronoi_regionalizer.py` & `srai-0.2.0/srai/regionalizers/voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/utils/__init__.py` & `srai-0.2.0/srai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/utils/_optional.py` & `srai-0.2.0/srai/utils/_optional.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/utils/download.py` & `srai-0.2.0/srai/utils/download.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/utils/geocode.py` & `srai-0.2.0/srai/utils/geocode.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/utils/geometry.py` & `srai-0.2.0/srai/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/utils/merge.py` & `srai-0.2.0/srai/utils/merge.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/srai/utils/typing.py` & `srai-0.2.0/srai/utils/typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/conftest.py` & `srai-0.2.0/tests/embedders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/constants.py` & `srai-0.2.0/tests/embedders/hex2vec/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/generation.py` & `srai-0.2.0/tests/embedders/hex2vec/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_embedder.py` & `srai-0.2.0/tests/embedders/hex2vec/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_features.parquet` & `srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_joint.parquet` & `srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_regions.parquet` & `srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_files/poz_8_result.parquet` & `srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_features.parquet` & `srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_joint.parquet` & `srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_regions.parquet` & `srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_files/wro_9_result.parquet` & `srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_model.py` & `srai-0.2.0/tests/embedders/hex2vec/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/hex2vec/test_neighbour_dataset.py` & `srai-0.2.0/tests/embedders/hex2vec/test_neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/test_contextual_count_embedder.py` & `srai-0.2.0/tests/embedders/test_contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/test_count_embedder.py` & `srai-0.2.0/tests/embedders/test_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/test_gtfs2vec_embedder.py` & `srai-0.2.0/tests/embedders/test_gtfs2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/embedders/test_highway2vec_embedder.py` & `srai-0.2.0/tests/embedders/test_highway2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/joiners/conftest.py` & `srai-0.2.0/tests/joiners/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/joiners/test_intersection_joiner.py` & `srai-0.2.0/tests/joiners/test_intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/conftest.py` & `srai-0.2.0/tests/loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/conftest.py` & `srai-0.2.0/tests/loaders/osm_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/filters/popular_filter_example.json` & `srai-0.2.0/tests/loaders/osm_loaders/filters/popular_filter_example.json`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/filters/test_merge_filter_types.py` & `srai-0.2.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py` & `srai-0.2.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `srai-0.2.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `srai-0.2.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `srai-0.2.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_files/poland.geojson` & `srai-0.2.0/tests/loaders/osm_loaders/test_files/poland.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson` & `srai-0.2.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_osm_online_loader.py` & `srai-0.2.0/tests/loaders/osm_loaders/test_osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_osm_pbf_loader.py` & `srai-0.2.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_osm_tile_data_collector.py` & `srai-0.2.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_loaders/test_osm_tile_loader.py` & `srai-0.2.0/tests/loaders/osm_loaders/test_osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl` & `srai-0.2.0/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl` & `srai-0.2.0/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl` & `srai-0.2.0/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl` & `srai-0.2.0/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl` & `srai-0.2.0/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl` & `srai-0.2.0/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/osm_way_loader/test_osm_way_loader.py` & `srai-0.2.0/tests/loaders/osm_way_loader/test_osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/test_files/example.parquet` & `srai-0.2.0/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/test_geoparquet_loader.py` & `srai-0.2.0/tests/loaders/test_geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/loaders/test_gtfs_loader.py` & `srai-0.2.0/tests/loaders/test_gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/miscellaneous/test_optional_dependencies.py` & `srai-0.2.0/tests/miscellaneous/test_optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/neighbourhoods/h3/test_no_regions.py` & `srai-0.2.0/tests/neighbourhoods/h3/test_no_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/neighbourhoods/h3/test_with_regions.py` & `srai-0.2.0/tests/neighbourhoods/h3/test_with_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/neighbourhoods/test_adjacency_neighbourhood.py` & `srai-0.2.0/tests/neighbourhoods/test_adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/neighbourhoods/test_neighbourhood.py` & `srai-0.2.0/tests/neighbourhoods/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/regionalizers/conftest.py` & `srai-0.2.0/tests/regionalizers/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/regionalizers/test_administrative_boundary_regionalizer.py` & `srai-0.2.0/tests/regionalizers/test_administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/regionalizers/test_h3_regionalizer.py` & `srai-0.2.0/tests/regionalizers/test_h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/regionalizers/test_s2_regionalizer.py` & `srai-0.2.0/tests/regionalizers/test_s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/regionalizers/test_slippy_map_regionalizer.py` & `srai-0.2.0/tests/regionalizers/test_slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/tests/regionalizers/test_voronoi_regionalizer.py` & `srai-0.2.0/tests/regionalizers/test_voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.1.4/PKG-INFO` & `srai-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai
-Version: 0.1.4
+Version: 0.2.0
 Summary: A set of python modules for geospatial machine learning and data mining
 Author: Piotr Gramacki, Kacper Leśniara, Kamil Raczycki, Szymon Woźniak
 Author-Email: SRAI Lab <spatialrepresentationsforai@gmail.com>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -36,23 +36,24 @@
 Requires-Dist: pyarrow
 Requires-Dist: topojson
 Requires-Dist: tqdm
 Requires-Dist: s2
 Requires-Dist: typeguard
 Requires-Dist: requests
 Requires-Dist: osmium; extra == "osm"
-Requires-Dist: osmnx; extra == "osm"
+Requires-Dist: osmnx<=1.4.0; extra == "osm"
 Requires-Dist: overpass; extra == "osm"
 Requires-Dist: pillow; extra == "osm"
 Requires-Dist: pymap3d; extra == "voronoi"
 Requires-Dist: haversine; extra == "voronoi"
 Requires-Dist: spherical-geometry; extra == "voronoi"
 Requires-Dist: gtfs-kit; extra == "gtfs"
 Requires-Dist: folium; extra == "plotting"
 Requires-Dist: mapclassify; extra == "plotting"
+Requires-Dist: matplotlib; extra == "plotting"
 Requires-Dist: plotly; extra == "plotting"
 Requires-Dist: kaleido<=0.2.1; extra == "plotting"
 Requires-Dist: pytorch-lightning; extra == "torch"
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: srai[gtfs,osm,plotting,torch,voronoi]; extra == "all"
 Provides-Extra: osm
 Provides-Extra: voronoi
@@ -332,14 +333,25 @@
 plot_numeric_data(regions, embeddings, 0, map=folium_map)
 ```
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/embedding_hex2vec_embedder.jpg" style="max-width:600px;width:100%"/>
 </p>
 
+### Pre-trained models usage
+
+We provide pre-trained models for some of the embedding methods. To use them, simply download them from [here](https://drive.google.com/drive/folders/14sH33-kNxA0q1O1abPWTpuix8raR_XbD?usp=drive_link) and load them using `load` method:
+
+```python
+from srai.embedders import Hex2VecEmbedder
+
+model_path = "path/to/model"
+embedder = Hex2VecEmbedder.load(model_path)
+```
+
 ### Plotting, utilities and more
 
 We also provide utilities for different spatial operations and plotting functions adopted to data formats used in `srai` For a full list of available methods, please refer to the [documentation](https://srai-lab.github.io/srai).
 
 ## Contributing
 
 If you are willing to contribute to `srai`, feel free to do so! Visit [our contributing guide](./CONTRIBUTING.md) for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: srai Version: 0.1.4 Summary: A set of python
+Metadata-Version: 2.1 Name: srai Version: 0.2.0 Summary: A set of python
 modules for geospatial machine learning and data mining Author: Piotr Gramacki,
 Kacper LeÅniara, Kamil Raczycki, Szymon WoÅºniak Author-Email: SRAI Lab
 gmail.com> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
@@ -15,25 +15,26 @@
 Project-URL: Documentation, https://srai-lab.github.io/srai Project-URL:
 Changelog, https://github.com/srai-lab/srai/blob/main/CHANGELOG.md Requires-
 Python: >=3.8 Requires-Dist: pandas Requires-Dist: geopandas Requires-Dist:
 shapely Requires-Dist: h3>=4.0.0b1 Requires-Dist: numpy Requires-Dist:
 geoparquet Requires-Dist: pyfunctional Requires-Dist: rtree Requires-Dist:
 scipy Requires-Dist: pyarrow Requires-Dist: topojson Requires-Dist: tqdm
 Requires-Dist: s2 Requires-Dist: typeguard Requires-Dist: requests Requires-
-Dist: osmium; extra == "osm" Requires-Dist: osmnx; extra == "osm" Requires-
-Dist: overpass; extra == "osm" Requires-Dist: pillow; extra == "osm" Requires-
-Dist: pymap3d; extra == "voronoi" Requires-Dist: haversine; extra == "voronoi"
-Requires-Dist: spherical-geometry; extra == "voronoi" Requires-Dist: gtfs-kit;
-extra == "gtfs" Requires-Dist: folium; extra == "plotting" Requires-Dist:
-mapclassify; extra == "plotting" Requires-Dist: plotly; extra == "plotting"
-Requires-Dist: kaleido<=0.2.1; extra == "plotting" Requires-Dist: pytorch-
-lightning; extra == "torch" Requires-Dist: torch; extra == "torch" Requires-
-Dist: srai[gtfs,osm,plotting,torch,voronoi]; extra == "all" Provides-Extra: osm
-Provides-Extra: voronoi Provides-Extra: gtfs Provides-Extra: plotting Provides-
-Extra: torch Provides-Extra: all Description-Content-Type: text/markdown
+Dist: osmium; extra == "osm" Requires-Dist: osmnx<=1.4.0; extra == "osm"
+Requires-Dist: overpass; extra == "osm" Requires-Dist: pillow; extra == "osm"
+Requires-Dist: pymap3d; extra == "voronoi" Requires-Dist: haversine; extra ==
+"voronoi" Requires-Dist: spherical-geometry; extra == "voronoi" Requires-Dist:
+gtfs-kit; extra == "gtfs" Requires-Dist: folium; extra == "plotting" Requires-
+Dist: mapclassify; extra == "plotting" Requires-Dist: matplotlib; extra ==
+"plotting" Requires-Dist: plotly; extra == "plotting" Requires-Dist:
+kaleido<=0.2.1; extra == "plotting" Requires-Dist: pytorch-lightning; extra ==
+"torch" Requires-Dist: torch; extra == "torch" Requires-Dist: srai
+[gtfs,osm,plotting,torch,voronoi]; extra == "all" Provides-Extra: osm Provides-
+Extra: voronoi Provides-Extra: gtfs Provides-Extra: plotting Provides-Extra:
+torch Provides-Extra: all Description-Content-Type: text/markdown
  [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/logos/srai-
                              logo-transparent.png]
   [GitHub] [Checks] [GitHub_Workflow_Status_-_DEV] [GitHub_Workflow_Status_-
  PROD] [pre-commit.ci_status] [CodeFactor_Grade] [Codecov] [Package_version]
                 [Supported_Python_versions] [PyPI_-_Downloads]
 # Spatial Representations for Artificial Intelligence
   â ï¸ð§ This library is under HEAVY development. Expect breaking changes
@@ -176,47 +177,52 @@
 (regions, features, joint) # Option 2: fit_transform embeddings =
 embedder.fit_transform(regions, features, joint, neighbourhood, batch_size=128)
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
 tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings, 0,
 map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                         embedding_hex2vec_embedder.jpg]
-### Plotting, utilities and more We also provide utilities for different
-spatial operations and plotting functions adopted to data formats used in
-`srai` For a full list of available methods, please refer to the
-[documentation](https://srai-lab.github.io/srai). ## Contributing If you are
-willing to contribute to `srai`, feel free to do so! Visit [our contributing
-guide](./CONTRIBUTING.md) for more details. ## Publications Some of the methods
-implemented in `srai` have been published in scientific journals and
-conferences. 1. Szymon WoÅºniak and Piotr SzymaÅski. 2021. Hex2vec: Context-
-Aware Embedding H3 Hexagons with OpenStreetMap Tags. In Proceedings of the 4th
-ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge Discovery
-(GEOAI '21). Association for Computing Machinery, New York, NY, USA, 61â71.
-[paper](https://doi.org/10.1145/3486635.3491076), [arXiv](https://arxiv.org/
-abs/2111.00970) 2. Piotr Gramacki, Szymon WoÅºniak, and Piotr SzymaÅski. 2021.
-Gtfs2vec: Learning GTFS Embeddings for comparing Public Transport Offer in
-Microregions. In Proceedings of the 1st ACM SIGSPATIAL International Workshop
-on Searching and Mining Large Collections of Geospatial Data (GeoSearch'21).
-Association for Computing Machinery, New York, NY, USA, 5â12. [paper](https:/
-/doi.org/10.1145/3486640.3491392), [arXiv](https://arxiv.org/abs/2111.00960) 3.
-Kamil Raczycki and Piotr SzymaÅski. 2021. Transfer learning approach to
-bicycle-sharing systems' station location planning using OpenStreetMap data. In
-Proceedings of the 4th ACM SIGSPATIAL International Workshop on Advances in
-Resilient and Intelligent Cities (ARIC '21). Association for Computing
-Machinery, New York, NY, USA, 1â12. [paper](https://doi.org/10.1145/
-3486626.3493434), [arXiv](https://arxiv.org/abs/2111.00990) 4. Kacper LeÅniara
-and Piotr SzymaÅski. 2022. Highway2vec: representing OpenStreetMap
-microregions with respect to their road network characteristics. In Proceedings
-of the 5th ACM SIGSPATIAL International Workshop on AI for Geographic Knowledge
-Discovery (GeoAI '22). Association for Computing Machinery, New York, NY, USA,
-18â29. [paper](https://doi.org/10.1145/3557918.3565865), [arXiv](https://
-arxiv.org/abs/2304.13865) ## Acknowledgements We would like to thank Piotr
-SzymaÅski PhD \([@niedakh](https://twitter.com/niedakh)\) for his invaluable
-guidance and support in the development of this library. His expertise and
-mentorship have been instrumental in shaping the library's design and
-functionality, and we are very grateful for his input. ## Citation TBD ##
-License This library is licensed under the [Apache License 2.0](https://
-github.com/srai-lab/srai/blob/main/LICENSE.md). The free [OpenStreetMap](https:
-//www.openstreetmap.org/) data, which is used for the development of SRAI, is
-licensed under the [Open Data Commons Open Database License](https://
-opendatacommons.org/licenses/odbl/) (ODbL) by the [OpenStreetMap Foundation]
-(https://osmfoundation.org/) (OSMF).
+### Pre-trained models usage We provide pre-trained models for some of the
+embedding methods. To use them, simply download them from [here](https://
+drive.google.com/drive/folders/14sH33-
+kNxA0q1O1abPWTpuix8raR_XbD?usp=drive_link) and load them using `load` method:
+```python from srai.embedders import Hex2VecEmbedder model_path = "path/to/
+model" embedder = Hex2VecEmbedder.load(model_path) ``` ### Plotting, utilities
+and more We also provide utilities for different spatial operations and
+plotting functions adopted to data formats used in `srai` For a full list of
+available methods, please refer to the [documentation](https://srai-
+lab.github.io/srai). ## Contributing If you are willing to contribute to
+`srai`, feel free to do so! Visit [our contributing guide](./CONTRIBUTING.md)
+for more details. ## Publications Some of the methods implemented in `srai`
+have been published in scientific journals and conferences. 1. Szymon WoÅºniak
+and Piotr SzymaÅski. 2021. Hex2vec: Context-Aware Embedding H3 Hexagons with
+OpenStreetMap Tags. In Proceedings of the 4th ACM SIGSPATIAL International
+Workshop on AI for Geographic Knowledge Discovery (GEOAI '21). Association for
+Computing Machinery, New York, NY, USA, 61â71. [paper](https://doi.org/
+10.1145/3486635.3491076), [arXiv](https://arxiv.org/abs/2111.00970) 2. Piotr
+Gramacki, Szymon WoÅºniak, and Piotr SzymaÅski. 2021. Gtfs2vec: Learning GTFS
+Embeddings for comparing Public Transport Offer in Microregions. In Proceedings
+of the 1st ACM SIGSPATIAL International Workshop on Searching and Mining Large
+Collections of Geospatial Data (GeoSearch'21). Association for Computing
+Machinery, New York, NY, USA, 5â12. [paper](https://doi.org/10.1145/
+3486640.3491392), [arXiv](https://arxiv.org/abs/2111.00960) 3. Kamil Raczycki
+and Piotr SzymaÅski. 2021. Transfer learning approach to bicycle-sharing
+systems' station location planning using OpenStreetMap data. In Proceedings of
+the 4th ACM SIGSPATIAL International Workshop on Advances in Resilient and
+Intelligent Cities (ARIC '21). Association for Computing Machinery, New York,
+NY, USA, 1â12. [paper](https://doi.org/10.1145/3486626.3493434), [arXiv]
+(https://arxiv.org/abs/2111.00990) 4. Kacper LeÅniara and Piotr SzymaÅski.
+2022. Highway2vec: representing OpenStreetMap microregions with respect to
+their road network characteristics. In Proceedings of the 5th ACM SIGSPATIAL
+International Workshop on AI for Geographic Knowledge Discovery (GeoAI '22).
+Association for Computing Machinery, New York, NY, USA, 18â29. [paper](https:
+//doi.org/10.1145/3557918.3565865), [arXiv](https://arxiv.org/abs/2304.13865)
+## Acknowledgements We would like to thank Piotr SzymaÅski PhD \([@niedakh]
+(https://twitter.com/niedakh)\) for his invaluable guidance and support in the
+development of this library. His expertise and mentorship have been
+instrumental in shaping the library's design and functionality, and we are very
+grateful for his input. ## Citation TBD ## License This library is licensed
+under the [Apache License 2.0](https://github.com/srai-lab/srai/blob/main/
+LICENSE.md). The free [OpenStreetMap](https://www.openstreetmap.org/) data,
+which is used for the development of SRAI, is licensed under the [Open Data
+Commons Open Database License](https://opendatacommons.org/licenses/odbl/)
+(ODbL) by the [OpenStreetMap Foundation](https://osmfoundation.org/) (OSMF).
```

