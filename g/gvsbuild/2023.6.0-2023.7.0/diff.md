# Comparing `tmp/gvsbuild-2023.6.0.tar.gz` & `tmp/gvsbuild-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvsbuild-2023.6.0.tar", max compression
+gzip compressed data, was "gvsbuild-2023.7.0.tar", max compression
```

## Comparing `gvsbuild-2023.6.0.tar` & `gvsbuild-2023.7.0.tar`

### file list

```diff
@@ -1,962 +1,961 @@
--rw-r--r--   0        0        0       37 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/__init__.py
--rw-r--r--   0        0        0    16308 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/build.py
--rw-r--r--   0        0        0     7322 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/deps.py
--rw-r--r--   0        0        0     2243 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/groups.py
--rw-r--r--   0        0        0     5637 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/list.py
--rw-r--r--   0        0        0     1811 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/main.py
--rw-r--r--   0        0        0     2683 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/outdated.py
--rw-r--r--   0        0        0     5700 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/adwaita-icon-theme/add_meson_build.patch
--rw-r--r--   0        0        0        0 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/adwaita-icon-theme/Adwaita/64x64/ui/.empty
--rw-r--r--   0        0        0        0 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/adwaita-icon-theme/Adwaita/96x96/ui/.empty
--rw-r--r--   0        0        0      213 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/check_utils.c
--rw-r--r--   0        0        0      537 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/check_utils.h
--rw-r--r--   0        0        0    18437 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/COPYING
--rw-r--r--   0        0        0     9831 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/meson.build
--rw-r--r--   0        0        0      175 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_atk.c
--rw-r--r--   0        0        0      167 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_cairo.c
--rw-r--r--   0        0        0      224 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_freetype2.c
--rw-r--r--   0        0        0      205 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_gdk-pixbuf.c
--rw-r--r--   0        0        0      170 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_glib.c
--rw-r--r--   0        0        0      183 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_jasper.c
--rw-r--r--   0        0        0      204 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_json_glib.c
--rw-r--r--   0        0        0      201 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libarchive.c
--rw-r--r--   0        0        0      191 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libcurl.c
--rw-r--r--   0        0        0      125 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libffi.c
--rw-r--r--   0        0        0      193 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libjpeg-turbo.c
--rw-r--r--   0        0        0      194 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libjpeg.c
--rw-r--r--   0        0        0      188 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libpng.c
--rw-r--r--   0        0        0      187 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libtiff-4.c
--rw-r--r--   0        0        0      179 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libxml2.c
--rw-r--r--   0        0        0      187 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_libyuv.c
--rw-r--r--   0        0        0      173 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_pango.c
--rw-r--r--   0        0        0      180 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_wing.c
--rw-r--r--   0        0        0      127 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/check-libs/test_zlib.c
--rw-r--r--   0        0        0     9047 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9101 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9557 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9085 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9033 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props
--rw-r--r--   0        0        0    10665 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.bld.win32.win32
--rw-r--r--   0        0        0    29220 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln
--rw-r--r--   0        0        0    50071 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am
--rw-r--r--   0        0        0    19138 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in
--rw-r--r--   0        0        0     4749 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt
--rw-r--r--   0        0        0     8818 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0    13484 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj
--rw-r--r--   0        0        0     5987 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters
--rw-r--r--   0        0        0      464 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filtersin
--rw-r--r--   0        0        0     9685 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin
--rw-r--r--   0        0        0     8719 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8822 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8728 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8738 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8715 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8722 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8818 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8809 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj
--rw-r--r--   0        0        0      527 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters
--rw-r--r--   0        0        0     9047 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9101 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9557 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9085 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9033 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props
--rw-r--r--   0        0        0    10665 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.bld.win32.win32
--rw-r--r--   0        0        0    27777 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln
--rw-r--r--   0        0        0    50071 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am
--rw-r--r--   0        0        0    19138 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in
--rw-r--r--   0        0        0     4749 2023-06-06 18:33:15.089511 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt
--rw-r--r--   0        0        0     8818 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0     8719 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8822 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8728 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8738 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8715 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8722 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8818 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8809 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj
--rw-r--r--   0        0        0      527 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters
--rw-r--r--   0        0        0     9126 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9180 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9636 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9164 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9112 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props
--rw-r--r--   0        0        0    10744 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.bld.win32.win32
--rw-r--r--   0        0        0    27909 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln
--rw-r--r--   0        0        0    50150 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    19138 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     4749 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt
--rw-r--r--   0        0        0     8897 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0     8798 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8976 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8901 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8807 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8817 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8803 2023-06-06 18:33:15.105136 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8794 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8803 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8801 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8888 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj
--rw-r--r--   0        0        0      527 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters
--rw-r--r--   0        0        0      316 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/001-cogl-missing-symbols.patch
--rw-r--r--   0        0        0      339 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/002-cogl-pango-missing-symbols.patch
--rw-r--r--   0        0        0     3533 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props
--rw-r--r--   0        0        0    10205 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8918 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9239 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props
--rw-r--r--   0        0        0    14290 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12851 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16347 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props
--rw-r--r--   0        0        0    12059 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln
--rw-r--r--   0        0        0    48250 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am
--rw-r--r--   0        0        0    19171 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in
--rw-r--r--   0        0        0     4783 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt
--rw-r--r--   0        0        0    13862 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0     3533 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props
--rw-r--r--   0        0        0    10205 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8918 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9239 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props
--rw-r--r--   0        0        0    14290 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12851 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16347 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props
--rw-r--r--   0        0        0    12059 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln
--rw-r--r--   0        0        0    48250 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am
--rw-r--r--   0        0        0    19171 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in
--rw-r--r--   0        0        0     4783 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt
--rw-r--r--   0        0        0    13862 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0     3533 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props
--rw-r--r--   0        0        0    10284 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8997 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9318 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props
--rw-r--r--   0        0        0    14369 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12930 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16426 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props
--rw-r--r--   0        0        0    12161 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln
--rw-r--r--   0        0        0    48329 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    19171 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     4783 2023-06-06 18:33:15.136389 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt
--rw-r--r--   0        0        0    13941 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0   244356 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/GL/glcorearb.h
--rw-r--r--   0        0        0   810011 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/GL/glext.h
--rw-r--r--   0        0        0    48113 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/GL/glxext.h
--rw-r--r--   0        0        0    44095 2023-06-06 18:33:15.120763 gvsbuild-2023.6.0/gvsbuild/patches/cogl/GL/wglext.h
--rw-r--r--   0        0        0     1121 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch
--rw-r--r--   0        0        0     1060 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch
--rw-r--r--   0        0        0      740 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch
--rw-r--r--   0        0        0     1135 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch
--rw-r--r--   0        0        0     1045 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/include/md5global.h
--rw-r--r--   0        0        0      312 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/pc-files/libsasl2.pc
--rw-r--r--   0        0        0      418 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/enchant/src/config.h
--rw-r--r--   0        0        0      660 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/enchant/src/libenchant.rc
--rw-r--r--   0        0        0    17426 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/enchant/src/makefile.mak
--rw-r--r--   0        0        0    11334 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/ffmpeg/0001-libavutil-libavcodec-add-support-for-MB_INFO.patch
--rw-r--r--   0        0        0     1950 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/ffmpeg/build/build.sh
--rw-r--r--   0        0        0      787 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch
--rw-r--r--   0        0        0     3296 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch
--rw-r--r--   0        0        0    33686 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/gettext-tools-c99.patch
--rw-r--r--   0        0        0      367 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/gettext-tools-gnulib-memset.patch
--rw-r--r--   0        0        0     9543 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/libtextstyle-c99.patch
--rw-r--r--   0        0        0     3065 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h
--rw-r--r--   0        0        0     7623 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h
--rw-r--r--   0        0        0    33617 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h
--rw-r--r--   0        0        0     2128 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h
--rw-r--r--   0        0        0     3334 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h
--rw-r--r--   0        0        0    26308 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h
--rw-r--r--   0        0        0    43681 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h
--rw-r--r--   0        0        0    27515 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h
--rw-r--r--   0        0        0     4377 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h
--rw-r--r--   0        0        0    32044 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h
--rw-r--r--   0        0        0    37498 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h
--rw-r--r--   0        0        0     4322 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h
--rw-r--r--   0        0        0    63279 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h
--rw-r--r--   0        0        0    63715 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h
--rw-r--r--   0        0        0    44998 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h
--rw-r--r--   0        0        0     3250 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h
--rw-r--r--   0        0        0    35655 2023-06-06 18:33:15.152011 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h
--rw-r--r--   0        0        0    81450 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h
--rw-r--r--   0        0        0    24256 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h
--rw-r--r--   0        0        0     2201 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h
--rw-r--r--   0        0        0     2239 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h
--rw-r--r--   0        0        0    62421 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h
--rw-r--r--   0        0        0    38906 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h
--rw-r--r--   0        0        0    20126 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h
--rw-r--r--   0        0        0    19299 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h
--rw-r--r--   0        0        0     3088 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h
--rw-r--r--   0        0        0     2708 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h
--rw-r--r--   0        0        0     7648 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h
--rw-r--r--   0        0        0     3065 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h
--rw-r--r--   0        0        0     2093 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h
--rw-r--r--   0        0        0    22716 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h
--rw-r--r--   0        0        0    30933 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h
--rw-r--r--   0        0        0     7623 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h
--rw-r--r--   0        0        0    33701 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h
--rw-r--r--   0        0        0    25904 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h
--rw-r--r--   0        0        0     2128 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h
--rw-r--r--   0        0        0     3334 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h
--rw-r--r--   0        0        0    26308 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h
--rw-r--r--   0        0        0    43508 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h
--rw-r--r--   0        0        0    27538 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h
--rw-r--r--   0        0        0     4658 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h
--rw-r--r--   0        0        0     6506 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h
--rw-r--r--   0        0        0     6869 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h
--rw-r--r--   0        0        0     6788 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h
--rw-r--r--   0        0        0     3460 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h
--rw-r--r--   0        0        0     4672 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h
--rw-r--r--   0        0        0    10171 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h
--rw-r--r--   0        0        0     6282 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h
--rw-r--r--   0        0        0    16639 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h
--rw-r--r--   0        0        0     8258 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h
--rw-r--r--   0        0        0    11135 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h
--rw-r--r--   0        0        0     5212 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h
--rw-r--r--   0        0        0     4904 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h
--rw-r--r--   0        0        0     5340 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h
--rw-r--r--   0        0        0     3505 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h
--rw-r--r--   0        0        0    42377 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h
--rw-r--r--   0        0        0    19481 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h
--rw-r--r--   0        0        0     4105 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h
--rw-r--r--   0        0        0     7632 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h
--rw-r--r--   0        0        0     5931 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h
--rw-r--r--   0        0        0     6544 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h
--rw-r--r--   0        0        0    28618 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h
--rw-r--r--   0        0        0     5930 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h
--rw-r--r--   0        0        0     3466 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h
--rw-r--r--   0        0        0    40837 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h
--rw-r--r--   0        0        0     4177 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h
--rw-r--r--   0        0        0    15497 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h
--rw-r--r--   0        0        0     4515 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h
--rw-r--r--   0        0        0     6648 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h
--rw-r--r--   0        0        0     5521 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h
--rw-r--r--   0        0        0    39148 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h
--rw-r--r--   0        0        0     5514 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h
--rw-r--r--   0        0        0    12396 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h
--rw-r--r--   0        0        0     7586 2023-06-06 18:33:15.167636 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h
--rw-r--r--   0        0        0     2646 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h
--rw-r--r--   0        0        0    14454 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h
--rw-r--r--   0        0        0     7099 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h
--rw-r--r--   0        0        0     3844 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h
--rw-r--r--   0        0        0     8732 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h
--rw-r--r--   0        0        0     6409 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h
--rw-r--r--   0        0        0     7070 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h
--rw-r--r--   0        0        0    11675 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h
--rw-r--r--   0        0        0    10024 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h
--rw-r--r--   0        0        0    23172 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h
--rw-r--r--   0        0        0    18374 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h
--rw-r--r--   0        0        0    21404 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h
--rw-r--r--   0        0        0     4892 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h
--rw-r--r--   0        0        0     4377 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h
--rw-r--r--   0        0        0    32067 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h
--rw-r--r--   0        0        0     1209 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h
--rw-r--r--   0        0        0    23409 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h
--rw-r--r--   0        0        0    37554 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h
--rw-r--r--   0        0        0    61302 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h
--rw-r--r--   0        0        0     4298 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h
--rw-r--r--   0        0        0    63335 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h
--rw-r--r--   0        0        0    63743 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h
--rw-r--r--   0        0        0    24900 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h
--rw-r--r--   0        0        0    32949 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h
--rw-r--r--   0        0        0    44998 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h
--rw-r--r--   0        0        0    29890 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h
--rw-r--r--   0        0        0     3250 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h
--rw-r--r--   0        0        0    24835 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h
--rw-r--r--   0        0        0    35681 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h
--rw-r--r--   0        0        0     7748 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h
--rw-r--r--   0        0        0    42529 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h
--rw-r--r--   0        0        0     4287 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h
--rw-r--r--   0        0        0     1625 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h
--rw-r--r--   0        0        0    81730 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h
--rw-r--r--   0        0        0    24256 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h
--rw-r--r--   0        0        0     2201 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h
--rw-r--r--   0        0        0     2239 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h
--rw-r--r--   0        0        0    24592 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h
--rw-r--r--   0        0        0    62584 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h
--rw-r--r--   0        0        0    38904 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h
--rw-r--r--   0        0        0    27214 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h
--rw-r--r--   0        0        0     1287 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h
--rw-r--r--   0        0        0    91289 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h
--rw-r--r--   0        0        0     4873 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h
--rw-r--r--   0        0        0    23344 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h
--rw-r--r--   0        0        0    46391 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h
--rw-r--r--   0        0        0     1629 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h
--rw-r--r--   0        0        0     3065 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h
--rw-r--r--   0        0        0     7648 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h
--rw-r--r--   0        0        0    33726 2023-06-06 18:33:15.183262 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h
--rw-r--r--   0        0        0    17539 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h
--rw-r--r--   0        0        0    26333 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h
--rw-r--r--   0        0        0    43508 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h
--rw-r--r--   0        0        0     4402 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h
--rw-r--r--   0        0        0    32092 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h
--rw-r--r--   0        0        0    37579 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h
--rw-r--r--   0        0        0     4333 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h
--rw-r--r--   0        0        0    63360 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h
--rw-r--r--   0        0        0    63768 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h
--rw-r--r--   0        0        0    45023 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h
--rw-r--r--   0        0        0     3275 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h
--rw-r--r--   0        0        0    13023 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h
--rw-r--r--   0        0        0    35677 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h
--rw-r--r--   0        0        0     7748 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h
--rw-r--r--   0        0        0    42529 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h
--rw-r--r--   0        0        0     4287 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h
--rw-r--r--   0        0        0    81764 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h
--rw-r--r--   0        0        0    24256 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h
--rw-r--r--   0        0        0     2201 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h
--rw-r--r--   0        0        0     2239 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h
--rw-r--r--   0        0        0    62609 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h
--rw-r--r--   0        0        0    38929 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h
--rw-r--r--   0        0        0    27563 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h
--rw-r--r--   0        0        0     4432 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h
--rw-r--r--   0        0        0     1392 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h
--rw-r--r--   0        0        0     1230 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h
--rw-r--r--   0        0        0    23446 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h
--rw-r--r--   0        0        0     3065 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h
--rw-r--r--   0        0        0     7643 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h
--rw-r--r--   0        0        0    33637 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h
--rw-r--r--   0        0        0     4938 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h
--rw-r--r--   0        0        0     5545 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h
--rw-r--r--   0        0        0     9729 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h
--rw-r--r--   0        0        0     2028 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h
--rw-r--r--   0        0        0     2257 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h
--rw-r--r--   0        0        0    10124 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h
--rw-r--r--   0        0        0     6212 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h
--rw-r--r--   0        0        0    16052 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h
--rw-r--r--   0        0        0     2765 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h
--rw-r--r--   0        0        0     6279 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h
--rw-r--r--   0        0        0    43677 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h
--rw-r--r--   0        0        0     4658 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h
--rw-r--r--   0        0        0     6506 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h
--rw-r--r--   0        0        0     6869 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h
--rw-r--r--   0        0        0     6788 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h
--rw-r--r--   0        0        0     3460 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h
--rw-r--r--   0        0        0     4672 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h
--rw-r--r--   0        0        0    10171 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h
--rw-r--r--   0        0        0     6282 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h
--rw-r--r--   0        0        0    16639 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h
--rw-r--r--   0        0        0     8258 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h
--rw-r--r--   0        0        0    11135 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h
--rw-r--r--   0        0        0     5212 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h
--rw-r--r--   0        0        0     4904 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h
--rw-r--r--   0        0        0     5340 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h
--rw-r--r--   0        0        0     3505 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h
--rw-r--r--   0        0        0    42377 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h
--rw-r--r--   0        0        0    19481 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h
--rw-r--r--   0        0        0     4105 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h
--rw-r--r--   0        0        0     7632 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h
--rw-r--r--   0        0        0     5931 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h
--rw-r--r--   0        0        0     6544 2023-06-06 18:33:15.198889 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h
--rw-r--r--   0        0        0    28618 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h
--rw-r--r--   0        0        0     5930 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h
--rw-r--r--   0        0        0     3466 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h
--rw-r--r--   0        0        0    40837 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h
--rw-r--r--   0        0        0     4177 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h
--rw-r--r--   0        0        0    15497 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h
--rw-r--r--   0        0        0     4515 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h
--rw-r--r--   0        0        0     6648 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h
--rw-r--r--   0        0        0     5521 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h
--rw-r--r--   0        0        0    39148 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h
--rw-r--r--   0        0        0     5514 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h
--rw-r--r--   0        0        0    12396 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h
--rw-r--r--   0        0        0     7586 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h
--rw-r--r--   0        0        0     2646 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h
--rw-r--r--   0        0        0    14454 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h
--rw-r--r--   0        0        0     7099 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h
--rw-r--r--   0        0        0     3844 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h
--rw-r--r--   0        0        0     8732 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h
--rw-r--r--   0        0        0     6409 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h
--rw-r--r--   0        0        0     7070 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h
--rw-r--r--   0        0        0    11675 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h
--rw-r--r--   0        0        0    10024 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h
--rw-r--r--   0        0        0    23172 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h
--rw-r--r--   0        0        0    18374 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h
--rw-r--r--   0        0        0    21404 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h
--rw-r--r--   0        0        0     4892 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h
--rw-r--r--   0        0        0     4396 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h
--rw-r--r--   0        0        0    37518 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h
--rw-r--r--   0        0        0     4873 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h
--rw-r--r--   0        0        0     4326 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h
--rw-r--r--   0        0        0    23157 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h
--rw-r--r--   0        0        0    63299 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h
--rw-r--r--   0        0        0    63735 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h
--rw-r--r--   0        0        0    46251 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h
--rw-r--r--   0        0        0    45018 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h
--rw-r--r--   0        0        0    29922 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h
--rw-r--r--   0        0        0     3272 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h
--rw-r--r--   0        0        0     1649 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h
--rw-r--r--   0        0        0     4432 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h
--rw-r--r--   0        0        0     1392 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h
--rw-r--r--   0        0        0     1230 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h
--rw-r--r--   0        0        0    35661 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h
--rw-r--r--   0        0        0    81477 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h
--rw-r--r--   0        0        0    24256 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h
--rw-r--r--   0        0        0     2201 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h
--rw-r--r--   0        0        0    62439 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h
--rw-r--r--   0        0        0    54409 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h
--rw-r--r--   0        0        0    23289 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75068 2023-06-06 18:33:15.214513 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97908 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93885 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23289 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75124 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23319 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75149 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49880 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93905 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    75079 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54408 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23289 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75065 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97907 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93885 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23289 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75121 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23319 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75146 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49880 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93905 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    75079 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54410 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74955 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97906 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75011 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    21997 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75036 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49879 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54407 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74958 2023-06-06 18:33:15.230136 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97900 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h
--rw-r--r--   0        0        0     1984 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75014 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75039 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49882 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54406 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74955 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97945 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h
--rw-r--r--   0        0        0     1984 2023-06-06 18:33:15.245780 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75011 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75036 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49882 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    22956 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak
--rw-r--r--   0        0        0     6490 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/config-msvc.mak
--rw-r--r--   0        0        0    16869 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak
--rwxr-xr-x   0        0        0      846 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/create-lists.bat
--rw-r--r--   0        0        0     5708 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak
--rw-r--r--   0        0        0      772 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak
--rw-r--r--   0        0        0     4576 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk
--rw-r--r--   0        0        0     8982 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk
--rw-r--r--   0        0        0     2466 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/libgettextlib.def
--rw-r--r--   0        0        0     2852 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def
--rw-r--r--   0        0        0     3788 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk
--rw-r--r--   0        0        0     2635 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/libtextstyle.def
--rw-r--r--   0        0        0     1051 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/Makefile.vc
--rw-r--r--   0        0        0     1582 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/glib/glib-package-installation-directory.patch
--rw-r--r--   0        0        0       30 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/glib-py-wrapper/glib-genmarshal.config
--rw-r--r--   0        0        0       27 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/glib-py-wrapper/glib-mkenums.config
--rw-r--r--   0        0        0     1123 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c
--rw-r--r--   0        0        0      394 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/glib-py-wrapper/meson.build
--rw-r--r--   0        0        0      611 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gobject-introspection/incorrect-giscanner-path.patch
--rw-r--r--   0        0        0     1468 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch
--rw-r--r--   0        0        0      759 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch
--rw-r--r--   0        0        0    21208 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gst-plugins-bad/wasapi2-Add-option-to-monitor-loopback-device-s-mute.patch
--rw-r--r--   0        0        0     2083 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch
--rw-r--r--   0        0        0     1958 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch
--rw-r--r--   0        0        0     1186 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch
--rw-r--r--   0        0        0     1920 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch
--rw-r--r--   0        0        0     1956 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak
--rw-r--r--   0        0        0     2185 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props
--rw-r--r--   0        0        0     2185 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props
--rw-r--r--   0        0        0    10679 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj
--rw-r--r--   0        0        0     1080 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters
--rw-r--r--   0        0        0    11397 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj
--rw-r--r--   0        0        0     3760 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters
--rw-r--r--   0        0        0    13364 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj
--rw-r--r--   0        0        0     4222 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters
--rw-r--r--   0        0        0     6519 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln
--rw-r--r--   0        0        0     3640 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props
--rw-r--r--   0        0        0    12279 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj
--rw-r--r--   0        0        0     4640 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters
--rw-r--r--   0        0        0     1962 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props
--rw-r--r--   0        0        0    23804 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props
--rw-r--r--   0        0        0     7938 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj
--rw-r--r--   0        0        0     9247 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj
--rw-r--r--   0        0        0      706 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters
--rw-r--r--   0        0        0     2185 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props
--rw-r--r--   0        0        0    26897 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj
--rw-r--r--   0        0        0    26470 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters
--rw-r--r--   0        0        0     9451 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj
--rw-r--r--   0        0        0     1756 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters
--rw-r--r--   0        0        0     3586 2023-06-06 18:33:15.261389 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt
--rw-r--r--   0        0        0      803 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/gtk-accel.patch
--rw-r--r--   0        0        0      599 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/gtk-bgimg.patch
--rw-r--r--   0        0        0      682 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch
--rw-r--r--   0        0        0     2154 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch
--rw-r--r--   0        0        0     1104 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk2/mod.md
--rw-r--r--   0        0        0     6104 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h
--rw-r--r--   0        0        0    11322 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h
--rw-r--r--   0        0        0     1630 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch
--rw-r--r--   0        0        0      102 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/hello-world/hello-world.c
--rw-r--r--   0        0        0       66 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/hello-world/meson.build
--rw-r--r--   0        0        0      359 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/icu/pc-files/icu-uc.pc
--rw-r--r--   0        0        0      360 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/icu/pc-files-debug/icu-uc.pc
--rw-r--r--   0        0        0     8062 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/install.vcxproj
--rw-r--r--   0        0        0      834 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/install.vcxproj.filters
--rw-r--r--   0        0        0     1649 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.def
--rw-r--r--   0        0        0     4615 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.filters
--rw-r--r--   0        0        0     3150 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.sln
--rw-r--r--   0        0        0    12181 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.vcxproj
--rw-r--r--   0        0        0     2813 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.cpp
--rw-r--r--   0        0        0    10799 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.vcxproj
--rw-r--r--   0        0        0     1339 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.vcxproj.filters
--rw-r--r--   0        0        0     1750 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/ReadMe.txt
--rw-r--r--   0        0        0      299 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/stdafx.cpp
--rw-r--r--   0        0        0      320 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/stdafx.h
--rw-r--r--   0        0        0      314 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/targetver.h
--rw-r--r--   0        0        0     3103 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/property.props
--rw-r--r--   0        0        0     8062 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/install.vcxproj
--rw-r--r--   0        0        0      834 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/install.vcxproj.filters
--rw-r--r--   0        0        0     1649 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.def
--rw-r--r--   0        0        0     4615 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.filters
--rw-r--r--   0        0        0     3148 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.sln
--rw-r--r--   0        0        0    12239 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.vcxproj
--rw-r--r--   0        0        0     2813 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.cpp
--rw-r--r--   0        0        0    10799 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.vcxproj
--rw-r--r--   0        0        0     1339 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.vcxproj.filters
--rw-r--r--   0        0        0     1750 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/ReadMe.txt
--rw-r--r--   0        0        0      299 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/stdafx.cpp
--rw-r--r--   0        0        0      320 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/stdafx.h
--rw-r--r--   0        0        0      314 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/targetver.h
--rw-r--r--   0        0        0     3103 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/property.props
--rw-r--r--   0        0        0     8064 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/install.vcxproj
--rw-r--r--   0        0        0      834 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/install.vcxproj.filters
--rw-r--r--   0        0        0     1649 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.def
--rw-r--r--   0        0        0     4615 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.filters
--rw-r--r--   0        0        0     3148 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.sln
--rw-r--r--   0        0        0    12241 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.vcxproj
--rw-r--r--   0        0        0     2813 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.cpp
--rw-r--r--   0        0        0    10801 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.vcxproj
--rw-r--r--   0        0        0     1339 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.vcxproj.filters
--rw-r--r--   0        0        0     1750 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/ReadMe.txt
--rw-r--r--   0        0        0      299 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/stdafx.cpp
--rw-r--r--   0        0        0      320 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/stdafx.h
--rw-r--r--   0        0        0      314 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/targetver.h
--rw-r--r--   0        0        0     3103 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/property.props
--rw-r--r--   0        0        0      787 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/port.h
--rw-r--r--   0        0        0     4361 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/port_win.cc
--rw-r--r--   0        0        0     4833 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/port_win.h
--rw-r--r--   0        0        0     1646 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/win/stdint.h
--rw-r--r--   0        0        0        0 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/win/unistd.h
--rw-r--r--   0        0        0    26562 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/leveldb/util/env_win.cc
--rw-r--r--   0        0        0      652 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/libcroco/mod.md
--rw-r--r--   0        0        0     3749 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2023-06-06 18:33:15.277014 gvsbuild-2023.6.0/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props
--rw-r--r--   0        0        0    30660 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample.patch
--rw-r--r--   0        0        0    31100 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libpng/CMakeLists.txt
--rw-r--r--   0        0        0       44 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libpng/mod.md
--rw-r--r--   0        0        0      318 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libpng/pc-files/libpng.pc
--rw-r--r--   0        0        0      318 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libpng/pc-files/libpng16.pc
--rw-r--r--   0        0        0      964 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libpsl/0001-localtime_r.patch
--rw-r--r--   0        0        0      830 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg/enable_specifying_rust_version.patch
--rw-r--r--   0        0        0     2998 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props
--rw-r--r--   0        0        0     2133 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props
--rw-r--r--   0        0        0     2326 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props
--rw-r--r--   0        0        0     2998 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props
--rw-r--r--   0        0        0     2133 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props
--rw-r--r--   0        0        0     2326 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props
--rw-r--r--   0        0        0     9178 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj
--rw-r--r--   0        0        0      937 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters
--rw-r--r--   0        0        0     4286 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln
--rw-r--r--   0        0        0      572 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    17549 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     3085 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt
--rw-r--r--   0        0        0     2998 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props
--rw-r--r--   0        0        0     8574 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj
--rw-r--r--   0        0        0     1026 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters
--rw-r--r--   0        0        0      931 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props
--rw-r--r--   0        0        0     2133 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props
--rw-r--r--   0        0        0     6578 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj
--rw-r--r--   0        0        0     2326 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props
--rw-r--r--   0        0        0     8979 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj
--rw-r--r--   0        0        0      925 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters
--rw-r--r--   0        0        0    14576 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj
--rw-r--r--   0        0        0     3427 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters
--rw-r--r--   0        0        0      866 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/vs2019-support.patch
--rw-r--r--   0        0        0      821 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libsoup3/0001-Fix-encoding-for-UTF-8-params.patch
--rw-r--r--   0        0        0     5490 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/config.h
--rw-r--r--   0        0        0     8059 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj
--rw-r--r--   0        0        0      834 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters
--rw-r--r--   0        0        0     3769 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln
--rw-r--r--   0        0        0     3074 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/property.props
--rw-r--r--   0        0        0    40095 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     5490 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/config.h
--rw-r--r--   0        0        0     8059 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj
--rw-r--r--   0        0        0      834 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters
--rw-r--r--   0        0        0     3767 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln
--rw-r--r--   0        0        0     3074 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/property.props
--rw-r--r--   0        0        0    40095 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     5490 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/config.h
--rw-r--r--   0        0        0     8138 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj
--rw-r--r--   0        0        0      834 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters
--rw-r--r--   0        0        0     3899 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln
--rw-r--r--   0        0        0     3074 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/property.props
--rw-r--r--   0        0        0    40174 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     1079 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libssh/mod.md
--rw-r--r--   0        0        0      809 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch
--rw-r--r--   0        0        0     2586 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch
--rw-r--r--   0        0        0     1251 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch
--rw-r--r--   0        0        0     1025 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/libxml2/include/libxml/meson.build
--rw-r--r--   0        0        0     1089 2023-06-06 18:33:15.292641 gvsbuild-2023.6.0/gvsbuild/patches/libxml2/LICENSE.build
--rw-r--r--   0        0        0     7284 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/libxml2/meson.build
--rw-r--r--   0        0        0      323 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/libxml2/pc-files/libxml-2.0.pc
--rw-r--r--   0        0        0      943 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/libyuv/001-win-build.patch
--rw-r--r--   0        0        0      392 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/libyuv/pc-files/libyuv.pc
--rw-r--r--   0        0        0      352 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/luajit/pc-files/luajit.pc
--rw-r--r--   0        0        0      971 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/luajit/set-paths.patch
--rw-r--r--   0        0        0      319 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/pc-files/liblz4.pc
--rw-r--r--   0        0        0     8964 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln
--rw-r--r--   0        0        0     8964 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln
--rw-r--r--   0        0        0     8966 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9317 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9317 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10138 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9145 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9206 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9309 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln
--rw-r--r--   0        0        0     8964 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc
--rw-r--r--   0        0        0     9976 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln
--rw-r--r--   0        0        0       93 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/mod.md
--rw-r--r--   0        0        0      733 2023-06-06 18:33:15.308265 gvsbuild-2023.6.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch
--rw-r--r--   0        0        0  1290625 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/openssl/certdata.txt
--rw-r--r--   0        0        0    19616 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/openssl/mk-ca-bundle.pl
--rw-r--r--   0        0        0      412 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/openssl/mod.md
--rw-r--r--   0        0        0      334 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/openssl/pc-files/openssl.pc
--rw-r--r--   0        0        0     1089 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/pcre2/LICENSE.build
--rw-r--r--   0        0        0     5641 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/pcre2/meson.build
--rw-r--r--   0        0        0      219 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/pcre2/meson_options.txt
--rw-r--r--   0        0        0     1241 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch
--rw-r--r--   0        0        0     1036 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch
--rw-r--r--   0        0        0     2647 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch
--rw-r--r--   0        0        0      319 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/protobuf-c/pc-files/libprotobuf-c.pc
--rw-r--r--   0        0        0      975 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/pygobject/pygobject_py3_8_load_dll.patch
--rw-r--r--   0        0        0      633 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/stack.props
--rw-r--r--   0        0        0     1565 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/win-iconv/COPYING
--rw-r--r--   0        0        0       92 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/win-iconv/mod.md
--rw-r--r--   0        0        0      341 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/x264/build/build.sh
--rw-r--r--   0        0        0      343 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/patches/zlib/pc-files/zlib.pc
--rw-r--r--   0        0        0     4190 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/__init__.py
--rw-r--r--   0        0        0     1712 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/adwaita_icon_theme.py
--rw-r--r--   0        0        0     2545 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/atk.py
--rw-r--r--   0        0        0     1853 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/boringssl.py
--rw-r--r--   0        0        0     1501 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/cairo.py
--rw-r--r--   0        0        0     1588 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/cairomm.py
--rw-r--r--   0        0        0     1991 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/check_libs.py
--rw-r--r--   0        0        0     1699 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/clutter.py
--rw-r--r--   0        0        0     1837 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/cogl.py
--rw-r--r--   0        0        0     2951 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/cyrus_sasl.py
--rw-r--r--   0        0        0     2923 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/dev_shell.py
--rw-r--r--   0        0        0     1727 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/emeus.py
--rw-r--r--   0        0        0     2886 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/enchant.py
--rw-r--r--   0        0        0     1564 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/expat.py
--rw-r--r--   0        0        0     3115 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/ffmpeg.py
--rw-r--r--   0        0        0     1661 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/fontconfig.py
--rw-r--r--   0        0        0     1817 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/freerdp.py
--rw-r--r--   0        0        0     1717 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/freetype.py
--rw-r--r--   0        0        0     2172 2023-06-06 18:33:15.323886 gvsbuild-2023.6.0/gvsbuild/projects/fribidi.py
--rw-r--r--   0        0        0     2199 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gdk_pixbuf.py
--rw-r--r--   0        0        0     4111 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gettext.py
--rw-r--r--   0        0        0     3290 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/glib.py
--rw-r--r--   0        0        0     1783 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/glibmm.py
--rw-r--r--   0        0        0     2733 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gobject_introspection.py
--rw-r--r--   0        0        0     1391 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gperf.py
--rw-r--r--   0        0        0     1772 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/graphene.py
--rw-r--r--   0        0        0     1892 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gsettings_desktop_schemas.py
--rw-r--r--   0        0        0     8385 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gstreamer.py
--rw-r--r--   0        0        0     5822 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gtk.py
--rw-r--r--   0        0        0     1885 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gtkmm.py
--rw-r--r--   0        0        0     2821 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/gtksourceview.py
--rw-r--r--   0        0        0     1742 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/harfbuzz.py
--rw-r--r--   0        0        0     1263 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/hello_world.py
--rw-r--r--   0        0        0     1461 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/hicolor_icon_theme.py
--rw-r--r--   0        0        0     2318 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/icu.py
--rw-r--r--   0        0        0     1911 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/json_glib.py
--rw-r--r--   0        0        0     1457 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/jsonc.py
--rw-r--r--   0        0        0     1458 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/leveldb.py
--rw-r--r--   0        0        0     1496 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/lgi.py
--rw-r--r--   0        0        0     2059 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libadwaita.py
--rw-r--r--   0        0        0     2154 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libarchive.py
--rw-r--r--   0        0        0     1575 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libcroco.py
--rw-r--r--   0        0        0     1982 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libcurl.py
--rw-r--r--   0        0        0     1526 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libepoxy.py
--rw-r--r--   0        0        0     1406 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libffi.py
--rw-r--r--   0        0        0     2093 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libgxps.py
--rw-r--r--   0        0        0     1810 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libjpeg_turbo.py
--rw-r--r--   0        0        0     2398 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libmicrohttpd.py
--rw-r--r--   0        0        0     1537 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libpng.py
--rw-r--r--   0        0        0     1723 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libpsl.py
--rw-r--r--   0        0        0     2498 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/librsvg.py
--rw-r--r--   0        0        0     1816 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libsigcplusplus.py
--rw-r--r--   0        0        0     3547 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libsoup.py
--rw-r--r--   0        0        0     2260 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libssh.py
--rw-r--r--   0        0        0     1665 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libtiff.py
--rw-r--r--   0        0        0     1594 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libuv.py
--rw-r--r--   0        0        0     1588 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libvorbis.py
--rw-r--r--   0        0        0     3345 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libvpx.py
--rw-r--r--   0        0        0     1628 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libxml2.py
--rw-r--r--   0        0        0     1655 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libyuv.py
--rw-r--r--   0        0        0     1489 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/libzip.py
--rw-r--r--   0        0        0     1505 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/lmdb.py
--rw-r--r--   0        0        0     1846 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/luajit.py
--rw-r--r--   0        0        0     1858 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/lz4.py
--rw-r--r--   0        0        0     2302 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/mit_kerberos.py
--rw-r--r--   0        0        0     1666 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/nghttp2.py
--rw-r--r--   0        0        0     1554 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/ogg.py
--rw-r--r--   0        0        0     1601 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/openh264.py
--rw-r--r--   0        0        0     2854 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/openssl.py
--rw-r--r--   0        0        0     1674 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/opus.py
--rw-r--r--   0        0        0     1937 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/pango.py
--rw-r--r--   0        0        0     1820 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/pangomm.py
--rw-r--r--   0        0        0      712 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/pcre2.py
--rw-r--r--   0        0        0     2007 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/pixman.py
--rw-r--r--   0        0        0     1774 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/pkgconf.py
--rw-r--r--   0        0        0     2790 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/protobuf.py
--rw-r--r--   0        0        0     2076 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/pycairo.py
--rw-r--r--   0        0        0     2522 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/pygobject.py
--rw-r--r--   0        0        0     1697 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/sqlite.py
--rw-r--r--   0        0        0     1687 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/win_iconv.py
--rw-r--r--   0        0        0     1549 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/wing.py
--rw-r--r--   0        0        0     1965 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/x264.py
--rw-r--r--   0        0        0     2499 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/projects/zlib.py
--rw-r--r--   0        0        0     7627 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/tools.py
--rw-r--r--   0        0        0       30 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/__init__.py
--rw-r--r--   0        0        0     8591 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/base_builders.py
--rw-r--r--   0        0        0    15284 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/base_expanders.py
--rw-r--r--   0        0        0     1461 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/base_group.py
--rw-r--r--   0        0        0    20449 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/base_project.py
--rw-r--r--   0        0        0     2828 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/base_tool.py
--rw-r--r--   0        0        0    38145 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/builder.py
--rw-r--r--   0        0        0     9978 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/simple_ui.py
--rw-r--r--   0        0        0     3925 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/gvsbuild/utils/utils.py
--rw-r--r--   0        0        0     1482 2023-06-06 18:33:15.339514 gvsbuild-2023.6.0/pyproject.toml
--rw-r--r--   0        0        0     8320 2023-06-06 18:33:15.073888 gvsbuild-2023.6.0/README.md
--rw-r--r--   0        0        0    18790 1970-01-01 00:00:00.000000 gvsbuild-2023.6.0/setup.py
--rw-r--r--   0        0        0     9088 1970-01-01 00:00:00.000000 gvsbuild-2023.6.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/__init__.py
+-rw-r--r--   0        0        0    16483 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/build.py
+-rw-r--r--   0        0        0     7322 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/deps.py
+-rw-r--r--   0        0        0     2243 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/groups.py
+-rw-r--r--   0        0        0     5637 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/list.py
+-rw-r--r--   0        0        0     1811 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/main.py
+-rw-r--r--   0        0        0     2683 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/outdated.py
+-rw-r--r--   0        0        0     5700 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/adwaita-icon-theme/add_meson_build.patch
+-rw-r--r--   0        0        0        0 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/adwaita-icon-theme/Adwaita/64x64/ui/.empty
+-rw-r--r--   0        0        0        0 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/adwaita-icon-theme/Adwaita/96x96/ui/.empty
+-rw-r--r--   0        0        0      213 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/check_utils.c
+-rw-r--r--   0        0        0      537 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/check_utils.h
+-rw-r--r--   0        0        0    18437 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/COPYING
+-rw-r--r--   0        0        0     9831 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/meson.build
+-rw-r--r--   0        0        0      175 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_atk.c
+-rw-r--r--   0        0        0      167 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_cairo.c
+-rw-r--r--   0        0        0      224 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_freetype2.c
+-rw-r--r--   0        0        0      205 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_gdk-pixbuf.c
+-rw-r--r--   0        0        0      170 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_glib.c
+-rw-r--r--   0        0        0      183 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_jasper.c
+-rw-r--r--   0        0        0      204 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_json_glib.c
+-rw-r--r--   0        0        0      201 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libarchive.c
+-rw-r--r--   0        0        0      191 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libcurl.c
+-rw-r--r--   0        0        0      125 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libffi.c
+-rw-r--r--   0        0        0      193 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libjpeg-turbo.c
+-rw-r--r--   0        0        0      194 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libjpeg.c
+-rw-r--r--   0        0        0      188 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libpng.c
+-rw-r--r--   0        0        0      187 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libtiff-4.c
+-rw-r--r--   0        0        0      179 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libxml2.c
+-rw-r--r--   0        0        0      187 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_libyuv.c
+-rw-r--r--   0        0        0      173 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_pango.c
+-rw-r--r--   0        0        0      180 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_wing.c
+-rw-r--r--   0        0        0      127 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/check-libs/test_zlib.c
+-rw-r--r--   0        0        0     9047 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9101 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9557 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9085 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9033 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props
+-rw-r--r--   0        0        0    10665 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    29220 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln
+-rw-r--r--   0        0        0    50071 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am
+-rw-r--r--   0        0        0    19138 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in
+-rw-r--r--   0        0        0     4749 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt
+-rw-r--r--   0        0        0     8818 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0    13484 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj
+-rw-r--r--   0        0        0     5987 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters
+-rw-r--r--   0        0        0      464 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0     9685 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin
+-rw-r--r--   0        0        0     8719 2023-07-05 16:37:42.444877 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8822 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8728 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8738 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8715 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8722 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8818 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8809 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters
+-rw-r--r--   0        0        0     9047 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9101 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9557 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9085 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9033 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props
+-rw-r--r--   0        0        0    10665 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    27777 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln
+-rw-r--r--   0        0        0    50071 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am
+-rw-r--r--   0        0        0    19138 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in
+-rw-r--r--   0        0        0     4749 2023-07-05 16:37:42.460551 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt
+-rw-r--r--   0        0        0     8818 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8719 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8822 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8728 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8738 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8715 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8722 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8818 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8809 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters
+-rw-r--r--   0        0        0     9126 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9180 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9636 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9164 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9112 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props
+-rw-r--r--   0        0        0    10744 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    27909 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln
+-rw-r--r--   0        0        0    50150 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    19138 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     4749 2023-07-05 16:37:42.476156 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0     8897 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8798 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8976 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8901 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8807 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8817 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8803 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8794 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8803 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8801 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8888 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters
+-rw-r--r--   0        0        0      316 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/cogl/001-cogl-missing-symbols.patch
+-rw-r--r--   0        0        0      339 2023-07-05 16:37:42.491779 gvsbuild-2023.7.0/gvsbuild/patches/cogl/002-cogl-pango-missing-symbols.patch
+-rw-r--r--   0        0        0     3533 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props
+-rw-r--r--   0        0        0    10205 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8918 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9239 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props
+-rw-r--r--   0        0        0    14290 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12851 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16347 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props
+-rw-r--r--   0        0        0    12059 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln
+-rw-r--r--   0        0        0    48250 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am
+-rw-r--r--   0        0        0    19171 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in
+-rw-r--r--   0        0        0     4783 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt
+-rw-r--r--   0        0        0    13862 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0     3533 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props
+-rw-r--r--   0        0        0    10205 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8918 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9239 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props
+-rw-r--r--   0        0        0    14290 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12851 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16347 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props
+-rw-r--r--   0        0        0    12059 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln
+-rw-r--r--   0        0        0    48250 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am
+-rw-r--r--   0        0        0    19171 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in
+-rw-r--r--   0        0        0     4783 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt
+-rw-r--r--   0        0        0    13862 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0     3533 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props
+-rw-r--r--   0        0        0    10284 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8997 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9318 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props
+-rw-r--r--   0        0        0    14369 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12930 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16426 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props
+-rw-r--r--   0        0        0    12161 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln
+-rw-r--r--   0        0        0    48329 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    19171 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     4783 2023-07-05 16:37:42.523543 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0    13941 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0   244356 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/GL/glcorearb.h
+-rw-r--r--   0        0        0   810011 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/GL/glext.h
+-rw-r--r--   0        0        0    48113 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/GL/glxext.h
+-rw-r--r--   0        0        0    44095 2023-07-05 16:37:42.508020 gvsbuild-2023.7.0/gvsbuild/patches/cogl/GL/wglext.h
+-rw-r--r--   0        0        0     1121 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch
+-rw-r--r--   0        0        0     1060 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch
+-rw-r--r--   0        0        0      740 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch
+-rw-r--r--   0        0        0     1135 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch
+-rw-r--r--   0        0        0     1045 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/include/md5global.h
+-rw-r--r--   0        0        0      312 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/pc-files/libsasl2.pc
+-rw-r--r--   0        0        0      418 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/enchant/src/config.h
+-rw-r--r--   0        0        0      660 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/enchant/src/libenchant.rc
+-rw-r--r--   0        0        0    17426 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/enchant/src/makefile.mak
+-rw-r--r--   0        0        0    11334 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/ffmpeg/0001-libavutil-libavcodec-add-support-for-MB_INFO.patch
+-rw-r--r--   0        0        0     1950 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/ffmpeg/build/build.sh
+-rw-r--r--   0        0        0      787 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch
+-rw-r--r--   0        0        0     3296 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch
+-rw-r--r--   0        0        0    33686 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/gettext/gettext-tools-c99.patch
+-rw-r--r--   0        0        0      367 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/gettext/gettext-tools-gnulib-memset.patch
+-rw-r--r--   0        0        0     9543 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/gettext/libtextstyle-c99.patch
+-rw-r--r--   0        0        0     3065 2023-07-05 16:37:42.539221 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h
+-rw-r--r--   0        0        0     7623 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h
+-rw-r--r--   0        0        0    33617 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h
+-rw-r--r--   0        0        0     2128 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h
+-rw-r--r--   0        0        0     3334 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h
+-rw-r--r--   0        0        0    26308 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h
+-rw-r--r--   0        0        0    43681 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h
+-rw-r--r--   0        0        0    27515 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h
+-rw-r--r--   0        0        0     4377 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h
+-rw-r--r--   0        0        0    32044 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h
+-rw-r--r--   0        0        0    37498 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h
+-rw-r--r--   0        0        0     4322 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h
+-rw-r--r--   0        0        0    63279 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h
+-rw-r--r--   0        0        0    63715 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h
+-rw-r--r--   0        0        0    44998 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h
+-rw-r--r--   0        0        0     3250 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h
+-rw-r--r--   0        0        0    35655 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h
+-rw-r--r--   0        0        0    81450 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h
+-rw-r--r--   0        0        0    24256 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h
+-rw-r--r--   0        0        0     2201 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h
+-rw-r--r--   0        0        0     2239 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h
+-rw-r--r--   0        0        0    62421 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h
+-rw-r--r--   0        0        0    38906 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h
+-rw-r--r--   0        0        0    20126 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h
+-rw-r--r--   0        0        0    19299 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h
+-rw-r--r--   0        0        0     3088 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h
+-rw-r--r--   0        0        0     2708 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h
+-rw-r--r--   0        0        0     7648 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h
+-rw-r--r--   0        0        0     3065 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h
+-rw-r--r--   0        0        0     2093 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h
+-rw-r--r--   0        0        0    22716 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h
+-rw-r--r--   0        0        0    30933 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h
+-rw-r--r--   0        0        0     7623 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h
+-rw-r--r--   0        0        0    33701 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h
+-rw-r--r--   0        0        0    25904 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h
+-rw-r--r--   0        0        0     2128 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h
+-rw-r--r--   0        0        0     3334 2023-07-05 16:37:42.554849 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h
+-rw-r--r--   0        0        0    26308 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h
+-rw-r--r--   0        0        0    43508 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h
+-rw-r--r--   0        0        0    27538 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h
+-rw-r--r--   0        0        0     4658 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h
+-rw-r--r--   0        0        0     6506 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h
+-rw-r--r--   0        0        0     6869 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h
+-rw-r--r--   0        0        0     6788 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h
+-rw-r--r--   0        0        0     3460 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h
+-rw-r--r--   0        0        0     4672 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h
+-rw-r--r--   0        0        0    10171 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h
+-rw-r--r--   0        0        0     6282 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h
+-rw-r--r--   0        0        0    16639 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h
+-rw-r--r--   0        0        0     8258 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h
+-rw-r--r--   0        0        0    11135 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h
+-rw-r--r--   0        0        0     5212 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h
+-rw-r--r--   0        0        0     4904 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h
+-rw-r--r--   0        0        0     5340 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h
+-rw-r--r--   0        0        0     3505 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h
+-rw-r--r--   0        0        0    42377 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h
+-rw-r--r--   0        0        0    19481 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h
+-rw-r--r--   0        0        0     4105 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h
+-rw-r--r--   0        0        0     7632 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h
+-rw-r--r--   0        0        0     5931 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h
+-rw-r--r--   0        0        0     6544 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h
+-rw-r--r--   0        0        0    28618 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h
+-rw-r--r--   0        0        0     5930 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h
+-rw-r--r--   0        0        0     3466 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h
+-rw-r--r--   0        0        0    40837 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h
+-rw-r--r--   0        0        0     4177 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h
+-rw-r--r--   0        0        0    15497 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h
+-rw-r--r--   0        0        0     4515 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h
+-rw-r--r--   0        0        0     6648 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h
+-rw-r--r--   0        0        0     5521 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h
+-rw-r--r--   0        0        0    39148 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h
+-rw-r--r--   0        0        0     5514 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h
+-rw-r--r--   0        0        0    12396 2023-07-05 16:37:42.570472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h
+-rw-r--r--   0        0        0     7586 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h
+-rw-r--r--   0        0        0     2646 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h
+-rw-r--r--   0        0        0    14454 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h
+-rw-r--r--   0        0        0     7099 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h
+-rw-r--r--   0        0        0     3844 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h
+-rw-r--r--   0        0        0     8732 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h
+-rw-r--r--   0        0        0     6409 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h
+-rw-r--r--   0        0        0     7070 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h
+-rw-r--r--   0        0        0    11675 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h
+-rw-r--r--   0        0        0    10024 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h
+-rw-r--r--   0        0        0    23172 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h
+-rw-r--r--   0        0        0    18374 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h
+-rw-r--r--   0        0        0    21404 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h
+-rw-r--r--   0        0        0     4892 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h
+-rw-r--r--   0        0        0     4377 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h
+-rw-r--r--   0        0        0    32067 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h
+-rw-r--r--   0        0        0     1209 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h
+-rw-r--r--   0        0        0    23409 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h
+-rw-r--r--   0        0        0    37554 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h
+-rw-r--r--   0        0        0    61302 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h
+-rw-r--r--   0        0        0     4298 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h
+-rw-r--r--   0        0        0    63335 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h
+-rw-r--r--   0        0        0    63743 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h
+-rw-r--r--   0        0        0    24900 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h
+-rw-r--r--   0        0        0    32949 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h
+-rw-r--r--   0        0        0    44998 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h
+-rw-r--r--   0        0        0    29890 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h
+-rw-r--r--   0        0        0     3250 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h
+-rw-r--r--   0        0        0    24835 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h
+-rw-r--r--   0        0        0    35681 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h
+-rw-r--r--   0        0        0     7748 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h
+-rw-r--r--   0        0        0    42529 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h
+-rw-r--r--   0        0        0     4287 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h
+-rw-r--r--   0        0        0     1625 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h
+-rw-r--r--   0        0        0    81730 2023-07-05 16:37:42.586108 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h
+-rw-r--r--   0        0        0    24256 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h
+-rw-r--r--   0        0        0     2201 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h
+-rw-r--r--   0        0        0     2239 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h
+-rw-r--r--   0        0        0    24592 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h
+-rw-r--r--   0        0        0    62584 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h
+-rw-r--r--   0        0        0    38904 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h
+-rw-r--r--   0        0        0    27214 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h
+-rw-r--r--   0        0        0     1287 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h
+-rw-r--r--   0        0        0    91289 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h
+-rw-r--r--   0        0        0     4873 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h
+-rw-r--r--   0        0        0    23344 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h
+-rw-r--r--   0        0        0    46391 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h
+-rw-r--r--   0        0        0     1629 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h
+-rw-r--r--   0        0        0     3065 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h
+-rw-r--r--   0        0        0     7648 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h
+-rw-r--r--   0        0        0    33726 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h
+-rw-r--r--   0        0        0    17539 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h
+-rw-r--r--   0        0        0    26333 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h
+-rw-r--r--   0        0        0    43508 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h
+-rw-r--r--   0        0        0     4402 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h
+-rw-r--r--   0        0        0    32092 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h
+-rw-r--r--   0        0        0    37579 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h
+-rw-r--r--   0        0        0     4333 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h
+-rw-r--r--   0        0        0    63360 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h
+-rw-r--r--   0        0        0    63768 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h
+-rw-r--r--   0        0        0    45023 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h
+-rw-r--r--   0        0        0     3275 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h
+-rw-r--r--   0        0        0    13023 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h
+-rw-r--r--   0        0        0    35677 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h
+-rw-r--r--   0        0        0     7748 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h
+-rw-r--r--   0        0        0    42529 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h
+-rw-r--r--   0        0        0     4287 2023-07-05 16:37:42.601720 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h
+-rw-r--r--   0        0        0    81764 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h
+-rw-r--r--   0        0        0    24256 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h
+-rw-r--r--   0        0        0     2201 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h
+-rw-r--r--   0        0        0     2239 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h
+-rw-r--r--   0        0        0    62609 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h
+-rw-r--r--   0        0        0    38929 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h
+-rw-r--r--   0        0        0    27563 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h
+-rw-r--r--   0        0        0     4432 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h
+-rw-r--r--   0        0        0     1392 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h
+-rw-r--r--   0        0        0     1230 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h
+-rw-r--r--   0        0        0    23446 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h
+-rw-r--r--   0        0        0     3065 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h
+-rw-r--r--   0        0        0     7643 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h
+-rw-r--r--   0        0        0    33637 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h
+-rw-r--r--   0        0        0     4938 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h
+-rw-r--r--   0        0        0     5545 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h
+-rw-r--r--   0        0        0     9729 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h
+-rw-r--r--   0        0        0     2028 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h
+-rw-r--r--   0        0        0     2257 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h
+-rw-r--r--   0        0        0    10124 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h
+-rw-r--r--   0        0        0     6212 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h
+-rw-r--r--   0        0        0    16052 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h
+-rw-r--r--   0        0        0     2765 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h
+-rw-r--r--   0        0        0     6279 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h
+-rw-r--r--   0        0        0    43677 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h
+-rw-r--r--   0        0        0     4658 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h
+-rw-r--r--   0        0        0     6506 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h
+-rw-r--r--   0        0        0     6869 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h
+-rw-r--r--   0        0        0     6788 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h
+-rw-r--r--   0        0        0     3460 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h
+-rw-r--r--   0        0        0     4672 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h
+-rw-r--r--   0        0        0    10171 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h
+-rw-r--r--   0        0        0     6282 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h
+-rw-r--r--   0        0        0    16639 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h
+-rw-r--r--   0        0        0     8258 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h
+-rw-r--r--   0        0        0    11135 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h
+-rw-r--r--   0        0        0     5212 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h
+-rw-r--r--   0        0        0     4904 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h
+-rw-r--r--   0        0        0     5340 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h
+-rw-r--r--   0        0        0     3505 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h
+-rw-r--r--   0        0        0    42377 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h
+-rw-r--r--   0        0        0    19481 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h
+-rw-r--r--   0        0        0     4105 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h
+-rw-r--r--   0        0        0     7632 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h
+-rw-r--r--   0        0        0     5931 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h
+-rw-r--r--   0        0        0     6544 2023-07-05 16:37:42.617310 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h
+-rw-r--r--   0        0        0    28618 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h
+-rw-r--r--   0        0        0     5930 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h
+-rw-r--r--   0        0        0     3466 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h
+-rw-r--r--   0        0        0    40837 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h
+-rw-r--r--   0        0        0     4177 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h
+-rw-r--r--   0        0        0    15497 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h
+-rw-r--r--   0        0        0     4515 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h
+-rw-r--r--   0        0        0     6648 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h
+-rw-r--r--   0        0        0     5521 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h
+-rw-r--r--   0        0        0    39148 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h
+-rw-r--r--   0        0        0     5514 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h
+-rw-r--r--   0        0        0    12396 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h
+-rw-r--r--   0        0        0     7586 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h
+-rw-r--r--   0        0        0     2646 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h
+-rw-r--r--   0        0        0    14454 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h
+-rw-r--r--   0        0        0     7099 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h
+-rw-r--r--   0        0        0     3844 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h
+-rw-r--r--   0        0        0     8732 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h
+-rw-r--r--   0        0        0     6409 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h
+-rw-r--r--   0        0        0     7070 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h
+-rw-r--r--   0        0        0    11675 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h
+-rw-r--r--   0        0        0    10024 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h
+-rw-r--r--   0        0        0    23172 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h
+-rw-r--r--   0        0        0    18374 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h
+-rw-r--r--   0        0        0    21404 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h
+-rw-r--r--   0        0        0     4892 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h
+-rw-r--r--   0        0        0     4396 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h
+-rw-r--r--   0        0        0    37518 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h
+-rw-r--r--   0        0        0     4873 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h
+-rw-r--r--   0        0        0     4326 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h
+-rw-r--r--   0        0        0    23157 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h
+-rw-r--r--   0        0        0    63299 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h
+-rw-r--r--   0        0        0    63735 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h
+-rw-r--r--   0        0        0    46251 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h
+-rw-r--r--   0        0        0    45018 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h
+-rw-r--r--   0        0        0    29922 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h
+-rw-r--r--   0        0        0     3272 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h
+-rw-r--r--   0        0        0     1649 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h
+-rw-r--r--   0        0        0     4432 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h
+-rw-r--r--   0        0        0     1392 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h
+-rw-r--r--   0        0        0     1230 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h
+-rw-r--r--   0        0        0    35661 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h
+-rw-r--r--   0        0        0    81477 2023-07-05 16:37:42.632991 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h
+-rw-r--r--   0        0        0    24256 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h
+-rw-r--r--   0        0        0     2201 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h
+-rw-r--r--   0        0        0    62439 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h
+-rw-r--r--   0        0        0    54409 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23289 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75068 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97908 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93885 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23289 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75124 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23319 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75149 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49880 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93905 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    75079 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54408 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23289 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75065 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97907 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93885 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23289 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75121 2023-07-05 16:37:42.648596 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23319 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75146 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49880 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93905 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    75079 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54410 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74955 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97906 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75011 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    21997 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75036 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49879 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54407 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74958 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97900 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h
+-rw-r--r--   0        0        0     1984 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75014 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75039 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49882 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2023-07-05 16:37:42.664245 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54406 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74955 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97945 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1984 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75011 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75036 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49882 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2023-07-05 16:37:42.679810 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    22956 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak
+-rw-r--r--   0        0        0     6490 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/config-msvc.mak
+-rw-r--r--   0        0        0    16869 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak
+-rwxr-xr-x   0        0        0      846 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/create-lists.bat
+-rw-r--r--   0        0        0     5708 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak
+-rw-r--r--   0        0        0      772 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak
+-rw-r--r--   0        0        0     4576 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk
+-rw-r--r--   0        0        0     8982 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk
+-rw-r--r--   0        0        0     2466 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/libgettextlib.def
+-rw-r--r--   0        0        0     2852 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def
+-rw-r--r--   0        0        0     3788 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk
+-rw-r--r--   0        0        0     2635 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/libtextstyle.def
+-rw-r--r--   0        0        0     1051 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/Makefile.vc
+-rw-r--r--   0        0        0     1582 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/glib/glib-package-installation-directory.patch
+-rw-r--r--   0        0        0       30 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/glib-py-wrapper/glib-genmarshal.config
+-rw-r--r--   0        0        0       27 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/glib-py-wrapper/glib-mkenums.config
+-rw-r--r--   0        0        0     1123 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c
+-rw-r--r--   0        0        0      394 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/glib-py-wrapper/meson.build
+-rw-r--r--   0        0        0      611 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gobject-introspection/incorrect-giscanner-path.patch
+-rw-r--r--   0        0        0     1468 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch
+-rw-r--r--   0        0        0      759 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch
+-rw-r--r--   0        0        0    21208 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gst-plugins-bad/wasapi2-Add-option-to-monitor-loopback-device-s-mute.patch
+-rw-r--r--   0        0        0     2083 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch
+-rw-r--r--   0        0        0     1958 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch
+-rw-r--r--   0        0        0     1186 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch
+-rw-r--r--   0        0        0     1920 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch
+-rw-r--r--   0        0        0     1956 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak
+-rw-r--r--   0        0        0     2185 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props
+-rw-r--r--   0        0        0     2185 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props
+-rw-r--r--   0        0        0    10679 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj
+-rw-r--r--   0        0        0     1080 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters
+-rw-r--r--   0        0        0    11397 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj
+-rw-r--r--   0        0        0     3760 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters
+-rw-r--r--   0        0        0    13364 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj
+-rw-r--r--   0        0        0     4222 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters
+-rw-r--r--   0        0        0     6519 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln
+-rw-r--r--   0        0        0     3640 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props
+-rw-r--r--   0        0        0    12279 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj
+-rw-r--r--   0        0        0     4640 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters
+-rw-r--r--   0        0        0     1962 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props
+-rw-r--r--   0        0        0    23804 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props
+-rw-r--r--   0        0        0     7938 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj
+-rw-r--r--   0        0        0     9247 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj
+-rw-r--r--   0        0        0      706 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters
+-rw-r--r--   0        0        0     2185 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props
+-rw-r--r--   0        0        0    26897 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj
+-rw-r--r--   0        0        0    26470 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters
+-rw-r--r--   0        0        0     9451 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj
+-rw-r--r--   0        0        0     1756 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters
+-rw-r--r--   0        0        0     3586 2023-07-05 16:37:42.695472 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0      803 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/gtk-accel.patch
+-rw-r--r--   0        0        0      599 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/gtk-bgimg.patch
+-rw-r--r--   0        0        0      682 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch
+-rw-r--r--   0        0        0     2154 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch
+-rw-r--r--   0        0        0     1104 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk2/mod.md
+-rw-r--r--   0        0        0     6104 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h
+-rw-r--r--   0        0        0    11322 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h
+-rw-r--r--   0        0        0     1630 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch
+-rw-r--r--   0        0        0      102 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/hello-world/hello-world.c
+-rw-r--r--   0        0        0       66 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/hello-world/meson.build
+-rw-r--r--   0        0        0      359 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/icu/pc-files/icu-uc.pc
+-rw-r--r--   0        0        0      360 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/icu/pc-files-debug/icu-uc.pc
+-rw-r--r--   0        0        0     8062 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/install.vcxproj
+-rw-r--r--   0        0        0      834 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/install.vcxproj.filters
+-rw-r--r--   0        0        0     1649 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.def
+-rw-r--r--   0        0        0     4615 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.filters
+-rw-r--r--   0        0        0     3150 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.sln
+-rw-r--r--   0        0        0    12181 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.vcxproj
+-rw-r--r--   0        0        0     2813 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.cpp
+-rw-r--r--   0        0        0    10799 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.vcxproj
+-rw-r--r--   0        0        0     1339 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.vcxproj.filters
+-rw-r--r--   0        0        0     1750 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/ReadMe.txt
+-rw-r--r--   0        0        0      299 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/stdafx.cpp
+-rw-r--r--   0        0        0      320 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/stdafx.h
+-rw-r--r--   0        0        0      314 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/targetver.h
+-rw-r--r--   0        0        0     3103 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/property.props
+-rw-r--r--   0        0        0     8062 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/install.vcxproj
+-rw-r--r--   0        0        0      834 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/install.vcxproj.filters
+-rw-r--r--   0        0        0     1649 2023-07-05 16:37:42.711079 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.def
+-rw-r--r--   0        0        0     4615 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.filters
+-rw-r--r--   0        0        0     3148 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.sln
+-rw-r--r--   0        0        0    12239 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.vcxproj
+-rw-r--r--   0        0        0     2813 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.cpp
+-rw-r--r--   0        0        0    10799 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.vcxproj
+-rw-r--r--   0        0        0     1339 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.vcxproj.filters
+-rw-r--r--   0        0        0     1750 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/ReadMe.txt
+-rw-r--r--   0        0        0      299 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/stdafx.cpp
+-rw-r--r--   0        0        0      320 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/stdafx.h
+-rw-r--r--   0        0        0      314 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/targetver.h
+-rw-r--r--   0        0        0     3103 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/property.props
+-rw-r--r--   0        0        0     8064 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/install.vcxproj
+-rw-r--r--   0        0        0      834 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/install.vcxproj.filters
+-rw-r--r--   0        0        0     1649 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.def
+-rw-r--r--   0        0        0     4615 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.filters
+-rw-r--r--   0        0        0     3148 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.sln
+-rw-r--r--   0        0        0    12241 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.vcxproj
+-rw-r--r--   0        0        0     2813 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.cpp
+-rw-r--r--   0        0        0    10801 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.vcxproj
+-rw-r--r--   0        0        0     1339 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.vcxproj.filters
+-rw-r--r--   0        0        0     1750 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/ReadMe.txt
+-rw-r--r--   0        0        0      299 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/stdafx.cpp
+-rw-r--r--   0        0        0      320 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/stdafx.h
+-rw-r--r--   0        0        0      314 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/targetver.h
+-rw-r--r--   0        0        0     3103 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/property.props
+-rw-r--r--   0        0        0      787 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/port.h
+-rw-r--r--   0        0        0     4361 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/port_win.cc
+-rw-r--r--   0        0        0     4833 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/port_win.h
+-rw-r--r--   0        0        0     1646 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/win/stdint.h
+-rw-r--r--   0        0        0        0 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/win/unistd.h
+-rw-r--r--   0        0        0    26562 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/leveldb/util/env_win.cc
+-rw-r--r--   0        0        0      652 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libcroco/mod.md
+-rw-r--r--   0        0        0     3749 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props
+-rw-r--r--   0        0        0     3749 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props
+-rw-r--r--   0        0        0    30660 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample.patch
+-rw-r--r--   0        0        0    31100 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libpng/CMakeLists.txt
+-rw-r--r--   0        0        0       44 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libpng/mod.md
+-rw-r--r--   0        0        0      318 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libpng/pc-files/libpng.pc
+-rw-r--r--   0        0        0      318 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libpng/pc-files/libpng16.pc
+-rw-r--r--   0        0        0      964 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/libpsl/0001-localtime_r.patch
+-rw-r--r--   0        0        0     2998 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props
+-rw-r--r--   0        0        0     2133 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props
+-rw-r--r--   0        0        0     2326 2023-07-05 16:37:42.726743 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props
+-rw-r--r--   0        0        0     2998 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props
+-rw-r--r--   0        0        0     2133 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props
+-rw-r--r--   0        0        0     2326 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props
+-rw-r--r--   0        0        0     9178 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj
+-rw-r--r--   0        0        0      937 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters
+-rw-r--r--   0        0        0     4286 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln
+-rw-r--r--   0        0        0      572 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    17549 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     3085 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0     2998 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props
+-rw-r--r--   0        0        0     8574 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj
+-rw-r--r--   0        0        0     1026 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters
+-rw-r--r--   0        0        0      931 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props
+-rw-r--r--   0        0        0     2133 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props
+-rw-r--r--   0        0        0     6578 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj
+-rw-r--r--   0        0        0     2326 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props
+-rw-r--r--   0        0        0     8979 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj
+-rw-r--r--   0        0        0      925 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters
+-rw-r--r--   0        0        0    14576 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj
+-rw-r--r--   0        0        0     3427 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters
+-rw-r--r--   0        0        0      866 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/vs2019-support.patch
+-rw-r--r--   0        0        0      821 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libsoup3/0001-Fix-encoding-for-UTF-8-params.patch
+-rw-r--r--   0        0        0     5490 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/config.h
+-rw-r--r--   0        0        0     8059 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj
+-rw-r--r--   0        0        0      834 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters
+-rw-r--r--   0        0        0     3769 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/property.props
+-rw-r--r--   0        0        0    40095 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     5490 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/config.h
+-rw-r--r--   0        0        0     8059 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj
+-rw-r--r--   0        0        0      834 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters
+-rw-r--r--   0        0        0     3767 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/property.props
+-rw-r--r--   0        0        0    40095 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     5490 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/config.h
+-rw-r--r--   0        0        0     8138 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj
+-rw-r--r--   0        0        0      834 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters
+-rw-r--r--   0        0        0     3899 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2023-07-05 16:37:42.742334 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/property.props
+-rw-r--r--   0        0        0    40174 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     1079 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libssh/mod.md
+-rw-r--r--   0        0        0      809 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch
+-rw-r--r--   0        0        0     2586 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch
+-rw-r--r--   0        0        0     1251 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch
+-rw-r--r--   0        0        0     1025 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libxml2/include/libxml/meson.build
+-rw-r--r--   0        0        0     1089 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libxml2/LICENSE.build
+-rw-r--r--   0        0        0     7284 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libxml2/meson.build
+-rw-r--r--   0        0        0      323 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libxml2/pc-files/libxml-2.0.pc
+-rw-r--r--   0        0        0      943 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libyuv/001-win-build.patch
+-rw-r--r--   0        0        0      392 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/libyuv/pc-files/libyuv.pc
+-rw-r--r--   0        0        0      352 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/luajit/pc-files/luajit.pc
+-rw-r--r--   0        0        0      971 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/luajit/set-paths.patch
+-rw-r--r--   0        0        0      319 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/pc-files/liblz4.pc
+-rw-r--r--   0        0        0     8964 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln
+-rw-r--r--   0        0        0     8964 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2023-07-05 16:37:42.757971 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln
+-rw-r--r--   0        0        0     8966 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9317 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9317 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10138 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9145 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9206 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9309 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln
+-rw-r--r--   0        0        0     8964 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc
+-rw-r--r--   0        0        0     9976 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln
+-rw-r--r--   0        0        0       93 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/mod.md
+-rw-r--r--   0        0        0      733 2023-07-05 16:37:42.773599 gvsbuild-2023.7.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch
+-rw-r--r--   0        0        0  1290625 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/openssl/certdata.txt
+-rw-r--r--   0        0        0    19616 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/openssl/mk-ca-bundle.pl
+-rw-r--r--   0        0        0      412 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/openssl/mod.md
+-rw-r--r--   0        0        0      334 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/openssl/pc-files/openssl.pc
+-rw-r--r--   0        0        0     1089 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/pcre2/LICENSE.build
+-rw-r--r--   0        0        0     5641 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/pcre2/meson.build
+-rw-r--r--   0        0        0      219 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/pcre2/meson_options.txt
+-rw-r--r--   0        0        0     1241 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch
+-rw-r--r--   0        0        0     1036 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch
+-rw-r--r--   0        0        0     2647 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch
+-rw-r--r--   0        0        0      319 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/protobuf-c/pc-files/libprotobuf-c.pc
+-rw-r--r--   0        0        0      975 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/pygobject/pygobject_py3_8_load_dll.patch
+-rw-r--r--   0        0        0      633 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/stack.props
+-rw-r--r--   0        0        0     1565 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/win-iconv/COPYING
+-rw-r--r--   0        0        0       92 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/win-iconv/mod.md
+-rw-r--r--   0        0        0      341 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/x264/build/build.sh
+-rw-r--r--   0        0        0      343 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/patches/zlib/pc-files/zlib.pc
+-rw-r--r--   0        0        0     4190 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/__init__.py
+-rw-r--r--   0        0        0     1712 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/adwaita_icon_theme.py
+-rw-r--r--   0        0        0     2545 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/atk.py
+-rw-r--r--   0        0        0     1853 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/boringssl.py
+-rw-r--r--   0        0        0     1501 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/cairo.py
+-rw-r--r--   0        0        0     1588 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/cairomm.py
+-rw-r--r--   0        0        0     1991 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/check_libs.py
+-rw-r--r--   0        0        0     1699 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/clutter.py
+-rw-r--r--   0        0        0     1837 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/cogl.py
+-rw-r--r--   0        0        0     2951 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/cyrus_sasl.py
+-rw-r--r--   0        0        0     2923 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/dev_shell.py
+-rw-r--r--   0        0        0     1727 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/emeus.py
+-rw-r--r--   0        0        0     2886 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/enchant.py
+-rw-r--r--   0        0        0     2158 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/expat.py
+-rw-r--r--   0        0        0     3115 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/ffmpeg.py
+-rw-r--r--   0        0        0     1661 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/fontconfig.py
+-rw-r--r--   0        0        0     1817 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/freerdp.py
+-rw-r--r--   0        0        0     1717 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/freetype.py
+-rw-r--r--   0        0        0     2172 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/fribidi.py
+-rw-r--r--   0        0        0     2199 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gdk_pixbuf.py
+-rw-r--r--   0        0        0     4111 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gettext.py
+-rw-r--r--   0        0        0     3290 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/glib.py
+-rw-r--r--   0        0        0     1783 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/glibmm.py
+-rw-r--r--   0        0        0     2733 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gobject_introspection.py
+-rw-r--r--   0        0        0     1391 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gperf.py
+-rw-r--r--   0        0        0     1772 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/graphene.py
+-rw-r--r--   0        0        0     1892 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gsettings_desktop_schemas.py
+-rw-r--r--   0        0        0     8385 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gstreamer.py
+-rw-r--r--   0        0        0     5822 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gtk.py
+-rw-r--r--   0        0        0     1885 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gtkmm.py
+-rw-r--r--   0        0        0     2821 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/gtksourceview.py
+-rw-r--r--   0        0        0     1742 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/harfbuzz.py
+-rw-r--r--   0        0        0     1263 2023-07-05 16:37:42.789223 gvsbuild-2023.7.0/gvsbuild/projects/hello_world.py
+-rw-r--r--   0        0        0     1461 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/hicolor_icon_theme.py
+-rw-r--r--   0        0        0     2318 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/icu.py
+-rw-r--r--   0        0        0     1911 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/json_glib.py
+-rw-r--r--   0        0        0     1457 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/jsonc.py
+-rw-r--r--   0        0        0     1458 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/leveldb.py
+-rw-r--r--   0        0        0     1496 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/lgi.py
+-rw-r--r--   0        0        0     2059 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libadwaita.py
+-rw-r--r--   0        0        0     2154 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libarchive.py
+-rw-r--r--   0        0        0     1575 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libcroco.py
+-rw-r--r--   0        0        0     1982 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libcurl.py
+-rw-r--r--   0        0        0     1526 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libepoxy.py
+-rw-r--r--   0        0        0     1406 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libffi.py
+-rw-r--r--   0        0        0     2093 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libgxps.py
+-rw-r--r--   0        0        0     1810 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libjpeg_turbo.py
+-rw-r--r--   0        0        0     2398 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libmicrohttpd.py
+-rw-r--r--   0        0        0     1537 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libpng.py
+-rw-r--r--   0        0        0     1723 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libpsl.py
+-rw-r--r--   0        0        0     2516 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/librsvg.py
+-rw-r--r--   0        0        0     1816 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libsigcplusplus.py
+-rw-r--r--   0        0        0     3547 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libsoup.py
+-rw-r--r--   0        0        0     2260 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libssh.py
+-rw-r--r--   0        0        0     1665 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libtiff.py
+-rw-r--r--   0        0        0     1594 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libuv.py
+-rw-r--r--   0        0        0     1588 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libvorbis.py
+-rw-r--r--   0        0        0     3345 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libvpx.py
+-rw-r--r--   0        0        0     1628 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libxml2.py
+-rw-r--r--   0        0        0     1655 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libyuv.py
+-rw-r--r--   0        0        0     1490 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/libzip.py
+-rw-r--r--   0        0        0     1505 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/lmdb.py
+-rw-r--r--   0        0        0     1846 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/luajit.py
+-rw-r--r--   0        0        0     1858 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/lz4.py
+-rw-r--r--   0        0        0     2302 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/mit_kerberos.py
+-rw-r--r--   0        0        0     1666 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/nghttp2.py
+-rw-r--r--   0        0        0     1554 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/ogg.py
+-rw-r--r--   0        0        0     1601 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/openh264.py
+-rw-r--r--   0        0        0     2854 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/openssl.py
+-rw-r--r--   0        0        0     1674 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/opus.py
+-rw-r--r--   0        0        0     1937 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/pango.py
+-rw-r--r--   0        0        0     1847 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/pangomm.py
+-rw-r--r--   0        0        0      712 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/pcre2.py
+-rw-r--r--   0        0        0     1753 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/pixman.py
+-rw-r--r--   0        0        0     1771 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/pkgconf.py
+-rw-r--r--   0        0        0     2790 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/protobuf.py
+-rw-r--r--   0        0        0     2076 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/pycairo.py
+-rw-r--r--   0        0        0     2522 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/pygobject.py
+-rw-r--r--   0        0        0     1697 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/sqlite.py
+-rw-r--r--   0        0        0     1687 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/win_iconv.py
+-rw-r--r--   0        0        0     1549 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/wing.py
+-rw-r--r--   0        0        0     1965 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/x264.py
+-rw-r--r--   0        0        0     2499 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/projects/zlib.py
+-rw-r--r--   0        0        0     7627 2023-07-05 16:37:42.804849 gvsbuild-2023.7.0/gvsbuild/tools.py
+-rw-r--r--   0        0        0       30 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/__init__.py
+-rw-r--r--   0        0        0     8591 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/base_builders.py
+-rw-r--r--   0        0        0    15284 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/base_expanders.py
+-rw-r--r--   0        0        0     1461 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/base_group.py
+-rw-r--r--   0        0        0    20449 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/base_project.py
+-rw-r--r--   0        0        0     2828 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/base_tool.py
+-rw-r--r--   0        0        0    38145 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/builder.py
+-rw-r--r--   0        0        0     9978 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/simple_ui.py
+-rw-r--r--   0        0        0     3925 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/gvsbuild/utils/utils.py
+-rw-r--r--   0        0        0     1504 2023-07-05 16:37:42.820486 gvsbuild-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8320 2023-07-05 16:37:42.429241 gvsbuild-2023.7.0/README.md
+-rw-r--r--   0        0        0    18755 1970-01-01 00:00:00.000000 gvsbuild-2023.7.0/setup.py
+-rw-r--r--   0        0        0     9088 1970-01-01 00:00:00.000000 gvsbuild-2023.7.0/PKG-INFO
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/build.py` & `gvsbuild-2023.7.0/gvsbuild/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,21 +103,24 @@
         Configuration.debug_optimized,
         help='The configuration to build for. "debug-optimized" only '
         "includes debug symbols for Meson and CMake projects - other "
         'projects\' build tools will interpret the option as "release"',
     ),
     build_dir: Path = typer.Option(
         Path(r"C:\gtk-build"),
-        help="The directory to build in",
+        help="The full or relative path of the directory to build in",
         rich_help_panel="Directory Options",
     ),
     msys_dir: Path = typer.Option(
         None,
         help="The directory of the msys installation. If not specified, automatically searches in common locations",
         rich_help_panel="Directory Options",
+        exists=True,
+        dir_okay=True,
+        resolve_path=True,
     ),
     archives_download_dir: Path = typer.Option(
         None,
         help="The directory to download the source archives to. It will be created. "
         "If a source archive already exists here, it won't be downloaded again. "
         "Default is the build-dir\\src.",
         rich_help_panel="Directory Options",
@@ -193,15 +196,15 @@
         rich_help_panel="Skip and Cleanup Options",
     ),
     msbuild_opts: str = typer.Option(
         None,
         help="Command line options to pass to msbuild.",
         rich_help_panel="Options to Pass to Build Systems",
     ),
