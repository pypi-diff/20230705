# Comparing `tmp/PyQt-Fluent-Widgets-1.0.0.tar.gz` & `tmp/PyQt-Fluent-Widgets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt-Fluent-Widgets-1.0.0.tar", last modified: Sun Jul  2 14:17:09 2023, max compression
+gzip compressed data, was "dist\PyQt-Fluent-Widgets-1.0.1.tar", last modified: Wed Jul  5 03:26:55 2023, max compression
```

## Comparing `PyQt-Fluent-Widgets-1.0.0.tar` & `PyQt-Fluent-Widgets-1.0.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.591021 PyQt-Fluent-Widgets-1.0.0/
--rw-rw-rw-   0        0        0    35825 2023-07-01 10:54:40.000000 PyQt-Fluent-Widgets-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4866 2023-07-02 14:17:09.588468 PyQt-Fluent-Widgets-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.433636 PyQt-Fluent-Widgets-1.0.0/PyQt_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4866 2023-07-02 14:17:09.000000 PyQt-Fluent-Widgets-1.0.0/PyQt_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4018 2023-07-02 14:17:09.000000 PyQt-Fluent-Widgets-1.0.0/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 14:17:09.000000 PyQt-Fluent-Widgets-1.0.0/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-02 14:17:09.000000 PyQt-Fluent-Widgets-1.0.0/PyQt_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-02 14:17:09.000000 PyQt-Fluent-Widgets-1.0.0/PyQt_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4090 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.435636 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/
--rw-rw-rw-   0        0        0      515 2023-07-02 13:02:26.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.439134 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  6256748 2023-07-02 11:35:02.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.473711 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10659 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      803 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    12165 2023-07-02 11:36:47.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4783 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3866 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0     4851 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7211 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      452 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.475140 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.485453 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2084 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21160 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7455 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19077 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5783 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.496126 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14724 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5291 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11337 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3238 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2500 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.503265 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5433 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1301 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.515132 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      535 2023-06-26 15:48:09.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0    10717 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8131 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    19795 2023-07-01 14:48:25.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    14603 2023-07-02 11:41:30.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6202 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     1386 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.526952 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5316 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8027 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6034 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2840 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13119 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1586 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.580432 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     2704 2023-07-02 10:45:02.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4598 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    21499 2023-07-02 02:34:02.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     3064 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     1609 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    13267 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19387 2023-07-02 05:17:08.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     7881 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    15887 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2043 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1329 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    17204 2023-07-02 01:30:28.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    18934 2023-07-02 10:44:34.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0     6834 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    10004 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3860 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    35966 2023-07-02 04:48:38.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     7520 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6321 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2479 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17756 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     5132 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4397 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6334 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5790 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     9027 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     8730 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    22249 2023-07-02 07:45:33.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10384 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2693 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:17:09.587469 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      115 2023-07-02 06:08:02.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    10170 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2846 2023-07-02 07:12:36.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1590 2023-07-01 06:27:12.000000 PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2023-07-02 14:17:09.591021 PyQt-Fluent-Widgets-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-07-02 13:02:17.000000 PyQt-Fluent-Widgets-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.228676 PyQt-Fluent-Widgets-1.0.1/
+-rw-rw-rw-   0        0        0    35825 2023-07-05 03:04:14.000000 PyQt-Fluent-Widgets-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5062 2023-07-05 03:26:55.226327 PyQt-Fluent-Widgets-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.055039 PyQt-Fluent-Widgets-1.0.1/PyQt_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5062 2023-07-05 03:26:54.000000 PyQt-Fluent-Widgets-1.0.1/PyQt_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4018 2023-07-05 03:26:54.000000 PyQt-Fluent-Widgets-1.0.1/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 03:26:54.000000 PyQt-Fluent-Widgets-1.0.1/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-05 03:26:54.000000 PyQt-Fluent-Widgets-1.0.1/PyQt_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-05 03:26:54.000000 PyQt-Fluent-Widgets-1.0.1/PyQt_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4286 2023-07-05 03:24:25.000000 PyQt-Fluent-Widgets-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.057689 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/
+-rw-rw-rw-   0        0        0      515 2023-07-05 03:24:56.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.061696 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  6256748 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.097383 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10659 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      803 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    12165 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4783 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3866 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4851 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7211 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      452 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.099381 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.109998 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2084 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21160 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7455 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19077 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5783 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.123227 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14724 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5291 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11337 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3238 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2500 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.131418 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5433 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1301 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.146545 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      535 2023-06-26 15:48:09.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0    10717 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8131 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    19795 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    14634 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6202 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     1386 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.161105 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5316 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8027 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6034 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2840 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13119 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1586 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.217745 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     2704 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4598 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    21499 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     3064 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     1609 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    13267 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19344 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     7881 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    15887 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2043 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1329 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    17204 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    18934 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0     6834 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    10004 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3860 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    36003 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     7520 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6321 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2479 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17756 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     5132 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4397 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6334 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5790 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     9027 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     8730 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    22249 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10384 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2693 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2023-07-05 03:26:55.224328 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      115 2023-07-02 14:53:20.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    10201 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2846 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1590 2023-07-05 03:04:15.000000 PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 03:26:55.228676 PyQt-Fluent-Widgets-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-07-05 03:24:43.000000 PyQt-Fluent-Widgets-1.0.1/setup.py
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/LICENSE` & `PyQt-Fluent-Widgets-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/PKG-INFO` & `PyQt-Fluent-Widgets-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 1.0.0
+Version: 1.0.1
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
@@ -24,25 +24,29 @@
   PyQt-Fluent-Widgets
 </h1>
 <p align="center">
   A fluent design widgets library based on PyQt5
 </p>
 
 <p align="center">
