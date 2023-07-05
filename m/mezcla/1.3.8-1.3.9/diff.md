# Comparing `tmp/mezcla-1.3.8.tar.gz` & `tmp/mezcla-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.3.8.tar", last modified: Wed Jun 21 08:36:51 2023, max compression
+gzip compressed data, was "mezcla-1.3.9.tar", last modified: Wed Jul  5 20:42:19 2023, max compression
```

## Comparing `mezcla-1.3.8.tar` & `mezcla-1.3.9.tar`

### file list

```diff
@@ -1,161 +1,165 @@
--rw-r--r--   0        0        0      542 2023-06-18 00:28:36.095854 mezcla-1.3.8/.coveragerc
--rw-r--r--   0        0        0     1042 2023-06-18 00:28:36.095854 mezcla-1.3.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1937 2023-06-18 00:29:02.178395 mezcla-1.3.8/.gitignore
--rw-r--r--   0        0        0     2621 2023-06-18 00:28:36.095854 mezcla-1.3.8/Dockerfile
--rw-r--r--   0        0        0     7370 2023-06-18 00:28:36.095854 mezcla-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0      777 2023-06-18 00:28:36.095854 mezcla-1.3.8/README.txt
--rw-r--r--   0        0        0      380 2023-06-18 00:28:36.095854 mezcla-1.3.8/TODO.txt
--rw-r--r--   0        0        0      130 2023-06-18 00:28:36.095854 mezcla-1.3.8/mezcla/TODO.md
--rwxr-xr-x   0        0        0     1927 2023-06-21 08:32:51.710523 mezcla-1.3.8/mezcla/__init__.py
--rwxr-xr-x   0        0        0    10860 2023-06-18 00:28:36.095854 mezcla-1.3.8/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    13025 2023-06-18 00:36:41.989782 mezcla-1.3.8/mezcla/audio.py
--rwxr-xr-x   0        0        0     4707 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/bash_ast.py
--rwxr-xr-x   0        0        0    16055 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25702 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     7625 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     8925 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14338 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0    22279 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/cut.py
--rwxr-xr-x   0        0        0     4307 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    47920 2023-06-18 00:29:02.182396 mezcla-1.3.8/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0        0 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12834 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3608 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/download_user_gist.py
--rwxr-xr-x   0        0        0     6477 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8779 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0    28364 2023-06-21 06:10:44.430553 mezcla-1.3.8/mezcla/examples/hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     3338 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     3922 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/iris.csv
--rw-r--r--   0        0        0    23345 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/plot_forest_importances.py
--rwxr-xr-x   0        0        0    12989 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     1938 2023-06-21 06:10:44.430553 mezcla-1.3.8/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0     5006 2023-06-21 06:10:44.430553 mezcla-1.3.8/mezcla/examples/tests/test_hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     3607 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     4031 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     7708 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     2998 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32894 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    32756 2023-06-21 06:10:44.430553 mezcla-1.3.8/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0    32492 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     4708 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17916 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    45741 2023-06-21 08:32:51.714523 mezcla-1.3.8/mezcla/main.py
--rwxr-xr-x   0        0        0     9307 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11717 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0    11641 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0     9779 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    13776 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0      737 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31436 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      828 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     7053 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     7604 2023-06-18 00:29:02.182396 mezcla-1.3.8/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40529 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39613 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/run_bert_classifier.py
--rwxr-xr-x   0        0        0    17400 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     1508 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    19931 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     3011 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/sys_version_info_hack.py
--rwxr-xr-x   0        0        0    50554 2023-06-21 06:10:44.434553 mezcla-1.3.8/mezcla/system.py
--rwxr-xr-x   0        0        0    45776 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     5594 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/template.py
--rw-r--r--   0        0        0     7370 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      462 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/TODO.md
--rw-r--r--   0        0        0     1082 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/adhoc-tests.batspp
--rw-r--r--   0        0        0      204 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/misc-tests.batspp
--rwxr-xr-x   0        0        0     3905 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/misc_doctests.py
--rw-r--r--   0        0        0      810 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars-csv-len-3.txt
--rw-r--r--   0        0        0      113 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      602 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars-tsv-len-3.txt
--rw-r--r--   0        0        0      659 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      655 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0     1152 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0       65 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/word-POS.freq
--rw-r--r--   0        0        0      254 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     4816 2023-06-18 00:29:02.182396 mezcla-1.3.8/mezcla/tests/template.py
--rwxr-xr-x   0        0        0     2489 2023-06-18 00:29:02.182396 mezcla-1.3.8/mezcla/tests/test___init__.py
--rwxr-xr-x   0        0        0     4736 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/test_audio.py
--rwxr-xr-x   0        0        0      969 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/test_bert_multi_classification.py
--rwxr-xr-x   0        0        0      834 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/test_bing_search.py
--rwxr-xr-x   0        0        0     1974 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_compute_tfidf.py
--rwxr-xr-x   0        0        0     2905 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_cut.py
--rwxr-xr-x   0        0        0     2464 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    15032 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_debug.py
--rwxr-xr-x   0        0        0     1030 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4429 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2939 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0     2562 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    15711 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0    13008 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_html_utils.py
--rwxr-xr-x   0        0        0      892 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_kenlm_example.py
--rwxr-xr-x   0        0        0     2114 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0     8972 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_main.py
--rwxr-xr-x   0        0        0     2725 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_merge_files.py
--rwxr-xr-x   0        0        0     1291 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     6565 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     2882 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_my_regex.py
--rwxr-xr-x   0        0        0      916 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_ngram_tfidf.py
--rwxr-xr-x   0        0        0      931 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_os_utils.py
--rwxr-xr-x   0        0        0     8323 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_pandas_sklearn.py
--rwxr-xr-x   0        0        0     1215 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_plot_utils.py
--rwxr-xr-x   0        0        0      854 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2869 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_rgb_color_name.py
--rwxr-xr-x   0        0        0      895 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_run_albert_classifier.py
--rwxr-xr-x   0        0        0      930 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_run_bert_classifier.py
--rwxr-xr-x   0        0        0     1602 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_show_bert_representation.py
--rwxr-xr-x   0        0        0      916 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_simple_main_example.py
--rwxr-xr-x   0        0        0     2083 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_spacy_nlp.py
--rwxr-xr-x   0        0        0      882 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    33402 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     1769 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     3714 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_text_categorizer.py
--rwxr-xr-x   0        0        0     7264 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7362 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    21785 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_tpo_common.py
--rwxr-xr-x   0        0        0      715 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_train_language_model.py
--rwxr-xr-x   0        0        0      725 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_train_text_categorizer.py
--rwxr-xr-x   0        0        0      686 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_transpose_data.py
--rwxr-xr-x   0        0        0     2859 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_xml_utils.py
--rwxr-xr-x   0        0        0      676 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/tests/tfidf/test_corpus.py
--rwxr-xr-x   0        0        0      697 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/tests/tfidf/test_dockeyword.py
--rwxr-xr-x   0        0        0      688 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/tests/tfidf/test_document.py
--rwxr-xr-x   0        0        0      697 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    33807 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    23204 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    16223 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0    18423 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     2282 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7983 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/document.py
-lrwxr-xr-x   0        0        0        0 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
--rwxr-xr-x   0        0        0    16163 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/preprocess.py
--rwxr-xr-x   0        0        0    59862 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5267 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5098 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6778 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/transpose_data.py
--rwxr-xr-x   0        0        0    13361 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/xml_utils.py
--rw-r--r--   0        0        0      958 2023-06-18 00:28:36.139858 mezcla-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     2432 2023-06-18 00:29:02.186396 mezcla-1.3.8/requirements.txt
--rwxr-xr-x   0        0        0     1162 2023-06-21 08:32:51.714523 mezcla-1.3.8/setup.py
--rwxr-xr-x   0        0        0    45023 2023-06-18 00:28:36.139858 mezcla-1.3.8/temp/simple_batspp.py
--rwxr-xr-x   0        0        0      862 2023-06-18 00:28:36.139858 mezcla-1.3.8/tools/run_tests.bash
--rw-r--r--   0        0        0      612 2023-06-18 00:28:36.139858 mezcla-1.3.8/tox.ini
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mezcla-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-04-30 22:44:00.000000 mezcla-1.3.9/.coveragerc
+-rw-r--r--   0        0        0     1253 2023-07-04 06:24:29.977415 mezcla-1.3.9/.github/workflows/act.yml
+-rw-r--r--   0        0        0     1042 2023-06-01 22:36:35.000000 mezcla-1.3.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1937 2023-06-10 03:29:46.000000 mezcla-1.3.9/.gitignore
+-rw-r--r--   0        0        0     4950 2023-07-01 21:24:22.402445 mezcla-1.3.9/Dockerfile
+-rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0      777 2022-06-03 04:33:57.000000 mezcla-1.3.9/README.txt
+-rw-r--r--   0        0        0      380 2023-06-01 22:36:35.000000 mezcla-1.3.9/TODO.txt
+-rw-r--r--   0        0        0      130 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/TODO.md
+-rwxr-xr-x   0        0        0     2259 2023-07-04 06:10:43.446939 mezcla-1.3.9/mezcla/__init__.py
+-rwxr-xr-x   0        0        0    10872 2023-07-01 01:05:14.785985 mezcla-1.3.9/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    13025 2023-06-18 00:32:33.000000 mezcla-1.3.9/mezcla/audio.py
+-rwxr-xr-x   0        0        0     4707 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/bash_ast.py
+-rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.000000 mezcla-1.3.9/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25718 2023-07-01 01:12:47.735987 mezcla-1.3.9/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     7625 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     9241 2023-06-29 05:58:21.372447 mezcla-1.3.9/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14284 2023-07-01 01:05:14.785985 mezcla-1.3.9/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0     3145 2023-07-02 23:54:56.761692 mezcla-1.3.9/mezcla/convert_emoticons.py
+-rwxr-xr-x   0        0        0    22279 2023-07-01 01:12:47.739987 mezcla-1.3.9/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4307 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    48772 2023-07-05 20:15:46.458028 mezcla-1.3.9/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0        0 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12874 2023-07-01 01:12:47.739987 mezcla-1.3.9/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3644 2023-07-01 01:12:47.739987 mezcla-1.3.9/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/download_user_gist.py
+-rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.000000 mezcla-1.3.9/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.000000 mezcla-1.3.9/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8811 2023-07-01 01:12:47.739987 mezcla-1.3.9/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0    30001 2023-07-05 20:16:25.630128 mezcla-1.3.9/mezcla/examples/hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     3338 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     3922 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.3.9/mezcla/examples/iris.csv
+-rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.3.9/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.000000 mezcla-1.3.9/mezcla/examples/plot_forest_importances.py
+-rwxr-xr-x   0        0        0    13004 2023-07-01 01:56:03.422567 mezcla-1.3.9/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     2068 2023-07-02 23:30:29.556473 mezcla-1.3.9/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/examples/tensorflow_matrix_multiply.py
+-rwxr-xr-x   0        0        0     5070 2023-06-29 06:26:07.199936 mezcla-1.3.9/mezcla/examples/tests/test_hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     3617 2023-07-01 01:05:14.793985 mezcla-1.3.9/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     4031 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     7708 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.3.9/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     2998 2021-09-30 12:02:57.000000 mezcla-1.3.9/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32976 2023-07-01 21:43:17.040662 mezcla-1.3.9/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    33811 2023-07-03 00:58:21.152566 mezcla-1.3.9/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0    35278 2023-07-05 20:22:18.399100 mezcla-1.3.9/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     4708 2021-09-30 12:02:57.000000 mezcla-1.3.9/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17916 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    46774 2023-07-02 23:33:30.418758 mezcla-1.3.9/mezcla/main.py
+-rwxr-xr-x   0        0        0     9307 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11717 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0    11648 2023-07-01 01:58:45.279182 mezcla-1.3.9/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0     9993 2023-07-02 23:34:27.331430 mezcla-1.3.9/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    13776 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0      737 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31508 2023-07-01 01:12:47.743987 mezcla-1.3.9/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      828 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     7053 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     7604 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40529 2022-03-01 08:46:55.000000 mezcla-1.3.9/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39613 2022-06-16 07:59:25.000000 mezcla-1.3.9/mezcla/run_bert_classifier.py
+-rwxr-xr-x   0        0        0    17400 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     1508 2021-09-30 12:02:57.000000 mezcla-1.3.9/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    19931 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3011 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.3.9/mezcla/sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    51914 2023-07-05 20:23:04.687235 mezcla-1.3.9/mezcla/system.py
+-rwxr-xr-x   0        0        0    45776 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     5625 2023-07-02 23:50:24.908274 mezcla-1.3.9/mezcla/template.py
+-rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.3.9/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      462 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/TODO.md
+-rw-r--r--   0        0        0     1082 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/adhoc-tests.batspp
+-rw-r--r--   0        0        0      204 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/misc-tests.batspp
+-rwxr-xr-x   0        0        0     3905 2022-06-03 04:33:57.000000 mezcla-1.3.9/mezcla/tests/misc_doctests.py
+-rw-r--r--   0        0        0      810 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/resources/cars-csv-len-3.txt
+-rw-r--r--   0        0        0      113 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      602 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/resources/cars-tsv-len-3.txt
+-rw-r--r--   0        0        0      659 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      655 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0     1152 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0       65 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/resources/word-POS.freq
+-rw-r--r--   0        0        0      254 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     4836 2023-07-02 23:52:07.820771 mezcla-1.3.9/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     2489 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/test___init__.py
+-rwxr-xr-x   0        0        0     4736 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0      834 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     1974 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_compute_tfidf.py
+-rw-r--r--   0        0        0     3523 2023-07-02 23:26:56.041382 mezcla-1.3.9/mezcla/tests/test_convert_emoticons.py
+-rwxr-xr-x   0        0        0     2905 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2464 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    16047 2023-07-01 02:00:52.582153 mezcla-1.3.9/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     1030 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4429 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2939 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0     3449 2023-07-01 21:45:57.905414 mezcla-1.3.9/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    15711 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0    13008 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0      892 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     2114 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0     8972 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2725 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     6565 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     2886 2023-07-01 02:02:49.768496 mezcla-1.3.9/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0      916 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0      991 2023-07-01 01:12:47.747987 mezcla-1.3.9/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8297 2023-07-01 01:12:47.747987 mezcla-1.3.9/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0     1183 2023-07-01 02:02:49.768496 mezcla-1.3.9/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0      854 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2873 2023-07-01 02:02:49.768496 mezcla-1.3.9/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0      916 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     2083 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0      882 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    33490 2023-07-04 06:33:21.263049 mezcla-1.3.9/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     1769 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     3714 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0     7264 2023-04-30 22:47:21.000000 mezcla-1.3.9/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7362 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    21785 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0      725 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0      686 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_transpose_data.py
+-rwxr-xr-x   0        0        0     2859 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/tests/test_xml_utils.py
+-rwxr-xr-x   0        0        0      676 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/tfidf/test_corpus.py
+-rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/tfidf/test_dockeyword.py
+-rwxr-xr-x   0        0        0      688 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/tfidf/test_document.py
+-rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.3.9/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    33820 2023-07-01 01:05:14.801984 mezcla-1.3.9/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    23204 2023-06-01 22:36:35.000000 mezcla-1.3.9/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    16223 2023-04-30 22:44:00.000000 mezcla-1.3.9/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2022-07-10 04:39:58.000000 mezcla-1.3.9/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0    18423 2023-07-04 06:13:52.451491 mezcla-1.3.9/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     2282 2023-07-04 06:13:52.451491 mezcla-1.3.9/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7983 2023-07-04 06:13:52.451491 mezcla-1.3.9/mezcla/tfidf/document.py
+lrwxr-xr-x   0        0        0        0 2022-06-03 04:33:57.000000 mezcla-1.3.9/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
+-rwxr-xr-x   0        0        0    16168 2023-07-04 06:13:52.451491 mezcla-1.3.9/mezcla/tfidf/preprocess.py
+-rwxr-xr-x   0        0        0    59922 2023-07-01 01:05:14.805985 mezcla-1.3.9/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5267 2022-04-12 04:31:30.000000 mezcla-1.3.9/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5098 2021-10-22 05:45:54.000000 mezcla-1.3.9/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6778 2021-09-30 12:02:57.000000 mezcla-1.3.9/mezcla/transpose_data.py
+-rwxr-xr-x   0        0        0    13455 2023-07-02 23:53:11.409104 mezcla-1.3.9/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.3.9/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      958 2022-06-03 04:33:57.000000 mezcla-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2469 2023-07-01 05:11:48.148105 mezcla-1.3.9/requirements.txt
+-rwxr-xr-x   0        0        0     1162 2023-07-04 06:10:43.450939 mezcla-1.3.9/setup.py
+-rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.000000 mezcla-1.3.9/temp/simple_batspp.py
+-rw-r--r--   0        0        0      697 2023-07-01 19:46:38.387644 mezcla-1.3.9/tools/local-workflows.sh
+-rwxr-xr-x   0        0        0      862 2023-06-01 22:36:35.000000 mezcla-1.3.9/tools/run_tests.bash
+-rw-r--r--   0        0        0      612 2023-06-01 22:36:35.000000 mezcla-1.3.9/tox.ini
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mezcla-1.3.9/PKG-INFO
```

### Comparing `mezcla-1.3.8/.coveragerc` & `mezcla-1.3.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/.github/workflows/tests.yml` & `mezcla-1.3.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/.gitignore` & `mezcla-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/LICENSE.txt` & `mezcla-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/README.txt` & `mezcla-1.3.9/README.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/__init__.py` & `mezcla-1.3.9/mezcla/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-__VERSION__ = '1.3.8'
+__VERSION__ = '1.3.9'
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
 
 # Note: requires python 3 or higher
 PYTHON3_PLUS = (sys.version_info[0] >= 3)
@@ -42,19 +42,24 @@
 ##     import mezcla
 ##     from mezcla import debug
 ##     from mezcla import system
 ##     TL = debug.TL
 ##     ## DEBUG: debug.trace_expr(TL.DEFAULT, debug, mezcla, system, TL)
 ## else:
 ##     TL = None
-## TODO: drop mezcla
-import mezcla
 from mezcla import debug
 from mezcla import glue_helpers as gh
+from mezcla.my_regex import my_re
 from mezcla import system
 
 # Constants
 TL = debug.TL
 
 # Expose commonly used modules
-# TODO: drop mezcla
-__all__ = ["debug", "gh", "mezcla", "system", "TL"]
+__all__ = ["debug", "gh", "my_re", "system", "TL"]
+
+## OLD:
+## if __name__ == '__main__':
+##     debug.trace(TL.USUAL, f"Version: {__VERSION__}")
+##     system.print_error(f"Warning: {__file__} is not intended to be run standalone\n")
+## NOTE: See https://stackoverflow.com/questions/43393764/python-3-6-project-structure-leads-to-runtimewarning
+debug.trace(TL.DETAILED, f"mezcla version: {__VERSION__}")
```

### Comparing `mezcla-1.3.8/mezcla/analyze_tfidf.py` & `mezcla-1.3.9/mezcla/analyze_tfidf.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     parser.add_argument("--save", default=None, help="Filename to save hash with mapping from docid to related keyword information")
     # TODO: parser.add_argument("filename", nargs='?', default=None, help="Input data")
     parser.add_argument("filename", nargs='?', default="-", help="Input data")
     args = vars(parser.parse_args())
     debug_print("args = %s" % args, 5)
     input_file = sys.stdin
     if (args['filename'] != "-"):
