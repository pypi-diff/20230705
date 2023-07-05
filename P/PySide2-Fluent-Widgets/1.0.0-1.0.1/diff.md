# Comparing `tmp/PySide2-Fluent-Widgets-1.0.0.tar.gz` & `tmp/PySide2-Fluent-Widgets-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Fluent-Widgets-1.0.0.tar", last modified: Sun Jul  2 14:51:34 2023, max compression
+gzip compressed data, was "dist\PySide2-Fluent-Widgets-1.0.1.tar", last modified: Wed Jul  5 04:30:20 2023, max compression
```

## Comparing `PySide2-Fluent-Widgets-1.0.0.tar` & `PySide2-Fluent-Widgets-1.0.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.999588 PySide2-Fluent-Widgets-1.0.0/
--rw-rw-rw-   0        0        0    35821 2023-07-02 14:44:23.000000 PySide2-Fluent-Widgets-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4191 2023-07-02 14:51:33.997010 PySide2-Fluent-Widgets-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.842061 PySide2-Fluent-Widgets-1.0.0/PySide2_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4191 2023-07-02 14:51:33.000000 PySide2-Fluent-Widgets-1.0.0/PySide2_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4033 2023-07-02 14:51:33.000000 PySide2-Fluent-Widgets-1.0.0/PySide2_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 14:51:33.000000 PySide2-Fluent-Widgets-1.0.0/PySide2_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-07-02 14:51:33.000000 PySide2-Fluent-Widgets-1.0.0/PySide2_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-02 14:51:33.000000 PySide2-Fluent-Widgets-1.0.0/PySide2_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3381 2023-07-02 14:41:11.000000 PySide2-Fluent-Widgets-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.844111 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/
--rw-rw-rw-   0        0        0      524 2023-07-02 14:41:31.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.847112 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  6258165 2023-07-02 14:46:03.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.881643 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10643 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      807 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    12175 2023-07-02 14:41:31.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4785 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0     4865 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7217 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      454 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.883161 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.894320 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2082 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21150 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7449 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19071 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5781 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.903958 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14725 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5269 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11331 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3205 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2492 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.911735 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5437 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1305 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.923412 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      535 2023-06-26 15:48:09.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0    10711 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8080 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    19779 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    14589 2023-07-02 14:41:31.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6200 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     1390 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.936451 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5314 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8029 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6028 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2838 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13113 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1590 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.988834 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     2692 2023-07-02 14:45:20.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4596 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    21469 2023-07-02 14:45:23.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     3062 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     1615 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    13720 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19389 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     7879 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    15885 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2049 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1327 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    17210 2023-07-02 14:45:36.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    18932 2023-07-02 14:41:31.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0     6855 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    10006 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3854 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    36001 2023-07-02 14:41:31.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     7494 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6317 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2520 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17730 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     5151 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4357 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6335 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5795 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8985 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     8738 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    22255 2023-07-02 14:41:31.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10402 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2737 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2023-07-02 14:51:33.995980 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      115 2023-07-02 14:41:31.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    10176 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2854 2023-07-02 14:46:27.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1586 2023-07-02 14:41:12.000000 PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2023-07-02 14:51:33.999588 PySide2-Fluent-Widgets-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-07-02 14:44:28.000000 PySide2-Fluent-Widgets-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.386770 PySide2-Fluent-Widgets-1.0.1/
+-rw-rw-rw-   0        0        0    35821 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4387 2023-07-05 04:30:20.385768 PySide2-Fluent-Widgets-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.206452 PySide2-Fluent-Widgets-1.0.1/PySide2_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4387 2023-07-05 04:30:19.000000 PySide2-Fluent-Widgets-1.0.1/PySide2_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4033 2023-07-05 04:30:20.000000 PySide2-Fluent-Widgets-1.0.1/PySide2_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 04:30:19.000000 PySide2-Fluent-Widgets-1.0.1/PySide2_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-07-05 04:30:19.000000 PySide2-Fluent-Widgets-1.0.1/PySide2_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-05 04:30:19.000000 PySide2-Fluent-Widgets-1.0.1/PySide2_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3577 2023-07-05 04:27:58.000000 PySide2-Fluent-Widgets-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.207867 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/
+-rw-rw-rw-   0        0        0      524 2023-07-05 04:27:58.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.212148 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  6258165 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.254215 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3657 2023-06-26 15:48:09.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10643 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      807 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    12175 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4785 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4865 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7217 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      454 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.256752 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.267953 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2082 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21150 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7449 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19071 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5781 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.280524 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14725 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5269 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11331 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3205 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2492 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.289185 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5437 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1305 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.301316 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      535 2023-06-26 15:48:09.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0    10711 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8080 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    19779 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    14620 2023-07-05 04:27:58.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6200 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     1390 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.313843 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5314 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8029 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6028 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2838 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13113 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1590 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.376247 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     2692 2023-07-05 04:18:35.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4596 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    21469 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     3062 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     1615 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    13720 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19346 2023-07-05 04:27:58.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     7879 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    15885 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2049 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1327 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    17210 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    18932 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0     6855 2023-07-05 04:27:46.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    10006 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3854 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    36038 2023-07-05 04:28:09.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     7494 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6317 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2520 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17730 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     5151 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4357 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6335 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5795 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8985 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     8738 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    22255 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10402 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2737 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2023-07-05 04:30:20.383753 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      115 2023-07-02 14:53:20.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    10207 2023-07-05 04:27:58.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2854 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1586 2023-07-05 04:27:47.000000 PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 04:30:20.387775 PySide2-Fluent-Widgets-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-07-05 04:28:04.000000 PySide2-Fluent-Widgets-1.0.1/setup.py
```

### Comparing `PySide2-Fluent-Widgets-1.0.0/LICENSE` & `PySide2-Fluent-Widgets-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/PKG-INFO` & `PySide2-Fluent-Widgets-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Fluent-Widgets
-Version: 1.0.0
+Version: 1.0.1
 Summary: A fluent design widgets library based on PySide2
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
@@ -24,25 +24,29 @@
   PySide2-Fluent-Widgets
 </h1>
 <p align="center">
   A fluent design widgets library based on PySide2
 </p>
 
 <p align="center">