-    skip: str = typer.Option(
+    skip: List[str] = typer.Option(
         None,
         help="Project to avoid building, can be run multiple times.",
         rich_help_panel="Skip and Cleanup Options",
     ),
     use_env: bool = typer.Option(
         False,
         help="Use and keep the calling environment for LIB, LIBPATH, INCLUDE and PATH",
@@ -317,14 +320,16 @@
 
     gvsbuild build --skip gtk4 --skip pycairo all
         Build everything except gtk4 and pycairo
     """
     opts = Options()
     opts.verbose = verbose
     opts.debug = debug
+    if build_dir:
+        build_dir = Path(build_dir).resolve()
     opts.build_dir = str(build_dir)
     log.configure(str(build_dir / "logs"), opts)
     opts.platform = platform.value
     opts.configuration = configuration.value
     if opts.configuration == Configuration.debug_optimized:
         # Some build systems take "opts.configuration" directly, and won't support our
         # custom "debug-optimized" string. Convert it back to the standard
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/deps.py` & `gvsbuild-2023.7.0/gvsbuild/deps.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/groups.py` & `gvsbuild-2023.7.0/gvsbuild/groups.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/list.py` & `gvsbuild-2023.7.0/gvsbuild/list.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/main.py` & `gvsbuild-2023.7.0/gvsbuild/main.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/outdated.py` & `gvsbuild-2023.7.0/gvsbuild/outdated.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/adwaita-icon-theme/add_meson_build.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/adwaita-icon-theme/add_meson_build.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/check-libs/check_utils.h` & `gvsbuild-2023.7.0/gvsbuild/patches/check-libs/check_utils.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/check-libs/COPYING` & `gvsbuild-2023.7.0/gvsbuild/patches/check-libs/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/check-libs/meson.build` & `gvsbuild-2023.7.0/gvsbuild/patches/check-libs/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/GL/glcorearb.h` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/GL/glcorearb.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/GL/glext.h` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/GL/glext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/GL/glxext.h` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/GL/glxext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cogl/GL/wglext.h` & `gvsbuild-2023.7.0/gvsbuild/patches/cogl/GL/wglext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/cyrus-sasl/include/md5global.h` & `gvsbuild-2023.7.0/gvsbuild/patches/cyrus-sasl/include/md5global.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/enchant/src/libenchant.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/enchant/src/libenchant.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/enchant/src/makefile.mak` & `gvsbuild-2023.7.0/gvsbuild/patches/enchant/src/makefile.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/ffmpeg/0001-libavutil-libavcodec-add-support-for-MB_INFO.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/ffmpeg/0001-libavutil-libavcodec-add-support-for-MB_INFO.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/ffmpeg/build/build.sh` & `gvsbuild-2023.7.0/gvsbuild/patches/ffmpeg/build/build.sh`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/gettext-tools-c99.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/gettext-tools-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/libtextstyle-c99.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/libtextstyle-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/config-msvc.mak` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/config-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/create-lists.bat` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/create-lists.bat`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/libgettextlib.def` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/libgettextlib.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/libtextstyle.def` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/libtextstyle.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gettext/nmake/Makefile.vc` & `gvsbuild-2023.7.0/gvsbuild/patches/gettext/nmake/Makefile.vc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/glib/glib-package-installation-directory.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/glib/glib-package-installation-directory.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c` & `gvsbuild-2023.7.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gobject-introspection/incorrect-giscanner-path.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gobject-introspection/incorrect-giscanner-path.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gst-plugins-bad/wasapi2-Add-option-to-monitor-loopback-device-s-mute.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gst-plugins-bad/wasapi2-Add-option-to-monitor-loopback-device-s-mute.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/gtk-accel.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/gtk-accel.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/gtk-bgimg.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/gtk-bgimg.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk2/mod.md` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk2/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/install.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.def` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.cpp` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.cpp`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/leveldb_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/ReadMe.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/leveldb_test/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs12/property.props` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs12/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/install.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.def` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.cpp` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.cpp`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/leveldb_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/ReadMe.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/leveldb_test/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs14/property.props` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs14/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/install.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.def` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.cpp` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.cpp`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/leveldb_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/ReadMe.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/leveldb_test/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/build/win32/vs15/property.props` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/build/win32/vs15/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/port.h` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/port.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/port_win.cc` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/port_win.cc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/port_win.h` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/port_win.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/port/win/stdint.h` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/port/win/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/leveldb/util/env_win.cc` & `gvsbuild-2023.7.0/gvsbuild/patches/leveldb/util/env_win.cc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libcroco/mod.md` & `gvsbuild-2023.7.0/gvsbuild/patches/libcroco/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libpng/CMakeLists.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/libpng/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libpsl/0001-localtime_r.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/libpsl/0001-localtime_r.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/librsvg-legacy/vs2019-support.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/librsvg-legacy/vs2019-support.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libsoup3/0001-Fix-encoding-for-UTF-8-params.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/libsoup3/0001-Fix-encoding-for-UTF-8-params.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/property.props` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/property.props` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/config.h` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/property.props` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/property.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libssh/mod.md` & `gvsbuild-2023.7.0/gvsbuild/patches/libssh/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libxml2/include/libxml/meson.build` & `gvsbuild-2023.7.0/gvsbuild/patches/libxml2/include/libxml/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libxml2/LICENSE.build` & `gvsbuild-2023.7.0/gvsbuild/patches/libxml2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libxml2/meson.build` & `gvsbuild-2023.7.0/gvsbuild/patches/libxml2/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/libyuv/001-win-build.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/libyuv/001-win-build.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/luajit/set-paths.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/luajit/set-paths.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln` & `gvsbuild-2023.7.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/openssl/certdata.txt` & `gvsbuild-2023.7.0/gvsbuild/patches/openssl/certdata.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/openssl/mk-ca-bundle.pl` & `gvsbuild-2023.7.0/gvsbuild/patches/openssl/mk-ca-bundle.pl`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/pcre2/LICENSE.build` & `gvsbuild-2023.7.0/gvsbuild/patches/pcre2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/pcre2/meson.build` & `gvsbuild-2023.7.0/gvsbuild/patches/pcre2/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/pygobject/pygobject_py3_8_load_dll.patch` & `gvsbuild-2023.7.0/gvsbuild/patches/pygobject/pygobject_py3_8_load_dll.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/stack.props` & `gvsbuild-2023.7.0/gvsbuild/patches/stack.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/patches/win-iconv/COPYING` & `gvsbuild-2023.7.0/gvsbuild/patches/win-iconv/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/__init__.py` & `gvsbuild-2023.7.0/gvsbuild/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/adwaita_icon_theme.py` & `gvsbuild-2023.7.0/gvsbuild/projects/adwaita_icon_theme.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/atk.py` & `gvsbuild-2023.7.0/gvsbuild/projects/atk.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/boringssl.py` & `gvsbuild-2023.7.0/gvsbuild/projects/boringssl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/cairo.py` & `gvsbuild-2023.7.0/gvsbuild/projects/cairo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/cairomm.py` & `gvsbuild-2023.7.0/gvsbuild/projects/cairomm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/check_libs.py` & `gvsbuild-2023.7.0/gvsbuild/projects/check_libs.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/clutter.py` & `gvsbuild-2023.7.0/gvsbuild/projects/clutter.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/cogl.py` & `gvsbuild-2023.7.0/gvsbuild/projects/cogl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/cyrus_sasl.py` & `gvsbuild-2023.7.0/gvsbuild/projects/cyrus_sasl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/dev_shell.py` & `gvsbuild-2023.7.0/gvsbuild/projects/dev_shell.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/emeus.py` & `gvsbuild-2023.7.0/gvsbuild/projects/emeus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/enchant.py` & `gvsbuild-2023.7.0/gvsbuild/projects/enchant.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/expat.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libpng.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
+
 from gvsbuild.utils.base_builders import CmakeProject
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Expat(Tarball, CmakeProject):
+class Libpng(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
-            "expat",
-            version="2.5.0",
-            repository="libexpat",
-            archive_url="https://github.com/libexpat/libexpat/releases/download/R_{major}_{minor}_{micro}/expat-{version}.tar.xz",
-            hash="ef2420f0232c087801abf705e89ae65f6257df6b7931d37846a193ef2e8cdcbe",
-            dependencies=["cmake", "ninja"],
+            "libpng",
+            version="1.6.39",
+            archive_url="http://prdownloads.sourceforge.net/libpng/libpng-{version}.tar.xz",
+            hash="1f4696ce70b4ee5f85f1e1623dc1229b210029fa4b7aee573df3e2ba7b036937",
+            dependencies=["cmake", "ninja", "zlib"],
         )
 
     def build(self):
         CmakeProject.build(self, use_ninja=True)
-        self.install(r".\COPYING share\doc\expat")
+
+        self.install_pc_files()
+        self.install(r"LICENSE share\doc\libpng")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/ffmpeg.py` & `gvsbuild-2023.7.0/gvsbuild/projects/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/fontconfig.py` & `gvsbuild-2023.7.0/gvsbuild/projects/fontconfig.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/freerdp.py` & `gvsbuild-2023.7.0/gvsbuild/projects/freerdp.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/freetype.py` & `gvsbuild-2023.7.0/gvsbuild/projects/freetype.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 @project_add
 class Freetype(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "freetype",
-            version="2.13.0",
+            version="2.13.1",
             repository="https://gitlab.freedesktop.org/freetype/freetype",
             archive_url="https://gitlab.freedesktop.org/freetype/freetype/-/archive/VER-{major}-{minor}-{micro}/freetype-VER-{major}-{minor}-{micro}.tar.gz",
-            hash="a683f1091aee95d2deaca9292d976f87415610b8ae1ea186abeebcb08e83ab12",
+            hash="6d2349a5f4f8400ef63ce600c2038dbc3144c99246f7bc88e8f89eb3d318a3c2",
             dependencies=["pkgconf", "ninja", "libpng"],
             patches=["0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch"],
         )
 
     def build(self):
         Meson.build(self)
         self.install(r".\docs\LICENSE.TXT share\doc\freetype")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/fribidi.py` & `gvsbuild-2023.7.0/gvsbuild/projects/fribidi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gdk_pixbuf.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gdk_pixbuf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gettext.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gettext.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/glib.py` & `gvsbuild-2023.7.0/gvsbuild/projects/glib.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,19 +52,19 @@
 
 @project_add
 class GLibNetworking(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "glib-networking",
-            version="2.76.0",
+            version="2.76.1",
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/glib-networking",
             archive_url="https://download.gnome.org/sources/glib-networking/{major}.{minor}/glib-networking-{version}.tar.xz",
-            hash="149a05a179e629a538be25662aa324b499d7c4549c5151db5373e780a1bf1b9a",
+            hash="5c698a9994dde51efdfb1026a56698a221d6250e89dc50ebcddda7b81480a42b",
             dependencies=[
                 "pkgconf",
                 "ninja",
                 "meson",
                 "glib",
                 "openssl",
                 "gsettings-desktop-schemas",
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/glibmm.py` & `gvsbuild-2023.7.0/gvsbuild/projects/glibmm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gobject_introspection.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gobject_introspection.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gperf.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gperf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/graphene.py` & `gvsbuild-2023.7.0/gvsbuild/projects/graphene.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gsettings_desktop_schemas.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gsettings_desktop_schemas.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gstreamer.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gstreamer.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 @project_add
 class GStreamer(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gstreamer",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.22.3",
+            version="1.22.4",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gstreamer/gstreamer-{version}.tar.xz",
-            hash="9ffeab95053f9f6995eb3b3da225e88f21c129cd60da002d3f795db70d6d5974",
+            hash="11cb0498bc16b93d8b99d22f75f829b8d0abfd8254840b2120618db5532dc655",
             dependencies=["meson", "ninja", "glib", "orc"],
         )
 
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             enable_gi = "enabled"
         else:
@@ -88,18 +88,18 @@
 @project_add
 class GstPluginsBase(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-plugins-base",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.22.3",
+            version="1.22.4",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-plugins-base/gst-plugins-base-{version}.tar.xz",
-            hash="1c596289a0d4207380233eba8c36a932c4d1aceba19932937d9b57c24cef89f3",
+            hash="292424e82dea170528c42b456f62a89532bcabc0508f192e34672fb86f68e5b8",
             dependencies=[
                 "meson",
                 "ninja",
                 "gstreamer",
                 "opus",
                 "ogg",
             ],
@@ -125,18 +125,18 @@
 @project_add
 class GstPluginsGood(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-plugins-good",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.22.3",
+            version="1.22.4",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-plugins-good/gst-plugins-good-{version}.tar.xz",
-            hash="af81154b3a2ef3f4d2feba395f25696feea6fd13ec62c92d3c7a973470710273",
+            hash="d7120c1146a9d723d53d5bfe8074da2575a81f0598438752937f39bb7c833b6a",
             dependencies=[
                 "meson",
                 "ninja",
                 "gst-plugins-base",
                 "libvpx",
             ],
         )
@@ -149,18 +149,18 @@
 @project_add
 class GstPluginsBad(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-plugins-bad",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.22.3",
+            version="1.22.4",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-plugins-bad/gst-plugins-bad-{version}.tar.xz",
-            hash="e1798fee2d86127f0637481c607f983293bf0fd81aad70a5c7b47205af3621d8",
+            hash="eaaf53224565eaabd505ca39c6d5769719b45795cf532ce1ceb60e1b2ebe99ac",
             dependencies=["meson", "ninja", "gst-plugins-base"],
             patches=[
                 "wasapisink-reduce-buffer-latency.patch",
                 "wasapi2-Add-option-to-monitor-loopback-device-s-mute.patch",
             ],
         )
         self.add_param("-Dcurl=disabled")
@@ -174,18 +174,18 @@
 @project_add
 class GstPluginsUgly(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-plugins-ugly",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.22.3",
+            version="1.22.4",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-plugins-ugly/gst-plugins-ugly-{version}.tar.xz",
-            hash="3dc98ed5c2293368b3c4e6ce55d89be834a0a62e9bf88ef17928cf03b7d5a360",
+            hash="ffb461fda6c06d316c4be5682632cc8901454ed72b1098b1e0221bc55e673cd7",
             dependencies=["meson", "ninja", "gst-plugins-base"],
         )
 
     def build(self):
         Meson.build(self)
         self.install(r".\COPYING share\doc\gst-plugins-ugly")
 
@@ -193,18 +193,18 @@
 @project_add
 class GstDevTools(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-devtools",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.22.3",
+            version="1.22.4",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-devtools/gst-devtools-{version}.tar.xz",
-            hash="446ac9c42d502cbfd9081737cc1b853b3c1f50db77ca7ccd01aea10f687550c1",
+            hash="4c52053ce8c1df72fd81721e9f53de3b146edcf2de28f607be705bce4cf909d1",
             dependencies=["meson", "ninja", "json-glib"],
         )
 
     def build(self):
         Meson.build(self)
         self.install(r".\COPYING share\doc\gst-devtools")
 
@@ -212,17 +212,17 @@
 @project_add
 class GstPython(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-python",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.22.3",
+            version="1.22.4",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-python/gst-python-{version}.tar.xz",
-            hash="70bed3fabe634bc622ef6de4e6eb1c33bc9cefd64bdab200f6fa316b468c731c",
+            hash="e1302dcc0f2451b64380dcc0dd3b82735795e8951dc812d938d8ba91f388163e",
             dependencies=["meson", "ninja", "pygobject", "gst-plugins-base"],
         )
 
     def build(self):
         Meson.build(self)
         self.install(r".\COPYING share\doc\gst-python")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gtk.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gtk.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,20 +120,20 @@
 @project_add
 class Gtk4(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gtk4",
             prj_dir="gtk4",
-            version="4.10.3",
+            version="4.10.4",
             lastversion_major=4,
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/gtk",
             archive_url="https://download.gnome.org/sources/gtk/{major}.{minor}/gtk-{version}.tar.xz",
-            hash="4545441ad79e377eb6e0a705026dc7a46886e46a1b034db40912909da801cea9",
+            hash="7725400482e0685e28265e226c62847f4e73cfca9e9b416ac5838207f5377a24",
             dependencies=[
                 "gdk-pixbuf",
                 "pango",
                 "libepoxy",
                 "graphene",
                 "cairo",
                 "harfbuzz",
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gtkmm.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gtkmm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/gtksourceview.py` & `gvsbuild-2023.7.0/gvsbuild/projects/gtksourceview.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/harfbuzz.py` & `gvsbuild-2023.7.0/gvsbuild/projects/harfbuzz.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/hello_world.py` & `gvsbuild-2023.7.0/gvsbuild/projects/hello_world.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/hicolor_icon_theme.py` & `gvsbuild-2023.7.0/gvsbuild/projects/hicolor_icon_theme.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/icu.py` & `gvsbuild-2023.7.0/gvsbuild/projects/icu.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 @project_add
 class Icu(Tarball, Project):
     def __init__(self):
         Project.__init__(
             self,
             "icu",
             repository="https://github.com/unicode-org/icu",
-            version="73.1",
+            version="73.2",
             archive_url="https://github.com/unicode-org/icu/releases/download/release-{major}-{minor}/icu4c-{major}_{minor}-src.zip",
-            hash="b7e2d8462c990e08e79f568529f75c5f628acf7213a057d19f171e711cb61c02",
+            hash="2c4300315141942178502f85f1167c0a6a65847c9b683e95c79535b373c1e369",
         )
 
     def build(self):
         bindir = r".\bin"
         libdir = r".\lib"
         if not self.builder.x86:
             bindir += "64"
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/json_glib.py` & `gvsbuild-2023.7.0/gvsbuild/projects/json_glib.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/jsonc.py` & `gvsbuild-2023.7.0/gvsbuild/projects/jsonc.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/leveldb.py` & `gvsbuild-2023.7.0/gvsbuild/projects/leveldb.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/lgi.py` & `gvsbuild-2023.7.0/gvsbuild/projects/lgi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libadwaita.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libadwaita.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libarchive.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libarchive.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libcroco.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libcroco.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libcurl.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libcurl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libepoxy.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libepoxy.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libffi.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libffi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libgxps.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libgxps.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libjpeg_turbo.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libjpeg_turbo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libmicrohttpd.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libmicrohttpd.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libpng.py` & `gvsbuild-2023.7.0/gvsbuild/projects/lmdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-from gvsbuild.utils.base_builders import CmakeProject
-from gvsbuild.utils.base_expanders import Tarball
+from gvsbuild.utils.base_builders import Meson
+from gvsbuild.utils.base_expanders import GitRepo
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Libpng(Tarball, CmakeProject):
+class Lmdb(GitRepo, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "libpng",
-            version="1.6.39",
-            archive_url="http://prdownloads.sourceforge.net/libpng/libpng-{version}.tar.xz",
-            hash="1f4696ce70b4ee5f85f1e1623dc1229b210029fa4b7aee573df3e2ba7b036937",
-            dependencies=["cmake", "ninja", "zlib"],
+            "lmdb",
+            repo_url="https://github.com/wingtk/lmdb.git",
+            fetch_submodules=False,
+            tag="mdb.RE/0.9-meson",
+            dependencies=[
+                "ninja",
+                "meson",
+            ],
         )
 
     def build(self):
-        CmakeProject.build(self, use_ninja=True)
-
-        self.install_pc_files()
-        self.install(r"LICENSE share\doc\libpng")
+        self.push_location(r".\libraries\liblmdb")
+        Meson.build(self)
+        self.install(r"LICENSE share\doc\lmdb")
+        self.pop_location()
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libpsl.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libpsl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/librsvg.py` & `gvsbuild-2023.7.0/gvsbuild/projects/librsvg.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,38 +22,40 @@
 
 @project_add
 class Librsvg(Tarball, Project):
     def __init__(self):
         Project.__init__(
             self,
             "librsvg",
-            version="2.56.0",
+            version="2.56.2",
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/librsvg",
             archive_url="https://download.gnome.org/sources/librsvg/{major}.{minor}/librsvg-{version}.tar.xz",
-            hash="194b5097d9cd107495f49c291cf0da65ec2b4bb55e5628369751a3f44ba222b3",
+            hash="3ec3c4d8f73e0ba4b9130026969e8371c092b734298d36e2fdb3eb4afcec1200",
             dependencies=[
                 "cargo",
                 "cairo",
                 "pango",
                 "gdk-pixbuf",
                 "libxml2",
             ],
-            patches=["enable_specifying_rust_version.patch"],
         )
         if Project.opts.enable_gi:
             self.add_dependency("gobject-introspection")
 
     def build(self):
         self.builder.mod_env("INCLUDE", "include\\cairo", add_gtk=True)
 
         b_dir = f"{self.builder.working_dir}\\{self.name}\\win32"
 
-        # TODO: The TOOLCHAIN_VERSION should come from the installed Rust version
-        cmd = f"nmake -f makefile.vc CFG={self.builder.opts.configuration} PREFIX={self.builder.gtk_dir} PYTHON={sys.executable} TOOLCHAIN_VERSION=1.69.0 install"
+        config = self.builder.opts.configuration
+        gtk_dir = self.builder.gtk_dir
+        rust_ver = Project.get_project("cargo").version
+        python = sys.executable
+        cmd = f"nmake -f makefile.vc CFG={config} PREFIX={gtk_dir} CARGO=cargo RUSTUP=rustup PYTHON={python} TOOLCHAIN_VERSION={rust_ver} install"
 
         if Project.opts.enable_gi:
             cmd += " INTROSPECTION=1"
 
         self.push_location(b_dir)
         self.exec_vs(cmd)
         self.pop_location()
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libsigcplusplus.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libsigcplusplus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libsoup.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libsoup.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libssh.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libssh.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libtiff.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libtiff.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 @project_add
 class Libtiff4(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
             "libtiff-4",
-            version="4.5.0",
+            version="4.5.1",
             repository="https://gitlab.com/libtiff/libtiff",
             archive_url="http://download.osgeo.org/libtiff/tiff-{version}.tar.gz",
-            hash="c7a1d9296649233979fa3eacffef3fa024d73d05d589cb622727b5b08c423464",
+            hash="d7f38b6788e4a8f5da7940c5ac9424f494d8a79eba53d555f4a507167dca5e2b",
             dependencies=["cmake", "ninja", "libjpeg-turbo"],
             patches=[
                 "0001-cmake-remove-.d-postfix.patch",
             ],
         )
 
     def build(self):
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libuv.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libuv.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 @project_add
 class Libuv(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
             "libuv",
-            version="1.45.0",
+            version="1.46.0",
             archive_file_name="libuv-v{version}.tar.gz",
             archive_url="https://github.com/libuv/libuv/archive/v{version}.tar.gz",
-            hash="458e34d5ef7f3c0394a2bfd8c39d757cb1553baa5959b9b4b45df63aa027a228",
+            hash="7aa66be3413ae10605e1f5c9ae934504ffe317ef68ea16fdaa83e23905c681bd",
             dependencies=[
                 "cmake",
                 "ninja",
             ],
         )
 
     def build(self):
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libvorbis.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libvorbis.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libvpx.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libvpx.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libxml2.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libxml2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libyuv.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libyuv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/libzip.py` & `gvsbuild-2023.7.0/gvsbuild/projects/libzip.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 @project_add
 class Libzip(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
             "libzip",
-            version="1.9.2",
+            version="1.10.0",
             archive_url="https://libzip.org/download/libzip-{version}.tar.gz",
-            hash="fd6a7f745de3d69cf5603edc9cb33d2890f0198e415255d0987a0cf10d824c6f",
+            hash="52a60b46182587e083b71e2b82fcaaba64dd5eb01c5b1f1bc71069a3858e40fe",
             dependencies=["cmake", "ninja", "zlib"],
         )
 
     def build(self):
         CmakeProject.build(self, use_ninja=True)
         self.install(r".\LICENSE share\doc\libzip")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/lmdb.py` & `gvsbuild-2023.7.0/gvsbuild/projects/openh264.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 from gvsbuild.utils.base_builders import Meson
-from gvsbuild.utils.base_expanders import GitRepo
+from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Lmdb(GitRepo, Meson):
+class OpenH264(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "lmdb",
-            repo_url="https://github.com/wingtk/lmdb.git",
-            fetch_submodules=False,
-            tag="mdb.RE/0.9-meson",
+            "openh264",
+            version="2.3.1",
+            archive_url="https://github.com/cisco/openh264/archive/refs/tags/v{version}.tar.gz",
+            archive_file_name="openh264-{version}.tar.gz",
+            hash="453afa66dacb560bc5fd0468aabee90c483741571bca820a39a1c07f0362dc32",
             dependencies=[
                 "ninja",
                 "meson",
+                "nasm",
             ],
         )
 
     def build(self):
-        self.push_location(r".\libraries\liblmdb")
         Meson.build(self)
-        self.install(r"LICENSE share\doc\lmdb")
-        self.pop_location()
+        self.install(r"LICENSE share\doc\openh264")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/luajit.py` & `gvsbuild-2023.7.0/gvsbuild/projects/luajit.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/lz4.py` & `gvsbuild-2023.7.0/gvsbuild/projects/lz4.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/mit_kerberos.py` & `gvsbuild-2023.7.0/gvsbuild/projects/mit_kerberos.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/nghttp2.py` & `gvsbuild-2023.7.0/gvsbuild/projects/ogg.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,34 +10,28 @@
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
-
 from gvsbuild.utils.base_builders import CmakeProject
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Nghttp2(Tarball, CmakeProject):
+class Ogg(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
-            "nghttp2",
-            version="1.53.0",
-            archive_url="https://github.com/nghttp2/nghttp2/releases/download/v{version}/nghttp2-{version}.tar.xz",
-            hash="b867184254e5a29b0ba68413aa14f8b0ce1142a371761374598dec092dabb809",
-            dependencies=[
-                "cmake",
-                "zlib",
-                "ninja",
-            ],
-            patches=["0001-Define-ssize_t-if-not-defined.patch"],
+            "ogg",
+            version="1.3.5",
+            repository="https://github.com/xiph/ogg",
+            archive_url="https://github.com/xiph/ogg/releases/download/v{version}/libogg-{version}.tar.xz",
+            hash="c4d91be36fc8e54deae7575241e03f4211eb102afb3fc0775fbbc1b740016705",
+            dependencies=["cmake", "ninja"],
         )
 
     def build(self):
         CmakeProject.build(self, use_ninja=True)
-
-        self.install(r".\COPYING share\doc\nghttp2")
+        self.install(r".\COPYING share\doc\ogg")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/ogg.py` & `gvsbuild-2023.7.0/gvsbuild/projects/wing.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
-from gvsbuild.utils.base_builders import CmakeProject
+
+from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Ogg(Tarball, CmakeProject):
+class Wing(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "ogg",
-            version="1.3.5",
-            repository="https://github.com/xiph/ogg",
-            archive_url="https://github.com/xiph/ogg/releases/download/v{version}/libogg-{version}.tar.xz",
-            hash="c4d91be36fc8e54deae7575241e03f4211eb102afb3fc0775fbbc1b740016705",
-            dependencies=["cmake", "ninja"],
+            "wing",
+            version="0.3.18",
+            repository="https://gitlab.gnome.org/GNOME/wing",
+            archive_url="https://gitlab.gnome.org/GNOME/wing/-/archive/v{version}/wing-v{version}.tar.gz",
+            hash="6d15984c917d9bdf2c88a06072991daf39a226d2024ec5b196a1c9ed8e81e962",
+            dependencies=["ninja", "meson", "pkgconf", "glib"],
         )
 
     def build(self):
-        CmakeProject.build(self, use_ninja=True)
-        self.install(r".\COPYING share\doc\ogg")
+        Meson.build(self)
+        self.install(r".\COPYING share\doc\wing")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/openh264.py` & `gvsbuild-2023.7.0/gvsbuild/projects/pangomm.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,30 +13,39 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
-from gvsbuild.utils.base_project import Project, project_add
+from gvsbuild.utils.base_project import project_add
 
 
 @project_add
-class OpenH264(Tarball, Meson):
+class Pangomm(Tarball, Meson):
     def __init__(self):
-        Project.__init__(
+        Meson.__init__(
             self,
-            "openh264",
-            version="2.3.1",
-            archive_url="https://github.com/cisco/openh264/archive/refs/tags/v{version}.tar.gz",
-            archive_file_name="openh264-{version}.tar.gz",
-            hash="453afa66dacb560bc5fd0468aabee90c483741571bca820a39a1c07f0362dc32",
+            "pangomm",
+            prj_dir="pangomm",
+            version="2.50.1",
+            lastversion_even=True,
+            repository="https://gitlab.gnome.org/GNOME/pangomm",
+            archive_url="https://download.gnome.org/sources/pangomm/{major}.{minor}/pangomm-{version}.tar.xz",
+            hash="ccc9923413e408c2bff637df663248327d72822f11e394b423e1c5652b7d9214",
             dependencies=[
-                "ninja",
                 "meson",
-                "nasm",
+                "ninja",
+                "libsigc++",
+                "cairomm",
+                "pango",
+                "glibmm",
             ],
         )
 
     def build(self):
-        Meson.build(self)
-        self.install(r"LICENSE share\doc\openh264")
+        Meson.build(
+            self,
+            meson_params="-Dbuild-documentation=false",
+        )
+
+        self.install(r".\COPYING share\doc\glibmm")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/openssl.py` & `gvsbuild-2023.7.0/gvsbuild/projects/openssl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/opus.py` & `gvsbuild-2023.7.0/gvsbuild/projects/opus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/pango.py` & `gvsbuild-2023.7.0/gvsbuild/projects/pango.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/pangomm.py` & `gvsbuild-2023.7.0/gvsbuild/projects/pycairo.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,40 +11,39 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
+from pathlib import Path
+
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import project_add
 
 
 @project_add
-class Pangomm(Tarball, Meson):
+class Pycairo(Tarball, Meson):
     def __init__(self):
         Meson.__init__(
             self,
-            "pangomm",
-            prj_dir="pangomm",
-            version="2.50.1",
-            lastversion_even=True,
-            repository="https://gitlab.gnome.org/GNOME/pangomm",
-            archive_url="https://download.gnome.org/sources/pangomm/{major}.{minor}/pangomm-{version}.tar.xz",
-            hash="ccc9923413e408c2bff637df663248327d72822f11e394b423e1c5652b7d9214",
-            dependencies=[
-                "meson",
-                "ninja",
-                "libsigc++",
-                "cairomm",
-                "pango",
-            ],
+            "pycairo",
+            version="1.24.0",
+            archive_url="https://github.com/pygobject/pycairo/releases/download/v{version}/pycairo-{version}.tar.gz",
+            hash="1444d52f1bb4cc79a4a0c0fe2ccec4bd78ff885ab01ebe1c0f637d8392bcafb6",
+            dependencies=["cairo"],
         )
 
     def build(self):
-        Meson.build(
-            self,
-            meson_params="-Dbuild-documentation=false",
-        )
-
-        self.install(r".\COPYING share\doc\glibmm")
+        Meson.build(self)
+        cairo_inc = Path(self.builder.gtk_dir) / "include" / "cairo"
+        self.builder.mod_env("INCLUDE", str(cairo_inc))
+        self.exec_vs(r"%(python_dir)s\python.exe -m build")
+        dist_dir = Path(self.build_dir) / "dist"
+        for path in dist_dir.rglob("*.whl"):
+            self.exec_vs(r"%(python_dir)s\python.exe -m pip install " + str(path))
+        if self.builder.opts.py_wheel:
+            self.install_dir("dist", "python")
+        self.install(r".\COPYING share\doc\pycairo")
+        self.install(r".\COPYING-LGPL-2.1 share\doc\pycairo")
+        self.install(r".\COPYING-MPL-1.1 share\doc\pycairo")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/pcre2.py` & `gvsbuild-2023.7.0/gvsbuild/projects/pcre2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/pixman.py` & `gvsbuild-2023.7.0/gvsbuild/projects/pixman.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,44 +11,35 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-import os
+from gvsbuild.utils.base_builders import Meson
 
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Pixman(Tarball, Project):
+class Pixman(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "pixman",
             repository="https://gitlab.freedesktop.org/pixman/pixman",
             version="0.42.2",
             lastversion_even=True,
             archive_url="http://cairographics.org/releases/pixman-{version}.tar.gz",
             hash="ea1480efada2fd948bc75366f7c349e1c96d3297d09a3fe62626e38e234a625e",
+            dependencies=["ninja", "meson"],
         )
 
     def build(self):
-        optimizations = "SSE2=on SSSE3=on" + (
-            " MMX=off" if self.builder.x64 else " MMX=on"
-        )
-
-        add_path = os.path.join(self.builder.opts.msys_dir, "usr", "bin")
-
-        self.exec_vs(
-            f"make -f Makefile.win32 pixman CFG=%(configuration)s {optimizations}",
-            add_path=add_path,
+        enable_mmx = "disabled" if self.builder.x64 else "enabled"
+        Meson.build(
+            self,
+            meson_params=f"-Dsse2=enabled -Dssse3=enabled -Dmmx={enable_mmx} -Dtests=disabled",
         )
 
-        self.install(r".\pixman\%(configuration)s\pixman-1.lib lib")
-
-        self.install(r".\pixman\pixman.h include\pixman-1")
-        self.install(r".\pixman\pixman-version.h include\pixman-1")
-
         self.install(r".\COPYING share\doc\pixman")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/pkgconf.py` & `gvsbuild-2023.7.0/gvsbuild/projects/pkgconf.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class PkgConf(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "pkgconf",
             prj_dir="pkgconf",
             version="1.9.5",
-            archive_url="https://distfiles.dereferenced.org/pkgconf/pkgconf-{version}.tar.gz",
+            archive_url="https://distfiles.ariadne.space/pkgconf/pkgconf-{version}.tar.gz",
             hash="6466efd2e38c4c0ac5de4e345f0dc6dad57e689efb08c31f2a71547683d20dc7",
             dependencies=["ninja", "meson"],
             patches=["0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch"],
         )
         self.add_param("-Dtests=disabled")
 
     def build(self):
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/protobuf.py` & `gvsbuild-2023.7.0/gvsbuild/projects/protobuf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/pycairo.py` & `gvsbuild-2023.7.0/gvsbuild/projects/pygobject.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,35 +15,47 @@
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
-from gvsbuild.utils.base_project import project_add
+from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Pycairo(Tarball, Meson):
+class PyGObject(Tarball, Meson):
     def __init__(self):
-        Meson.__init__(
+        Project.__init__(
             self,
-            "pycairo",
-            version="1.23.0",
-            archive_url="https://github.com/pygobject/pycairo/releases/download/v{version}/pycairo-{version}.tar.gz",
-            hash="9b61ac818723adc04367301317eb2e814a83522f07bbd1f409af0dada463c44c",
-            dependencies=["cairo"],
+            "pygobject",
+            version="3.44.1",
+            lastversion_even=True,
+            repository="https://gitlab.gnome.org/GNOME/pygobject",
+            archive_url="https://download.gnome.org/sources/pygobject/{major}.{minor}/pygobject-{version}.tar.xz",
+            hash="3c6805d1321be90cc32e648215a562430e0d3d6edcda8f4c5e7a9daffcad5710",
+            dependencies=["pycairo", "gobject-introspection", "libffi"],
+            patches=[
+                "pygobject_py3_8_load_dll.patch",
+            ],
         )
 
     def build(self):
         Meson.build(self)
-        cairo_inc = Path(self.builder.gtk_dir) / "include" / "cairo"
-        self.builder.mod_env("INCLUDE", str(cairo_inc))
+        gtk_dir = self.builder.gtk_dir
+        add_inc = [
+            str(Path(gtk_dir) / "include" / "cairo"),
+            str(Path(gtk_dir) / "include" / "gobject-introspection-1.0"),
+            str(Path(gtk_dir) / "include" / "glib-2.0"),
+            str(Path(gtk_dir) / "lib" / "glib-2.0" / "include"),
+        ]
+        self.builder.mod_env("INCLUDE", ";".join(add_inc))
         self.exec_vs(r"%(python_dir)s\python.exe -m build")
         dist_dir = Path(self.build_dir) / "dist"
         for path in dist_dir.rglob("*.whl"):
-            self.exec_vs(r"%(python_dir)s\python.exe -m pip install " + str(path))
+            self.exec_vs(
+                r"%(python_dir)s\python.exe -m pip install --force-reinstall "
+                + str(path)
+            )
         if self.builder.opts.py_wheel:
             self.install_dir("dist", "python")
-        self.install(r".\COPYING share\doc\pycairo")
-        self.install(r".\COPYING-LGPL-2.1 share\doc\pycairo")
-        self.install(r".\COPYING-MPL-1.1 share\doc\pycairo")
+        self.install(r".\COPYING share\doc\pygobject")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/sqlite.py` & `gvsbuild-2023.7.0/gvsbuild/projects/sqlite.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/win_iconv.py` & `gvsbuild-2023.7.0/gvsbuild/projects/win_iconv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/wing.py` & `gvsbuild-2023.7.0/gvsbuild/projects/nghttp2.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,28 +11,33 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-from gvsbuild.utils.base_builders import Meson
+from gvsbuild.utils.base_builders import CmakeProject
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Wing(Tarball, Meson):
+class Nghttp2(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
-            "wing",
-            version="0.3.18",
-            repository="https://gitlab.gnome.org/GNOME/wing",
-            archive_url="https://gitlab.gnome.org/GNOME/wing/-/archive/v{version}/wing-v{version}.tar.gz",
-            hash="6d15984c917d9bdf2c88a06072991daf39a226d2024ec5b196a1c9ed8e81e962",
-            dependencies=["ninja", "meson", "pkgconf", "glib"],
+            "nghttp2",
+            version="1.54.0",
+            archive_url="https://github.com/nghttp2/nghttp2/releases/download/v{version}/nghttp2-{version}.tar.xz",
+            hash="20533c9354fbb6aa689b6aa0ddb77f91da1d242587444502832e1864308152df",
+            dependencies=[
+                "cmake",
+                "zlib",
+                "ninja",
+            ],
+            patches=["0001-Define-ssize_t-if-not-defined.patch"],
         )
 
     def build(self):
-        Meson.build(self)
-        self.install(r".\COPYING share\doc\wing")
+        CmakeProject.build(self, use_ninja=True)
+
+        self.install(r".\COPYING share\doc\nghttp2")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/x264.py` & `gvsbuild-2023.7.0/gvsbuild/projects/x264.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/projects/zlib.py` & `gvsbuild-2023.7.0/gvsbuild/projects/zlib.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/tools.py` & `gvsbuild-2023.7.0/gvsbuild/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 @tool_add
 class ToolCargo(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "cargo",
-            version="1.69.0",
+            version="1.70.0",
             repository="rust-lang/rust",
             archive_url="https://win.rustup.rs/x86_64",
             archive_file_name="rustup-init.exe",
             exe_name="cargo.exe",
         )
 
     def load_defaults(self):
@@ -207,17 +207,17 @@
 
 @tool_add
 class ToolGo(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "go",
-            version="1.20.4",
+            version="1.20.5",
             archive_url="https://go.dev/dl/go{version}.windows-amd64.zip",
-            hash="e7528da720f470b711fbd826814167a5fe1bc02a479ab1958dcf839a8294e6d2",
+            hash="c04a4ed73c3624d5b4c4f62e44a141549cc0bfd83a7492c31ca8b86b3752f077",
             dir_part="go-{version}",
         )
 
     def load_defaults(self):
         Tool.load_defaults(self)
         self.tool_path = os.path.join(self.build_dir, "bin")
         self.full_exe = os.path.join(self.tool_path, "go.exe")
```

### Comparing `gvsbuild-2023.6.0/gvsbuild/utils/base_builders.py` & `gvsbuild-2023.7.0/gvsbuild/utils/base_builders.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/utils/base_expanders.py` & `gvsbuild-2023.7.0/gvsbuild/utils/base_expanders.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/utils/base_group.py` & `gvsbuild-2023.7.0/gvsbuild/utils/base_group.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/utils/base_project.py` & `gvsbuild-2023.7.0/gvsbuild/utils/base_project.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/utils/base_tool.py` & `gvsbuild-2023.7.0/gvsbuild/utils/base_tool.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/utils/builder.py` & `gvsbuild-2023.7.0/gvsbuild/utils/builder.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/utils/simple_ui.py` & `gvsbuild-2023.7.0/gvsbuild/utils/simple_ui.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/gvsbuild/utils/utils.py` & `gvsbuild-2023.7.0/gvsbuild/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/pyproject.toml` & `gvsbuild-2023.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "gvsbuild"
-version = "2023.6.0"
+version = "2023.7.0"
 description = "GTK stack for Windows"
 authors = ["Ignacio Casal Quinteiro <qignacio@amazon.com>", "Dan Yeaw <dan@yeaw.me>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Build Tools",
     "Environment :: X11 Applications :: GTK",
     "Operating System :: Microsoft :: Windows",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 build = ">=0.9,<0.11"
-lastversion = { version = "^2.4.2", optional = true }
+lastversion = { version = ">=2.4.2,<4.0.0", optional = true }
 packaging = { version = ">=21.3,<24.0", optional = true }
 typer = {extras = ["all"], version = ">=0.6.1,<0.10.0"}
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.1"
 pytest = "^7.1.3"
 tox = "^4.1.2"
@@ -38,22 +38,23 @@
 profile = "black"
 skip = ".venv"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
-envlist = py38, py39, py310, py311
+envlist = py{38,39,310,311,312}
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
+    3.12: py312
 
 [testenv]
 commands = pytest
 deps = pytest
 """
 
 [tool.ruff]
```

### Comparing `gvsbuild-2023.6.0/README.md` & `gvsbuild-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2023.6.0/setup.py` & `gvsbuild-2023.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
               'patches/libpng/*',
               'patches/libpng/pc-files/*',
               'patches/libpsl/*',
               'patches/librsvg-legacy/*',
               'patches/librsvg-legacy/build/win32/vs12/*',
               'patches/librsvg-legacy/build/win32/vs14/*',
               'patches/librsvg-legacy/build/win32/vs15/*',
-              'patches/librsvg/*',
               'patches/libsoup3/*',
               'patches/libssh/*',
               'patches/libssh/build/vs12/*',
               'patches/libssh/build/vs14/*',
               'patches/libssh/build/vs15/*',
               'patches/libtiff-4/*',
               'patches/libvpx/*',
@@ -185,22 +184,22 @@
               'patches/x264/build/*',
               'patches/zlib/pc-files/*']}
 
 install_requires = \
 ['build>=0.9,<0.11', 'typer[all]>=0.6.1,<0.10.0']
 
 extras_require = \