-        input_file = open(args['filename'])
+        input_file = system.open_file(args['filename'])
     verbose_output = args['verbose'] or INCLUDE_CONTEXT
     save_mapping = args['save']
 
     # Read supporting files
     inclusion_keywords = exclusion_keywords = None
     if INCLUSION_FILE:
         inclusion_keywords = tpo.create_boolean_lookup_table(INCLUSION_FILE)
```

### Comparing `mezcla-1.3.8/mezcla/audio.py` & `mezcla-1.3.9/mezcla/audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/bash_ast.py` & `mezcla-1.3.9/mezcla/bash_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/bert_multi_classification.py` & `mezcla-1.3.9/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/bert_text_classification.py` & `mezcla-1.3.9/mezcla/bert_text_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 #   doesn't work with TensorFlow 2.0 and BERT from 2018.
 #
 
 """Run text categorization over input file (or Predict the News Category Hackathon)"""
 
 # Standard packages
 from datetime import datetime
-import hashlib
-import os
+## OLD: import hashlib
+## OLD: import os
 
 # Installed packages
 import pandas as pd
 import tensorflow as tf
 import tensorflow_hub as hub
 from sklearn.model_selection import train_test_split
 # Import BERT modules
```

### Comparing `mezcla-1.3.8/mezcla/bing_search.py` & `mezcla-1.3.9/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/check_html_javascript.py` & `mezcla-1.3.9/mezcla/check_html_javascript.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # (e.g., window) and JQuery ($ selector function). It also optionally runs
 # in strict mode to help check other potential errors (e.g., undefined vars).
 #
 #
 
 """Run JavaScript embedded in <script> tags through lint-style code checkers"""
 
-# Standard packages
+# Standard modules
 from collections import defaultdict
 import re
 import tempfile
 
-# Local packages
+# Local modules
 # TODO: def tomas_import(name): ... components = eval(name).split(); ... import nameN-1.nameN as nameN
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.main import Main
 from mezcla.my_regex import my_re
 from mezcla import system
 
@@ -35,43 +35,52 @@
 TEMP_SUFFIX = system.getenv_text("TEMP_SUFFIX", "-",
                                  "Temporary file suffix (see tempfile.mkstemp)")
 # NOTE: see tempfile.mkstemp for NamedTemporaryFile keyword args
 DEFAULT_TEMP_BASE = tempfile.NamedTemporaryFile(prefix=TEMP_PREFIX, suffix=TEMP_SUFFIX).name
 TEMP_BASE = system.getenv_text("TEMP_BASE", DEFAULT_TEMP_BASE,
                                "Basename with directory for temporary files")
 #
+MAX_ERRORS = system.getenv_int("MAX_ERRORS", 10000,
+                               "Maxmium number of erros to report")
+#
+# note: see DEFAULT_JAVASCRIPT_HEADER below for other options
 JSLINT = "jslint"
-JSLINT_OPTIONS = system.getenv_text("JSLINT_OPTIONS", "--maxerr 10000 --white",
+JSLINT_OPTIONS = system.getenv_text("JSLINT_OPTIONS", f"--maxerr {MAX_ERRORS} --white",
                                     "Options for jslint")
 JSHINT = "jshint"
 JSHINT_OPTIONS = system.getenv_text("JSHINT_OPTIONS", "--show-non-errors",
                                     "Options for jshint")
 DEFAULT_CODE_CHECKERS = system.getenv_text("CODE_CHECKERS",
                                            f"{JSLINT},  {JSHINT}",
                                            "JavaScript code checking commands")
 SAFEMODE_HEADER = """
 'use strict';            // Added for sanity checking (e.g., undefined variables)
 """
 
 # TODO: use separate headers for jslint and jshint
-DEFAULT_JAVASCRIPT_HEADER = """
+DEFAULT_JAVASCRIPT_HEADER = f"""
 // Start of added header (JavaScript and jQuery definitions)
-function $(selector, context) { selector = context; }
+function $(selector, context) {{ selector = context; }}
 var document;
 var window;
 var jQuery;
 
 // Stuff for jslint:
 //    global $, jQuery, alert
 //    jslint browser: true
 //    jslint devel          // Allow console.log() and friends.
 //    jslint long           // Allow long lines.
 //    jslint white          // Allow messy whitespace.
+
+// Stuff for jshint:
+//    jshint maxerr: {MAX_ERRORS}
+
 // End of added header
 """
+# TODO3: add pointer to definition (e.g., https://www.jslint.com)
 
 class Script(Main):
     """Input processing class"""
     # TODO: -or-: """Adhoc script class (e.g., no I/O loop, just run calls)"""
     code_checkers = DEFAULT_CODE_CHECKERS
     strip_indent = False
     skip_safe_mode = False
```

### Comparing `mezcla-1.3.8/mezcla/compute_tfidf.py` & `mezcla-1.3.9/mezcla/compute_tfidf.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,15 @@
     corpus = tfidf_corpus(gramsize=max_ngram_size, min_ngram_size=MIN_NGRAM_SIZE, all_ngrams=False, preprocessor=my_pp)
 
     # Process each of the arguments
     doc_filenames = {}
     for i, filename in enumerate(args):
         # If CSS file, treat each row as separate document, using ID from first column and data from second
         if csv_file:
-            ## TODO: with open(filename, encoding="utf-8") as fh:
-            with open(filename) as fh:
+            with system.open_file(filename) as fh:
                 csv_reader = csv.reader(iter(fh.readlines()), delimiter=DELIMITER, quotechar='"')
                 # TODO: skip over the header line
                 line = 0
                 for row in csv_reader:
                     debug.trace_fmt(6, "{l}: {r}", l=line, r=row)
                     doc_id = row[0]
                     try:
```

### Comparing `mezcla-1.3.8/mezcla/cut.py` & `mezcla-1.3.9/mezcla/cut.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,15 @@
     debug.trace_fmt(4, "Environment options: {eo}",
                     eo=system.formatted_environment_option_descriptions())
     app = Script(
         description=__doc__,
         skip_input=False,
         manual_input=True,
         multiple_files=True,
-        boolean_options=[(CSV, "Comma-separated values (Excel as per csv module)".format(xls=EXCEL_STYLE)),
+        boolean_options=[(CSV, "Comma-separated values ({xls} as per csv module)".format(xls=EXCEL_STYLE)),
                          (TSV, "Tab-separated values"),
                          OUTPUT_CSV, OUTPUT_TSV,
                          (CONVERT_DELIM, "Convert csv to tsv (or vice versa)"),
                          (SNIFFER_ARG, "Detect csv dialect by lookahead (file-input only)"),
                          ## TODO: INPUT_CSV, OUTPUT_CSV, INPUT_TSV, OUTPUT_TSV,
                          (FIX, "Fix up sloppy input (e.g., multiple spaces into tab)--csv fixup not yet supported"),
                          (ALL_FIELDS, "Alternative to {f} option".format(f=FIELDS)),
```

### Comparing `mezcla-1.3.8/mezcla/data_utils.py` & `mezcla-1.3.9/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/debug.py` & `mezcla-1.3.9/mezcla/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,24 @@
 #     debug.trace(TL.USUAL, f"Look ma: TL.VERBOSE={int(TL.VERBOSE)}")
 #
 #   - use DEBUG_LEVEL env. var. to set level
 #
 #     python -c 'from mezcla import debug; debug.trace(debug.DEFAULT + 1, "Not visible")'
 #     DEBUG_LEVEL=3 python -c 'from mezcla import debug; debug.trace(3, "Visible")'
 #
+# TODO1:
+# - Add sanity check to trace_fmt for when keyword in kaargs unused.
+#
 # TODO:
 # - * Add sanity checks for unused environment variables specified on command line (e.g., FUBAR=1 python script.py ...)!
 # - Rename as debug_utils so clear that non-standard package.
 # - Add exception handling throughout (e.g., more in trace_object).
 # - Apply format_value consistently.
 #
+#
 
 """Debugging functions (e.g., tracing)"""
 
 # Standard packages
 import atexit
 from datetime import datetime
 import enum
@@ -241,21 +245,24 @@
 
     def trace_fmtd(level, text, **kwargs):
         """Print TEXT with formatting using optional format KWARGS if at trace LEVEL or higher, including newline"""
         # Note: To avoid interpolated text as being interpreted as variable
         # references, this function does the formatting.
         # TODO: weed out calls that use (level, text.format(...)) rather than (level, text, ...)
         if (trace_level >= level):
+            max_len = kwargs.get('_max_len') or kwargs.get('max_len')
             try:
                 try:
                     # TODO: add version of assertion that doesn't use trace or trace_fmtd
                     ## TODO: assertion(re.search(r"{\S*}", text))
                     ## OLD: assertion("{" in text)
                     ## OLD: trace(level, text.format(**kwargs))
-                    kwargs_unicode = {k: _to_unicode(_to_string(v)) for (k, v) in list(kwargs.items())}
+                    ## OLD: kwargs_unicode = {k: _to_unicode(_to_string(v)) for (k, v) in list(kwargs.items())}
+                    kwargs_unicode = {k: format_value(_to_unicode(_to_string(v)), max_len=max_len)
+                                      for (k, v) in list(kwargs.items())}
                     trace(level, _to_unicode(text).format(**kwargs_unicode))
                 except(KeyError, ValueError, UnicodeEncodeError):
                     raise_exception(max(VERBOSE, level + 1))
                     sys.stderr.write("Warning: Problem in trace_fmtd: {exc}\n".
                                      format(exc=sys.exc_info()))
                     # Show arguments so trace contents recoverable
                     sys.stderr.write("   text=%r\n" % _to_utf8(clip_value(text)))
@@ -343,27 +350,32 @@
                     logging.debug(_to_utf8((indentation + member + ": " + value_spec)))
                 continue
             # Include unless special member (or if no filtering)
             ## DEBUG: trace_expr(QUITE_VERBOSE, member.startswith("__"), re.search(r"^<.*(method|module|function).*>$", value_spec))
             include_member = (show_all or (not (member.startswith("__") or 
                                                 re.search(r"^<.*(method|module|function).*>$", value_spec))))
             # Optionally, process recursively (TODO: make INDENT an env. option)
-            if ((max_depth > 0) and include_member and (not isinstance(value, SIMPLE_TYPES))):
+            is_simple_type = isinstance(value, SIMPLE_TYPES)
+            if ((max_depth > 0) and include_member and (not is_simple_type)):
                 # TODO: add helper for formatting type & address (for use here and above)
                 member_type_id_label = (member + " [" + str(type(value)) + " " + hex(id(value)) + "]")
                 trace_object(level, value, label=member_type_id_label, show_all=show_all,
                              indentation=(indentation + INDENT), pretty_print=None,
                              max_depth=(max_depth - 1), max_value_len=max_value_len,
                              regular_standard=regular_standard)
                 continue
             # Otherwise, derive value spec. (trapping for various exceptions)
             ## TODO: pprint.pprint(member, stream=sys.stderr, indent=4, width=512)
             try:
                 try:
-                    value_spec = format_value("%s" % ((value),), max_len=max_value_len)
+                    ## OLD: value_spec = format_value("%r" % ((value),), max_len=max_value_len)
+                    if is_simple_type and not isinstance(value, str):
+                        value_spec = value
+                    else:
+                        value_spec = format_value("%r" % ((value),), max_len=max_value_len)
                 except(TypeError, ValueError):
                     trace_fmtd(QUITE_VERBOSE, "Warning: Problem in tracing member {m}: {exc}",
                                m=member, exc=sys.exc_info())
                     value_spec = "__n/a__"
             except(AttributeError):
                 # Note: This can occur when profile_function set
                 trace_fmtd(QUITE_VERBOSE, "Error: unexpected problem in trace_object: {exc}",
@@ -426,14 +438,15 @@
 
 
     def trace_expr(level, *values, **kwargs):
         """Trace each of the arguments (if at trace LEVEL or higher), using introspection
         to derive label for each expression. By default, the following format is used:
            expr1=value1; ... exprN=valueN
         Notes:
+        - Warning: introspection fails to resolve expressions if statement split across lines.
         - For simplicity, the values are assumed to separated by ', ' (or expression _SEP)--barebones parsing applied.
         - Use DELIM to specify delimiter; otherwise '; ' used;
           if so, NO_EOL applies to intermediate values (EOL always used at end).
         - Use USE_REPR=False to use tracing via str instead of repr.
         - Use _KW_ARG for KW_ARG in case of conflict, as in following:
           trace_expr(DETAILED, term, _term="; ")
         - Use MAX_LEN to specify maximum value length.
@@ -454,15 +467,15 @@
         in_no_eol = no_eol
         use_repr = kwargs.get('_use_repr') or kwargs.get('use_repr')
         max_len = kwargs.get('_max_len') or kwargs.get('max_len')
         prefix = kwargs.get('_prefix') or kwargs.get('prefix')
         if sep is None:
             sep = ", "
         if no_eol is None:
-            no_eol = (delim == "\n")
+            no_eol = (delim and ("\n" in delim))
         if delim is None:
             delim = "; "
             if in_no_eol is None:
                 no_eol = True
         if use_repr is None:
             use_repr = True
         if prefix is None:
@@ -577,18 +590,17 @@
             raise                       # pylint: disable=misplaced-bare-raise
         return
 
 
     def assertion(expression, message=None, assert_level=None):
         """Issue warning if EXPRESSION doesn't hold, along with optional MESSAGE
         Note:
+        - Warning: introspection fails to resolve expression if split across lines.
         - This is a "soft assertion" that doesn't raise an exception (n.b., provided the test doesn't do so).
-        - Currently, the expression text is not resolved properly under ipython (or Jupyter).
         - The optional ASSERT_LEVEL overrides use of ALWAYS.
-        - Uses introspection to derive text for assertion expression.
         - Returns expression text or None if not triggered.
         """
         # EX: assertion((2 + 2) != 5)
         # TODO: have streamlined version using sys.write that can be used for trace and trace_fmtd sanity checks about {}'s
         # TODO: trace out local and globals to aid in diagnosing assertion failures; ex: add automatic tarcing of variables used in the assertion expression)
         expression_text = None
         if (assert_level is None):
@@ -698,15 +710,17 @@
     ## val = non_debug_stub
     ##
     def val(_expression):
         """Non-debug stub for value()--a no-op function"""
         # Note: implemented separately from non_debug_stub to ensure no return value
         return
     ##
-    assert val(1) is None, "non-debug val() should not return a non-Null value"
+    ## OLD: assert val(1) is None, "non-debug val() should not return a non-Null value"
+    if val(1) is None:
+        system.print_error("Warning: non-debug val() should return Null")
 
 # Aliases for terse functions
     
 cond_code = code
 
 cond_val = val
     
@@ -906,14 +920,15 @@
 # Utility functions useful for debugging (e.g., for trace output)
 
 # TODO: CLIPPED_MAX = system-ish.getenv_int("CLIPPED_MAX", 132)
 CLIPPED_MAX = 132
 #
 def clip_value(value, max_len=CLIPPED_MAX):
     """Return clipped version of VALUE (e.g., first MAX_LEN chars)"""
+    # TODO3: replace with format_value
     # TODO: omit conversion to text if already text [DUH!]
     clipped = "%s" % value
     if (len(clipped) > max_len):
         clipped = clipped[:max_len] + "..."
     return clipped
 
 def read_line(filename, line_number):
@@ -1004,15 +1019,15 @@
     def debug_init():
         """Debug-only initialization"""
         time_start = time.time()
         trace(DETAILED, f"in debug_init(); {timestamp()}")
         # note: shows command invocation unless invoked via "python -c ..."
         command_line = " ".join(sys.argv)
         assertion(command_line)
-        if (command_line and (command_line != "-c")):
+        if (command_line and (command_line != "-c") and (command_line != "-m")):
             trace(USUAL, command_line)
         trace_expr(DETAILED, sys.argv)
         open_debug_file()
 
         # Determine whether tracing include time and date
         global output_timestamps
         ## OLD
@@ -1048,15 +1063,15 @@
         trace_fmt(DETAILED, "{pre}environment: {{\n\t{env}\n}}{post}",
                   env="\n\t".join([(k + ': ' + format_value(os.environ[k]))
                                    for k in sorted(dict(os.environ))]),
                   pre=pre, post=post)
 
         # Likewise show additional information during verbose debug tracing
         # Note: use debug.trace_current_context() in client module to show module-specific globals like __name__
-        trace_expr(VERBOSE, globals(), max_len=65536)
+        trace_expr(MOST_DETAILED, globals(), max_len=65536)
 
         # Register to show shuttdown time and elapsed seconds
         # TODO: rename to reflect generic-exit nature
         def display_ending_time_etc():
             """Display ending time information"""
             # note: does nothing if stderr closed (e.g., other monitor)
             # TODO: resolve pylint issue with sys.stderr.closed
@@ -1082,11 +1097,13 @@
 
     
     # Do the initialization
     debug_init()
 
 #-------------------------------------------------------------------------------
 
+trace_expr(MOST_VERBOSE, 888)
+#
 if __name__ == '__main__':
     main(sys.argv)
 else:
     trace_expr(MOST_VERBOSE, 999)
```

### Comparing `mezcla-1.3.8/mezcla/docs/audio_uml.svg` & `mezcla-1.3.9/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.3.9/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
             feature_data = dataset.data
             target_data = dataset.target
         else:
             dataset_filename = DATASET_NAME if system.file_exists(DATASET_NAME) else (DATASET_NAME + ".csv")
             dataset = du.read_csv(dataset_filename)
             # TODO: add CLASS_POS?
             class_var = CLASS_VAR if CLASS_VAR else dataset.columns[-1]
+            # pylint: disable=no-member
             feature_data = dataset.copy()
             feature_data.drop(class_var, axis=1)
             ## OLD: class_index = list(dataset.columns).index(class_var)
             ## BAD: features_indices = dataset.columns[0:class_index] + dataset.columns[class_index + 1:]
             ## BAD2: features_indices = dataset.columns[0:class_index]
             ## BAD2: features_indices.append(dataset.columns[class_index + 1:])
             ## BAD3: features_indices = pd.concat(dataset.columns[0:class_index], dataset.columns[class_index + 1:])
```

### Comparing `mezcla-1.3.8/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.3.9/mezcla/examples/brownlee_ml_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     # predict probabilities for test set
     if USE_KERAS:
         yhat_probs = model.predict(testX, verbose=0)
     else:
         yhat_probs = model.predict_proba(testX)
     # predict crisp classes for test set
     if USE_KERAS:
+        # pylint: disable=no-member
         yhat_classes = model.predict_classes(testX, verbose=0)
     else:
         yhat_classes = model.predict(testX)
     # reduce to 1d array
     yhat_probs = yhat_probs[:, 0]
     ## BAD: yhat_classes = yhat_classes[:, 0]
     if (len(yhat_classes.shape) > 1):
```

### Comparing `mezcla-1.3.8/mezcla/examples/consume_all_memory.py` & `mezcla-1.3.9/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/download_user_gist.py` & `mezcla-1.3.9/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/dump_checkpoints.py` & `mezcla-1.3.9/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/encoded-iris.csv` & `mezcla-1.3.9/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/feature_importance.py` & `mezcla-1.3.9/mezcla/examples/feature_importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,16 @@
         dataset = np.loadtxt(data_path, delimiter=",", skiprows=1)
         labels = [f"_F{i + 1}" for i in range(dataset.shape[1])]
     else:
         in_dtype = None if not FORCE_FLOAT else np.float64
         dataset = du.read_csv(data_path, delimiter=",", dtype=in_dtype)
         labels = list(dataset.columns)
         if not USE_DATAFRAME:
-            dataset = dataset.values
+            dataset = dataset.values    # pylint: disable=no-member
+
     class_col = (len(labels) - 1)
     class_var = labels[class_col]
     feature_labels = labels[0: class_col]
     debug.trace_expr(5, dataset, labels, class_col, delim='\n')
 
     # split data into X and y
     if USE_DATAFRAME:
```

### Comparing `mezcla-1.3.8/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.3.9/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/hf_stable_diffusion.py` & `mezcla-1.3.9/mezcla/examples/hf_stable_diffusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,33 @@
 # also uses https://huggingface.co/CompVis/stable-diffusion-v1-4
 # and https://stackoverflow.com/questions/48273205/accessing-incoming-post-data-in-flask
 #
 # Note:
 # - For tips on parameter settings, see
 #   https://getimg.ai/guides/interactive-guide-to-stable-diffusion-guidance-scale-parameter
 #
+# TODO:
+# - Set GRADIO_SERVER_NAME to 0.0.0.0?
+#
 
 """Image generation via HF Stable Diffusion (SD) API"""
 
 # Standard modules
 import base64
 import json
 import time
 
 # Installed modules
-
-from datasets import load_dataset
-## NOTE: slows down startup and not needed for client
-## OLD: from diffusers import StableDiffusionPipeline
-## OLD: import flask
+import diskcache
 from flask import Flask, request
-import gradio as gr
 import PIL
 import requests
-import torch
+import gradio as gr
 
 # Local modules
-
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.main import Main
 from mezcla.my_regex import my_re
 from mezcla import system
 
 # Constants/globals
@@ -44,15 +41,15 @@
 PROMPT = system.getenv_text("PROMPT", "your favorite politician in a tutu",
                             "Textual prompt describing image")
 NEGATIVE_PROMPT = system.getenv_text("NEGATIVE_PROMPT", "photo realistic",
                             "Negative tips for image")
 GUIDANCE_SCALE = system.getenv_int("GUIDANCE_SCALE", 7,
                                    "How much the image generation follows the prompt")
 SD_URL = system.getenv_value("SD_URL", None,
-                             "URL for SD TCP/restful server")
+                             "URL for SD TCP/restful serve--new via flask or remote")
 SD_PORT = system.getenv_int("SD_PORT", 9700,
                             "TCP port for SD server")
 SD_DEBUG = system.getenv_int("SD_DEBUG", False,
                              "Run SD server in debug mode")
 USE_HF_API = system.getenv_bool("USE_HF_API", not SD_URL,
                                 "Use Huggingface API instead of TCP server")
 CHECK_UNSAFE = system.getenv_bool("CHECK_UNSAFE", False,
@@ -61,23 +58,33 @@
                                "Number of images to generated")
 BASENAME = system.getenv_text("BASENAME", "sd-app-image",
                               "Basename for saving images")
 LOW_MEMORY = system.getenv_bool("LOW_MEMORY", False,
                                 "Use low memory computations such as via float16")
 DUMMY_RESULT = system.getenv_bool("DUMMY_RESULT", False,
                                   "Mock up SD server result")