-  <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  <a href="https://pypi.org/project/PyQt-Fluent-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyqt-fluent-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
     <img src="https://static.pepy.tech/personalized-badge/pyside2-fluent-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
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
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 1.0.1 Summary: A
 fluent design widgets library based on PySide2 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2 Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2 Project-URL: Bug Tracker,
 https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyside2 fluent
 widgets Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Description-Content-Type: text/markdown Provides-
 Extra: full License-File: LICENSE
                                     [logo]
                      ****** PySide2-Fluent-Widgets ******
                A fluent design widgets library based on PySide2
-              [Platform Win32 | Linux | macOS] [Download] [GPLv3]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/
 master/docs/source/_static/Interface.jpg) ## Install To install lite version
 (`AcrylicLabel` is not available): ```shell pip install PySide2-Fluent-Widgets
 -i https://pypi.org/simple/ ``` Or install full-featured version: ```shell pip
 install "PySide2-Fluent-Widgets[full]" -i https://pypi.org/simple/ ``` ## Run
 Example After installing PySide2-Fluent-Widgets package using pip, you can run
```

### Comparing `PySide2-Fluent-Widgets-1.0.0/PySide2_Fluent_Widgets.egg-info/PKG-INFO` & `PySide2-Fluent-Widgets-1.0.1/PySide2_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Fluent-Widgets
-Version: 1.0.0
+Version: 1.0.1
 Summary: A fluent design widgets library based on PySide2
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
@@ -24,25 +24,29 @@
   PySide2-Fluent-Widgets
 </h1>
 <p align="center">
   A fluent design widgets library based on PySide2
 </p>
 
 <p align="center">
-  <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  <a href="https://pypi.org/project/PyQt-Fluent-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyqt-fluent-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
     <img src="https://static.pepy.tech/personalized-badge/pyside2-fluent-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
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
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 1.0.1 Summary: A
 fluent design widgets library based on PySide2 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2 Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2 Project-URL: Bug Tracker,
 https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyside2 fluent
 widgets Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Description-Content-Type: text/markdown Provides-
 Extra: full License-File: LICENSE
                                     [logo]
                      ****** PySide2-Fluent-Widgets ******
                A fluent design widgets library based on PySide2
-              [Platform Win32 | Linux | macOS] [Download] [GPLv3]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/
 master/docs/source/_static/Interface.jpg) ## Install To install lite version
 (`AcrylicLabel` is not available): ```shell pip install PySide2-Fluent-Widgets
 -i https://pypi.org/simple/ ``` Or install full-featured version: ```shell pip
 install "PySide2-Fluent-Widgets[full]" -i https://pypi.org/simple/ ``` ## Run
 Example After installing PySide2-Fluent-Widgets package using pip, you can run