-{'outdated': ['lastversion>=2.4.2,<3.0.0', 'packaging>=21.3,<24.0']}
+{'outdated': ['lastversion>=2.4.2,<4.0.0', 'packaging>=21.3,<24.0']}
 
 entry_points = \
 {'console_scripts': ['gvsbuild = gvsbuild.main:run']}
 
 setup_kwargs = {
     'name': 'gvsbuild',
-    'version': '2023.6.0',
+    'version': '2023.7.0',
     'description': 'GTK stack for Windows',
     'long_description': '# gvsbuild\n\n![CI](https://github.com/wingtk/gvsbuild/workflows/CI/badge.svg)\n\nThis python script helps you build a full [GTK](https://www.gtk.org/) library\nstack for Windows using Visual Studio. Currently, GTK 3 and GTK 4 are supported.\n\nThe script supports multiple versions of Visual Studio - at the moment we are\nfocusing on VS 2022, but we include projects for other versions, and we gladly\naccept patches.\n\nThe script focuses on GTK and the surrounding ecosystem (e.g. GStreamer).\nHowever, we are open to adding more libraries as long as the contributor takes\non the responsibility for keeping it up to date. The supported projects are\nmodules in the\n[projects](https://github.com/wingtk/gvsbuild/blob/master/gvsbuild/projects)\ndirectory.\n\nThe script requires a working installation of [Visual Studio for Windows\nDesktop](http://www.visualstudio.com), [Python 3](https://www.python.org) and\n[msys2](https://msys2.github.io). The script will download any additional tools\nrequired to build the libraries and will use them from a local directory,\nwithout any installation. As of today these tools include cmake, meson, ninja,\nnuget and perl.\n\nThe script fetches source tarballs for the projects from their original\nlocations, however in some cases it might be necessary to host a patched tarball\non GitHub. To ensure integrity of the downloaded files, the script checks the\nSHA256 hash of each download. Downloads are done using TLS, using SSL\ncertificates provided by the system, but in case of error the download is tried\nagain ignoring certificate errors.\n\n## Development Environment\n\n### Choco\nWe recommend using [Chocolately](https://chocolatey.org/) as a package manager\nin Windows.\n\nTo install it, open PowerShell as an administrator, then execute:\n\n```PowerShell\nSet-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString(\'https://community.chocolatey.org/install.ps1\'))\n```\nTo run local scripts in follow-on steps, also execute\n`Set-ExecutionPolicy RemoteSigned`. This allows for local PowerShell scripts\nto run without signing, but still requires signing for remote scripts.\n\n### Git\nTo setup a development environment in Windows install\n[Git](https://gitforwindows.org) by executing as an administrator:\n\n```PowerShell\nchoco install git\n```\n\n### MSYS2\nBoth of the development environments in the next steps need MSYS2 installed.\n\nInstall [MSYS2](http://www.msys2.org/):\n\nKeep PowerShell open as administrator and execute:\n```PowerShell\nchoco install msys2\n```\n\n### Building GTK\n\nFirst we will install the gvsbuild dependencies:\n1. Visual C++ build tools workload for Visual Studio 2022 Build Tools\n2. Python\n\n#### Install Visual Studio 2022\nWith your admin PowerShell terminal:\n\n```PowerShell\nchoco install visualstudio2022-workload-vctools\n```\n\nNote: Visual Studio versions 2013 (not for all projects), 2015, 2017, 2019, and 2022 are currently supported.\n\n#### Install the Latest Python\n\nDownload and install the latest version of Python:\n\n1. Install from Chocolately with `choco install python` with admin PowerShell\n1. Restart your PowerShell terminal as a normal user and check that `python --version` is correct.\n\nNote: If you are going to install Python using an alternative means, like the\nofficial Windows installers, we suggest to install Python in C:\\Python3x, for\nexample C:\\Python310. Other Python distributions like [Miniconda\n3](https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe)\nshould also work.\n\n#### Install gvsbuild\nThe recommended way to install gvsbuild is with pipx. Open a new regular user\nPowerShell terminal and execute:\n\n```PowerShell\npython -m pip install --user pipx\npython -m pipx ensurepath\npipx install gvsbuild\n```\n\nAlternatively, you can also use git to clone the repository and install it.\nOpen a new regular user PowerShell terminal and execute:\n\n```PowerShell\nmkdir C:\\gtk-build\\github\ncd C:\\gtk-build\\github\ngit clone https://github.com/wingtk/gvsbuild.git\ncd C:\\gtk-build\\github\\gvsbuild\npython -m venv .venv\n.\\.venv\\Scripts\\activate.ps1\npip install .\n```\n\n#### Build GTK\n\nIn the same PowerShell terminal, execute:\n\n```PowerShell\ngvsbuild build gtk3\n```\n\nAlternatively, if you want to build GTK 4, execute:\n```PowerShell\ngvsbuild build gtk4\n```\n\nGrab a coffee, the build will take a few minutes to complete.\n\n#### Add GTK to Your Environmental Variables\n\n```PowerShell\n$env:Path = "C:\\gtk-build\\gtk\\x64\\release\\bin;" + $env:Path\n$env:LIB = "C:\\gtk-build\\gtk\\x64\\release\\lib;" + $env:LIB\n$env:INCLUDE = "C:\\gtk-build\\gtk\\x64\\release\\include;C:\\gtk-build\\gtk\\x64\\release\\include\\cairo;C:\\gtk-build\\gtk\\x64\\release\\include\\glib-2.0;C:\\gtk-build\\gtk\\x64\\release\\include\\gobject-introspection-1.0;C:\\gtk-build\\gtk\\x64\\release\\lib\\glib-2.0\\include;" + $env:INCLUDE\n```\n\n#### Use PyGObject\n\nAdd the `--enable-gi` and `--py-wheel` options like:\n\n```PowerShell\ngvsbuild build --enable-gi --py-wheel gtk4 pygobject\n```\n\nOnce that finishes, then you need to use the gvsbuild generated wheels with your\n[Python virtualenv](https://docs.python.org/3/tutorial/venv.html) in order to\nwork around this [PyGObject\nbug](https://gitlab.gnome.org/GNOME/pygobject/-/issues/545):\n\n```PowerShell\npip install --force-reinstall (Resolve-Path C:\\gtk-build\\build\\x64\\release\\pygobject\\dist\\PyGObject*.whl)\npip install --force-reinstall (Resolve-Path C:\\gtk-build\\build\\x64\\release\\pycairo\\dist\\pycairo*.whl)\n```\n\n#### Other Options\n\n For more information about the possible commands run:\n\n ```\n gvsbuild --help\n ```\n\n To get detailed help on the build command run:\n\n ```\n gvsbuild build --help\n ```\n\n It is possible to set some parameters from a file, e.g. vs2015-release.pro, putting\n the @ character before the file name. The file contains the option, one per\n line, separated by a carriage return:\n\n ```\n --vs-ver\n 14\n --win-sdk\n 8.1\n --configuration\n release\n ```\n\n Even if the format is not the easier to write or read in this way we eliminate\n the problem of escaping spaces is file names and directories. Then you can use\n it:\n\n ```\n gvsbuild build @vs2015-release.pro gtk3-full\n ```\n\n## Troubleshooting\n\n- If a build fails, try rebuilding it with `--clean`, if that fails, try\nrebuilding it with `--from-scratch`\n- If the download of a tarball fails a partial file will not pass the hash check,\ndelete the file and try again.\n\n## OpenSSL\n\nIn addition to the setup instructions above, to build OpenSSL you also need the\nVisual C++ 2013 Redistributable Package installed. To install it, open PowerShell\nas administrator and execute:\n\n```PowerShell\nchoco install vcredist2013\n```\n\nSimilar to other packages, you can build OpenSSL by executing:\n```\ngvsbuild build openssl\n```\n\n## Dependency Graph\n\nTo see and analyze the dependency between the various projects, in text or in a\nGraphviz format, use the script deps.py:\n\n ```\ngvsbuild deps --graph --gv-file test.gv\n ```\n\nWithout option a simple dependency of all the projects is printed, as usual with\n--help a summary of the options/commands is printed.\n\n## License\n\nThis build script is licensed under the GPL2.0 license, see the COPYING file for\nthe full text.\n\nThe binaries produced by the build script are licensed under the license terms\nof the project that is built (ie glib is LGPL so you can use glib.dll built\nwith this script under the terms of LGPL).\n\nPatches included in the repository are licensed under the license terms of the\nproject they apply to.\n\n## Credits\n\nThis tool originated from a gtk-win32 PowerShell script created by the\n[HexChat](https://hexchat.github.io/) developers for building it for Windows.\nAlthough this project is now archived, you can explore the original project if you\nare interested in the history at https://github.com/hexchat/gtk-win32.\n\nCompiling the GTK stack on MSVC would not be possible without the incredible\nwork by [Fan Chun-wei](https://github.com/fanc999). If you are interested in more\ndetails of how this works, please see [Compiling the GTK+ (and Clutter) stack using\nVisual C++ 2008 and\nlater](https://wiki.gnome.org/Projects/GTK/Win32/MSVCCompilationOfGTKStack).\n',
     'author': 'Ignacio Casal Quinteiro',
     'author_email': 'qignacio@amazon.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `gvsbuild-2023.6.0/PKG-INFO` & `gvsbuild-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvsbuild
-Version: 2023.6.0
+Version: 2023.7.0
 Summary: GTK stack for Windows
 License: GPL-2.0-only
 Author: Ignacio Casal Quinteiro
 Author-email: qignacio@amazon.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: outdated
 Requires-Dist: build (>=0.9,<0.11)
-Requires-Dist: lastversion (>=2.4.2,<3.0.0); extra == "outdated"
+Requires-Dist: lastversion (>=2.4.2,<4.0.0); extra == "outdated"
 Requires-Dist: packaging (>=21.3,<24.0); extra == "outdated"
 Requires-Dist: typer[all] (>=0.6.1,<0.10.0)
 Description-Content-Type: text/markdown
 
 # gvsbuild
 
 ![CI](https://github.com/wingtk/gvsbuild/workflows/CI/badge.svg)
```