+DISK_CACHE = system.getenv_value("SD_DISK_CACHE", None,
+                                 "Path to directory with disk cache")
 
 BATCH_ARG = "batch"
 SERVER_ARG = "server"
 UI_ARG = "UI"
 PORT_ARG = "port"
 PROMPT_ARG = "prompt"
 NEGATIVE_ARG = "negative"
 GUIDANCE_ARG = "guidance"
 
+# Conditional imports for HG/PyTorch
+torch = None
+load_dataset = None
+if USE_HF_API:
+    # pylint: disable=import-outside-toplevel, import-error
+    from datasets import load_dataset
+    import torch
+
 word_list = []
 if CHECK_UNSAFE:
     word_list_dataset = load_dataset("stabilityai/word-list", data_files="list.txt", use_auth_token=True)
     word_list = word_list_dataset["train"]['text']
     debug.trace_expr(5, word_list)
 
 sd_instance = None
@@ -93,35 +100,43 @@
 #-------------------------------------------------------------------------------
 # Main Stable Diffusion support
 
 class StableDiffusion:
     """Class providing Stable Diffusion generative AI (e.g., text-to-image)"""
 
     def __init__(self, use_hf_api=None, server_url=None, server_port=None, low_memory=None):
-        debug.trace(4, f"__init__{(use_hf_api, server_url, server_port)}")
+        debug.trace(4, f"{self.__class__.__name__}.__init__{(use_hf_api, server_url, server_port)}")
         if use_hf_api is None:
             use_hf_api = USE_HF_API
         self.use_hf_api = use_hf_api
         if (server_url is None) and (not self.use_hf_api):
             server_url = SD_URL
         self.server_url = server_url
         if server_port is None:
             server_port = SD_PORT
         if self.server_url and not my_re.search(r"^https?", self.server_url):
+            # note: remote flask server (e.g., on GPU server)
             self.server_url = f"http://{self.server_url}"
             debug.trace(4, f"Added http protocol to URL: {self.server_url}")
         if self.server_url and not my_re.search(r":\d+", self.server_url):
             # TODO3: http://base-url/path => http://base-url:port/path
             self.server_url += f":{server_port}"
         else:
             system.print_stderr(f"Warning: ignoring port {server_port} as already in URL {self.server_url}")
         if low_memory is None:
             low_memory = LOW_MEMORY
         self.low_memory = low_memory
         self.pipe = None
+        self.cache = None
+        if DISK_CACHE:
+            self.cache = diskcache.Cache(
+                DISK_CACHE,                   # path to dir
+                disk=diskcache.core.JSONDisk, # avoid serialization issue
+                disk_compress_level=0,        # no compression
+                cull_limit=0)                 # no automatic pruning
         debug.assertion(bool(self.use_hf_api) != bool(self.server_url))
         debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
     
     def init_pipeline(self):
         """Initialize Stable Diffusion"""
         debug.trace(4, "init_pipeline()")
         # pylint: disable=import-outside-toplevel
@@ -142,31 +157,49 @@
 
     def infer(self, prompt=None, negative_prompt=None, scale=None, num_images=None,
               skip_img_spec=False):
         """Generate images using positive PROMPT and NEGATIVE one, along with guidance SCALE
         Returns list of NUM image specifications in base64 format (e.g., for use in HTML)
         Note: If SKIP_IMG_SPEC specified, result is formatted for HTML IMG tag
         """
-        ## TODO: def infer(prompt, negative_prompt, scale) -> List(PIL.Image.Image):
-        debug.trace(4, f"StableDiffusion.infer{(prompt, negative_prompt, scale, num_images)}")
+        ## OLD: debug.trace(4, f"{self.__class__.__name__}.infer{(prompt, negative_prompt, scale, num_images)}")
+        debug.trace_expr(4, prompt, negative_prompt, scale, num_images, skip_img_spec, prefix=f"in {self.__class__.__name__}.infer:\n\t", delim="\n\t", max_len=1024)
         if num_images is None:
             num_images = NUM_IMAGES
         if scale is None:
             scale = GUIDANCE_SCALE
         for prompt_filter in word_list:
             if my_re.search(rf"\b{prompt_filter}\b", prompt):
                 raise gr.Error("Unsafe content found. Please try again with different prompts.")
     
         images = []
-    
+        params = (prompt, negative_prompt, scale, num_images, skip_img_spec)
+
+        if self.cache is not None:
+            images = self.cache.get(params)
+        if images and len(images) > 0:
+            ## TEST:
+            ## debug.trace_fmt(6, "Using cached result for params {p}: ({r})",
+            ##                 p=params, r=images)
+            debug.trace_fmt(5, "Using cached infer result: ({r})", r=images)
+        else:
+            images = self.infer_non_cached(prompt, negative_prompt, scale, num_images, skip_img_spec)
+            if self.cache is not None:
+                self.cache.set(params, images)
+                debug.trace_fmt(6, "Setting cached result (r={r})", r=images)
+        return images
+            
+    def infer_non_cached(self, prompt, negative_prompt, scale, num_images, skip_img_spec):
+        """Non-cached version of infer"""
+        debug.trace(5, f"{self.__class__.__name__}.infer_non_cached{(prompt, negative_prompt, scale, num_images)}")
+        images = []
         if self.use_hf_api:
-            ## HACK:
             if DUMMY_RESULT:
                 result = ["iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPAgMAAABGuH3ZAAAADFBMVEUAAMzMzP////8AAABGA1scAAAAJUlEQVR4nGNgAAFGQUEowRoa6sCABBZowAgsgBEIGUQCRALAPACMHAOQvR4HGwAAAABJRU5ErkJggg=="]
-                debug.trace(5, f"early exit infer() => {result}")
+                debug.trace(5, f"early exit infer_non_cached() => {result}")
                 return result
 
             if not self.pipe:
                 self.pipe = self.init_pipeline()
             start_time = time.time()
             image_info = self.pipe(prompt, negative_prompt=negative_prompt, guidance_scale=scale,
                                    num_images_per_prompt=num_images)
@@ -178,14 +211,15 @@
                 debug.trace_object(5, image, "image")
                 b64_encoding = image
                 debug.assertion(isinstance(image, PIL.Image.Image))
                 try:
                     image_path = f"{BASENAME}-{i + 1}.png"
                     image.save(image_path)
                     num_generated += 1
+                    # note: "decodes" base-64 encoded bytes object into UTF-8 string
                     b64_encoding = (base64.b64encode(system.read_binary_file(image_path))).decode()
                 except:
                     system.print_exception_info("image-to-base64")
                 images.append(b64_encoding)
             elapsed = round(time.time() - start_time, 3)
             debug.trace(4, f"{elapsed} seconds to generate {num_images} images")
             debug.assertion(num_generated == num_images)
@@ -200,52 +234,42 @@
             debug.trace_expr(5, payload, images_request, images_request.json(), delim="\n")
             for image in images_request.json()["images"]:
                 image_b64 = image
                 if not skip_img_spec:
                     image_b64 = (f"data:image/png;base64,{image_b64}")
                 images.append(image_b64)
         result = images
-        debug.trace(5, f"infer() => {debug.format_value(result)}")
+        debug.trace_fmt(5, "infer_non_cached() => {r}", r=result)
         
         return result
 
 #-------------------------------------------------------------------------------
 # Middleware
 
 @flask_app.route('/', methods=['GET', 'POST'])
 def handle_infer():
     """Process request to do inference to generate image from text"""
-    debug.trace(6, "handle_infer()")
+    debug.trace(6, "[flask_app /] handle_infer()")
     # TODO3: request => flask_request
     debug.trace_object(5, request)
-    ## OLD:
-    ## params = {
-    ##     'prompt': request.values.get('prompt'),
-    ##     'negative_prompt': request.values.get('negative_prompt'),
-    ##     'scale': request.values.get('guidance_scale'),
-    ## }
-    ## params = flask.Request.get_json()
     params = request.get_json()
     debug.trace_expr(5, params)
     images_spec = {"images": sd_instance.infer(**params)}
-    ## OLD: return flask.Response(status=200, mimetype='application/json', response=json.dumps(images_spec))
-    ## BAD: result = flask.Response(status=200, mimetype='application/json', response=images_spec)
-    ## TEST: result = (images_spec, 200)
     # note: see https://stackoverflow.com/questions/45412228/sending-json-and-status-code-with-a-flask-response
     result = (json.dumps(images_spec), 200)
     debug.trace_object(7, result)
-    debug.trace(7, f"handle_infer() => {result}")
+    debug.trace_fmt(7, "handle_infer() => {r}", r=result)
     return result
 
 
 def infer(prompt=None, negative_prompt=None, scale=None, num_images=None, skip_img_spec=None):
     """Wrapper around StableDiffusion.infer()
     Note: intended just for the gradio UI"
     """
-    debug.trace(6, f"infer{(prompt, negative_prompt, scale, skip_img_spec)}")
+    debug.trace(6, f"[sd_instance] infer{(prompt, negative_prompt, scale, skip_img_spec)}")
     return sd_instance.infer(prompt=prompt, negative_prompt=negative_prompt, scale=scale, num_images=num_images, skip_img_spec=skip_img_spec)
 
 #-------------------------------------------------------------------------------
 # User interface
 
 def run_ui():
     """Run user interface via gradio serving by default at localhost:7860
@@ -465,14 +489,15 @@
                     >.</a>
                   </p>
                 </div>
             """
         )
         with gr.Group():
             with gr.Box():
