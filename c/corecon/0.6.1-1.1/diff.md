# Comparing `tmp/corecon-0.6.1.tar.gz` & `tmp/corecon-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/corecon-0.6.1.tar", last modified: Fri Feb 10 13:03:42 2023, max compression
+gzip compressed data, was "dist/corecon-1.1.tar", last modified: Wed Jul  5 09:28:32 2023, max compression
```

## Comparing `corecon-0.6.1.tar` & `corecon-1.1.tar`

### file list

```diff
@@ -1,183 +1,204 @@
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    34444 2022-07-14 05:00:23.000000 corecon-0.6.1/LICENSE.txt
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      116 2022-07-14 05:00:23.000000 corecon-0.6.1/MANIFEST.in
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1821 2023-02-10 13:03:42.000000 corecon-0.6.1/PKG-INFO
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      757 2022-07-14 05:00:23.000000 corecon-0.6.1/README.md
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8926 2022-12-21 16:57:54.000000 corecon-0.6.1/corecon/DataEntryClass.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     7119 2022-12-21 16:57:54.000000 corecon-0.6.1/corecon/FieldClass.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1802 2022-12-21 16:57:54.000000 corecon-0.6.1/corecon/InternalFunctions.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6010 2023-02-10 10:45:40.000000 corecon-0.6.1/corecon/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2176 2023-02-10 10:37:43.000000 corecon-0.6.1/corecon/check_updates.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/HeII_to_HI_column_density_ratio/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    19889 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/HeII_to_HI_column_density_ratio/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1104 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      964 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      830 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      754 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      792 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      885 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      918 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      885 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Garzilli_et_al_2012.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1145 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Hiss_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      970 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Lidz_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1081 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Rorai_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1551 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Schaye_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1579 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Walther_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/IGM_temperature_mean_density/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5003 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/Croft_et_al_2002.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2674 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/DAloisio_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     9025 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/McDonald_et_al_2006.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    26999 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_fourier.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    25486 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_likelihood.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/Lya_spike_galaxy_correlation/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2219 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/Lya_spike_galaxy_correlation/Kakiichi_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1530 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3433 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-07-18 13:13:33.000000 corecon-0.6.1/corecon/data/Lya_spike_galaxy_correlation/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1828 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Atek_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1785 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Atek_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5909 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1229 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1813 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      927 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1129 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Bowler_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1070 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Bowler_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      898 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Castellano_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1970 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Donnan_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5256 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      848 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1976 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Harikane_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4562 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1170 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4335 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Livermore_et_al_2017.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1075 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/McLeod_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1984 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/McLure_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      889 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Morishita_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      888 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Naidu_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1235 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Oesch_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1283 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1217 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/UV_luminosity_function/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/UV_slope/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1511 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_slope/Atek_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3110 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_slope/Austin_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4278 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_slope/Cullen_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1106 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_slope/Curtis-Lake_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1950 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_slope/Tacchella_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_slope/Topping_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1210 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_slope/Whitler_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3277 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/UV_slope/Whitler_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-07-18 13:13:33.000000 corecon-0.6.1/corecon/data/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      507 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/data_entry_template.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/dust_mass/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      843 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/dust_mass/Laporte_et_al_2017.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/effective_optical_depth_HI_Lya/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5850 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6987 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4076 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/effective_optical_depth_HI_Lya/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/effective_optical_depth_HeII_Lya/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6007 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/effective_optical_depth_HeII_Lya/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/galaxy_main_sequence/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2019 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/galaxy_main_sequence/Chen_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      867 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1642 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2885 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1538 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1863 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/ionized_fraction/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      689 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Bolton_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1129 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Bosman_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      710 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Chornock_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      729 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Choudhury_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1247 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Davies_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      632 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Dijkstra_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1105 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Fan_et_al_2006.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      661 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Greig_et_al_2017.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      664 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Greig_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      695 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Hoag_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      730 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Jensen_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      868 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Jung_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1391 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Lu_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      635 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Mason_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      800 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Mason_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      658 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/McGreer_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      674 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/McGreer_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      731 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Mesinger_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      657 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Mortlock_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      684 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Ono_et_al_2012.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      699 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Ota_et_al_2008.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      927 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Ouchi_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      957 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Pentericci_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Robertson_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      688 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Schenker_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      678 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Schroeder_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      661 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Sobacchi_Mesinger_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      936 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Tilvi_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1094 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Totani_et_al_2006.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      872 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Wang_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Yang_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1126 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/ionized_fraction/Yang_et_al_2020b.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-07-18 13:13:33.000000 corecon-0.6.1/corecon/data/ionized_fraction/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      724 2022-12-21 17:29:47.000000 corecon-0.6.1/corecon/data/make_data_archive.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/mass_gas_metallicity_relation/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      846 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mass_gas_metallicity_relation/Curti_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1357 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2834 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1043 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/mass_stellar_metallicity_relation/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1948 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1690 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/mean_free_path/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mean_free_path/Fumagalli_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      783 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mean_free_path/OMeara_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      931 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mean_free_path/Prochaska_et_al_2009.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      852 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/mean_free_path/Worseck_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/mean_free_path/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1017 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/Pagani_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      845 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/Paoletti_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      850 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/Planck_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      997 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/Planck_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1058 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/Planck_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      848 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/WMAP_5yr.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      840 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/WMAP_7yr.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      849 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/WMAP_9yr.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      860 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1348 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1337 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1040 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1147 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      897 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    28572 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1266 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4498 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Ross_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1078 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Willott_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1027 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/Yang_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-12-19 11:14:17.000000 corecon-0.6.1/corecon/data/quasar_luminosity_function/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon/data/sfrd/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      980 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/sfrd/Donnan_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      982 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/sfrd/Harikane_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4720 2023-02-10 10:44:44.000000 corecon-0.6.1/corecon/data/sfrd/Madau_and_Dickinson_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2022-07-18 13:13:33.000000 corecon-0.6.1/corecon/data/sfrd/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     7219 2022-12-21 16:57:54.000000 corecon-0.6.1/corecon/fields_info.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8796 2022-12-21 17:39:18.000000 corecon-0.6.1/corecon/loaders.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)       22 2023-02-10 13:02:45.000000 corecon-0.6.1/corecon/version.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon.egg-info/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1821 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon.egg-info/PKG-INFO
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8255 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon.egg-info/SOURCES.txt
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        1 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon.egg-info/dependency_links.txt
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        6 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon.egg-info/requires.txt
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        8 2023-02-10 13:03:42.000000 corecon-0.6.1/corecon.egg-info/top_level.txt
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)       79 2023-02-10 13:03:42.000000 corecon-0.6.1/setup.cfg
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1358 2022-12-19 11:14:17.000000 corecon-0.6.1/setup.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)    34444 2020-05-11 19:32:45.000000 corecon-1.1/LICENSE.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)      116 2020-05-11 19:32:45.000000 corecon-1.1/MANIFEST.in
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1831 2023-07-05 09:28:32.000000 corecon-1.1/PKG-INFO
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2023-07-04 09:42:56.000000 corecon-1.1/README.md
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     9015 2023-06-19 16:03:09.000000 corecon-1.1/corecon/DataEntryClass.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6926 2023-06-19 16:03:09.000000 corecon-1.1/corecon/FieldClass.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1802 2023-06-19 16:03:09.000000 corecon-1.1/corecon/InternalFunctions.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6010 2023-06-19 16:03:09.000000 corecon-1.1/corecon/__init__.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2176 2023-06-19 16:03:09.000000 corecon-1.1/corecon/check_updates.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/HeII_to_HI_column_density_ratio/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    19889 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/HeII_to_HI_column_density_ratio/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1104 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      964 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      830 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      754 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      792 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      885 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      918 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      885 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Garzilli_et_al_2012.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1145 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Hiss_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      970 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Lidz_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1081 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Rorai_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1551 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Schaye_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1579 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/Walther_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/IGM_temperature_mean_density/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/Lya_flux_power_spectrum/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5003 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/Lya_flux_power_spectrum/Croft_et_al_2002.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2674 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/Lya_flux_power_spectrum/DAloisio_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     9025 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/Lya_flux_power_spectrum/McDonald_et_al_2006.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    26999 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_fourier.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    25486 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_likelihood.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/Lya_flux_power_spectrum/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/Lya_spike_galaxy_correlation/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2219 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/Lya_spike_galaxy_correlation/Kakiichi_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1530 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3433 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2020.py
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-06-27 13:38:09.000000 corecon-1.1/corecon/data/Lya_spike_galaxy_correlation/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/UV_luminosity_function/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1828 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Atek_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1785 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Atek_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5909 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1229 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1813 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1038 2023-07-05 09:15:20.000000 corecon-1.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1129 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Bowler_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1070 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Bowler_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      898 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Castellano_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1970 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Donnan_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5256 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      848 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1976 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Harikane_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4562 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1170 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4335 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Livermore_et_al_2017.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1075 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/McLeod_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1984 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/McLure_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      889 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Morishita_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      888 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Naidu_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1235 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Oesch_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1283 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1217 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/UV_luminosity_function/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/UV_slope/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1511 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Atek_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3110 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Austin_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2565 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Bouwens_et_al_2009.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4278 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Cullen_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1106 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Curtis-Lake_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8626 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Endsley_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)   243506 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Finkelstein_et_al_2012.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2242 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Simmonds_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1950 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Tacchella_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Topping_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1210 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Whitler_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3277 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/UV_slope/Whitler_et_al_2023.py
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-05-11 19:32:45.000000 corecon-1.1/corecon/data/__init__.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      507 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/data_entry_template.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/dust_mass/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      843 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/dust_mass/Laporte_et_al_2017.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/effective_optical_depth_HI_Lya/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5850 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6987 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4076 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/effective_optical_depth_HI_Lya/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/effective_optical_depth_HeII_Lya/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6007 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/effective_optical_depth_HeII_Lya/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/galaxy_main_sequence/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2019 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/galaxy_main_sequence/Chen_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      867 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1642 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2885 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1538 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1863 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/ionized_fraction/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      689 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Bolton_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1129 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Bosman_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      710 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Chornock_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      729 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Choudhury_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1247 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Davies_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      632 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Dijkstra_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1105 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Fan_et_al_2006.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      661 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Greig_et_al_2017.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      664 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Greig_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      695 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Hoag_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      730 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Jensen_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      868 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Jung_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1391 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Lu_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      635 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Mason_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      800 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Mason_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      658 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/McGreer_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      674 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/McGreer_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      731 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Mesinger_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      657 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Mortlock_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      684 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Ono_et_al_2012.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      699 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Ota_et_al_2008.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      927 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Ouchi_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      957 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Pentericci_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Robertson_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      688 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Schenker_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      678 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Schroeder_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      661 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Sobacchi_Mesinger_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      936 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Tilvi_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1094 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Totani_et_al_2006.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      872 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Wang_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Yang_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1126 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionized_fraction/Yang_et_al_2020b.py
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-05-11 19:32:45.000000 corecon-1.1/corecon/data/ionized_fraction/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1023 2023-07-05 08:58:40.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Bouwens_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1380 2023-07-05 09:01:28.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Endsley_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      912 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Harikane_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      878 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Jung_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1124 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Lam_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      788 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Maseda_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    67827 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Prieto-Lyon_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1160 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Saxena_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2242 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/ionizing_photons_production_efficiency/Simmonds_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      724 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/make_data_archive.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      925 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Boyett_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      900 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Bunker_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      868 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Curti_et_al_2023a.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1357 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1463 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Fujimoto_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1793 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Langeroodi_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    37184 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Nakajima_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2834 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1076 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1097 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Trump_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1038 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_gas_metallicity_relation/Williams_et_al_2023.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/mass_stellar_metallicity_relation/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1948 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1690 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/mean_free_path/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mean_free_path/Fumagalli_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      783 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mean_free_path/OMeara_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      931 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mean_free_path/Prochaska_et_al_2009.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      852 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/mean_free_path/Worseck_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/mean_free_path/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/optical_depth_CMB/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1017 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/Pagani_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      845 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/Paoletti_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      850 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/Planck_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      997 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/Planck_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1058 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/Planck_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      848 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/WMAP_5yr.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      840 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/WMAP_7yr.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      849 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/WMAP_9yr.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/optical_depth_CMB/__init__.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      860 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/quasar_luminosity_function/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1348 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1337 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1040 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1147 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      897 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    28572 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1266 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4498 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Ross_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1078 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Willott_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1027 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/quasar_luminosity_function/Yang_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.1/corecon/data/quasar_luminosity_function/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon/data/sfrd/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      980 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/sfrd/Donnan_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      982 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/sfrd/Harikane_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4720 2023-07-05 08:45:19.000000 corecon-1.1/corecon/data/sfrd/Madau_and_Dickinson_2014.py
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-06-23 15:25:46.000000 corecon-1.1/corecon/data/sfrd/__init__.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     7732 2023-07-04 09:55:09.000000 corecon-1.1/corecon/fields_info.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8799 2023-06-20 08:06:03.000000 corecon-1.1/corecon/loaders.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)       20 2023-07-05 09:25:43.000000 corecon-1.1/corecon/version.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2023-07-05 09:28:32.000000 corecon-1.1/corecon.egg-info/
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)     1831 2023-07-05 09:28:32.000000 corecon-1.1/corecon.egg-info/PKG-INFO
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)     9557 2023-07-05 09:28:32.000000 corecon-1.1/corecon.egg-info/SOURCES.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        1 2023-07-05 09:28:32.000000 corecon-1.1/corecon.egg-info/dependency_links.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        6 2023-07-05 09:28:32.000000 corecon-1.1/corecon.egg-info/requires.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        8 2023-07-05 09:28:32.000000 corecon-1.1/corecon.egg-info/top_level.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)       79 2023-07-05 09:28:32.000000 corecon-1.1/setup.cfg
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1358 2023-06-19 16:03:09.000000 corecon-1.1/setup.py
```

### Comparing `corecon-0.6.1/LICENSE.txt` & `corecon-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/PKG-INFO` & `corecon-1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: corecon
-Version: 0.6.1
+Version: 1.1
 Summary: an open collection of constraints on the Epoch of Reionization
 Home-page: https://github.com/EGaraldi/corecon