-  <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  <a href="https://pypi.org/project/PyQt-Fluent-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyqt-fluent-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
     <img src="https://static.pepy.tech/personalized-badge/pyqt-fluent-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
+
+  <a style="text-decoration:none">
+    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  </a>
 </p>
 
 <p align="center">
 English | <a href="docs/README_zh.md">简体中文</a>
 </p>
 
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/master/docs/source/_static/Interface.jpg)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.0.1 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyqt fluent widgets
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown Provides-Extra: full
 License-File: LICENSE
                                     [logo]
                        ****** PyQt-Fluent-Widgets ******
                 A fluent design widgets library based on PyQt5
-              [Platform Win32 | Linux | macOS] [Download] [GPLv3]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/
 master/docs/source/_static/Interface.jpg) ## Install To install lite version
 (`AcrylicLabel` is not available): ```shell pip install PyQt-Fluent-Widgets -
 i https://pypi.org/simple/ ``` Or install full-featured version: ```shell pip
 install "PyQt-Fluent-Widgets[full]" -i https://pypi.org/simple/ ``` If you are
 using PySide2, PySide6 or PyQt6, you can download the code in [PySide2](https:/
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/PyQt_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt-Fluent-Widgets-1.0.1/PyQt_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 1.0.0
+Version: 1.0.1
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
@@ -24,25 +24,29 @@
   PyQt-Fluent-Widgets
 </h1>
 <p align="center">
   A fluent design widgets library based on PyQt5
 </p>
 
 <p align="center">
-  <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  <a href="https://pypi.org/project/PyQt-Fluent-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyqt-fluent-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
     <img src="https://static.pepy.tech/personalized-badge/pyqt-fluent-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
+
+  <a style="text-decoration:none">
+    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  </a>
 </p>
 
 <p align="center">
 English | <a href="docs/README_zh.md">简体中文</a>
 </p>
 
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/master/docs/source/_static/Interface.jpg)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.0.1 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyqt fluent widgets
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown Provides-Extra: full
 License-File: LICENSE
                                     [logo]
                        ****** PyQt-Fluent-Widgets ******
                 A fluent design widgets library based on PyQt5
-              [Platform Win32 | Linux | macOS] [Download] [GPLv3]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/
 master/docs/source/_static/Interface.jpg) ## Install To install lite version
 (`AcrylicLabel` is not available): ```shell pip install PyQt-Fluent-Widgets -
 i https://pypi.org/simple/ ``` Or install full-featured version: ```shell pip
 install "PyQt-Fluent-Widgets[full]" -i https://pypi.org/simple/ ``` If you are
 using PySide2, PySide6 or PyQt6, you can download the code in [PySide2](https:/
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/PyQt_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt-Fluent-Widgets-1.0.1/PyQt_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/README.md` & `PyQt-Fluent-Widgets-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,29 @@
   PyQt-Fluent-Widgets
 </h1>
 <p align="center">
   A fluent design widgets library based on PyQt5
 </p>
 
 <p align="center">
-  <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  <a href="https://pypi.org/project/PyQt-Fluent-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyqt-fluent-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
     <img src="https://static.pepy.tech/personalized-badge/pyqt-fluent-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
   </a>
 
   <a style="text-decoration:none">
     <img src="https://img.shields.io/badge/License-GPLv3-blue?color=#4ec820" alt="GPLv3"/>
   </a>
+
+  <a style="text-decoration:none">
+    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  </a>
 </p>
 
 <p align="center">
 English | <a href="docs/README_zh.md">简体中文</a>
 </p>
 
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/master/docs/source/_static/Interface.jpg)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                                     [logo]
                        ****** PyQt-Fluent-Widgets ******
                 A fluent design widgets library based on PyQt5