+                ## TODO: drop 'rounded', border, margin, and other options no longer supported (see log)
                 with gr.Row(elem_id="prompt-container").style(mobile_collapse=False, equal_height=True):
                     with gr.Column():
                         prompt_control = gr.Textbox(
                             label="Enter your prompt",
                             show_label=False,
                             max_lines=1,
                             placeholder="Enter your prompt",
@@ -595,25 +620,26 @@
 
     # Invoke UI via HTTP unless in batch mode
     global sd_instance
     sd_instance = StableDiffusion(use_hf_api=server_mode)
     if batch_mode:
         images = infer(prompt, negative_prompt, guidance, skip_img_spec=True)
         for i, image_encoding in enumerate(images):
+            # note: "encodes" UTF-8 text of base-64 encoding as bytes object for str, and then decodes into image bytes
             image_data = base64.decodebytes(image_encoding.encode())
             system.write_binary_file(f"{BASENAME}-{i + 1}.png", image_data)
         # TODO2: get list of files via infer()
         file_spec = " ".join(gh.get_matching_files(f"{BASENAME}*png"))  
         print(f"See {file_spec} for output image(s).")
     elif server_mode:
         debug.assertion(SD_URL)
+        debug.assertion(not sd_instance.server_url)
         debug.trace_object(5, flask_app)
         flask_app.run(host=SD_URL, port=SD_PORT, debug=SD_DEBUG)
     else:
         debug.assertion(ui_mode)
         run_ui()
-    ## OLD: show_gpu_usage()
 
 
 if __name__ == '__main__':
     debug.trace_current_context(level=TL.QUITE_DETAILED)
     main()
```

### Comparing `mezcla-1.3.8/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.3.9/mezcla/examples/hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/hugging_face_translation.py` & `mezcla-1.3.9/mezcla/examples/hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.3.9/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/iris.csv` & `mezcla-1.3.9/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.3.9/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/plot_forest_importances.py` & `mezcla-1.3.9/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.3.9/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 # ---------------------------------
 #
 # Dataset and model
 # .................
 #
 # We will use a Linear SVC classifier to differentiate two types of irises.
 import numpy as np
+import sklearn
 from sklearn.datasets import load_iris
 from sklearn.model_selection import train_test_split
 
 # pylint: disable=ungrouped-imports
 
 from mezcla import debug
 from mezcla import text_utils
```

### Comparing `mezcla-1.3.8/mezcla/examples/template.py` & `mezcla-1.3.9/mezcla/examples/template.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #! /usr/bin/env python
+# TODO: # -*- coding: utf-8 -*-
 #
 # Based on following:
 #   TODO: url
 #
 
 """
 TODO: what module does (brief)
@@ -52,14 +53,17 @@
                     ## TODO: boolean_boolean_options=[(TODO_OPT1, "TODO desc1")]
                     skip_input=False)
     debug.assertion(main_app.parsed_args)
     ## TODO_OPT1 = main_app.get_parsed_option(TODO_OPT1)
 
     ## TODO:
     system.print_error("Error: Implement me!")
+    ## ALT TODO:
+    ## for line in map_app.read_entire_input():
+    ##     print(modify_fn(line))
     return
 
 #-------------------------------------------------------------------------------
 
 if __name__ == '__main__':
-    debug.trace_current_context(level=TL.QUITE_DETAILED)
+    debug.trace_current_context(level=TL.QUITE_VERBOSE)
     main()
```

### Comparing `mezcla-1.3.8/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.3.9/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/examples/tests/test_hf_stable_diffusion.py` & `mezcla-1.3.9/mezcla/examples/tests/test_hf_stable_diffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,26 +90,27 @@
         assert (len(system.intersection(actual, expect)) > 2)
         return
 
     
     @pytest.mark.xfail                   # TODO: remove xfail
     @pytest.mark.skipif(not extcolors, reason="extcolors package missing")
     def test_something_else(self):
-        """TODO: flesh out test for something else"""
+        """Make sure prompted color is used"""
         debug.trace(4, f"TestIt2.test_something_else(); self={self}")
         sd = THE_MODULE.StableDiffusion(use_hf_api=True, low_memory=True)
         images = sd.infer(prompt="a ripe orange", scale=30)
-        image_data = (base64.decodebytes(images[0].encode())).decode()
-        ## OLD: image_path = gh.create_temp_file(image_data)
+        # note: encodes image base-64 str data into bytes and then decodes into image bytes
+        image_data = (base64.decodebytes(images[0].encode()))
         image_path = gh.create_temp_file(image_data, binary=True)
         # note: use of rgb_color_name.py allows for fudge factor
         # $ extcolors sd-app-image-1.png | rgb_color_name.py - | grep orange
         # <(255, 92, 0), orangered>   :  47.07% (123388)
         # <(255, 153, 0), orange>  :   6.13% (16074)
-        output = gh.run(f"extcolors '{image_path}' | rgb_color_name.py -")
+        output = gh.run(f"extcolors '{image_path}' | rgb_color_name.py - 2> /dev/null")
+        debug.trace_expr(4, output)
         assert ("orange" in output)
         assert (len(images) == 1)
         return
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
```

### Comparing `mezcla-1.3.8/mezcla/examples/tracemalloc_display.py` & `mezcla-1.3.9/mezcla/examples/tracemalloc_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                                    "File with word list")
 
 class TraceMalloc:
     """Wrapper class around tracemalloc"""
 
     def __init__(self, limit=None):
         """Class intiializer"""
-        debug.trace(4, f"TraceMalloc.__init__()")
+        debug.trace(4, "TraceMalloc.__init__()")
         self.snapshot = None
         self.limit = limit
         tracemalloc.start()
     
     
     def display_top(self, key_type=None, limit=None):
         """Show top usages"""
@@ -71,15 +71,15 @@
 
     def take_snapshot(self):
         """Take snapshot or memory usage"""
         self.snapshot = tracemalloc.take_snapshot()
     
     def display(self, limit=None):
         """Display current snapshot"""
-        debug.trace(3, f"TraceMalloc.display()")
+        debug.trace(3, "TraceMalloc.display()")
 
         if not self.snapshot:
             self.take_snapshot()
         self.display_top(limit=limit)
 
 #-------------------------------------------------------------------------------
         
@@ -91,15 +91,15 @@
     dummy_app = Main(description=__doc__, skip_input=False, manual_input=False)
     debug.assertion(dummy_app.parsed_args)
 
     trace_malloc = TraceMalloc(limit=NUM_ITEMS)
     
     counts = Counter()
     fname = WORDLIST_FILE
-    with open(fname) as wordlist_file:
+    with system.open_file(fname) as wordlist_file:
         words = list(wordlist_file)
         for word in words:
             prefix = word[:PREFIX_LEN]
             counts[prefix] += 1
     print('Top prefixes:', counts.most_common(3))
 
     trace_malloc.display()
```

### Comparing `mezcla-1.3.8/mezcla/extract_document_text.py` & `mezcla-1.3.9/mezcla/extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/file_utils.py` & `mezcla-1.3.9/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/filter_random.py` & `mezcla-1.3.9/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/format_profile.py` & `mezcla-1.3.9/mezcla/format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/gensim_test.py` & `mezcla-1.3.9/mezcla/gensim_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 import sys
 import tempfile
 
 # Installed packages
 from gensim import corpora, models, similarities
 
 # Local packages
-import mezcla.system as system
+from mezcla import system
 import mezcla.tpo_common as tpo
-import mezcla.debug as debug
+from mezcla import debug
 import mezcla.glue_helpers as gh
 
 # Environment options
 # Note: These are for internal options not intended for end users (e.g., for default values).
 # This also allows for defining options in one place rather than say 3+ for argparse.
 # TODO: XYZ => DEFAULT_XYZ
 MAX_SIMILAR = tpo.getenv_integer("MAX_SIMILAR", 10)
@@ -401,15 +401,15 @@
 def create_ordered_lookup_table(filename):
     """Create lookup hash table from 0-based line number as string to labels specified in FILENAME
     Note: case is preserved but leading and trailing whitespace is removed"""
     tpo.debug_print("create_ordered_lookup_table(%s)" % filename, 5)
     lookup_hash = OrderedDict()
     f = None
     try:
-        f = open(filename)
+        f = system.open_file(filename)
         line_num = 0
         for line in f:
             lookup_hash[str(line_num)] = line.strip()
             line_num += 1
     except (IOError, ValueError):
         tpo.debug_print("Warning: Exception creating lookup table from %s: %s" % (filename, str(sys.exc_info())), 2)
     finally:
@@ -645,7 +645,10 @@
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     ## OLD:
     main()
     ## TODO: main(sys.argv)
+
+## TEST (for testing tests/test_gensim_test.py conditional loading):
+## fubar
```

### Comparing `mezcla-1.3.8/mezcla/glue_helpers.py` & `mezcla-1.3.9/mezcla/glue_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,27 +58,35 @@
 FILE_BASE = system.getenv_text("FILE_BASE", "_temp",
                                "Basename for output files including dir")
 TEMP_PREFIX = (FILE_BASE + "-")
 NTF_ARGS = {'prefix': TEMP_PREFIX,
             'delete': not debug.detailed_debugging(),
             ## TODO: 'suffix': "-"
             }
-TEMP_FILE = system.getenv_text("TEMP_FILE", tempfile.NamedTemporaryFile(**NTF_ARGS).name,
-                               description="Basename for temporary files")
+USE_TEMP_BASE_DIR = system.getenv_bool("USE_TEMP_BASE_DIR", False,
+                                       "Whether TEMP_BASE should be a dir instead of prefix")
+TEMP_BASE = system.getenv_value("TEMP_BASE", None,
+                                "Override for temporary file basename")
+TEMP_FILE_DEFAULT = None
+if TEMP_BASE:
+    TEMP_FILENAME = "temp-file.list"
+    TEMP_FILE_DEFAULT = (form_path(TEMP_BASE, TEMP_FILENAME) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{TEMP_FILENAME}")
+TEMP_FILE = system.getenv_value("TEMP_FILE", TEMP_FILE_DEFAULT,
+                                "Override for temporary filename")
 
 
 #------------------------------------------------------------------------
 
 def get_temp_file(delete=None):
     """Return name of unique temporary file, optionally with DELETE"""
     # Note: delete defaults to False if detailed debugging
     # TODO: allow for overriding other options to NamedTemporaryFile
     if ((delete is None) and tpo.detailed_debugging()):
         delete = False
-    temp_file_name = TEMP_FILE
+    temp_file_name = (TEMP_FILE or tempfile.NamedTemporaryFile(**NTF_ARGS).name)
     debug.assertion(not delete, "Support for delete not implemented")
     debug_format("get_temp_file() => {r}", 5, r=temp_file_name)
     return temp_file_name
 #
 TEMP_LOG_FILE = tpo.getenv_text("TEMP_LOG_FILE", get_temp_file() + "-log",
                                 "Log file for stderr such as for issue function")
 TEMP_SCRIPT_FILE = tpo.getenv_text("TEMP_SCRIPT_FILE", get_temp_file() + "-script",
@@ -181,16 +189,18 @@
     debug_format("resolve_path({f}) => {p}", 4, f=filename, p=path)
     return path
 
 
 def form_path(*filenames):
     """Wrapper around os.path.join over FILENAMEs (with tracing)
     Note: includes sanity check about absolute filenames except for first
+    Warning: This will be deprecated: uses system.form_path instead.
     """
-    debug.assertion(not any(f.startswith(os.path.sep) for f in filenames[1:]))
+    ## TODO3: return system.form_path(*filenames)
+    debug.assertion(not any(f.startswith(system.path_separator()) for f in filenames[1:]))
     path = os.path.join(*filenames)
     debug_format("form_path{f} => {p}", 6, f=tuple(filenames), p=path)
     return path
 
 
 def is_directory(path):
     """Determins wther PATH represents a directory"""
@@ -306,17 +316,18 @@
     default_subtrace_level = 0
 
 
 def run(command, trace_level=4, subtrace_level=None, just_issue=False, **namespace):
     """Invokes COMMAND via system shell, using TRACE_LEVEL for debugging output, returning result. The command can use format-style templates, resolved from caller's namespace. The optional SUBTRACE_LEVEL sets tracing for invoked commands (default is same as TRACE_LEVEL); this works around problem with stderr not being separated, which can be a problem when tracing unit tests.
    Notes:
    - The result includes stderr, so direct if not desired (see issue):
-         gh.run("ls /tmp/fubar 2> /dev/null")
+         run("ls /tmp/fubar 2> /dev/null")
    - This is only intended for running simple commands. It would be better to create a subprocess for any complex interactions.
    - This function doesn't work fully under Win32. Tabs are not preserved, so redirect stdout to a file if needed.
+   - If TEMP_FILE or TEMP_BASE defined, these are modified to be unique to avoid conflicts across processeses.
    """
     # TODO: add automatic log file support as in run_script from unittest_wrapper.py
     # TODO: make sure no template markers left in command text (e.g., "tar cvfz {tar_file}")
     # EX: "root" in run("ls /")
     # Note: Script tracing controlled DEBUG_LEVEL environment variable.
     debug.assertion(isinstance(trace_level, int))
     debug_print("run(%s, [trace_level=%s], [subtrace_level=%s])" % (command, trace_level, subtrace_level), (trace_level + 2))
@@ -324,14 +335,20 @@
     # Keep track of current debug level setting
     debug_level_env = None
     if subtrace_level is None:
         subtrace_level = default_subtrace_level
     if subtrace_level != trace_level:
         debug_level_env = os.getenv("DEBUG_LEVEL")
         setenv("DEBUG_LEVEL", str(subtrace_level))
+    save_temp_base = TEMP_BASE
+    if TEMP_BASE:
+         setenv("TEMP_BASE", TEMP_BASE + "_subprocess_")
+    save_temp_file = TEMP_FILE
+    if TEMP_FILE:
+        setenv("TEMP_FILE", TEMP_FILE + "_subprocess_")
     # Expand the command template
     # TODO: make this optional
     command_line = command
     if re.search("{.*}", command):
         command_line = tpo.format(command_line, indirect_caller=True, ignore_exception=False, **namespace)
     debug_print("issuing: %s" % command_line, trace_level)
     # Run the command
@@ -345,14 +362,18 @@
     debug.assertion(">|" not in command_line)
     result = None
     ## TODO: if (just_issue or not wait): ... else: ...
     result = getoutput(command_line) if wait else str(os.system(command_line))
     # Restore debug level setting in environment
     if debug_level_env:
         setenv("DEBUG_LEVEL", debug_level_env)
+    if save_temp_base:
+        setenv("TEMP_BASE", save_temp_base)
+    if save_temp_file:
+        setenv("TEMP_FILE", save_temp_file)
     debug_print("run(_) => {\n%s\n}" % indent_lines(result), (trace_level + 1))
     return result
 
 
 def run_via_bash(command, trace_level=4, subtrace_level=None, init_file=None,
                  enable_aliases=False,
                  **namespace):
@@ -440,16 +461,15 @@
     # Note: modelled after extract_matches.perl
     # TODO: make multiple the default
     debug_print("extract_matches(%s, _, [fld=%s], [m=%s], [flg=%s], [para=%s])" % (pattern, fields, multiple, re_flags, para_mode), 6)
     ## TODO
     ## if re_flags is None:
     ##     re_flags = re.DOTALL
     debug.trace_values(6, lines, "lines")
-    ## assert type(lines) == list
-    assert isinstance(lines, list)
+    debug.assertion(isinstance(lines, list))
     if pattern.find("(") == -1:
         pattern = "(" + pattern + ")"
     if (re_flags and (re_flags & re.DOTALL)):
         lines = [ "\n".join(lines) + "\n" ]
         debug.trace_expr(6, lines)
     if para_mode:
         lines = re.split(r"\n\s*\n", ("\n".join(lines)))
```

### Comparing `mezcla-1.3.8/mezcla/html_utils.py` & `mezcla-1.3.9/mezcla/html_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -263,14 +263,15 @@
     result = (param_dict if (param_dict is not None) else user_parameters)
     debug.trace(7, f"get_param_dict([pd={param_dict}]) => {result}")
     return result
 
 
 def set_param_dict(param_dict):
     """Sets global user_parameters to value of PARAM_DICT"""
+    # EX: set_param_dict({"param1": "a+b+c", "param2": "a%2Bb%2Bc"}); len(user_parameters) => 2
     debug.trace(7, f"set_param_dict({param_dict})")
     global issued_param_dict_warning
     global user_parameters
 
     # Make update, issuing warning if first time
     if not issued_param_dict_warning:
         issued_param_dict_warning = True
@@ -284,24 +285,38 @@
     if default_value is None:
         default_value = ""
     param_dict = (get_param_dict(param_dict) or {})
     value = param_dict.get(name, default_value)
     value = system.to_unicode(value)
     if escaped:
         value = escape_html_value(value)
-    debug.trace_fmtd(4, "get_url_param({n}, [{d}]) => {v})",
-                     n=name, d=default_value, v=value)
+    debug.trace_fmt(5, "get_url_param({n}, [{d}]) => {v})",
+                    n=name, d=default_value, v=value)
     return value
 #
 get_url_parameter = get_url_param
 
 
+def get_url_text(name, param_dict=None):
+    """Get TEXT value for URL encoded parameter, using current PARAM_DICT"""
+    # EX: get_url_text("param1") => "a b c"
+    encoded_vaue = get_url_parameter(name, param_dict)
+    value = unescape_html_value(system.unquote_url_text(encoded_vaue))
+    debug.trace_fmt(6, "get_url_text({n}, [d={d}]) => {v})",
+                    n=name, d=param_dict, v=value)
+    return value
+#
+# EX: get_url_text("param2") => "a b c"
+   
+
 def get_url_param_checkbox_spec(name, default_value="", param_dict=None):
     """Get value of boolean parameters formatted for checkbox (i.e., 'checked' iff True or on) from PARAM_DICT
     Note: the value is only specified/submitted if checked"""
+    # EX: get_url_param_checkbox_spec("param", param_dict={"param": "on"}) => "checked"
+    # EX: get_url_param_checkbox_spec("param", param_dict={"param": "off"}) => ""
     # NOTE: 1 also treated as True
     # TODO: implement in terms of get_url_param
     param_dict = (get_param_dict(param_dict) or {})
     param_value = param_dict.get(name, default_value)
     param_value = system.to_unicode(param_value)
     ## OLD: value = "checked" if (param_value in [True, "on"]) else ""
     value = "checked" if (param_value in ["1", "on", True]) else ""
@@ -640,14 +655,45 @@
             link_src = web_site_url + link_src
         elif base_url and not link_src.startswith("http"):
             link_src = base_url + "/" + link_src
         links.append(link_src)
     debug.trace_fmtd(6, "extract_html_links() => {i}", i=links)
     return links
 
+
+def format_checkbox(param_name, label=None, default_value=False, disabled=False):
+    """Returns HTML specification for input checkbox
+    Warning: includes separate hidden field for explicit off state"""
+    ## Note: Checkbox valuee are only submitted if checked, so a hidden field is used to provide explicit off.
+    ## This requires use of html_utils.fix_url_parameters to give preference to final value specified (see results.mako).
+    ## See https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/checkbox for hidden field tip.
+    ## Also see https://stackoverflow.com/questions/155291/can-html-checkboxes-be-set-to-readonly
+    ## EX: format_checkbox("disable-touch") => '<label>Disable touch? <input id="disable-touch" type="checkbox" name="disable-touch" ></label>&nbsp;"'
+    ## EX: format_checkbox("disable-touch", disabled=True) => '<label>Disable touch? <input id="disable-touch" type="checkbox" name="disable-touch" disabled></label>&nbsp;"'
+    checkbox_spec = get_url_param_checkbox_spec(param_name, default_value)
+    disabled_spec = ("disabled" if disabled else "")
+    status_spec = f"{checkbox_spec} {disabled_spec}".strip()
+    if (label is None):
+        label = (param_name.replace("-", " ").capitalize() + "?")
+    result = ""
+    ## TODO: use hidden only if (default_value in ["1", "on", True])???
+    result = f"<input type='hidden' name='{param_name}' value='off'>"
+    result += f"<label>{label} <input type='checkbox' id='{param_name}-id' name='{param_name}' {status_spec}></label>&nbsp;"
+    debug.trace(6, f"format_checkbox({param_name}, [def={default_value}]) => {result}")
+    return result
+
+def format_url_param(name):
+    """Return URL parameter NAME formatted for an HTML form (e.g., escaped)"""
+    # EX: html_utils.set_param_dict({"q": '"hot dog"'}); format_url_param("q") => '&quot;hot dog&quot;'
+    value_spec = (get_url_param(name) or "")
+    if value_spec:
+        value_spec = system.escape_html_text(value_spec)
+    debug.trace(5, f"format_url_param({name}) => {value_spec!r}")
+    return value_spec
+
 #-------------------------------------------------------------------------------
 
 def main(args):
     """Supporting code for command-line processing"""
     debug.trace_fmtd(6, "main({a})", a=args)
     user = system.getenv_text("USER")
     system.print_stderr("Warning, {u}: this is not intended for direct invocation".format(u=user))
```

### Comparing `mezcla-1.3.8/mezcla/kenlm_example.py` & `mezcla-1.3.9/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/keras_param_search.py` & `mezcla-1.3.9/mezcla/keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/main.py` & `mezcla-1.3.9/mezcla/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,28 @@
 PERL_SWITCH_PARSING = system.getenv_bool("PERL_SWITCH_PARSING", False,
                                          "Preprocess args to expand Perl-style -var[=[val=1]] to --var=val")
 ## HACK: This is needed if boolean options default to true based on run-time initialization
 NEGATIVE_BOOL_ARGS = system.getenv_bool("NEGATIVE_BOOL_ARGS", False,
                                         "Add negation option for each boolean option")
 SHORT_OPTIONS = system.getenv_bool("SHORT_OPTIONS", False,
                                    "Automatically derive short options")
+## TEST
+## TEMP_BASE = system.getenv_value("TEMP_BASE", None,
+##                                 "Override for temporary file basename")
+TEMP_BASE = gh.TEMP_BASE
+## OLD:
+## USE_TEMP_BASE_DIR = system.getenv_bool("USE_TEMP_BASE_DIR", False,
+##                                        "Whether TEMP_BASE should be a dir instead of prefix")
+USE_TEMP_BASE_DIR = gh.USE_TEMP_BASE_DIR
+## TEST
+## TEMP_FILE = system.getenv_value("TEMP_FILE", None,
+##                                 "Override for temporary filename")
+TEMP_FILE = gh.TEMP_FILE
+KEEP_TEMP_FILES = system.getenv_bool("KEEP_TEMP_FILES", debug.detailed_debugging(),
+                                     "Retain temporary files")
 
 #-------------------------------------------------------------------------------
 
 class Main(object):
     """Class encompassing common script processing"""
     argument_parser = None
     force_unicode = False
@@ -219,60 +233,59 @@
             track_pages = TRACK_PAGES
         self.track_pages = track_pages
         self.short_options = (short_options if (short_options is not None) else SHORT_OPTIONS)
 
         # Check miscellaneous options
         BINARY_INPUT_OPTION = "binary_input"
         PERL_SWITCH_PARSING_OPTION = "perl_switch_parsing"
-        debug.assertion(not (system.difference(kwargs.keys(), [BINARY_INPUT_OPTION, PERL_SWITCH_PARSING_OPTION])))
+        bad_options = system.difference(kwargs.keys(), [BINARY_INPUT_OPTION, PERL_SWITCH_PARSING_OPTION])
+        debug.assertion(not bad_options, f"Extraneous kwargs: {bad_options}")
         self.binary_input = kwargs.get(BINARY_INPUT_OPTION, False)
 
         # Setup temporary file and/or base directory
         # Note: Uses NamedTemporaryFile (hence ntf_args)
         # TODO: allow temp_base handling to be overridable by constructor options
         # TODO: reconcile with unittest_wrapper.py.get_temp_dir
         prefix = (FILE_BASE + "-")
         ntf_args = {"prefix": prefix,
                     "delete": not debug.detailed_debugging(),
                     ## TODO: "suffix": "-"
                     }
-        self.temp_base = system.getenv_text("TEMP_BASE",
-                                            tempfile.NamedTemporaryFile(**ntf_args).name)
+        self.temp_base = (TEMP_BASE or tempfile.NamedTemporaryFile(**ntf_args).name)
         # TODO: self.use_temp_base_dir = gh.dir_exists(gh.basename(self.temp_base))
         # -or-: temp_base_dir = system.getenv_text("TEMP_BASE_DIR", " "); self.use_temp_base_dir = bool(temp_base_dir.strip()); ...
         if use_temp_base_dir is None:
-            use_temp_base_dir = system.getenv_bool("USE_TEMP_BASE_DIR", False)
+            use_temp_base_dir = USE_TEMP_BASE_DIR
         self.use_temp_base_dir = use_temp_base_dir
         if self.use_temp_base_dir:
             ## TODO: gh.full_mkdir
             ## TEMP HACK: remove file if not a dir (n.b., quirk with NamedTemporaryFile
             if system.is_regular_file(self.temp_base):
                 gh.delete_file(self.temp_base)
             gh.run("mkdir -p {dir}", dir=self.temp_base)
             default_temp_file = gh.form_path(self.temp_base, "temp.txt")
         else:
             default_temp_file = self.temp_base
-        self.temp_file = system.getenv_text("TEMP_FILE", default_temp_file)
+        self.temp_file = (TEMP_FILE or default_temp_file)
 
-        # Get arguments from specified parameter or via command line
         # Note: --help assumed for input-less scripts with command line options
         # to avoid inadvertent script processing.
         #
         if ((runtime_args is None) and (not skip_args)):
             runtime_args = sys.argv[1:]
             debug.trace(4, f"Using sys.argv[1:] for runtime args: {runtime_args}")
             if self.auto_help and not runtime_args:
                 help_arg = (USAGE_ARG if self.brief_usage else HELP_ARG)
                 debug.trace(4, f"FYI: Adding {help_arg} to command line (as per auto_help)")
                 runtime_args = [help_arg]
         #
         # Process special hook for converting Perl-style switches like -fu=123 to --fu=123
         # See -s option under perlrun man page for enabling this rudimentary switch parsing.
         # Note: mainly just intended for when porting Perl scripts.
-        self.perl_switch_parsing = kwargs.get("perl_switch_parsing", PERL_SWITCH_PARSING)
+        self.perl_switch_parsing = kwargs.get(PERL_SWITCH_PARSING_OPTION, PERL_SWITCH_PARSING)
         if self.perl_switch_parsing and runtime_args:
             debug.trace(4, "FYI: Enabling Perl-style options")
             debug.assertion(not re.search(r"--\w+", " ".join(runtime_args)),
                             "Shouldn't use Python arguments with PERL_SWITCH_PARSING")
             for i, arg in enumerate(runtime_args):
                 if arg in ["-", "--"]:
                     break
@@ -855,18 +868,26 @@
         tpo.debug_format("Main.wrap_up() stub: self={s}", 5, s=self)
         return
 
     def clean_up(self):
         """Removes temporary files, etc."""
         # note: not intended to be overridden
         tpo.debug_format("Main.clean_up(): self={s}", 5, s=self)
-        if not tpo.detailed_debugging():
+        if not KEEP_TEMP_FILES:
+            ## TODO2: 3=>6
+            debug.trace_fmt(3, "Deleting any temporary files: {files}",
+                            files=gh.run(f"echo {self.temp_base}* {self.temp_file}* | sort -u"))
+                                
+            # Remove all temp_base* files (or the temp_base directory)
             if self.use_temp_base_dir:
                 gh.run("rm -rvf {dir}", dir=self.temp_base)
             else:
+                gh.run("rm -vf {file}*", file=self.temp_base)
+            # Likewise remove all temp_file* files
+            if (self.temp_file != self.temp_base):
                 gh.run("rm -vf {file}*", file=self.temp_file)
         return
 
 #-------------------------------------------------------------------------------
 # Global instance for convenient adhoc usage
 # 
 # note: useful for temporary file support (e.g., dummy_app.temp_file)
```

### Comparing `mezcla-1.3.8/mezcla/merge_files.py` & `mezcla-1.3.9/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/merge_notes.py` & `mezcla-1.3.9/mezcla/merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/misc_utils.py` & `mezcla-1.3.9/mezcla/misc_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     debug.trace_fmtd(4, "read_tabular_file({f})", f=filename)
     table = {}
     with system.open_file(filename) as f:
         for (i, line) in enumerate(f):
             line = system.from_utf8(line)
             items = line.split("\t")
             if len(items) == 2:
-                assert(items[0].lower() not in table)
+                debug.assertion(items[0].lower() not in table)
                 table[items[0].lower()] = items[1]
             else:
                 debug.trace_fmtd(4, "Ignoring item w/ unexpected format at line {num}",
                                  num=(i + 1))
     ## debug.trace_fmtd(7, "table={t}", t=table)
     debug.trace_values(7, table, "table")
     return table
@@ -97,15 +97,15 @@
     if (num <= 3):
         is_prime_num = (num > 1)
         if not is_prime_num:
             debug.trace_fmt(4, "{n} not prime as less than 3 and not 2.", n=num)
         return is_prime_num
 
     # Next, make sure not divisible by 2 or 3
-    elif ((num % 2 == 0) or (num % 3 == 0)):
+    if ((num % 2 == 0) or (num % 3 == 0)):
         debug.trace_fmt(4, "{n} not prime as divisible by 2 or 3.", n=num)
         return False
 
     # Otherwise, check (6k +/- 1) values to see if divisible by 2 or 3,
     # stopping when value exceeds sqrt(n).
     last_possible = math.ceil(math.sqrt(num))
     i = 5
```

### Comparing `mezcla-1.3.8/mezcla/my_regex.py` & `mezcla-1.3.9/mezcla/my_regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,25 +118,29 @@
             system.print_exception_info("__init__ re.* importation")
 
     def check_pattern(self, regex):
         """Apply sanity checks to REGEX when debugging
         Note: Added to account for potential f-string confusion"""
         # TODO: Add way to disable check
         debug.reference_var(self)
-        if (debug.debugging(1) and re.search(r"[^{]\{[A-Fa-f0-9][^{}]+\}[^}]", regex)):
+        check_regex = r"[^{]\{[A-Fa-f0-9][^{}]+\}[^}]"
+        if isinstance(regex, bytes):
+            check_regex = check_regex.encode()
+        if (debug.debugging(1) and re.search(check_regex, regex)):
             system.print_error(f"Warning: potentially unresolved f-string in {regex}")
 
     def search(self, regex, text, flags=0, base_trace_level=None):
         """Search for REGEX in TEXT with optional FLAGS and BASE_TRACE_LEVEL (e.g., 6)"""
         ## TODO: rename as match_anywhere for clarity
         if base_trace_level is None:
             base_trace_level = self.TRACE_LEVEL
         debug.trace_fmtd((1 + base_trace_level), "my_regex.search({r!r}, {t!r}, {f}): self={s}",
                          r=regex, t=text, f=flags, s=self)
-        debug.assertion(isinstance(text, six.string_types))
+        ## OLD: debug.assertion(isinstance(text, six.string_types))
+        debug.assertion(isinstance(text, (str, bytes)) and (type(regex) == type(text)))
         self.check_pattern(regex)
         self.match_result = re.search(regex, text, flags)
         if self.match_result:
             debug.trace_fmt(base_trace_level, "match: {m!r}; regex: {r!r}", m=self.grouping(), r=regex)
         return self.match_result
 
     def match(self, regex, text, flags=0, base_trace_level=None):
```

### Comparing `mezcla-1.3.8/mezcla/ngram_tfidf.py` & `mezcla-1.3.9/mezcla/ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/os_utils.py` & `mezcla-1.3.9/mezcla/os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/pandas_sklearn.py` & `mezcla-1.3.9/mezcla/pandas_sklearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,15 @@
         system.print_exception_info("du.read_csv")
         debug.trace(3, "Using pandas read_csv directly as fallback")
         dataset = pd.read_csv(data_file, sep=FIELD_SEP)
 
     # Reorder columns so classication variable last
     if (CLASS_VAR and (CLASS_VAR != dataset.columns[-1])):
         debug.trace_fmtd(4, "Re-arranging columns")
+        # pylint: disable=no-member
         columns = system.difference(list(dataset.columns), CLASS_VAR)
         columns.append(CLASS_VAR)
         dataset = dataset[columns]
 
     # Show features proper and classificaiton variable
     feature_names = list(dataset.columns[0:-1])
     class_var = dataset.columns[-1]
@@ -321,14 +322,15 @@
         X = dataset[features_indices[0:num_features]]
         y = dataset[features_indices[num_features]]
         if COERCE_FLOAT:
             X = X.astype(np.float64)
         if NUMERIC_CLASSES:
             y = y.astype(np.float64)
     else:
+        # pylint: disable=no-member
         array = dataset.values
         debug.trace_object(7, array, "array")
         num_features = (array.shape[1] - 1)
         X = array[:, 0:num_features]
         y = array[:, num_features]
         # TODO: COERCE_FLOAT
         # TODO: NUMERIC_CLASSES
```

### Comparing `mezcla-1.3.8/mezcla/plot_utils.py` & `mezcla-1.3.9/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/randomize_lines.py` & `mezcla-1.3.9/mezcla/randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/rgb_color_name.py` & `mezcla-1.3.9/mezcla/rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/run_albert_classifier.py` & `mezcla-1.3.9/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/run_bert_classifier.py` & `mezcla-1.3.9/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/show_bert_representation.py` & `mezcla-1.3.9/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/simple_main_example.py` & `mezcla-1.3.9/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/spacy_nlp.py` & `mezcla-1.3.9/mezcla/spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/spell.py` & `mezcla-1.3.9/mezcla/spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/sys_version_info_hack.py` & `mezcla-1.3.9/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/system.py` & `mezcla-1.3.9/mezcla/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,42 +13,48 @@
 # - Reconcile against functions in tpo_common.py (e.g., to make sure functionality covered and similar tracing supported).
 # - Make sure format-based function tracing is well formed:
 #   ex: "is_dir{p}" => "is_dir({p})".
 # - ** Define generic function for creating simple wrappers:
 #   ex: def fu(): r = sys.fu(); trace(N, f"fub() returned {r}"); return r
 #       => fu = define_wrapper(trace_level=N, sys.fu)
 #
+# TODO2:
+# - convert additional open() calls to open_file()
+# - drop python 2 support
+#
 
 """System-related functions"""
 
 # Standard packages
 from collections import defaultdict, OrderedDict
 import datetime
 import inspect
 import os
 import pickle
 import re
-import six
 import sys
 import time
-## OLD: import urllib
 
 # Installed packages
-## OLD: import requests
+import six
 
 # Local packages
 from mezcla import debug
 from mezcla.debug import UTF8
 
 # Constants
 STRING_TYPES = six.string_types
 MAX_SIZE = six.MAXSIZE
 MAX_INT = MAX_SIZE
 TEMP_DIR = None
 
+## TODO: debug.assertion(python_maj_min_version() >= 3.8, "Require Python 3.8+ for function def's with '/' or '*'")
+## See https://stackoverflow.com/questions/9079036/how-do-i-detect-the-python-version-at-runtime
+debug.assertion(sys.version_info >= (3, 8), "Require Python 3.8+ for function def's with '/' or '*'")
+
 #-------------------------------------------------------------------------------
 # Support for needless python changes
 
 def maxint():
     """Maximum size for an integer"""
     # Note: this is just a sanity check
     debug.assertion(MAX_INT == MAX_SIZE)
@@ -61,28 +67,25 @@
 env_options = {}
 env_defaults = {}
 #
 def register_env_option(var, description, default):
     """Register environment VAR as option with DESCRIPTION and DEFAULT"""
     # Note: The default value is typically the default value passes into the
     # getenv_xyz call, not the current value from the environment.
-    ## OLD: debug.trace_fmt(7, "register_env_option({v}, {d})", v=var, d=description)
     debug.trace_fmt(7, "register_env_option({v}, {dsc}, {dft})",
                     v=var, dsc=description, dft=default)
     global env_options
     global env_defaults
-    ## OLD: env_options[var] = (description or "")
     env_options[var] = description
     env_defaults[var] = default
     return
 
 
 def get_registered_env_options():
     """Returns list of environment options registered via register_env_option"""
-    ## OLD: option_names = [k for k in env_options if (env_options[k] and env_options[k].strip())]
     ## TEMP
     # pylint: disable=consider-using-dict-items
     option_names = [k for k in env_options if (env_options[k] is not None)]
     debug.trace_fmt(5, "get_registered_env_options() => {on}", on=option_names)
     return option_names
 
 
@@ -101,15 +104,14 @@
         include_default = True
     if not include_default:
         indent = ''
     #
     def _format_env_option(opt):
         """Returns OPT description and optionally default value (if INCLUDE_DEFAULT)"""
         debug.trace_fmt(7, "_format_env_option({o})", o=opt)
-        ## OLD: desc_spec = env_options.get(opt, "_")
         ## TEST: Uses unicode O-with-stoke (U+00D8) to indicate n/a
         ## TEMP: desc_spec = to_text(env_options.get(opt))
         env_desc = env_options.get(opt)
         ## TEST: desc_spec = ("\u00D8 " if (env_options.get(opt) is None) else env_desc)
         desc_spec = ("n/a" if (env_options.get(opt) is None) else env_desc)
         default_spec = ""
         if include_default:
@@ -159,15 +161,14 @@
     # Note: default is empty string to ensure result is string (not NoneType)
     ## TODO: add way to block registration
     register_env_option(var, description, default)
     if default is None:
         debug.trace(4, f"Warning: getenv_text treats default None as ''; consider using getenv_value for '{var}' instead")
         default = ""
     text_value = os.getenv(var)
-    ## OLD: if not text_value:
     ## TODO?: if ((not helper and (text_value is None)) or (not text_value)):
     if (text_value is None):
         debug.trace_fmtd(6, "getenv_text: no value for var {v}", v=var)
         text_value = default
     trace_level = 6 if helper else 5
     ## DEBUG: sys.stderr.write("debug.trace_fmtd({trace_level} \"getenv_text('{v}', [def={dft}], [desc={desc}], [helper={hlpr}]) => {r}\"".format(trace_level=trace_level, v=var, dft=default, desc=description, hlpr=helper, r=text_value))
     debug.trace_fmtd(trace_level, "getenv_text('{v}', [def={dft}], [desc={desc}], [helper={hlpr}]) => {r}",
@@ -287,23 +288,26 @@
     print_error("Error during {t}: {exc}".
                  format(t=task, exc=get_exception()))
     if show_stack:
         print_full_stack()
     return
 
 
-def exit(message=None, **namespace):    # pylint: disable=redefined-builtin
+def exit(message=None, status_code=None, **namespace):    # pylint: disable=redefined-builtin
     """Display error MESSAGE to stderr and then exit, using optional
-    NAMESPACE for format"""
+    NAMESPACE for format. The STATUS_CODE can be overrided (n.b., 0 if None)."""
+    # EX: exit("Error: {reason}!", reason="Whatever")
     debug.trace(6, f"system.exit{(message, namespace)})")
     if namespace:
         message = message.format(**namespace)
     if message:
         print_stderr(message)
-    return sys.exit()
+        if status_code is None:
+            status_code = 1
+    return sys.exit(status_code)
 
 
 def setenv(var, value):
     """Set environment VAR to VALUE"""
     debug.trace_fmtd(5, "setenv({v}, {val})", v=var, val=value)
     os.environ[var] = value
     return
@@ -352,27 +356,31 @@
         current_frame = inspect.stack()[1]
         function_name = current_frame[3]
     except:
         debug.trace_fmtd(3, "Unable to resolve function name: {exc}", exc=get_exception())
     return function_name
 
 
-def open_file(filename, encoding=None, errors=None, **kwargs):
+def open_file(filename, /, mode="r", *, encoding=None, errors=None, **kwargs):
     """Wrapper around around open() with FILENAME using UTF-8 encoding and ignoring ERRORS (both by default)
-    Note: mode is left at default (i.e., 'r')"""
-    # TODO: implement as with-style context
-    ## OLD: if encoding is None:
-    if (encoding is None) and (kwargs.get("mode") != "rb"):
+    Notes:
+    - The mode is left at default (i.e., 'r')
+    - As with open(), result can be used in a with statement:
+        with system.open_file(filename) as f: ...
+    """
+    # Note: position-only args precedes / and keyword only follow * (based on https://stackoverflow.com/questions/24735311/what-does-the-slash-mean-when-help-is-listing-method-signatures):
+    #   def f(pos_only1, pos_only2, /, pos_or_kw1, pos_or_kw2, *, kw_only1, kw_only2): pass
+    if (encoding is None) and ("b" not in mode):
         encoding = "UTF-8"
     if (encoding and (errors is None)):
         errors = 'ignore'
     result = None
     try:
         # pylint: disable=consider-using-with; note: bogus 'Bad option value' warning
-        result = open(filename, encoding=encoding, errors=errors, **kwargs)
+        result = open(filename, mode=mode, encoding=encoding, errors=errors, **kwargs)
     except IOError:
         debug.trace_fmtd(3, "Unable to open {f}: {exc}", f=filename, exc=get_exception())
     debug.trace_fmt(5, "open({f}, [{enc}, {err}], kwargs={kw}) => {r}",
                     f=filename, enc=encoding, err=errors, kw=kwargs, r=result)
     return result
 
 
@@ -393,15 +401,14 @@
 def load_object(file_name, ignore_error=False):
     """Loads object from FILE_NAME in pickle format"""
     # Note: Reads in binary mode to avoid unicode decode error. See
     #    https://stackoverflow.com/questions/32957708/python-pickle-error-unicodedecodeerror
     obj = None
     try:
         with open(file_name, mode='rb') as f:
-            ## OLD: obj = pickle.load(f)
             try:
                 obj = pickle.load(f)
             except (UnicodeDecodeError):
                 if (sys.version_info.major > 2):
                     # note: treats strings in python2-pickled files as bytes (not Ascii)
                     obj = pickle.load(f, encoding='bytes') 
     except (AttributeError, IOError, TypeError, ValueError):
@@ -418,15 +425,14 @@
     # EX: quote_url_text("<2/") => "%3C2%2f"
     # EX: quote_url_text("Joe's hat") => "Joe%27s+hat"
     # EX: quote_url_text("Joe%27s+hat") => "Joe%2527s%2Bhat"
     debug.trace_fmtd(7, "in quote_url_text({t})", t=text)
     result = text
     quote = (not unquote)
     try:
-        ## BAD: if not re.search("%[0-9A-F]{2}", text):
         proceed = True
         if proceed:
             # pylint: disable=no-member
             fn = None
             ## TODO: debug.trace_object(6, "urllib", urllib, show_all=True)
             if sys.version_info.major > 2:
                 ## TODO: debug.trace_object(6, "urllib.parse", urllib.parse, show_all=True)
@@ -445,18 +451,18 @@
     return result
 #
 def unquote_url_text(text):
     """Unquotes URL TEXT:
     Note: Wrapper around quote_url_text w/ UNQUOTE set"""
     return quote_url_text(text, unquote=True)
 
+
 def escape_html_text(text):
     """Add entity encoding to TEXT to make suitable for HTML"""
-    # Note: This is wrapper around html.escape and just handles
-    # '&', '<', '>', and '"'.
+    # Note: This is wrapper around html.escape and just handles '&', '<', '>', "'", and '"'.
     # EX: escape_html_text("<2/") => "&lt;2/"
     # EX: escape_html_text("Joe's hat") => "Joe&#x27;s hat"
     debug.trace_fmtd(7, "in escape_html_text({t})", t=text)
     result = ""
     if (sys.version_info.major > 2):
         # TODO: move import to top
         import html                    # pylint: disable=import-outside-toplevel, import-error
@@ -465,15 +471,15 @@
         import cgi                     # pylint: disable=import-outside-toplevel, import-error
         result = cgi.escape(text, quote=True)    # pylint: disable=deprecated-method, no-member
     debug.trace_fmtd(6, "out escape_html_text({t}) => {r}", t=text, r=result)
     return result
 
 
 def unescape_html_text(text):
-    """Remove entity encoding, etc. from TEXT (i.e., undo"""
+    """Remove entity encoding, etc. from TEXT (i.e., undo)"""
     # Note: This is wrapper around html.unescape (Python 3+) or
     # HTMLParser.unescape (Python 2).
     # See https://stackoverflow.com/questions/21342549/unescaping-html-with-special-characters-in-python-2-7-3-raspberry-pi.
     # EX: unescape_html_text("&lt;2/") => "<2/"
     # EX: unescape_html_text("Joe&#x27;s hat") => "Joe's hat"
     debug.trace_fmtd(7, "in unescape_html_text({t})", t=text)
     result = ""
@@ -544,22 +550,22 @@
 def read_entire_file(filename, **kwargs):
     """Read all of FILENAME and return as a string
     Note: optional arguments to open() passed along (e.g., encoding amd error handling)"""
     # TODO: allow for overriding handling of newlines (e.g., block \r being treated as line delim)
     # EX: write_file("/tmp/fu123", "1\n2\n3\n"); read_entire_file("/tmp/fu123") => "1\n2\n3\n"
     data = ""
     try:
-        ## OLD: with open(filename) as f:
-        with open_file(filename, **kwargs) as f:
-            data = from_utf8(f.read())
-    ## OLD except IOError:
+        ## TODO: with open_file(filename, **kwargs) as f:
+        with open(filename, encoding="UTF-8", **kwargs) as f:
+            data = f.read()
     except (AttributeError, IOError):
-        # TODO: use print_stderr so that shown in optimized version
-        Level = 4 if (kwargs.get("errors") == "ignore") else 1
-        debug.trace_fmtd(Level, "Error: Unable to read file '{f}': {exc}",
+        debug.trace_exception(1, "read_entire_file/IOError")
+        report_errors = (kwargs.get("errors") != "ignore")
+        if report_errors:
+            print_stderr("Error: Unable to read file '{f}': {exc}",
                          f=filename, exc=get_exception())
     debug.trace_fmtd(8, "read_entire_file({f}) => {r}", f=filename, r=data)
     return data
 #
 read_file = read_entire_file
 
 
@@ -581,15 +587,15 @@
 def read_binary_file(filename):
     """Read FILENAME as byte stream"""
     debug.trace_fmt(7, "read_binary_file({f}, _)", f=filename)
     data = []
     try:
         with open(filename, mode="rb") as f:
             data = f.read()
-    except (IOError, ValueError):
+    except (AttributeError, IOError, ValueError):
         debug.trace_fmtd(1, "Error: Problem reading file '{f}': {exc}",
                          f=filename, exc=get_exception())
     ## TODO: output hexdump excerpt (e.g., via https://pypi.org/project/hexdump)
     return data
 
 
 def read_directory(directory):
@@ -620,37 +626,34 @@
     """Reads FILENAME and returns as hash lookup, optionally SKIP[ing]_HEADER and using DELIM (tab by default).
     Note: Input is made lowercase unless RETAIN_CASE."""
     # Note: the hash lookup uses defaultdict
     debug.trace_fmt(4, "read_lookup_table({f}, [skip_header={sh}, delim={d}, retain_case={rc}])", 
                     f=filename, sh=skip_header, d=delim, rc=retain_case)
     if delim is None:
         delim = "\t"
-    ## OLD: hash_table = {}
     hash_table = defaultdict(str)
     line_num = 0
     try:
         # TODO: use csv.reader
-        with open(filename, encoding="UTF-8") as f:
+        with open_file(filename) as f:
             for line in f:
                 line_num += 1
                 if (skip_header and (line_num == 1)):
                     continue
-                ## OLD: line = from_utf8(line)
-                ## OLD: line = from_utf8(line.rstrip())
                 line = from_utf8(line.rstrip("\n"))
                 if not retain_case:
                     line = line.lower()
                 if delim in line:
                     (key, value) = line.split(delim, 1)
                     hash_table[key] = value
                 else:
                     delim_spec = ("\\t" if (delim == "\t") else delim)
                     debug.trace_fmt(2, "Warning: Ignoring line {n} w/o delim ({d}): {l}", 
                                     n=line_num, d=delim_spec, l=line)
-    except (IOError, ValueError):
+    except (AttributeError, IOError, ValueError):
         debug.trace_fmtd(1, "Error creating lookup from '{f}': {exc}",
                          f=filename, exc=get_exception())
     debug.trace_fmtd(7, "read_lookup_table({f}) => {r}", f=filename, r=hash_table)
     return hash_table
 
 
 def create_boolean_lookup_table(filename, delim=None, retain_case=False, **kwargs):
@@ -663,26 +666,23 @@
     if delim is None:
         delim = "\t"
     # TODO: allow for tab-delimited value to be ignored
     debug.trace_fmt(4, "create_boolean_lookup_table({f}, [retain_case={rc}])", 
                     f=filename, rc=retain_case)
     lookup_hash = defaultdict(bool)
     try:
-        ## with open(filename) as f:
         with open_file(filename, **kwargs) as f:
             for line in f:
-                ## OLD: key = line.strip().lower()
                 key = line.strip()
                 if not retain_case:
                     key = key.lower()
-                ## OLD: debug.assertion(delim not in key)
                 if delim in key:
                     key = key.split(delim)[0]
                 lookup_hash[key] = True
-    except (IOError, ValueError, AttributeError):
+    except (AttributeError, IOError, ValueError):
         debug.trace_fmtd(1, "Error: Creating boolean lookup from '{f}': {exc}",
                          f=filename, exc=get_exception())
     debug.trace_fmt(7, "create_boolean_lookup_table => {h}", h=lookup_hash)
     return lookup_hash
 
 
 def lookup_entry(hash_table, entry, retain_case=False):
@@ -702,57 +702,55 @@
     debug.trace_fmt(7, "write_file({f}, {t})", f=filename, t=text)
     # EX: f = "/tmp/_it.list"; write_file(f, "it"); read_file(f) => "it\n"
     # EX: write_file(f, "it", skip_newline=True); read_file(f) => "it"
     debug.assertion(isinstance(text, str))
     try:
         if not isinstance(text, STRING_TYPES):
             text = to_string(text)
-        ## OLD: mode = 'a' if append else 'w'
-        debug.assertion(not binary and append)
+        debug.assertion(not (binary and append))
         mode = "wb" if binary else "a" if append else "w"
         with open(filename, encoding="UTF-8", mode=mode) as f:
             f.write(to_utf8(text))
             if not text.endswith("\n"):
                 if not skip_newline:
                     f.write("\n")
-    except (IOError, ValueError):
+    except (AttributeError, IOError, ValueError):
         debug.trace_fmtd(1, "Error: Problem writing file '{f}': {exc}",
                          f=filename, exc=get_exception())
     return
 #
 # EX: write_file(f, "new", append=True); read_file(f) => "itnew\n"
 
 
 def write_binary_file(filename, data):
     """Create FILENAME with binary DATA"""
     debug.trace_fmt(7, "write_binary_file({f}, _)", f=filename)
     debug.assertion(isinstance(data, bytes))
     try:
         with open(filename, mode="wb") as f:
             f.write(data)
-    except (IOError, ValueError):
+    except (AttributeError, IOError, ValueError):
         debug.trace_fmtd(1, "Error: Problem writing file '{f}': {exc}",
                          f=filename, exc=get_exception())
     return
 
 
 def write_lines(filename, text_lines, append=False):
     """Creates FILENAME using TEXT_LINES with newlines added and optionally for APPEND"""
     debug.trace_fmt(5, "write_lines({f}, _, {a})", f=filename, a=append)
     debug.trace_fmt(6, "    text_lines={tl}", tl=text_lines)
     debug.assertion(isinstance(text_lines, list))
     f = None
     try:
         mode = 'a' if append else 'w'
-        ## OLD f = open(filename, mode)
         with open(filename, encoding="UTF-8", mode=mode) as f:
             for line in text_lines:
                 line = to_utf8(line)
                 f.write(line + "\n")
-    except IOError:
+    except (AttributeError, IOError, ValueError):
         debug.trace_fmt(2, "Warning: Exception writing file {f}: {e}",
                         f=filename, e=get_exception())
     finally:
         if f:
             f.close()
     return
 
@@ -773,14 +771,26 @@
         mod_time = os.path.getmtime(filename)
         if not as_float:
             mod_time = str(datetime.datetime.fromtimestamp(mod_time))
     debug.trace_fmtd(5, "get_file_modification_time({f}) => {t}", f=filename, t=mod_time)
     return mod_time
 
 
+def filename_proper(path):
+    """Return PATH sans directories"""
+    # EX: filename_proper("/tmp/document.pdf") => "document.pdf")
+    # EX: filename_proper("/tmp") => "tmp")
+    # EX: filename_proper("/") => "/")
+    (directory, filename) = os.path.split(path)
+    if not filename:
+        filename = directory
+    debug.trace(6, f"filename_proper({path}) => {filename}")
+    return filename
+
+
 def remove_extension(filename, extension=None):
     """Return FILENAME without final EXTENSION
     Note: Unless extension specified, only last dot is included"""
     # EX: remove_extension("/tmp/document.pdf") => "/tmp/document")
     # EX: remove_extension("it.abc.def") => "it.abc")
     # EX: remove_extension("it.abc.def", "abc.def") => "it")
     in_extension = extension
@@ -821,16 +831,35 @@
     size = -1
     if file_exists(filename):
         size = os.path.getsize(filename)
     debug.trace_fmtd(5, "get_file_size({f}) => {s}", f=filename, s=size)
     return size
 
 
+def path_separator(sysname=None):
+    """Return text used to separate paths components under current OS (e.g., / or \\).
+    This is basically a wrapper around os.path.sep with tracing, added to avoid using non-existent os.path.delim.
+    Note: can overide SYSNAME to get separator for another system; see os.uname()"""
+    # EX: path_separator(sysname="???") => "/"
+    # TODO: define-tracing-fn path_separator os.path.sep 7
+    result = os.path.sep
+    if (sysname != os.uname().sysname):
+        default_sep = "/"
+        result = "\\" if sysname == "Windows" else default_sep
+    debug.trace(7, f"path_separator() => {result}")
+    return result
+#    
+# EX: path_separator(sysname="Windows") => "\\"
+# EX-SETUP: def when(cond, value): return value if cond else None
+# EX: path_separator() => (when((os.uname().sysname == "Linux"), "/"))
+
+
 def form_path(*filenames):
     """Wrapper around os.path.join over FILENAMEs (with tracing)"""
+    debug.assertion(not any(f.startswith(path_separator()) for f in filenames[1:]))
     path = os.path.join(*filenames)
     debug.trace_fmt(6, "form_path({f}) => {p}", f=tuple(filenames), p=path)
     return path
 
 
 def is_directory(path):
     """Determines whether PATH represents a directory"""
@@ -928,15 +957,14 @@
             encoding = UTF8
         result = result.encode(encoding, 'ignore')
     debug.trace_fmtd(8, "from_unicode({t}, [{e}]) => {r}", t=text, e=encoding, r=result)
     return result
 
 
 def to_string(text):
-    ## OLD: """Ensure TEXT is a string type
     """Ensure VALUE is a string type
     Note: under Python 2, result is str or Unicode; but for Python 3+, it is always str"""
     # EX: to_string(123) => "123"
     # EX: to_string(u"\u1234") => u"\u1234"
     # EX: to_string(None) => "None"
     # Notes: Uses string formatting operator % for proper Unicode handling.
     # Gotta hate Python: doubly stupid changes from version 2 to 3 required special case handling: Unicode type dropped and bytes not automatically treated as string!
@@ -963,15 +991,15 @@
                     t=text, sep=line_separator, r=result)
     return result
 
 
 def normalize_dir(path):
     """Normalize the directory PATH (e.g., removing ending path delim)"""
     # EX: normalize_dir("/etc/") => "/etc")
-    result = chomp(path, os.path.sep)
+    result = chomp(path, path_separator())
     debug.trace(6, f"normalize_dir({path}) => {result}")
     return result
 
 
 def non_empty_file(filename):
     """Whether file exists and is non-empty"""
     non_empty = (file_exists(filename) and (os.path.getsize(filename) > 0))
@@ -1082,24 +1110,25 @@
 
 
 def just_one_true(in_list, strict=False):
     """True if only one element of IN_LIST is considered True (or all None unless STRICT)"""
     # Note: Consider using misc_utils.just1 (based on more_itertools.exactly_n)
     # TODO: Trap exceptions (e.g., string input)
     min_count = 1 if strict else 0
-    ## OLD: is_true = (1 == sum([int(bool(b)) for b in in_list]))         # pylint: disable=misplaced-comparison-constant
-    is_true = (min_count <= sum([int(bool(b)) for b in in_list]) <= 1)    # pylint: disable=misplaced-comparison-constant
+    ## OLD: is_true = (min_count <= sum([int(bool(b)) for b in in_list]) <= 1)    # pylint: disable=misplaced-comparison-constant
+    is_true = (min_count <= sum([int(bool(b)) for b in in_list]) <= 1)
     debug.trace_fmt(6, "just_one_true({l}) => {r}", l=in_list, r=is_true)
     return is_true
 
 
 def just_one_non_null(in_list, strict=False):
     """True if only one element of IN_LIST is not None (or all None unless STRICT)"""
     min_count = 1 if strict else 0
-    is_true = (min_count <= sum([int(x is not None) for x in in_list]) <= 1)    # pylint: disable=misplaced-comparison-constant
+    ## OLD: is_true = (min_count <= sum([int(x is not None) for x in in_list]) <= 1)    # pylint: disable=misplaced-comparison-constant
+    is_true = (min_count <= sum([int(x is not None) for x in in_list]) <= 1)
     debug.trace_fmt(6, "just_one_non_null({l}) => {r}", l=in_list, r=is_true)
     return is_true
 
 
 def unique_items(in_list, prune_empty=False):
     """Returns unique items from IN_LIST, preserving order and optionally PRUN[ing]_EMPTY items"""
     # EX: unique_items([1, 2, 3, 2, 1]) => [1, 2, 3]
@@ -1121,22 +1150,19 @@
         debug.trace_fmtd(6, "Exception in to_float: {exc}", exc=get_exception())
     debug.trace_fmtd(8, "to_float({v}) => {r}", v=text, r=result)
     return result
 #
 safe_float = to_float
 
 
-## OLD: def to_int(text, default_value=0):
 def to_int(text, default_value=0, base=None):
-    ## OLD: """Interpret TEXT as integer, using DEFAULT_VALUE"""
     """Interpret TEXT as integer with optional DEFAULT_VALUE and BASE"""
     # TODO: use generic to_num with argument specifying type
     result = default_value
     try:
-        ## OLD: result = int(text)
         result = int(text, base) if (base and isinstance(text, str)) else int(text)
     except (TypeError, ValueError):
         debug.trace_fmtd(6, "Exception in to_int: {exc}", exc=get_exception())
     debug.trace_fmtd(8, "to_int({v}) => {r}", v=text, r=result)
     return result
 #
 safe_int = to_int
@@ -1160,15 +1186,14 @@
 
 
 PRECISION = getenv_int("PRECISION", 6,
                        "Precision for rounding (e.g., decimal places)")
 #
 def round_num(value, precision=None):
     """Round VALUE [to PRECISION places, 6 by default]"""
-    ## BAD: """Round VALUE [to PRECISION places, {p} by default]""".format(p=PRECISION)
     # EX: round_num(3.15914, 3) => 3.159
     if precision is None:
         precision = PRECISION
     rounded_value = round(value, precision)
     debug.trace_fmtd(8, "round_num({v}, [prec={p}]) => {r}",
                      v=value, p=precision, r=rounded_value)
     return rounded_value
@@ -1193,15 +1218,15 @@
 
 
 def current_time(integral=False):
     """Return current time in seconds since 1970, optionally INTEGRAL"""
     secs = time.time()
     if integral:
         secs = int(round_num(secs, precision=0))
-    debug.trace(5, f"current_time([integral={integral}]) => {secs}")
+    debug.trace(7, f"current_time([integral={integral}]) => {secs}")
     return secs
 
 
 def time_in_secs():
     """Wrapper around current_time"""
     return current_time(integral=True)
 
@@ -1240,16 +1265,18 @@
 
 #-------------------------------------------------------------------------------
 # Command line usage
 
 def main(args):
     """Supporting code for command-line processing"""
     debug.trace_fmtd(6, "main({a})", a=args)
-    user = getenv_text("USER")
-    print_stderr("Warning, {u}: Not intended for direct invocation".format(u=user))
+    user = getenv_text("USER", "user")
+    print_stderr("Warning, {u}: {f} not intended for direct invocation!".
+                 format(u=user, f=filename_proper(__file__)))
     debug.trace_fmt(4, "FYI: maximum integer is {maxi}", maxi=maxint())
     return
 
+
 if __name__ == '__main__':
     main(get_args())
 else:
     debug.assertion(TEMP_DIR is not None)
```

### Comparing `mezcla-1.3.8/mezcla/temp/simple_batspp.py` & `mezcla-1.3.9/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/template.py` & `mezcla-1.3.9/mezcla/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #! /usr/bin/env python
+# TODO: # -*- coding: utf-8 -*-
 ## TODO: handle case when env installed elsewhere (e.g., maldito mac)
 ## #! env python
 # 
 # TODO what the script does (detailed)
 #
 ## TODO: see example/template.py for simpler version suitable for cut-n-paste from online examples
 #
@@ -134,11 +135,11 @@
     # Make sure no TODO_vars above (i.e., in namespace)
     debug.assertion(not any(my_re.search(r"^TODO_", m, my_re.IGNORECASE)
                             for m in dir(app)))    
     
 #-------------------------------------------------------------------------------
     
 if __name__ == '__main__':
-    debug.trace_current_context(level=TL.QUITE_DETAILED)
+    debug.trace_current_context(level=TL.QUITE_VERBOSE)
     debug.trace(5, f"main __doc__: {main.__doc__}")
     debug.assertion("TODO:" not in __doc__)
     main()
```

### Comparing `mezcla-1.3.8/mezcla/tests/LICENSE.txt` & `mezcla-1.3.9/mezcla/tests/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.3.9/mezcla/tests/adhoc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/misc_doctests.py` & `mezcla-1.3.9/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/cars-csv-len-3.txt` & `mezcla-1.3.9/mezcla/tests/resources/cars-csv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/cars-tsv-len-3.txt` & `mezcla-1.3.9/mezcla/tests/resources/cars-tsv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/cars.csv` & `mezcla-1.3.9/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/cars.tsv` & `mezcla-1.3.9/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/example_text.txt` & `mezcla-1.3.9/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.3.9/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/iris_output.txt` & `mezcla-1.3.9/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.3.9/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.3.9/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.3.9/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/template.py` & `mezcla-1.3.9/mezcla/tests/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 
 # Installed packages
 import pytest
 
 # Local packages
 from mezcla.unittest_wrapper import TestWrapper
 from mezcla import debug
-from mezcla.my_regex import my_re
 from mezcla import glue_helpers as gh
+from mezcla.my_regex import my_re
+from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:                  global module object
 #    TestTemplate.script_module:  path to file
 ## TODO (vvv): change template to new name; *** use commented out template below ***
 THE_MODULE = None           ## TODO: remove this line (n.b., used just to avoid syntax problems with <module> in following)
 ## TODO (^^^): import mezcla.<module> as THE_MODULE
@@ -75,25 +76,25 @@
     ##     return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_data_file(self):
         """Makes sure TODO works as expected"""
         debug.trace(4, f"TestIt.test_data_file(); self={self}")
         data = ["TODO1", "TODO2"]
-        gh.write_lines(self.temp_file, data)
+        system.write_lines(self.temp_file, data)
         ## TODO: add use_stdin=True to following if no file argument
         output = self.run_script(options="", data_file=self.temp_file)
         assert my_re.search(r"TODO-pattern", output.strip())
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_something_else(self):
         """TODO: flesh out test for something else"""
         debug.trace(4, f"TestIt.test_something_else(); self={self}")
-        self.fail("TODO: code test")
+        assert False
         ## ex: assert (THE_MODULE.TODO_function() == TODO_value)
         return
 
 
     ## TODO: optional cleanup methods
     ##
     ## def tearDown(self):
@@ -112,20 +113,20 @@
 ## TODO:
 ## #...............................................................................
 ##
 ## class TestIt2:
 ##     """Another class for testcase definition
 ##     Note: Needed to avoid error with pytest due to inheritance with unittest.TestCase via TestWrapper"""
 ##
-##    def test_whatever(self):
-##        """TODO: flesh out test for whatever"""
-##        debug.trace(4, f"TestIt2.test_whatever(); self={self}")
-##        assert False, "TODO: code test"
-##        ## ex: assert THE_MODULE.fast_sort() == THE_MODULE.slow_sort()
-##        return
+##     def test_whatever(self):
+##         """TODO: flesh out test for whatever"""
+##         debug.trace(4, f"TestIt2.test_whatever(); self={self}")
+##         assert False, "TODO: code test"
+##         ## ex: assert THE_MODULE.fast_sort() == THE_MODULE.slow_sort()
+##         return
 ##
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.8/mezcla/tests/test___init__.py` & `mezcla-1.3.9/mezcla/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_audio.py` & `mezcla-1.3.9/mezcla/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.3.9/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_bing_search.py` & `mezcla-1.3.9/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.3.9/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_cut.py` & `mezcla-1.3.9/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_data_utils.py` & `mezcla-1.3.9/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_debug.py` & `mezcla-1.3.9/mezcla/tests/test_debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # Installed packages
 import pytest
 
 # Local packages
 ## TODO: make sure atexit support disabled unless explcitly requested
 ##   import os; os.environ["SKIP_ATEXIT"] = os.environ.get("SKIP_ATEXIT", "1")
 from mezcla import debug
+from mezcla.my_regex import my_re
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 import mezcla.debug as THE_MODULE # pylint: disable=reimported
 
 class TestDebug:
     """Class for test case definitions"""
@@ -143,19 +144,33 @@
                 self.name = name
             def __repr__(self):
                 return f'Person("{self.name}")'
         THE_MODULE.trace_values(-1, [Person("Kiran")], use_repr=True)
         captured = capsys.readouterr()
         assert 'Person("Kiran")' in captured.err
 
-    def test_trace_expr(self):
-        """Ensure trace_expr works as expected"""
-        debug.trace(4, f"test_trace_expr(): self={self}")
-        ## TODO: WORK-IN-PROGRESS
-
+    def test_trace_expr(self, capsys):
+        """Make sure trace_expr shows 'expr1=value1; expr2=value2'"""
+        var1 = 3
+        var2 = 6
+        THE_MODULE.trace_expr(debug.get_level(), var1, var2)
+        captured = capsys.readouterr()
+        assert "var1=3;var2=6" in my_re.sub(r"\s+", "", captured.err)
+
+    @pytest.mark.xfail
+    def test_trace_expr_expression(self, capsys):
+        """Make sure trace_expr expression resolved when split across lines"""
+        var1 = 3
+        var2 = 6
+        THE_MODULE.trace_expr(debug.get_level(),
+                              var1,
+                              var2)
+        captured = capsys.readouterr()
+        assert "var1=3.*var2=6" in my_re.sub(r"\s+", "", captured.err)
+        
     def test_trace_current_context(self):
         """Ensure trace_current_context works as expected"""
         debug.trace(4, f"test_trace_current_context(): self={self}")
         ## TODO: WORK-IN-PROGRESS
 
     def test_trace_exception(self):
         """Ensure trace_exception works as expected"""
@@ -176,14 +191,24 @@
         assert 'failed' not in captured.err
         # Prints assertion failed in stderr
         THE_MODULE.assertion((2 + 2) == 5)
         captured = capsys.readouterr()
         assert "failed" in captured.err
         assert "(2 + 2) == 5" in captured.err
 
+    @pytest.mark.xfail
+    def test_assertion_expression(self, capsys):
+        """Make sure assertion expression split across lines resolved"""
+        debug.trace(4, f"test_assertion_expression(): self={self}")
+        THE_MODULE.assertion(2 +
+                             2 ==
+                             5)
+        captured = capsys.readouterr()
+        assert "2+2==5" in my_re.sub(r"\s+", "", captured.err)
+
     def test_val(self):
         """Ensure val works as expected"""
         debug.trace(4, f"test_val(): self={self}")
         save_trace_level = THE_MODULE.get_level()
         test_value = 22
         THE_MODULE.set_level(5)
         level5_value = THE_MODULE.val(5, test_value)
```

### Comparing `mezcla-1.3.8/mezcla/tests/test_extract_document_text.py` & `mezcla-1.3.9/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_file_utils.py` & `mezcla-1.3.9/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_filter_random.py` & `mezcla-1.3.9/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_gensim_test.py` & `mezcla-1.3.9/mezcla/tests/test_gensim_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,50 +18,77 @@
 """Tests for gensim_test module"""
 
 # Standard packages
 import re
 
 # Installed packages
 import pytest
+## TAKE1
+## # note: The gensim module is not installed by default, so tests skipped if not found
+## try:
+##     import gensim
+## except:
+##     gensim = None
 
 # Local packages
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla import tpo_common as tpo
 from mezcla.unittest_wrapper import TestWrapper
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
-import mezcla.gensim_test as THE_MODULE
+try:
+    import gensim
+    import mezcla.gensim_test as THE_MODULE
+except:
+    ## TEST (maldito pytest):
+    ## print("hey, hey, hey!")
+    debug.trace_exception(3, "importing gensim_test")
+    gensim = None
+    THE_MODULE = None
 
 class TestGensimTest(TestWrapper):
-    """Class for testcase definition"""
+    """Class for script-level testcase definition"""
     script_file = TestWrapper.get_module_file_path(__file__)
-    script_module = TestWrapper.derive_tested_module_name(__file__)
+    script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
 
+    @pytest.mark.skipif(not gensim, reason="gensim module missing")
     def test_data_file(self):
         """Tests results over a known data file (LICENSE.txt)"""
         tpo.debug_print("test_data_file()", 4)
         data_file = "LICENSE.txt"
         temp_data_file = self.temp_base + "-" + data_file
         gh.copy_file(gh.resolve_path(data_file), temp_data_file)
         output = self.run_script("--save", temp_data_file)
         ## TODO: assert re.search("storing corpus in Matrix Market format", output)
         assert gh.non_empty_file(temp_data_file.replace(".txt", ".bow.mm"))
         debug.trace_expr(5, output)
         return
 
+    @pytest.mark.skipif(not gensim, reason="gensim module missing")
     def test_vector_printing(self):
         """Test printing of corpus vector for simple input"""
         tpo.debug_print("test_vector_printing()", 4)
         temp_file = self.temp_base + ".txt"
         gh.write_file(temp_file, "My dog has fleas.\n")
         output = self.run_script("--print --verbose", temp_file)
         assert re.search(r"\(u?'dog', 1\),.*\(u?'has', 1\)", output)
         debug.trace_expr(5, output)
         return
 
+    
+class TestGensimTest2:
+     """Class for internal testcase definitions"""
+
+     @pytest.mark.skipif(not gensim, reason="gensim module missing")
+     def test_corpus_data(self):
+         """Test creation of corpus from a file"""
+         corpus = THE_MODULE.CorpusData(__file__)
+         # note: currently 81 unique tokens extracted
+         assert len(list(corpus)) > 50
+   
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.8/mezcla/tests/test_glue_helpers.py` & `mezcla-1.3.9/mezcla/tests/test_glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_html_utils.py` & `mezcla-1.3.9/mezcla/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_kenlm_example.py` & `mezcla-1.3.9/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_keras_param_search.py` & `mezcla-1.3.9/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_main.py` & `mezcla-1.3.9/mezcla/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_merge_files.py` & `mezcla-1.3.9/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_merge_notes.py` & `mezcla-1.3.9/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_misc_utils.py` & `mezcla-1.3.9/mezcla/tests/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_my_regex.py` & `mezcla-1.3.9/mezcla/tests/test_my_regex.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         ## TODO: WORK-IN-PROGRESS
 
     def test_simple_regex(self):
         """"Test regex search with capturing"""
         debug.trace(4, "test_simple_regex()")
         if not self.my_re.search(r"(\w+)\W+(\w+)", ">scrap ~!@\n#$ yard<",
                                  re.MULTILINE):
-            self.fail("simple regex search failed")
+            assert(False, "simple regex search failed")
         assert self.my_re.group(1) == "scrap"
         assert self.my_re.group(2) == "yard"
         return
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
```

### Comparing `mezcla-1.3.8/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.3.9/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_os_utils.py` & `mezcla-1.3.9/mezcla/tests/test_os_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 #    THE_MODULE:	    global module object
 ## TODO: import mezcla.os_utils as THE_MODULE
 
 class TestOsUtils:
     """Class for testcase definition"""
 
     def test_split_extension(self):
+        """Ensure test_split_extension works as expected"""
         assert(os_utils.split_extension("fubar.txt") == ("fubar", ".txt"))
 
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.8/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.3.9/mezcla/tests/test_pandas_sklearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # Installed packages
 import pytest
 
 # Local packages
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.unittest_wrapper import TestWrapper
-from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 import mezcla.pandas_sklearn as THE_MODULE
 
 # Constants
 EXAMPLES = f'{gh.dir_path(__file__)}/../examples'
```

### Comparing `mezcla-1.3.8/mezcla/tests/test_plot_utils.py` & `mezcla-1.3.9/mezcla/tests/test_plot_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 class TestPlotUtils:
     """Class for testcase definition"""
 
     @pytest.mark.skip
     def test_something(self):
         """TODO: flesh out test for something"""
         debug.trace(4, "TestIt.test_something()")
-        self.fail("TODO: code test")
+        assert False
         return
 
     @pytest.mark.xfail
     def test_something_else(self):
         """TODO: flesh out test for something else"""
         debug.trace(4, "TestIt.test_something_else()")
-        self.fail("TODO: code test")
+        assert False
         return
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.8/mezcla/tests/test_randomize_lines.py` & `mezcla-1.3.9/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.3.9/mezcla/tests/test_rgb_color_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             )
         return
 
     @pytest.mark.skip(reason="TODO: test not yet implemented")
     def test_something_else(self):
         """TODO: flesh out test for something else"""
         debug.trace(4, "test_something_else()")