-Download-URL: https://github.com/EGaraldi/corecon/archive/v0.6.1.tar.gz
+Download-URL: https://github.com/EGaraldi/corecon/archive/v1.1.tar.gz
 Author: Enrico Garaldi
 Author-email: enrico.garaldi@gmail.com
 License: gpl-3.0
 Keywords: constraints,reionization,cosmic,observations,data
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -21,15 +20,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.txt
 
 ![](logo.png)
 
-![](https://travis-ci.org/EGaraldi/corecon.svg?branch=master)
+[![DOI](https://zenodo.org/badge/224433919.svg)](https://zenodo.org/badge/latestdoi/224433919)
+
 
 CoReCon: open collection of Reionization Constraints
 ====================================================
 
 **CoReCon** is an open collection of constraints on various physical
 quantities linked to the *Epoch of Reionization (EoR)*.
 
@@ -38,9 +38,7 @@
 input data.
 
 CoReCon takes care of loading and interpreting the data, and presenting them
 in an organic and ready-to-use way. It also implement simple slicing capabilities,
 which allow to perform simple data filtering.
 
 See https://corecon.readthedocs.io/en/latest/ for the latest documentation.
-
-
```

### Comparing `corecon-0.6.1/README.md` & `corecon-1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ![](logo.png)
 
-![](https://travis-ci.org/EGaraldi/corecon.svg?branch=master)
+[![DOI](https://zenodo.org/badge/224433919.svg)](https://zenodo.org/badge/latestdoi/224433919)
+
 
 CoReCon: open collection of Reionization Constraints
 ====================================================
 
 **CoReCon** is an open collection of constraints on various physical
 quantities linked to the *Epoch of Reionization (EoR)*.
```

### Comparing `corecon-0.6.1/corecon/DataEntryClass.py` & `corecon-1.1/corecon/DataEntryClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         self.extra_data = np.array(self.extra_data)
 
         #create named entries
         setattr(self, parent_field, values[:])
         for k, descr in enumerate(dimensions_descriptors):
             descr = descr.replace(" ", "_")
             descr = ''.join(ch if ch.isalnum() or ch=="_" else '' for ch in descr)
-            setattr(self, descr, axes[:,k])
+            if ndim==1:
+                setattr(self, descr, axes)
+            else:
+                setattr(self, descr, axes[:,k])
 
     def __repr__(self):
         """string describing the class
         """
         return "corecon DataEntry class"
 
     def __str__(self):
```

### Comparing `corecon-0.6.1/corecon/FieldClass.py` & `corecon-1.1/corecon/FieldClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,26 +88,19 @@
             raise ValueError("zmax cannot be smaller than zmin, you provided zmin = "+str(zmin)+" and zmax="+str(zmax))
 
         dict_zslice = Field()
         dict_zslice.field_symbol      = self.field_symbol      
         dict_zslice.field_description = self.field_description 
 
         for k in self.keys():
-            w = (self[k].dimensions_descriptors == 'redshift')
-            if not np.any(w):
+            if not 'redshift' in self[k].dimensions_descriptors:
                 print("WARNING: missing redshift dimension for entry %s. Skipping it."%(k))
                 continue
-            zdim = np.where(w)[0][0]
             
-            if self[k].ndim == 1:
-                redshift = self[k].axes
-            else:
-                redshift = self[k].axes[:,zdim]
-
-            w = (zmin <= redshift) & (redshift < zmax)
+            w = (zmin <= self[k].redshift) & (self[k].redshift < zmax)
             if any(w):
                 dict_zslice[k] = copy.deepcopy(self[k])
                 dict_zslice[k].axes      = dict_zslice[k].axes     [w]
                 dict_zslice[k].values    = dict_zslice[k].values   [w]
                 dict_zslice[k].err_up    = dict_zslice[k].err_up   [w]
                 dict_zslice[k].err_down  = dict_zslice[k].err_down [w]
                 dict_zslice[k].upper_lim = dict_zslice[k].upper_lim[w]
@@ -184,13 +177,13 @@
                 dict_uls[k].axes      = dict_uls[k].axes     [self[k].upper_lim]
                 dict_uls[k].values    = dict_uls[k].values   [self[k].upper_lim]
                 dict_uls[k].err_up    = dict_uls[k].err_up   [self[k].upper_lim]
                 dict_uls[k].err_down  = dict_uls[k].err_down [self[k].upper_lim]
                 dict_uls[k].upper_lim = dict_uls[k].upper_lim[self[k].upper_lim]
                 dict_uls[k].lower_lim = dict_uls[k].lower_lim[self[k].upper_lim]
                 
-                for e in dict_ulls[k].extra_data:
-                    _temp = getattr(dict_ulls[k], e)
-                    setattr(dict_ulls[k], e, _temp[self[k].upper_lim])
+                for e in dict_uls[k].extra_data:
+                    _temp = getattr(dict_uls[k], e)
+                    setattr(dict_uls[k], e, _temp[self[k].upper_lim])
 
         return dict_uls
```

### Comparing `corecon-0.6.1/corecon/InternalFunctions.py` & `corecon-1.1/corecon/InternalFunctions.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/__init__.py` & `corecon-1.1/corecon/__init__.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/check_updates.py` & `corecon-1.1/corecon/check_updates.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py` & `corecon-1.1/corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2014.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2020.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Garzilli_et_al_2012.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Garzilli_et_al_2012.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Hiss_et_al_2018.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Hiss_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Lidz_et_al_2010.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Lidz_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Rorai_et_al_2018.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Rorai_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Schaye_et_al_2010.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Schaye_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/IGM_temperature_mean_density/Walther_et_al_2019.py` & `corecon-1.1/corecon/data/IGM_temperature_mean_density/Walther_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/Croft_et_al_2002.py` & `corecon-1.1/corecon/data/Lya_flux_power_spectrum/Croft_et_al_2002.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/DAloisio_et_al_2018.py` & `corecon-1.1/corecon/data/Lya_flux_power_spectrum/DAloisio_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/McDonald_et_al_2006.py` & `corecon-1.1/corecon/data/Lya_flux_power_spectrum/McDonald_et_al_2006.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_fourier.py` & `corecon-1.1/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_fourier.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_likelihood.py` & `corecon-1.1/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_likelihood.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/Lya_spike_galaxy_correlation/Kakiichi_et_al_2018.py` & `corecon-1.1/corecon/data/Lya_spike_galaxy_correlation/Kakiichi_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2019.py` & `corecon-1.1/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2020.py` & `corecon-1.1/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Atek_et_al_2015.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Atek_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Atek_et_al_2018.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Atek_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2022.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Bouwens_et_al_2022.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-dictionary_tag         = "Bouwens et al. 2022"
+dictionary_tag         = "Bouwens et al. 2023"
 
-reference              = "Bouwens, Stefanon, Brammer, Oesch, Herard-Demanche, Illingworth, et al., sub."
+reference              = "Bouwens, Stefanon, Brammer, Oesch, Herard-Demanche, Illingworth, et al., MNRAS 523, 1936 (2023)"
 
-url                    = "https://arxiv.org/pdf/2211.02607.pdf"
+url                    = "https://ui.adsabs.harvard.edu/abs/2023MNRAS.523.1036B/abstract"
 
 description            = \
 """
 Based on JWST NIRCam observations of galaxies in the HUDF. Total of 10 galaxies at 8 < z < 13.
 """
 
 data_structure         = "points" #grid or points
 
 extracted              = False
 
 ndim                   = 2
 
 dimensions_descriptors = ["redshift", "M_UV"]
 
-axes                   = [[8.7, -20.02], [8.7, -18.77], [10.5, -18.65], [12.6, -20.31], [12.6, -19.31]]
+axes                   = [[8.7, -20.02], [8.7, -18.77], [10.5, -18.9], [10.5, -17.9], [12.6, -20.06], [12.6, -18.81]]
 
-values                 = [0.000164, 0.000378, 0.00029 , 0.000116, 0.00019 ]
+values                 = [-3.77989191, -3.59859946, -4.06550155, -3.12726117, -4.1079054 ,-3.7212464 ]
+ 
+err_up                 = [0.25410818, 0.29930318, 0.37936877, 0.29869507, 0.25403343,  0.25527251]
 
-err_up                 = [0.29837375, 0.2575643 , 0.26023592, 0.25776131, 0.25527251]
-
-err_down               = [1.91381385, 0.7201593 , 0.74639465, 0.72203531, 0.69897   ]
+err_down               = [0.68862917, 2.10037055,     np.inf, 1.96964884, 0.68797462, 0.69897   ]
 
 upper_lim              = False
 
 lower_lim              = False
```

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Bowler_et_al_2015.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Bowler_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Bowler_et_al_2020.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Bowler_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Castellano_et_al_2016.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Castellano_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Donnan_et_al_2022.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Donnan_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Harikane_et_al_2022.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Harikane_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Livermore_et_al_2017.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Livermore_et_al_2017.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/McLeod_et_al_2016.py` & `corecon-1.1/corecon/data/UV_luminosity_function/McLeod_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/McLure_et_al_2013.py` & `corecon-1.1/corecon/data/UV_luminosity_function/McLure_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Morishita_et_al_2018.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Morishita_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Naidu_et_al_2022.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Naidu_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Oesch_et_al_2014.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Oesch_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py` & `corecon-1.1/corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_slope/Atek_et_al_2023.py` & `corecon-1.1/corecon/data/UV_slope/Atek_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_slope/Austin_et_al_2023.py` & `corecon-1.1/corecon/data/UV_slope/Austin_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_slope/Cullen_et_al_2023.py` & `corecon-1.1/corecon/data/UV_slope/Cullen_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_slope/Curtis-Lake_et_al_2022.py` & `corecon-1.1/corecon/data/UV_slope/Curtis-Lake_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_slope/Tacchella_et_al_2022.py` & `corecon-1.1/corecon/data/UV_slope/Tacchella_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_slope/Topping_et_al_2022.py` & `corecon-1.1/corecon/data/UV_slope/Topping_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_slope/Whitler_et_al_2022.py` & `corecon-1.1/corecon/data/UV_slope/Whitler_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/UV_slope/Whitler_et_al_2023.py` & `corecon-1.1/corecon/data/UV_slope/Whitler_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/dust_mass/Laporte_et_al_2017.py` & `corecon-1.1/corecon/data/dust_mass/Laporte_et_al_2017.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py` & `corecon-1.1/corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py` & `corecon-1.1/corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2020.py` & `corecon-1.1/corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py` & `corecon-1.1/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/galaxy_main_sequence/Chen_et_al_2022.py` & `corecon-1.1/corecon/data/galaxy_main_sequence/Chen_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py` & `corecon-1.1/corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py` & `corecon-1.1/corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py` & `corecon-1.1/corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py` & `corecon-1.1/corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py` & `corecon-1.1/corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Bolton_et_al_2011.py` & `corecon-1.1/corecon/data/ionized_fraction/Bolton_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Bosman_et_al_2022.py` & `corecon-1.1/corecon/data/ionized_fraction/Bosman_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Chornock_et_al_2013.py` & `corecon-1.1/corecon/data/ionized_fraction/Chornock_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Choudhury_et_al_2015.py` & `corecon-1.1/corecon/data/ionized_fraction/Choudhury_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Davies_et_al_2018.py` & `corecon-1.1/corecon/data/ionized_fraction/Davies_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Dijkstra_et_al_2011.py` & `corecon-1.1/corecon/data/ionized_fraction/Dijkstra_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Fan_et_al_2006.py` & `corecon-1.1/corecon/data/ionized_fraction/Fan_et_al_2006.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Greig_et_al_2017.py` & `corecon-1.1/corecon/data/ionized_fraction/Greig_et_al_2017.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Greig_et_al_2019.py` & `corecon-1.1/corecon/data/ionized_fraction/Greig_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Hoag_et_al_2019.py` & `corecon-1.1/corecon/data/ionized_fraction/Hoag_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Jensen_et_al_2013.py` & `corecon-1.1/corecon/data/ionized_fraction/Jensen_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Jung_et_al_2020.py` & `corecon-1.1/corecon/data/ionized_fraction/Jung_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Lu_et_al_2020.py` & `corecon-1.1/corecon/data/ionized_fraction/Lu_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Mason_et_al_2018.py` & `corecon-1.1/corecon/data/ionized_fraction/Mason_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Mason_et_al_2019.py` & `corecon-1.1/corecon/data/ionized_fraction/Mason_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/McGreer_et_al_2011.py` & `corecon-1.1/corecon/data/ionized_fraction/McGreer_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/McGreer_et_al_2015.py` & `corecon-1.1/corecon/data/ionized_fraction/McGreer_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Mesinger_et_al_2015.py` & `corecon-1.1/corecon/data/ionized_fraction/Mesinger_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Mortlock_et_al_2011.py` & `corecon-1.1/corecon/data/ionized_fraction/Mortlock_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Ono_et_al_2012.py` & `corecon-1.1/corecon/data/ionized_fraction/Ono_et_al_2012.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Ota_et_al_2008.py` & `corecon-1.1/corecon/data/ionized_fraction/Ota_et_al_2008.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Ouchi_et_al_2010.py` & `corecon-1.1/corecon/data/ionized_fraction/Ouchi_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Pentericci_et_al_2014.py` & `corecon-1.1/corecon/data/ionized_fraction/Pentericci_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Robertson_et_al_2013.py` & `corecon-1.1/corecon/data/ionized_fraction/Robertson_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Schenker_et_al_2014.py` & `corecon-1.1/corecon/data/ionized_fraction/Schenker_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Schroeder_et_al_2013.py` & `corecon-1.1/corecon/data/ionized_fraction/Schroeder_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Sobacchi_Mesinger_2015.py` & `corecon-1.1/corecon/data/ionized_fraction/Sobacchi_Mesinger_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Tilvi_et_al_2014.py` & `corecon-1.1/corecon/data/ionized_fraction/Tilvi_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Totani_et_al_2006.py` & `corecon-1.1/corecon/data/ionized_fraction/Totani_et_al_2006.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Wang_et_al_2020.py` & `corecon-1.1/corecon/data/ionized_fraction/Wang_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Yang_et_al_2020.py` & `corecon-1.1/corecon/data/ionized_fraction/Yang_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/ionized_fraction/Yang_et_al_2020b.py` & `corecon-1.1/corecon/data/ionized_fraction/Yang_et_al_2020b.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/make_data_archive.py` & `corecon-1.1/corecon/data/make_data_archive.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py` & `corecon-1.1/corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py` & `corecon-1.1/corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py` & `corecon-1.1/corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 dictionary_tag         = "Schaerer et al. 2022"
 
-reference              = "Schaerer, Marques-Chaves, Oesch, Naidu, Barrufet, et al.; subm. (2022)"
+reference              = "Schaerer, Marques-Chaves, Oesch, Naidu, Barrufet, et al.; A&A 665L 4 (2022)"
 
-url                    = "https://arxiv.org/pdf/2207.10034.pdf"
+url                    = "https://ui.adsabs.harvard.edu/abs/2022A%26A...665L...4S/abstract"
 
 description            = \
 """
 From the ERO JWST observations of SMACS J0723.3-7327 with NIRSpec. Based on two galaxies at z=7.7 and one at z=8.5.
 NOTE: The authors provide 3 determinations of O/H. We use as fiducial value the "direct" method when available and the "strong line" 
 when not. The upper/lower error encloses the range of values obtained with the three methods.
 """
```

### Comparing `corecon-0.6.1/corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py` & `corecon-1.1/corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py` & `corecon-1.1/corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/mean_free_path/Fumagalli_et_al_2013.py` & `corecon-1.1/corecon/data/mean_free_path/Fumagalli_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/mean_free_path/OMeara_et_al_2013.py` & `corecon-1.1/corecon/data/mean_free_path/OMeara_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/mean_free_path/Prochaska_et_al_2009.py` & `corecon-1.1/corecon/data/mean_free_path/Prochaska_et_al_2009.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/mean_free_path/Worseck_et_al_2014.py` & `corecon-1.1/corecon/data/mean_free_path/Worseck_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/Pagani_et_al_2020.py` & `corecon-1.1/corecon/data/optical_depth_CMB/Pagani_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/Paoletti_et_al_2020.py` & `corecon-1.1/corecon/data/optical_depth_CMB/Paoletti_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/Planck_2013.py` & `corecon-1.1/corecon/data/optical_depth_CMB/Planck_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/Planck_2015.py` & `corecon-1.1/corecon/data/optical_depth_CMB/Planck_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/Planck_2018.py` & `corecon-1.1/corecon/data/optical_depth_CMB/Planck_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/WMAP_5yr.py` & `corecon-1.1/corecon/data/optical_depth_CMB/WMAP_5yr.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/WMAP_7yr.py` & `corecon-1.1/corecon/data/optical_depth_CMB/WMAP_7yr.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/WMAP_9yr.py` & `corecon-1.1/corecon/data/optical_depth_CMB/WMAP_9yr.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py` & `corecon-1.1/corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Ross_et_al_2013.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Ross_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Willott_et_al_2010.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Willott_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/quasar_luminosity_function/Yang_et_al_2016.py` & `corecon-1.1/corecon/data/quasar_luminosity_function/Yang_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/sfrd/Donnan_et_al_2022.py` & `corecon-1.1/corecon/data/sfrd/Donnan_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/sfrd/Harikane_et_al_2022.py` & `corecon-1.1/corecon/data/sfrd/Harikane_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/data/sfrd/Madau_and_Dickinson_2014.py` & `corecon-1.1/corecon/data/sfrd/Madau_and_Dickinson_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-0.6.1/corecon/fields_info.py` & `corecon-1.1/corecon/fields_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
-__fields_info__ = {  "ionized_fraction"                  : { "synonyms" : ['x_HII', 'f_HII', 'x_ion', 'f_ion', 'ion_frac']                                                         , "description" : "Ionized fraction"                                            , "symbol" : r"$x_\mathrm{HII}$"                                                          , "units" : ""             , "remarks": "volume-averaged", "required_fields" : ["redshift"]}  ,
-                     "Lya_flux_power_spectrum"           : { "synonyms" : ['Lya_flux_PS']                                                                                          , "description" : "Ly-alpha flux power spectrum"                                , "symbol" : r"$P\, [\mathrm{km/s}]$"                                                     , "units" : "km/s"         , "remarks": ""               , "required_fields" : ["redshift"]}  , 
-                     "mean_free_path"                    : { "synonyms" : ['mfp', 'lambda_mfp', 'lambda_ion', 'lambda_912', 'mfp_912', 'mfp_ion']                                  , "description" : "Mean free path of ionising photons"                          , "symbol" : r"$\lambda_\mathrm{mfp} \, [h^{-1} \, \mathrm{Mpc}]$"                        , "units" : "Mpc/h"        , "remarks": ""               , "required_fields" : ["redshift"]}  , 
-                     "effective_optical_depth_HI_Lya"    : { "synonyms" : ['tau_HI', 'tau_eff_HI']                                                                                 , "description" : "HI Ly-alpha effective optical depth"                         , "symbol" : r"$\tau_\mathrm{eff, HI}$"                                                   , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
-                     "effective_optical_depth_HeII_Lya"  : { "synonyms" : ['tau_HeII', 'tau_eff_HeII']                                                                             , "description" : "HeII Ly-alpha effective optical depth"                       , "symbol" : r"$\tau_\mathrm{eff, HeII}$"                                                 , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
-                     "HeII_to_HI_column_density_ratio"   : { "synonyms" : ['eta']                                                                                                  , "description" : "HeII-to-HI column density ratio"                             , "symbol" : r"$\eta$"                                                                    , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
-                     "quasar_luminosity_function"        : { "synonyms" : ['QLF', 'QSOLF']                                                                                         , "description" : "Quasar luminosity function"                                  , "symbol" : r"$\log_{10} (phi_\mathrm{QSO}) \, [\mathrm{Mpc}^{-3} \, \mathrm{mag}^{-1}]$", "units" : "Mpc^-3 mag^-1", "remarks": ""               , "required_fields" : ["redshift", "M_1450"]}  , 
-                     "UV_luminosity_function"            : { "synonyms" : ['UVLF']                                                                                                 , "description" : "Galaxy UV luminosity function"                               , "symbol" : r"$\log_{10} (phi_\mathrm{UV}) \, [\mathrm{Mpc}^{-3} \, \mathrm{mag}^{-1}]$" , "units" : "Mpc^-3 mag^-1", "remarks": ""               , "required_fields" : ["redshift", "M_UV"]  }  , 
-                     "IGM_temperature_mean_density"      : { "synonyms" : ['T0']                                                                                                   , "description" : "IGM temperature at mean density"                             , "symbol" : r"T0 [K]"                                                                    , "units" : "K"            , "remarks": ""               , "required_fields" : ["redshift"]}  , 
-                     "optical_depth_CMB"                 : { "synonyms" : ['tau_cmb', 'tau_CMB']                                                                                   , "description" : "CMB optical depth"                                           , "symbol" : r"$\tau_\mathrm{CMB}$"                                                       , "units" : ""             , "remarks": ""               , "required_fields" : []          }  , 
-                     "sfrd"                              : { "synonyms" : ['SFRD', 'star formation rate density', 'star-formation-rate density', 'star-formation rate density']    , "description" : "Star-formation-rate density"                                 , "symbol" : r"$\log \Psi \, [\mathrm{M}_\odot \mathrm{yr}^{-1} \mathrm{Mpc}^{-3}]$"      , "units" : "Msun/yr/Mpc^3", "remarks": ""               , "required_fields" : ["redshift"]}  , 
-                     "Lya_spike_galaxy_correlation"      : { "synonyms" : []                                                                                                       , "description" : "Ly-alpha spike - galaxy correlation"                         , "symbol" : r"$\langle f \rangle / \bar{f} - 1$"                                         , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  ,
-                     "mass_stellar_metallicity_relation" : { "synonyms" : ['stellar MZR']                                                                                          , "description" : "Stellar metallicity as function of galaxy stellar mass"      , "symbol" : r"$\log(Z/Z_\odot)$"                                                         , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
-                     "mass_gas_metallicity_relation"     : { "synonyms" : ['gas MZR']                                                                                              , "description" : "Gas-phase O/H metallicity as function of galaxy stellar mass", "symbol" : r"$\log(O/H) + 12$"                                                          , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
-                     "galaxy_main_sequence"              : { "synonyms" : ['GMS']                                                                                                  , "description" : "Star formation rate  as function of galaxy stellar mass"     , "symbol" : r"SFR [M$_\odot$/yr]"                                                        , "units" : "Msun/yr"      , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
-                     "UV_slope"                          : { "synonyms" : ['beta_UV']                                                                                              , "description" : "Slope of the galaxy UV log flux density"                     , "symbol" : r"$\beta$"                                                                   , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  ,
+__fields_info__ = {  "ionized_fraction"                      : { "synonyms" : ['x_HII', 'f_HII', 'x_ion', 'f_ion', 'ion_frac']                                                         , "description" : "Ionized fraction"                                            , "symbol" : r"$x_\mathrm{HII}$"                                                          , "units" : ""             , "remarks": "volume-averaged", "required_fields" : ["redshift"]}  ,
+                     "Lya_flux_power_spectrum"               : { "synonyms" : ['Lya_flux_PS']                                                                                          , "description" : "Ly-alpha flux power spectrum"                                , "symbol" : r"$P\, [\mathrm{km/s}]$"                                                     , "units" : "km/s"         , "remarks": ""               , "required_fields" : ["redshift"]}  , 
+                     "mean_free_path"                        : { "synonyms" : ['mfp', 'lambda_mfp', 'lambda_ion', 'lambda_912', 'mfp_912', 'mfp_ion']                                  , "description" : "Mean free path of ionising photons"                          , "symbol" : r"$\lambda_\mathrm{mfp} \, [h^{-1} \, \mathrm{Mpc}]$"                        , "units" : "Mpc/h"        , "remarks": ""               , "required_fields" : ["redshift"]}  , 
+                     "effective_optical_depth_HI_Lya"        : { "synonyms" : ['tau_HI', 'tau_eff_HI']                                                                                 , "description" : "HI Ly-alpha effective optical depth"                         , "symbol" : r"$\tau_\mathrm{eff, HI}$"                                                   , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
+                     "effective_optical_depth_HeII_Lya"      : { "synonyms" : ['tau_HeII', 'tau_eff_HeII']                                                                             , "description" : "HeII Ly-alpha effective optical depth"                       , "symbol" : r"$\tau_\mathrm{eff, HeII}$"                                                 , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
+                     "HeII_to_HI_column_density_ratio"       : { "synonyms" : ['eta']                                                                                                  , "description" : "HeII-to-HI column density ratio"                             , "symbol" : r"$\eta$"                                                                    , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
+                     "quasar_luminosity_function"            : { "synonyms" : ['QLF', 'QSOLF']                                                                                         , "description" : "Quasar luminosity function"                                  , "symbol" : r"$\log_{10} (phi_\mathrm{QSO}) \, [\mathrm{Mpc}^{-3} \, \mathrm{mag}^{-1}]$", "units" : "Mpc^-3 mag^-1", "remarks": ""               , "required_fields" : ["redshift", "M_1450"]}  , 
+                     "UV_luminosity_function"                : { "synonyms" : ['UVLF']                                                                                                 , "description" : "Galaxy UV luminosity function"                               , "symbol" : r"$\log_{10} (phi_\mathrm{UV}) \, [\mathrm{Mpc}^{-3} \, \mathrm{mag}^{-1}]$" , "units" : "Mpc^-3 mag^-1", "remarks": ""               , "required_fields" : ["redshift", "M_UV"]  }  , 
+                     "IGM_temperature_mean_density"          : { "synonyms" : ['T0']                                                                                                   , "description" : "IGM temperature at mean density"                             , "symbol" : r"T0 [K]"                                                                    , "units" : "K"            , "remarks": ""               , "required_fields" : ["redshift"]}  , 
+                     "optical_depth_CMB"                     : { "synonyms" : ['tau_cmb', 'tau_CMB']                                                                                   , "description" : "CMB optical depth"                                           , "symbol" : r"$\tau_\mathrm{CMB}$"                                                       , "units" : ""             , "remarks": ""               , "required_fields" : []          }  , 
+                     "sfrd"                                  : { "synonyms" : ['SFRD', 'star formation rate density', 'star-formation-rate density', 'star-formation rate density']    , "description" : "Star-formation-rate density"                                 , "symbol" : r"$\log \Psi \, [\mathrm{M}_\odot \mathrm{yr}^{-1} \mathrm{Mpc}^{-3}]$"      , "units" : "Msun/yr/Mpc^3", "remarks": ""               , "required_fields" : ["redshift"]}  , 
+                     "Lya_spike_galaxy_correlation"          : { "synonyms" : []                                                                                                       , "description" : "Ly-alpha spike - galaxy correlation"                         , "symbol" : r"$\langle f \rangle / \bar{f} - 1$"                                         , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  ,
+                     "mass_stellar_metallicity_relation"     : { "synonyms" : ['stellar MZR']                                                                                          , "description" : "Stellar metallicity as function of galaxy stellar mass"      , "symbol" : r"$\log(Z/Z_\odot)$"                                                         , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
+                     "mass_gas_metallicity_relation"         : { "synonyms" : ['gas MZR']                                                                                              , "description" : "Gas-phase O/H metallicity as function of galaxy stellar mass", "symbol" : r"$\log(O/H) + 12$"                                                          , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
+                     "galaxy_main_sequence"                  : { "synonyms" : ['GMS']                                                                                                  , "description" : "Star formation rate  as function of galaxy stellar mass"     , "symbol" : r"SFR [M$_\odot$/yr]"                                                        , "units" : "Msun/yr"      , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
+                     "UV_slope"                              : { "synonyms" : ['beta_UV']                                                                                              , "description" : "Slope of the galaxy UV log flux density"                     , "symbol" : r"$\beta$"                                                                   , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  ,
+                     "ionizing_photons_production_efficiency": { "synonyms" : ['xi_ion', 'csi_ion', 'ionizing_photon_production_efficiency', 'UV_to_ionizing_photons_conversion']      , "description" : "Number of ionizing photons produced per unit UV luminosity"  , "symbol" : r"$\xi_\mathrm{ion}$"                                                        , "units" : "Hz erg^-1"    , "remarks": ""               , "required_fields" : ["redshift"]}  ,
                   }
```

### Comparing `corecon-0.6.1/corecon/loaders.py` & `corecon-1.1/corecon/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
             #assert( len(values) == Npts )
             for arr in [values, err_up, err_down, lower_lim, upper_lim]:
                 assert( len(arr) == Npts )
             for k in extra_data.keys():
                 assert( len(extra_data[k]) == Npts )
 
     #special treatment for 1-dim data
-    if ndim == 1:
-        axes = axes.reshape((*axes.shape,1))
+    #if ndim == 1:
+    #    axes = axes.reshape((*axes.shape,1))
 
 
     #transform a grid into a list
     if (ndim > 1) and (data_structure == 'grid'):
         values    = values   .flatten() 
         err_up    = err_up   .flatten() 
         err_down  = err_down .flatten() 
@@ -183,8 +183,8 @@
         for filename in files:
             if filename=='__init__.py':
                 continue
             filepath = os.path.join(fieldpath, filename)
             try:
                 _LoadDataIntoDictionary(filepath, dicts[field], field)
             except:
-                print(f"WARNING: Cannot load {filename}. Skipping it.")
+                print(f"WARNING: Cannot load {filename}. Skipping it.")
```

### Comparing `corecon-0.6.1/corecon.egg-info/PKG-INFO` & `corecon-1.1/corecon.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: corecon
-Version: 0.6.1
+Version: 1.1
 Summary: an open collection of constraints on the Epoch of Reionization
 Home-page: https://github.com/EGaraldi/corecon
-Download-URL: https://github.com/EGaraldi/corecon/archive/v0.6.1.tar.gz
+Download-URL: https://github.com/EGaraldi/corecon/archive/v1.1.tar.gz
 Author: Enrico Garaldi
 Author-email: enrico.garaldi@gmail.com
 License: gpl-3.0
 Keywords: constraints,reionization,cosmic,observations,data
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -21,15 +20,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.txt
 
 ![](logo.png)
 
-![](https://travis-ci.org/EGaraldi/corecon.svg?branch=master)
+[![DOI](https://zenodo.org/badge/224433919.svg)](https://zenodo.org/badge/latestdoi/224433919)
+
 
 CoReCon: open collection of Reionization Constraints
 ====================================================
 
 **CoReCon** is an open collection of constraints on various physical
 quantities linked to the *Epoch of Reionization (EoR)*.
 
@@ -38,9 +38,7 @@
 input data.
 
 CoReCon takes care of loading and interpreting the data, and presenting them
 in an organic and ready-to-use way. It also implement simple slicing capabilities,
 which allow to perform simple data filtering.
 
 See https://corecon.readthedocs.io/en/latest/ for the latest documentation.
-
-
```

### Comparing `corecon-0.6.1/corecon.egg-info/SOURCES.txt` & `corecon-1.1/corecon.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,20 @@
 corecon/data/UV_luminosity_function/Naidu_et_al_2022.py
 corecon/data/UV_luminosity_function/Oesch_et_al_2014.py
 corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py
 corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py
 corecon/data/UV_luminosity_function/__init__.py
 corecon/data/UV_slope/Atek_et_al_2023.py
 corecon/data/UV_slope/Austin_et_al_2023.py
+corecon/data/UV_slope/Bouwens_et_al_2009.py
 corecon/data/UV_slope/Cullen_et_al_2023.py
 corecon/data/UV_slope/Curtis-Lake_et_al_2022.py
+corecon/data/UV_slope/Endsley_et_al_2022.py
+corecon/data/UV_slope/Finkelstein_et_al_2012.py
+corecon/data/UV_slope/Simmonds_et_al_2023.py
 corecon/data/UV_slope/Tacchella_et_al_2022.py
 corecon/data/UV_slope/Topping_et_al_2022.py
 corecon/data/UV_slope/Whitler_et_al_2022.py
 corecon/data/UV_slope/Whitler_et_al_2023.py
 corecon/data/dust_mass/Laporte_et_al_2017.py
 corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py
 corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py
@@ -119,18 +123,34 @@
 corecon/data/ionized_fraction/Sobacchi_Mesinger_2015.py
 corecon/data/ionized_fraction/Tilvi_et_al_2014.py
 corecon/data/ionized_fraction/Totani_et_al_2006.py
 corecon/data/ionized_fraction/Wang_et_al_2020.py
 corecon/data/ionized_fraction/Yang_et_al_2020.py
 corecon/data/ionized_fraction/Yang_et_al_2020b.py
 corecon/data/ionized_fraction/__init__.py
-corecon/data/mass_gas_metallicity_relation/Curti_et_al_2022.py
+corecon/data/ionizing_photons_production_efficiency/Bouwens_et_al_2016.py
+corecon/data/ionizing_photons_production_efficiency/Endsley_et_al_2022.py
+corecon/data/ionizing_photons_production_efficiency/Harikane_et_al_2018.py
+corecon/data/ionizing_photons_production_efficiency/Jung_et_al_2023.py
+corecon/data/ionizing_photons_production_efficiency/Lam_et_al_2019.py
+corecon/data/ionizing_photons_production_efficiency/Maseda_et_al_2020.py
+corecon/data/ionizing_photons_production_efficiency/Prieto-Lyon_et_al_2023.py
+corecon/data/ionizing_photons_production_efficiency/Saxena_et_al_2023.py
+corecon/data/ionizing_photons_production_efficiency/Simmonds_et_al_2023.py
+corecon/data/mass_gas_metallicity_relation/Boyett_et_al_2023.py
+corecon/data/mass_gas_metallicity_relation/Bunker_et_al_2023.py
+corecon/data/mass_gas_metallicity_relation/Curti_et_al_2023a.py
 corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py
+corecon/data/mass_gas_metallicity_relation/Fujimoto_et_al_2023.py
+corecon/data/mass_gas_metallicity_relation/Langeroodi_et_al_2022.py
+corecon/data/mass_gas_metallicity_relation/Nakajima_et_al_2023.py
 corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py
 corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py
+corecon/data/mass_gas_metallicity_relation/Trump_et_al_2023.py
+corecon/data/mass_gas_metallicity_relation/Williams_et_al_2023.py
 corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py
 corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py
 corecon/data/mean_free_path/Fumagalli_et_al_2013.py
 corecon/data/mean_free_path/OMeara_et_al_2013.py
 corecon/data/mean_free_path/Prochaska_et_al_2009.py
 corecon/data/mean_free_path/Worseck_et_al_2014.py
 corecon/data/mean_free_path/__init__.py
```

### Comparing `corecon-0.6.1/setup.py` & `corecon-1.1/setup.py`

 * *Files identical despite different names*