-              [Platform Win32 | Linux | macOS] [Download] [GPLv3]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/
 master/docs/source/_static/Interface.jpg) ## Install To install lite version
 (`AcrylicLabel` is not available): ```shell pip install PyQt-Fluent-Widgets -
 i https://pypi.org/simple/ ``` Or install full-featured version: ```shell pip
 install "PyQt-Fluent-Widgets[full]" -i https://pypi.org/simple/ ``` If you are
 using PySide2, PySide6 or PyQt6, you can download the code in [PySide2](https:/
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/__init__.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/master/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from .components import *
 from .common import *
 from .window import *
 from ._rc import resource
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/_rc/resource.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/__init__.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/animation.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/auto_wrap.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/config.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/exception_handler.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/font.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/icon.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/image_utils.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/overload.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/router.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/smooth_scroll.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/common/style_sheet.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/calendar_picker.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/calendar_view.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/date_picker.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/picker_base.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/time_picker.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/expand_layout.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/flow_layout.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/__init__.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_bar.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         self.rotateAni.setEndValue(180 if isExpanded else 0)
         self.rotateAni.setDuration(150)
         self.rotateAni.start()
 
     def mouseReleaseEvent(self, e):
         super().mouseReleaseEvent(e)
         clickArrow = QRectF(self.width()-30, 8, 20, 20).contains(e.pos())
-        self.itemClicked.emit(True, clickArrow)
+        self.itemClicked.emit(True, clickArrow and not self.parent().isLeaf())
         self.update()
 
     def _canDrawIndicator(self):
         p = self.parent()   # type: NavigationTreeWidget
         if p.isLeaf() or p.isSelected:
             return p.isSelected
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/pivot.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/segmented_widget.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/__init__.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/setting_card.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/__init__.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/button.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/card_widget.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/check_box.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/combo_box.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/command_bar.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/command_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,28 +353,27 @@
 
         visibles = self._visibleWidgets()
         x = self.contentsMargins().left()
         h = self.height()
 
         for widget in visibles:
             widget.show()
-            w, h = widget.width(), widget.height()
             widget.move(x, (h - widget.height()) // 2)
-            x += (w + self.spacing())
+            x += (widget.width() + self.spacing())
 
         # show more actions button
         if self._hiddenActions or len(visibles) < len(self._widgets):
             self.moreButton.show()
             self.moreButton.move(x, (h - self.moreButton.height()) // 2)
 
         for widget in self._widgets[len(visibles):]:
             widget.hide()
             self._hiddenWidgets.append(widget)
 
-    def _visibleWidgets(self) -> List[QLayoutItem]:
+    def _visibleWidgets(self) -> List[QWidget]:
         """ return the visible widgets in layout """
         # have enough spacing to show all widgets
         if self.suitableWidth() <= self.width():
             return self._widgets
 
         w = self.moreButton.width()
         for index, widget in enumerate(self._widgets):
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/flyout.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/frameless_window.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/info_badge.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/info_bar.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/label.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/line_edit.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/list_view.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/menu.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from enum import Enum
 from typing import List, Union
 
 from qframelesswindow import WindowEffect
 from PyQt5.QtCore import (QEasingCurve, QEvent, QPropertyAnimation, QObject, QModelIndex,
                           Qt, QSize, QRectF, pyqtSignal, QPoint, QTimer, QParallelAnimationGroup)
 from PyQt5.QtGui import (QIcon, QColor, QPainter, QPen, QPixmap, QRegion, QCursor, QTextCursor, QHoverEvent,
-                         QFontMetrics)
+                         QFontMetrics, QKeySequence)
 from PyQt5.QtWidgets import (QAction, QApplication, QMenu, QProxyStyle, QStyle,
                              QGraphicsDropShadowEffect, QListWidget, QWidget, QHBoxLayout,
                              QListWidgetItem, QLineEdit, QTextEdit, QStyledItemDelegate, QStyleOptionViewItem)
 
 from ...common.icon import FluentIcon as FIF
 from ...common.icon import FluentIconEngine, Action, FluentIconBase, Icon
 from ...common.style_sheet import FluentStyleSheet, themeColor
@@ -145,15 +145,15 @@
             painter.setOpacity(0.5 if isDarkTheme() else 0.6)
 
         font = getFont(12)
         painter.setFont(font)
         painter.setPen(QColor(255, 255, 255, 200) if isDarkTheme() else QColor(0, 0, 0, 153))
 
         fm = QFontMetrics(font)
-        shortcut = action.shortcut().toString()
+        shortcut = action.shortcut().toString(QKeySequence.NativeText)
 
         sw = fm.width(shortcut)
         painter.translate(option.rect.width()-sw-20, 0)
 
         rect = QRectF(0, option.rect.y(), sw, option.rect.height())
         painter.drawText(rect, Qt.AlignLeft | Qt.AlignVCenter, shortcut)
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/progress_bar.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/progress_ring.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/scroll_bar.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/slider.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/spin_box.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/switch_button.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/table_view.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/teaching_tip.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/tree_view.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/window/fluent_window.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/window/fluent_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     def _onCurrentInterfaceChanged(self, index: int):
         widget = self.stackedWidget.widget(index)
         self.navigationInterface.setCurrentItem(widget.objectName())
         qrouter.push(self.stackedWidget, widget.objectName())
 
     def paintEvent(self, e):
+        super().paintEvent(e)
         painter = QPainter(self)
         painter.setPen(Qt.NoPen)
 
         if isDarkTheme():
             painter.setBrush(QColor(32, 32, 32))
         else:
             painter.setBrush(QColor(243, 243, 243))
```

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/window/splash_screen.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/qfluentwidgets/window/stacked_widget.py` & `PyQt-Fluent-Widgets-1.0.1/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.0.0/setup.py` & `PyQt-Fluent-Widgets-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt-Fluent-Widgets",
-    version="1.0.0",
+    version="1.0.1",
     keywords="pyqt fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt5",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