-        self.fail("TODO: code test")
+        assert(False, "TODO: code test")
         ## ex: assert THE_MODULE.TODO_function() == TODO_value
         return
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
```

### Comparing `mezcla-1.3.8/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.3.9/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.3.9/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.3.9/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_simple_main_example.py` & `mezcla-1.3.9/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.3.9/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.3.9/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_system.py` & `mezcla-1.3.9/mezcla/tests/test_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
     def test_print_exception_info(self, capsys):
         """Ensure print_exception_info works as expected"""
         debug.trace(4, "test_print_exception_info()")
         THE_MODULE.print_exception_info("Foobar")
         captured = capsys.readouterr()
         assert "Foobar" in captured.err
 
+    @pytest.mark.xfail
     def test_exit(self, monkeypatch, capsys):
         """Ensure exit works as expected"""
         debug.trace(4, "test_exit()")
         def sys_exit_mock():
             return 'exit'
         monkeypatch.setattr(sys, "exit", sys_exit_mock)
         assert THE_MODULE.exit('test exit {method}', method='method') == 'exit'
@@ -815,15 +816,16 @@
         monkeypatch.setattr("sys.argv", args)
         assert THE_MODULE.get_args() == args
 
     def test_main(self, capsys):
         """Ensure main works as expected"""
         THE_MODULE.main('some-arg')
         captured = capsys.readouterr()