```

### Comparing `PySide2-Fluent-Widgets-1.0.0/PySide2_Fluent_Widgets.egg-info/SOURCES.txt` & `PySide2-Fluent-Widgets-1.0.1/PySide2_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/README.md` & `PySide2-Fluent-Widgets-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,25 +5,29 @@
   PySide2-Fluent-Widgets
 </h1>
 <p align="center">
   A fluent design widgets library based on PySide2
 </p>
 
 <p align="center">
-  <a style="text-decoration:none">
-    <img src="https://img.shields.io/badge/Platform-Win32%20|%20Linux%20|%20macOS-blue?color=#4ec820" alt="Platform Win32 | Linux | macOS"/>
+  <a href="https://pypi.org/project/PyQt-Fluent-Widgets" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pyqt-fluent-widgets?color=%2334D058&label=Version" alt="Version">
   </a>
 
   <a style="text-decoration:none">
     <img src="https://static.pepy.tech/personalized-badge/pyside2-fluent-widgets?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Download"/>
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
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                                     [logo]
                      ****** PySide2-Fluent-Widgets ******
                A fluent design widgets library based on PySide2
-              [Platform Win32 | Linux | macOS] [Download] [GPLv3]
+         [Version] [Download] [GPLv3] [Platform Win32 | Linux | macOS]
                             English | ç®ä½ä¸­æ
 ![Interface](https://raw.githubusercontent.com/zhiyiYo/PyQt-Fluent-Widgets/
 master/docs/source/_static/Interface.jpg) ## Install To install lite version
 (`AcrylicLabel` is not available): ```shell pip install PySide2-Fluent-Widgets
 -i https://pypi.org/simple/ ``` Or install full-featured version: ```shell pip
 install "PySide2-Fluent-Widgets[full]" -i https://pypi.org/simple/ ``` ## Run
 Example After installing PySide2-Fluent-Widgets package using pip, you can run
```

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/__init__.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2/examples.
 
 :copyright: (c) 2023 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from .components import *
 from .common import *
 from .window import *
 from ._rc import resource
```

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/_rc/resource.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/__init__.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/animation.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/auto_wrap.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/config.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/exception_handler.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/font.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/icon.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/image_utils.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/overload.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/router.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/smooth_scroll.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/common/style_sheet.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/calendar_picker.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/calendar_view.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/date_picker.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/picker_base.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/date_time/time_picker.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/color_dialog.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/dialog.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/dialog_box/message_dialog.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/expand_layout.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/flow_layout.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/layout/v_box_layout.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/__init__.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_bar.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_interface.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_panel.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/navigation_widget.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/navigation_widget.py`

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

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/pivot.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/navigation/segmented_widget.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/__init__.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/expand_setting_card.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/options_setting_card.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/setting_card.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/settings/setting_card_group.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/__init__.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/acrylic_label.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/button.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/card_widget.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/check_box.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/combo_box.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/command_bar.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/command_bar.py`

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

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/flyout.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/frameless_window.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/icon_widget.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/info_badge.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/info_badge.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/info_bar.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/label.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/line_edit.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/list_view.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/menu.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from enum import Enum
 from typing import List, Union
 
 from qframelesswindow import WindowEffect
 from PySide2.QtCore import (QEasingCurve, QEvent, QPropertyAnimation, QObject, QModelIndex,
                           Qt, QSize, QRectF, Signal, QPoint, QTimer, QParallelAnimationGroup)
 from PySide2.QtGui import (QIcon, QColor, QPainter, QPen, QPixmap, QRegion, QCursor, QGuiApplication, QTextCursor, QHoverEvent,
-                         QFontMetrics)
+                         QFontMetrics, QKeySequence)
 from PySide2.QtWidgets import (QApplication, QAction, QMenu, QProxyStyle, QStyle,
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

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/progress_bar.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/progress_ring.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/scroll_area.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/scroll_bar.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/slider.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/spin_box.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/stacked_widget.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/state_tool_tip.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/switch_button.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/table_view.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/teaching_tip.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/tool_tip.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/components/widgets/tree_view.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/window/fluent_window.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/window/fluent_window.py`

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

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/window/splash_screen.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/qfluentwidgets/window/stacked_widget.py` & `PySide2-Fluent-Widgets-1.0.1/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.0.0/setup.py` & `PySide2-Fluent-Widgets-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Fluent-Widgets",
-    version="1.0.0",
+    version="1.0.1",
     keywords="pyside2 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PySide2",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