-        assert "Not intended for direct invocation" in captured.err
+        # ex: Warning, tomohara: system.py not intended for direct invocation!
+        assert "not intended" in captured.err.lower()
 
 
 def set_test_env_var():
     """Set enviroment vars to run tests"""
     THE_MODULE.env_options = {
         'VAR_STRING': 'this is a string variable',
         'ANOTHER_VAR': 'this is another env. var.'
```

### Comparing `mezcla-1.3.8/mezcla/tests/test_template.py` & `mezcla-1.3.9/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_text_categorizer.py` & `mezcla-1.3.9/mezcla/tests/test_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_text_processing.py` & `mezcla-1.3.9/mezcla/tests/test_text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_text_utils.py` & `mezcla-1.3.9/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_tpo_common.py` & `mezcla-1.3.9/mezcla/tests/test_tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_train_language_model.py` & `mezcla-1.3.9/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.3.9/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_transpose_data.py` & `mezcla-1.3.9/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/test_xml_utils.py` & `mezcla-1.3.9/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.3.9/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.3.9/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/tfidf/test_document.py` & `mezcla-1.3.9/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.3.9/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/text_categorizer.py` & `mezcla-1.3.9/mezcla/text_categorizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,29 +157,28 @@
     debug.trace_object(6, confusion, "confusion")
     return
 
 
 def create_tabular_file(filename, data):
     """Create tabular FILENAME with SkLearn DATA for use with read_categorization_data"""
     # Note: intended for comparing results here against tutorial (e.g., in ipython shell)
-    with open(filename, "w") as f:
+    with system.open_file(filename, "w") as f:
         for i in range(len(data.data)):
             text = system.to_utf8(re.sub("[\t\n]", " ", data.data[i]))
             f.write("{lbl}\t{txt}\n".format(lbl=data.target_names[data.target[i]], txt=text))
     return
 
 
 def read_categorization_data(filename):
     """Reads table with (non-unique) label and tab-separated value. 
     Note: label made lowercase; result returned as tuple (labels, values)"""
     debug.trace_fmtd(4, "read_categorization_data({f})", f=filename)
     labels = []
     values = []
-    # TODO: rework via system.open_file
-    with open(filename) as f:
+    with system.open_file(filename) as f:
         for (i, line) in enumerate(f):
             line = system.from_utf8(line)
             items = line.split("\t")
             if len(items) == 2:
                 labels.append(items[0].lower())
                 values.append(items[1])
             else:
@@ -222,14 +221,15 @@
         """Constructor: records CLASSIFIER"""
         debug.trace_fmt(6, "{cl}.__init__(clf={c})", c=classifier, cl=str(type(self)))
         self.classifier = classifier
         self.tfidf_vectorizer = None
 
     def _get_param_names(self):
         """Get parameter names for the estimator"""
+        # TODO: drop method
         # Note: This is not class method as in BaseEstimator.
         # pylint: disable=protected-access
         return self.classifier._get_param_names()
 
     def get_params(self, deep=True):
         """Return list of parameters supported"""
         return self.classifier.get_params(deep=deep)
@@ -482,15 +482,15 @@
             # TODO: for (i, actual_index) in enumerate(actual_indices)
             for (i, actual_index) in enumerate(actual_indices):
                 debug.assertion(actual_index == actual_indices[i])
                 if (actual_indices[i] != predicted_indices[i]):
                     text = values[i]
                     context = (text[:CONTEXT_LEN] + "...\n") if (len(text) > CONTEXT_LEN) else text
                     # TODO: why is pylint flagging the format string as invalid?
-                    bad_instances += u"{g}\t{b}\t{t}".format(
+                    bad_instances += "{g}\t{b}\t{t}\n".format(
                         g=self.keys[actual_indices[i]],
                         b=self.keys[predicted_indices[i]],
                         t=context)
             bad_filename = filename + ".bad"
             system.write_file(bad_filename, bad_instances)
             debug.trace_fmt(4, "Result ({f}):\n{r}", f=bad_filename, r=system.read_file(bad_filename))
         return accuracy
```

### Comparing `mezcla-1.3.8/mezcla/text_processing.py` & `mezcla-1.3.9/mezcla/text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/text_utils.py` & `mezcla-1.3.9/mezcla/text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/tfidf/corpus.py` & `mezcla-1.3.9/mezcla/tfidf/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,53 +240,53 @@
             raise Exception(ngram)
         num_occurrences = self.count_doc_occurrences(ngram)
         ## TPO: TEST
         ## # HACK: give singletons a max DF to lower IDF score
         ## if (num_occurrences == 1) and PENALIZE_SINGLETONS:
         ##     num_occurrences = len(self.__documents)
         idf = math.log(float(len(self)) / num_occurrences)
-        debug.trace_fmt(7, "idf_basic({ng} len(self)={l} max_doc_occ={mdo} num_occ={no} idf={idf})\n",
+        debug.trace_fmt(8, "idf_basic({ng} len(self)={l} max_doc_occ={mdo} num_occ={no} idf={idf})\n",
                         ng=ngram, l=len(self), mdo=self.max_doc_frequency, no=num_occurrences, idf={idf})
         return idf
 
     def idf_freq(self, ngram):
         """Returns inverse proper of DF (not N/DF)"""
         debug.assertion(self.count_doc_occurrences(ngram) >= 1)
         if self.count_doc_occurrences(ngram) == 0:
             raise Exception(ngram)
         num_occurrences = self.count_doc_occurrences(ngram)
         idf = 1 / num_occurrences
-        debug.trace_fmt(7, "idf_freq({ng} len(self)={l} max_doc_occ={mdo} num_occ={no} idf={idf})\n",
+        debug.trace_fmt(8, "idf_freq({ng} len(self)={l} max_doc_occ={mdo} num_occ={no} idf={idf})\n",
                         ng=ngram, l=len(self), mdo=self.max_doc_frequency, no=num_occurrences, idf={idf})
         return idf
 
     def idf_smooth(self, ngram):
         """Returns IDF using simple smoothing with add-1 relative frequency (prior to log)"""
         debug.assertion(self.count_doc_occurrences(ngram) >= 1)
         idf = math.log(1 + (float(len(self)) / self.count_doc_occurrences(ngram)))
-        debug.trace_fmt(7, "idf_smooth({ng} len(self)={l} doc_occ={do} idf={idf})\n",
+        debug.trace_fmt(8, "idf_smooth({ng} len(self)={l} doc_occ={do} idf={idf})\n",
                         ng=ngram, l=len(self), do=self.count_doc_occurrences(ngram), idf={idf})
         return idf
 
     def idf_max(self, ngram):
         ## TODO: make sure this interpretation makes sense; also, make sure float conversion not required
         """Use maximum ngram TF in place of N and also perform add-1 smoothing"""
         debug.assertion(self.count_doc_occurrences(ngram) >= 1)
         idf = math.log(1 + self.max_raw_frequency / self.count_doc_occurrences(ngram))
-        debug.trace_fmt(7, "idf_smooth({ng} len(self)={l} doc_occ={do} idf={idf})\n",
+        debug.trace_fmt(8, "idf_smooth({ng} len(self)={l} doc_occ={do} idf={idf})\n",
                         ng=ngram, l=len(self), do=self.count_doc_occurrences(ngram), idf={idf})
         return idf
 
     def idf_probabilistic(self, ngram):
         """Returns IDF via probabilistic interpretation: log((N - d)/d), where d is the document occcurrence count for the NGRAM"""
         debug.assertion(self.count_doc_occurrences(ngram) >= 1)
         ## TODO: shouldn't this be (float(len(self) / num_doc_occurrences))
         num_doc_occurrences = self.count_doc_occurrences(ngram)
         idf = math.log(float(len(self) - num_doc_occurrences) / num_doc_occurrences)
-        debug.trace_fmt(7, "idf_smooth({ng} len(self)={l} doc_occ={do} idf={idf})\n",
+        debug.trace_fmt(8, "idf_smooth({ng} len(self)={l} doc_occ={do} idf={idf})\n",
                         ng=ngram, l=len(self), do=num_doc_occurrences, idf={idf})
         return idf
 
     def idf(self, ngram, idf_weight='basic'):
         """Inverse document frequency (IDF) indicates ngram common-ness across the Corpus."""
         ## OLD: return w/ elif
         ## if idf_weight == 'smooth':
```

### Comparing `mezcla-1.3.8/mezcla/tfidf/dockeyword.py` & `mezcla-1.3.9/mezcla/tfidf/dockeyword.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     """Class for maintaining stemmed term and original"""
     
     def __init__(self, text, document=None, start=None, end=None):
         self.locations = set()
         self.text = text
         if (start is not None) and (end is not None):
             self.locations.add(Location(document, start, end))
-        ## TODO: debug.trace_object(8, self, "DocKeyword instance", show_all=False)
-        debug.trace_object(7, self, "DocKeyword instance", show_all=False)
+        ## TODO: debug.trace_object(9, self, "DocKeyword instance", show_all=False)
+        debug.trace_object(8, self, "DocKeyword instance", show_all=False)
 
     def update_locations(self, locations):
         """Add LOCATIONS to other locations"""
         self.locations = self.locations.union(locations)
 
     def __add__(self, other):
         assert self.text == other.text
@@ -68,8 +68,8 @@
     def __str__(self):
         return u'Stem:%s, Instances:%s, Count:%d' % (self.text, str(self.original_texts), len(self))
 
 #-------------------------------------------------------------------------------
     
 if __name__ == '__main__':
     system.print_stderr(f"Warning: {__file__} is not intended to be run standalone")
-    debug.trace_object(3, DocKeyword("monkeys"))
+    debug.trace_object(4, DocKeyword("monkeys"))
```

### Comparing `mezcla-1.3.8/mezcla/tfidf/document.py` & `mezcla-1.3.9/mezcla/tfidf/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     def tf_raw(self, ngram):
         """The (relative) frequency of an ngram in a document."""
         num_occurrences = len(self[ngram]) if ngram in self else 0
         # HACK: give singletons a max DF to lower IDF score
         if (num_occurrences == 1) and PENALIZE_SINGLETONS:
             num_occurrences = 0
         tf_raw = float(num_occurrences) / len(self)
-        debug.trace_fmt(6, "tf_raw({ng}): num_occ={no} len(self)={l} result={r}",
+        debug.trace_fmt(7, "tf_raw({ng}): num_occ={no} len(self)={l} result={r}",
                         ng=ngram, no=num_occurrences, l=len(self), r=tf_raw)
         return tf_raw
 
     def tf_log(self, ngram):
         """The log frequency of an ngram in a document."""
         # TODO: is this formula right? Wikipedia is often wrong...
         return 1 + math.log(self.tf_raw(ngram))
@@ -141,15 +141,15 @@
         """Double normalized ngram frequency."""
         term_frequency = self.tf_raw(ngram)
         return 0.5 + (0.5 * (term_frequency / self.max_raw_frequency))
 
     def tf_freq(self, ngram):
         """Returns frequency count for NGRAM"""
         num_occurrences = len(self[ngram]) if ngram in self else 0
-        debug.trace_fmt(6, "tf_freq({ng}): num_occ={no} len(self)={l} result={r}",
+        debug.trace_fmt(7, "tf_freq({ng}): num_occ={no} len(self)={l} result={r}",
                         ng=ngram, no=num_occurrences, l=len(self), r=num_occurrences)
         return num_occurrences
     
     def tf(self, ngram, tf_weight='basic', normalize=False):
         """Calculate term frequency.
 
         Normalizing (stemming) is slow, so it's assumed you're using the ngram.
@@ -206,15 +206,15 @@
         return self.preprocessor.yield_keywords(self.text, document=self)
 
 
 def main():
     """Entry point for script: just runs a simple test"""
     text = "my man fran is not a man"
     d = Document(text, Preprocessor(gramsize=1, stemmer=lambda x: x))
-    debug.trace_expr(4, [d.tf_freq(t) for t in text.split()])
+    debug.trace_expr(5, [d.tf_freq(t) for t in text.split()])
     debug.assertion(d.tf_freq("man") > d.tf_freq("fran"))
     
 #-------------------------------------------------------------------------------
     
 if __name__ == '__main__':
     system.print_stderr(f"Warning: {__file__} is not intended to be run standalone. A simple test willl be run.")
     main()
```

### Comparing `mezcla-1.3.8/mezcla/tfidf/preprocess.py` & `mezcla-1.3.9/mezcla/tfidf/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ## SKLEARN_TOKENIZER = system.getenv_bool("SKLEARN_TOKENIZER", False,
 ##                                        "Use sklearn CountVectorizer for ngrams")
 USE_SKLEARN_COUNTER = system.getenv_bool("USE_SKLEARN_COUNTER", False,
                                          "Use sklearn CountVectorizer for ngrams")
 
 
 if SPLIT_WORDS:
-    debug.trace(1, "Splitting by word token (not whitespace)\n")
+    debug.trace(2, "FYI: Splitting by word token (not whitespace)\n")
     ## BAD: True
 WORD_REGEX = r'\w+' if SPLIT_WORDS else r'\S+'
 
 def handle_unicode(text):
     """Needed for the description fields."""
     if re.search(r'\\+((u([0-9]|[a-z]|[A-Z]){4}))', text):
         text = text.encode('utf-8', 'ignore').decode('unicode-escape', 'ignore')
@@ -122,27 +122,27 @@
         text = handle_text_break_dash(text)
         text = text.lower()
 
         ## BAD: regex_subs = ['\t', '\n', '\r', '\s+', '&']
         regex_subs = ['\t', '\n', '\r', r'\s+', '&']
         for regex_sub in regex_subs:
             text = re.sub(regex_sub, ' ', text)
-    debug.trace(7, "clean_text({raw_text}) => {text}")
+    debug.trace(8, "clean_text({raw_text}) => {text}")
     return text
 
 
 def create_stemmer(language):
     """Return wordform stemmer for LANGUAGE (via SnowBall)"""
     stemmer = SnowballStemmer(language)
     
     # Define the stemmer for the particular language
     def stem_wordform(wordform):
         """Returned root of WORDFORM"""
         root = stemmer.stem(wordform)
-        debug.trace_fmt(8, "stem_wordform({wf}) => {r}", wf=wordform, r=root)
+        debug.trace_fmt(9, "stem_wordform({wf}) => {r}", wf=wordform, r=root)
         return root
 
     # Do sanity check
     if (language == "english"):
         debug.assertion(stem_wordform("running") == "run")
 
     return stem_wordform
@@ -215,15 +215,15 @@
                 self.__stemmer = create_stemmer(language)
             self.stopwords = get_stop_words(language)
         if stopwords_file:
             self._load_stopwords(stopwords_file)
         if stemmer:
             self.__stemmer = stemmer
         if not self.__stemmer:
-            debug.trace(3, "Warning: defining no-op stemmer in Preprocessor")
+            debug.trace(4, "Warning: defining no-op stemmer in Preprocessor")
             self.__stemmer = lambda x: x  # no change to word
         debug.assertion(not (gramsize and max_ngram_size))
         debug.assertion(not (all_ngrams and min_ngram_size))
         ## OLD: self.__gramsize = gramsize
         self.__gramsize = (max_ngram_size or gramsize)
         self.__all_ngrams = all_ngrams
         self.__min_ngram_size = (min_ngram_size or gramsize)
@@ -327,15 +327,15 @@
             debug.assertion(not gramlist)
             if gramlist:
                 sys.stderr.write("Error: ignoring obsolete all_ngrams and using min_ngram_size\n")
             gramlist = range(self.min_ngram_size, self.gramsize + 1)
         if not gramlist:
             gramlist = [self.gramsize]
         ## DEBUG: sys.stderr.write("gramlist={gl}\n".format(gl=gramlist))
-        debug.trace_fmt(7, "gramlist={gl}\n", gl=gramlist)
+        debug.trace_fmt(8, "gramlist={gl}\n", gl=gramlist)
 
         for sentence in positional_splitter(self.negative_gram_breaks, raw_text):
             words = positional_splitter(WORD_REGEX, sentence.text)
             # Remove all stopwords
             words_no_stopwords = []
             for w in words:
                 # Remove common contractions for stopwords when checking list
```

### Comparing `mezcla-1.3.8/mezcla/tpo_common.py` & `mezcla-1.3.9/mezcla/tpo_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,15 +645,15 @@
     return
 
 
 def redirect_stderr(filename):
     """Redirects error output to FILENAME"""
     global stderr
     assert(stderr == sys.stderr)
-    stderr = open(filename, "w")
+    stderr = system.open_file(filename, "w")
     assert(stderr)
 
 
 def restore_stderr():
     """Restores error output to system stderr, closing handle for redirection"""
     global stderr
     assert(stderr != sys.stderr)
@@ -988,25 +988,25 @@
     return
 
 
 def load_object(filename):
     """Load object data from FILENAME in pickle format"""
     debug_print("Loading object from %s" % filename, 3)
     object_data = None
-    f = open(filename, 'rb')
+    f = system.open_file(filename, 'rb')
     if f:
         object_data = pickle.load(f)
         f.close()
     return object_data
 
 
 def store_object(filename, object_data):
     """Store OBJECT_DATA in FILENAME using pickle format"""
     debug_print("Saving object to %s" % filename, 3)
-    f = open(filename, 'wb')
+    f = system.open_file(filename, 'wb')
     if f:
         pickle.dump(object_data, f)
         f.close()
     return
 
 
 def dump_stored_object(object_filename, dump_filename, level=1):
@@ -1026,15 +1026,15 @@
     """Create lookup hash table from string keys to string values (one pair per line, tab separated), optionally with the line number serving as implicit key. Note: The keys are made lowercase, and lines with multiple tabs are ignored."""
     # TODO: rename as create_lookup_hash? (see ShelveLookup.from_hash in table_lookup.py)
     # TODO: use enumerate(f); refine exception in except
     debug_print("create_lookup_table(%s)" % filename, 4)
     lookup_hash = {} if (not use_linenum) else OrderedDict()
     f = None
     try:
-        f = open(filename)
+        f = system.open_file(filename)
         line_num = 0
         for line in f:
             line = line.strip("\n")
             line_num += 1
             fields = line.split("\t")
             if len(fields) == 2:
                 key = fields[0].lower()
@@ -1061,15 +1061,15 @@
     return result
 
 def create_boolean_lookup_table(filename):
     """Create lookup hash table from string keys to boolean occurrence indicator. Note: The keys are made lowercase."""
     # TODO: allow for tab-delimited value to be ignored
     debug_print("create_boolean_lookup_table(%s)" % filename, 4)
     lookup_hash = {}
-    f = open(filename)
+    f = system.open_file(filename)
     for line in f:
         key = line.strip().lower()
         lookup_hash[key] = True
     if f:
         f.close()
     debug_print("create_boolean_lookup_table => %s" % lookup_hash, 8)
     return lookup_hash
```

### Comparing `mezcla-1.3.8/mezcla/train_language_model.py` & `mezcla-1.3.9/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/train_text_categorizer.py` & `mezcla-1.3.9/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/transpose_data.py` & `mezcla-1.3.9/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/mezcla/unittest_wrapper.py` & `mezcla-1.3.9/mezcla/unittest_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 
     @staticmethod
     def get_testing_module_name(test_filename, module_object=None):
         """Derive the name of the module being tested from TEST_FILENAME and MODULE_OBJECT
         Note: used as follows (see tests/test_template.py):
             script_module = TestWrapper.get_testing_module_name(__file__)
         """
+        # Note: Used to resolve module name given THE_MODULE (see template).
         module_name = os.path.split(test_filename)[-1]
         module_name = re.sub(r".py[oc]?$", "", module_name)
         module_name = re.sub(r"^test_", "", module_name)
         package_name = THIS_PACKAGE
         if module_object is not None:
            package_name = getattr(module_object, "__package__", "")
            debug.trace_expr(4, package_name)
@@ -236,42 +237,42 @@
         if not out_file:
             out_file = self.temp_file + ".out"
         # note: output is redirected to a file to preserve tabs
 
         # Set converage script path and command spec
         coverage_spec = ''
         if self.check_coverage:
-            gh.assertion(self.script_file)
+            debug.assertion(self.script_file)
             self.script_module = self.script_file
             coverage_spec = 'coverage run'
         else:
             debug.assertion(not self.script_module.endswith(".py"))
 
         gh.issue("{env} python -m {cov_spec} {module}  {opts}  {path} 1> {out} 2> {log}",
                  env=env_options, cov_spec=coverage_spec, module=self.script_module,
                  opts=options, path=data_path, out=out_file, log=log_file)
-        output = gh.read_file(out_file)
+        output = system.read_file(out_file)
         # note; trailing newline removed as with shell output
         if output.endswith("\n"):
             output = output[:-1]
         debug.trace_fmtd(trace_level, "output: {{\n{out}\n}}",
                          out=gh.indent_lines(output))
 
         # Make sure no python or bash errors. For example,
         #   "SyntaxError: invalid syntax" and "bash: python: command not found"
-        log_contents = gh.read_file(log_file)
+        log_contents = system.read_file(log_file)
         error_found = re.search(r"(\S+error:)|(no module)|(command not found)",
                                 log_contents.lower())
-        gh.assertion(not error_found)
+        debug.assertion(not error_found)
         debug.trace_fmt(trace_level + 1, "log contents: {{\n{log}\n}}",
                         log=gh.indent_lines(log_contents))
 
         # Do sanity check for python exceptions
         traceback_found = re.search("Traceback.*most recent call", log_contents)
-        gh.assertion(not traceback_found)
+        debug.assertion(not traceback_found)
 
         return output
 
     def tearDown(self):
         """Per-test cleanup: deletes temp file unless detailed debugging"""
         debug.trace(4, "TestWrapper.tearDown()")
         if not KEEP_TEMP:
```

### Comparing `mezcla-1.3.8/mezcla/xml_utils.py` & `mezcla-1.3.9/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/pyproject.toml` & `mezcla-1.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/requirements.txt` & `mezcla-1.3.9/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,102 +3,97 @@
 # By default only the cases used in multuiple scripts are installed.
 #
 # Note:
 # - Usage examples:
 #   1. Usual
 #      pip install -r requirements.txt
 #   2. Optional (i.e., including most optional):
-#      pip install --verbose $(perl -00 -pe 's/^#opt#\s*//gm;' ~/python/Mezcla/requirements.txt | grep -v '^#')
+#      pip install --verbose $(perl -pe 's/^#opt#\s*//;' ~/python/Mezcla/requirements.txt | grep -v '^#')
 #   3. Full (i.e., including all optional):
-#      pip install --verbose $(perl -00 -pe 's/^#full#\s*//gm;' ~/python/Mezcla/requirements.txt | grep -v '^#')
+#      pip install --verbose $(perl -pe 's/^#full#\s*//;' ~/python/Mezcla/requirements.txt | grep -v '^#')
 # - use `pip freeze` to get current list of package specifications (n.b., >= better than == unless specific version needed)
+# - installing textract from PyPI fails https://github.com/deanmalmgren/textract/issues/461
 #
-wheel==0.38.4
+# TODO:
+# - check absl module ($ grep -r "absl" .)
+# - add support for this to setup.py
+#...............................................................................
+# Regular requirements
+#
+HTMLParser==0.0.2
+absl_py==1.2.0
+albert==1.3.1
+beautifulsoup4==4.11.1
+bert==2.2.0
 bs4
-lxml
-# Note: installing textract from PyPI fails https://github.com/deanmalmgren/textract/issues/461
-git+https://github.com/tehabstract/textract.git
+cachetools
 cherrypy
+extcolors>=1.0.0
+git+https://github.com/tehabstract/textract.git
+gradio
+ibm_cloud_sdk_core==3.15.3
 lxml
-pyenchant
 mako
 matplotlib
 nltk
-## numpy
 numpy>=1.18.5
-## OLD: ordereddict
 pandas>=1.3.0
-pyenchant
-requests
-scipy
-## OLD: sklearn (PyPI package is deprecated, use 'scikit-learn')
-## TODO: put in setup.py
-six
-## OLD: stopwords
-xgboost
 pyaml
-## TODO: check absl module ($ grep -r "absl" .)
-absl_py==1.2.0
-albert==1.3.1
-beautifulsoup4==4.11.1
-bert==2.2.0
-HTMLParser==0.0.2
-ibm_cloud_sdk_core==3.15.3
+pyenchant
 pysbd==0.3.4
+pytest
+requests
 scikit-learn==1.1.2
+scipy
 scispacy==0.5.0
+six
 stop_words==2018.7.23
 tensorflow_hub==0.12.0
 vaderSentiment==3.3.2
-## OLD: extcolors==1.0.0
-extcolors>=1.0.0
+webcolors
+wheel==0.38.4
+xgboost
 #
 #...............................................................................
 # Optional requirements
 #
-## TODO:
+# TODO:
 # - download Spacy model(s):
 #   python -m spacy download en_core_web_lg
+# - install bash kernel
+#   python -m bash_kernel.install
+# - add '#opt#deprecated#' (e,.g., useful for deprecated functions/modules)
 # NOTE:
 # - tensorflow and related not installed by default due to size of repo and C compilation overhead.
+# - ipython, pylint, etc. used for setting up development environment
 #
-#opt# cachetools
+#opt# SpeechRecognition
+#opt# accelerate
+#opt# bash_kernel
+#opt# coverage
+#opt# datasets
+#opt# diffusers
+#opt# flask
+#opt# flit
 #opt# gensim
+#opt# ibm-watson
+#opt# ipython
+#opt# jupyter
 #opt# kenlm
-#full# lucene
-#full# bert-tensorflow
+#opt# librosa
 #opt# more_itertools
+#opt# pylint
 #opt# pyyaml
 #opt# selenium
 #opt# spacy>=3.0.0
-## TODO: python -m spacy download en
-#full# tensorflow
-#full# keras
-#
-#opt# librosa
-#opt# SpeechRecognition
-#opt# ibm-watson
-#
-## TODO: #opt# deprecated (this is useful for deprecated functions/modules)
+#opt# torch
+#opt# transformers
+#...............................................................................
+# "Fully optional" requirements
+# Note: these generally involve large or long installations.
 #
-# NOTE: the following are for setting up typical development environment
-#opt# ipython
-#opt# pylint
-#opt# jupyter
-#opt# bash_kernel
-## TODO: python -m bash_kernel.install
-#opt# webcolors
-#opt# flit
-#opt# gradio
-#opt# pytest
-#opt# coverage
-#opt# ipython
-#opt# pylint
-#opt# gradio
-#full# sentencepiece
+#full# bert-tensorflow
+#full# keras
+#full# lucene
 #full# sacremoses
-#opt# transformers
-#opt# torch
-#opt# accelerate
-#opt# datasets
-#opt# diffusers
-#opt# flask
+#full# sentencepiece
+#full# tensorflow
```

### Comparing `mezcla-1.3.8/setup.py` & `mezcla-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """Simple installer"""
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla'],
       module="mezcla",
-      version='1.3.8',
+      version='1.3.9',
       description-file="README.txt",
       dist-name="Mezcla",
       ## OLD: py_modules=PYTHON_MODULE_NAMES,
       author="Tom O'Hara",
       # TODO: find out which email key is preferred
       email="tomasohara@gmail.com",
       author-email="tomasohara@gmail.com"
```

### Comparing `mezcla-1.3.8/temp/simple_batspp.py` & `mezcla-1.3.9/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/tools/run_tests.bash` & `mezcla-1.3.9/tools/run_tests.bash`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/tox.ini` & `mezcla-1.3.9/tox.ini`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.8/PKG-INFO` & `mezcla-1.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mezcla
-Version: 1.3.8
+Version: 1.3.9
 Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
 Home-page: https://github.com/tomasohara/mezcla
 License: LGPLv3
 Author: Tomás O'Hara
 Author-email: tomasohara@gmail.com
 Description-Content-Type: text/plain
```

