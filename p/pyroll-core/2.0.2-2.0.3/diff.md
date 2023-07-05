# Comparing `tmp/pyroll_core-2.0.2.tar.gz` & `tmp/pyroll_core-2.0.3.tar.gz`

## Comparing `pyroll_core-2.0.2.tar` & `pyroll_core-2.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/__init__.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/config.py
--rw-r--r--   0        0        0    14207 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/hooks.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/log.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/repr.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/shapes.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/disk_elements/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/disk_elements/disk_element_unit.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/disk_elements/hookimpls.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/__init__.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/base.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/flat.py
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/generic_elongation.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/generic_elongation_solvers.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/hexagonal.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/spline.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/boxes/__init__.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/boxes/box.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/boxes/constricted_box.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/boxes/upset_box.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/diamonds/__init__.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/diamonds/diamond.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/diamonds/gothic.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/diamonds/square.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/__init__.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/circular_oval.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/constricted_circular_oval.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/constricted_swedish_oval.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/flat_oval.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/oval_3radii.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/oval_3radii_flanked.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/swedish_oval.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/upset_oval.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/rounds/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/rounds/false_round.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/rounds/round.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/profile/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/profile/hookimpls.py
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/profile/profile.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll/__init__.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll/hookimpls.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll/roll.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/deformation_unit.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/roll_pass.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/three_roll_pass.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/__init__.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/deformation_unit.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/disk_element.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/helpers.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/profile.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/roll.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/roll_pass.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/rotator/__init__.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/rotator/hookimpls.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/rotator/rotator.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/sequence/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/sequence/hookimpls.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/sequence/sequence.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/transport/__init__.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/transport/hookimpls.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/transport/transport.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/unit/__init__.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/unit/hookimpls.py
--rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/unit/unit.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/.gitignore
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/LICENSE
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/README.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/hatch.toml
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/__init__.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/config.py
+-rw-r--r--   0        0        0    14207 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/hooks.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/log.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/repr.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/shapes.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/disk_elements/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/disk_elements/disk_element_unit.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/disk_elements/hookimpls.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/__init__.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/base.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/flat.py
+-rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/generic_elongation.py
+-rw-r--r--   0        0        0    13557 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/generic_elongation_solvers.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/hexagonal.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/spline.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/boxes/__init__.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/boxes/box.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/boxes/constricted_box.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/boxes/upset_box.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/diamonds/__init__.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/diamonds/diamond.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/diamonds/gothic.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/diamonds/square.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/__init__.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/circular_oval.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/constricted_circular_oval.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/constricted_swedish_oval.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/flat_oval.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/oval_3radii.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/oval_3radii_flanked.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/swedish_oval.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/ovals/upset_oval.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/rounds/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/rounds/false_round.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/grooves/rounds/round.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/profile/__init__.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/profile/hookimpls.py
+-rw-r--r--   0        0        0    13443 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/profile/profile.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll/__init__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll/hookimpls.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll/roll.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/deformation_unit.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/roll_pass.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/three_roll_pass.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/__init__.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/deformation_unit.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/disk_element.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/helpers.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/profile.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/roll.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/roll_pass.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/rotator/__init__.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/rotator/hookimpls.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/rotator/rotator.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/sequence/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/sequence/hookimpls.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/sequence/sequence.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/transport/__init__.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/transport/hookimpls.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/transport/transport.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/unit/__init__.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/unit/hookimpls.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyroll/core/unit/unit.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/LICENSE
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/README.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/hatch.toml
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 pyroll_core-2.0.3/PKG-INFO
```

### Comparing `pyroll_core-2.0.2/pyroll/core/__init__.py` & `pyroll_core-2.0.3/pyroll/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .profile import Profile
 from .rotator import Rotator
 from .sequence import PassSequence
 from .hooks import Hook, HookHost, HookFunction, root_hooks
 from .disk_elements import DiskElementUnit
 from .config import Config, config
 
-VERSION = "2.0.2"
+VERSION = "2.0.3"
 
 root_hooks.update(
     {
         RollPass.roll_force,
         RollPass.Roll.roll_torque,
         Unit.OutProfile.cross_section,
         Unit.OutProfile.strain,
```

### Comparing `pyroll_core-2.0.2/pyroll/core/config.py` & `pyroll_core-2.0.3/pyroll/core/config.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/hooks.py` & `pyroll_core-2.0.3/pyroll/core/hooks.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/repr.py` & `pyroll_core-2.0.3/pyroll/core/repr.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/shapes.py` & `pyroll_core-2.0.3/pyroll/core/shapes.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/disk_elements/disk_element_unit.py` & `pyroll_core-2.0.3/pyroll/core/disk_elements/disk_element_unit.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/disk_elements/hookimpls.py` & `pyroll_core-2.0.3/pyroll/core/disk_elements/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/__init__.py` & `pyroll_core-2.0.3/pyroll/core/grooves/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/base.py` & `pyroll_core-2.0.3/pyroll/core/grooves/base.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/flat.py` & `pyroll_core-2.0.3/pyroll/core/grooves/flat.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/generic_elongation.py` & `pyroll_core-2.0.3/pyroll/core/grooves/generic_elongation.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,23 @@
             (commonly 0 for two-roll, π/6 for three-roll and π/4 for four-roll)
 
         :param classifiers: sequence of additional type classifiers
         """
 
         try:
             if usable_width is None:
-                usable_width = ground_width + 2 * depth / np.tan(flank_angle)
+                if np.isclose(depth, 0):
+                    usable_width = ground_width
+                else:
+                    usable_width = ground_width + 2 * depth / np.tan(flank_angle)
             elif ground_width is None:
-                ground_width = usable_width - 2 * depth / np.tan(flank_angle)
+                if np.isclose(depth, 0):
+                    ground_width = usable_width
+                else:
+                    ground_width = usable_width - 2 * depth / np.tan(flank_angle)
             elif flank_angle is None:
                 flank_angle = np.arctan(depth / (usable_width - ground_width) * 2)
             elif depth is None:
                 depth = (usable_width - ground_width) / 2 * np.tan(flank_angle)
             else:
                 raise TypeError("Too many arguments given.")
```

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/generic_elongation_solvers.py` & `pyroll_core-2.0.3/pyroll/core/grooves/generic_elongation_solvers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from typing import Optional
 
 import numpy as np
 from scipy.optimize import root_scalar, root, fixed_point
 
 
+# angle brackets for numerical solvers to prevent divide by zero
+MIN_ANGLE = 1e-6
+MAX_ANGLE = np.pi / 2 - MIN_ANGLE
+
+
 def solve_r124(
         r1: float,
 
         r2: Optional[float],
         depth: Optional[float],
         width: Optional[float],
 
@@ -53,26 +58,26 @@
             def fh(_alpha):
                 return 0
 
         if width is None:
             def f(_alpha):
                 return depth - r2 * (1 - np.cos(_alpha)) - l23(_alpha) * np.sin(_alpha) - fh(_alpha)
 
-            flank_angle = root_scalar(f, bracket=(0, np.pi / 2)).root
+            flank_angle = root_scalar(f, bracket=(MIN_ANGLE, MAX_ANGLE)).root
 
         elif depth is None:
             alpha4 = np.arccos(1 - indent / (r2 + r4))
 
             def f(_alpha):
                 return (
                         width / 2 - r2 * np.sin(_alpha) - l23(_alpha) * np.cos(_alpha)
                         - fw(_alpha) - (r2 + r4) * np.sin(alpha4)
                 )
 
-            raster = np.linspace(0, np.pi / 2, 100)
+            raster = np.linspace(MIN_ANGLE, MAX_ANGLE, 100)
             values = f(raster)
             lower = raster[values > 0][0]
             upper = raster[values < 0][-1]
             flank_angle = root_scalar(f, bracket=(lower, upper)).root
 
         elif r2 is None:
             def f(_alpha):
@@ -80,15 +85,15 @@
                 _alpha4 = np.arccos(1 - indent / (_r2 + r4))
 
                 return (
                         width / 2 - _r2 * np.sin(_alpha) - l23(_alpha) * np.cos(_alpha)
                         - fw(_alpha) - (_r2 + r4) * np.sin(_alpha4)
                 )
 
-            flank_angle = root_scalar(f, bracket=(0, np.pi / 2)).root
+            flank_angle = root_scalar(f, bracket=(MIN_ANGLE, MAX_ANGLE)).root
 
         else:
             raise TypeError("Give either usable_width or depth.")
 
     if r2 is not None:
         alpha4 = np.arccos(1 - indent / (r2 + r4))
 
@@ -108,14 +113,15 @@
     else:
         def f(_r2):
             _alpha4 = np.arccos(1 - indent / (_r2 + r4))
             return (
                     (depth - width / 2 * np.tan(flank_angle) + r4 * np.sin(_alpha4))
                     / (1 - np.cos(flank_angle) - np.sin(flank_angle) * np.tan(flank_angle) - np.sin(_alpha4))
             )
+
         r2 = fixed_point(f, width if width > depth else depth)
         alpha4 = np.arccos(1 - indent / (r2 + r4))
 
     return dict(
         width=width,
         depth=depth,
         r2=r2,
@@ -210,15 +216,15 @@
             _fw = width / 2 - r32 * np.sin(_alpha3) - r2 * np.cos(_gamma) - l23(flank_angle) * np.cos(flank_angle)
 
             return (
                     depth - r3 + r32 * np.cos(_alpha3) + r2 * np.sin(_gamma)
                     - _fw * np.tan(flank_angle) - l23(flank_angle) * np.sin(flank_angle)
             )
 
-        sol = root_scalar(f, bracket=(0, np.pi / 2)).root
+        sol = root_scalar(f, bracket=(MIN_ANGLE, MAX_ANGLE)).root
         alpha2 = sol
         alpha3 = flank_angle - sol
 
     return dict(
         flank_angle=flank_angle,
         alpha2=alpha2,
         alpha3=alpha3,
@@ -387,15 +393,15 @@
             if ground_width is not None:
                 flank_angle = np.arctan(depth / (usable_width - ground_width) * 2)
             elif even_ground_width is not None:
                 def f(_alpha):
                     _ground_width = even_ground_width + 2 * ((r4 + r2) * np.sin(alpha4) + r2 * np.tan(_alpha / 2))
                     return depth - (usable_width - _ground_width) / 2 * np.tan(_alpha)
 
-                flank_angle = root_scalar(f, bracket=(0, np.pi / 2)).root
+                flank_angle = root_scalar(f, bracket=(MIN_ANGLE, MAX_ANGLE)).root
                 ground_width = even_ground_width + 2 * ((r4 + r2) * np.sin(alpha4) + r2 * np.tan(flank_angle / 2))
             else:
                 raise TypeError("either ground_width or even_ground_width must not be None")
         else:
             raise TypeError("usable_width must not be None if flank_angle is None")
     elif ground_width is None and even_ground_width is None:
         if usable_width is not None:
```

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/hexagonal.py` & `pyroll_core-2.0.3/pyroll/core/grooves/hexagonal.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/spline.py` & `pyroll_core-2.0.3/pyroll/core/grooves/spline.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/boxes/box.py` & `pyroll_core-2.0.3/pyroll/core/grooves/boxes/box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/boxes/constricted_box.py` & `pyroll_core-2.0.3/pyroll/core/grooves/boxes/constricted_box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/boxes/upset_box.py` & `pyroll_core-2.0.3/pyroll/core/grooves/boxes/upset_box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/diamonds/diamond.py` & `pyroll_core-2.0.3/pyroll/core/grooves/diamonds/diamond.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/diamonds/gothic.py` & `pyroll_core-2.0.3/pyroll/core/grooves/diamonds/gothic.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/diamonds/square.py` & `pyroll_core-2.0.3/pyroll/core/grooves/diamonds/square.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/ovals/circular_oval.py` & `pyroll_core-2.0.3/pyroll/core/grooves/ovals/circular_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/ovals/constricted_circular_oval.py` & `pyroll_core-2.0.3/pyroll/core/grooves/ovals/constricted_circular_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/ovals/constricted_swedish_oval.py` & `pyroll_core-2.0.3/pyroll/core/grooves/ovals/constricted_swedish_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/ovals/flat_oval.py` & `pyroll_core-2.0.3/pyroll/core/grooves/ovals/flat_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/ovals/oval_3radii.py` & `pyroll_core-2.0.3/pyroll/core/grooves/ovals/oval_3radii.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/ovals/oval_3radii_flanked.py` & `pyroll_core-2.0.3/pyroll/core/grooves/ovals/oval_3radii_flanked.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/ovals/swedish_oval.py` & `pyroll_core-2.0.3/pyroll/core/grooves/ovals/swedish_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/ovals/upset_oval.py` & `pyroll_core-2.0.3/pyroll/core/grooves/ovals/upset_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/rounds/false_round.py` & `pyroll_core-2.0.3/pyroll/core/grooves/rounds/false_round.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/grooves/rounds/round.py` & `pyroll_core-2.0.3/pyroll/core/grooves/rounds/round.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/profile/profile.py` & `pyroll_core-2.0.3/pyroll/core/profile/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,21 +82,30 @@
     material = Hook[Union[str, Iterable[str]]]()
     """String or sequence of strings classifying the material of the profile.
     Can be used by material databases to retrieve respective data."""
 
     grain_size = Hook[float]()
     """Average grain size of the profile's material."""
 
+    heat_penetration_number = Hook[float]()
+    """Mean heat penetration number of the profile material."""
+
+    thermal_diffusivity = Hook[float]()
+    """Mean thermal diffusivity of the profile material."""
+
     chemical_composition = Hook[dict[str, float]]()
     """Chemical composition of the profile's material as dict of element symbols to atom fractions (0 to 1)."""
 
     microstructure_composition = Hook[dict[str, float]]()
     """Phase resp. constituent composition of the profile's material 
     as dict of constituent names to volume fractions (0 to 1)."""
 
+    scale_thickness = Hook[float]()
+    """Thickness of the scale covering the profile."""
+
     def __init__(self, **kwargs):
         """Using the ``__init__`` is not recommended, use one of the factory class methods instead."""
         self.__dict__.update(kwargs)
         super().__init__()
 
     @classmethod
     def _base_factory(cls, **kwargs):
```

### Comparing `pyroll_core-2.0.2/pyroll/core/roll/hookimpls.py` & `pyroll_core-2.0.3/pyroll/core/roll/hookimpls.py`

 * *Files 17% similar despite different names*

```diff
@@ -59,7 +59,19 @@
     return self.contour_points[:, 0]
 
 
 @Roll.surface_y
 def surface_y(self: Roll):
     local_radii = self.max_radius - self.contour_points[:, 1]
     return self.max_radius - np.sqrt(local_radii.reshape(-1, 1) ** 2 - self.surface_x ** 2)
+
+
+@Roll.heat_penetration_number
+def heat_penetration_number(self: Roll):
+    if hasattr(self, "thermal_conductivity") and hasattr(self, "density") and hasattr(self, "thermal_capacity"):
+        return np.sqrt(self.thermal_conductivity * self.density * self.thermal_capacity)
+
+
+@Roll.thermal_diffusivity
+def thermal_diffusivity(self: Roll):
+    if hasattr(self, "thermal_conductivity") and hasattr(self, "density") and hasattr(self, "thermal_capacity"):
+        return self.thermal_conductivity / (self.density * self.thermal_capacity)
```

### Comparing `pyroll_core-2.0.2/pyroll/core/roll/roll.py` & `pyroll_core-2.0.3/pyroll/core/roll/roll.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 
     center = Hook[np.ndarray]()
     """Center point of the roll as 1D array."""
 
     temperature = Hook[float]()
     """Mean temperature."""
 
+    core_temperature = Hook[float]()
+    """Effective core temperature."""
+
     surface_temperature = Hook[float]()
     """Effective surface temperature."""
 
     yield_strength = Hook[float]()
     """Yield strength of the roll material."""
 
     elastic_modulus = Hook[float]()
@@ -86,17 +89,35 @@
 
     surface_y = Hook[np.ndarray]()
     """
     Y-Values of the surface interpolation grid. Array of shape (n, m), 
     where ``n = len(self.surface_x)`` and ``m = len(self.surface_z)``.
     """
 
+    heat_penetration_number = Hook[float]()
+    """Mean heat penetration number of the roll material."""
+
+    thermal_diffusivity = Hook[float]()
+    """Mean thermal diffusivity of the roll material."""
+
     neutral_point = Hook[float]()
     """Point at the roll surface where the shear stress is zero."""
 
+    thermal_stress = Hook[float]()
+    """Thermal stress inside the roll body."""
+
+    centrifugal_force_stress = Hook[float]()
+    """Centrifugal stress inside the roll body."""
+
+    mounting_stress = Hook[float]()
+    """Stress inside the roll body caused by the roll mounting system."""
+
+    ultimate_tensile_strength = Hook[float]()
+    """Ultimate Tensile strength of the roll material."""
+
     def __init__(
             self,
             groove: GrooveBase,
             **kwargs
     ):
         """
         :param groove: the groove object defining the shape of the roll's surface
```

### Comparing `pyroll_core-2.0.2/pyroll/core/roll_pass/deformation_unit.py` & `pyroll_core-2.0.3/pyroll/core/roll_pass/deformation_unit.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/roll_pass/roll_pass.py` & `pyroll_core-2.0.3/pyroll/core/roll_pass/roll_pass.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/roll_pass/three_roll_pass.py` & `pyroll_core-2.0.3/pyroll/core/roll_pass/three_roll_pass.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/deformation_unit.py` & `pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/deformation_unit.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/helpers.py` & `pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/helpers.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/profile.py` & `pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/profile.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/roll.py` & `pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/roll.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/roll_pass.py` & `pyroll_core-2.0.3/pyroll/core/roll_pass/hookimpls/roll_pass.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,18 @@
             return True
 
         while True:
             if isinstance(prev, RollPass):
                 return True
             if isinstance(prev, Rotator):
                 return False
-            prev = prev.prev
+            try:
+                prev = prev.prev
+            except IndexError:
+                return True
 
 
 @RollPass.roll_force
 def roll_force(self: RollPass):
     return (self.in_profile.flow_stress + 2 * self.out_profile.flow_stress) / 3 * self.roll.contact_area
 
 
@@ -94,15 +97,22 @@
 def height(self):
     if self.has_set_or_cached("gap"):
         return self.gap + 2 * self.roll.groove.depth
 
 
 @ThreeRollPass.height
 def height3(self):
-    return -2 * self.contour_lines[1].bounds[1]
+    usable_contour = clip_by_rect(
+        self.contour_lines[1],
+        -self.roll.groove.usable_width / 2,
+        -math.inf,
+        self.roll.groove.usable_width / 2,
+        math.inf
+    )
+    return -2 * usable_contour.bounds[1]
 
 
 @RollPass.volume
 def volume(self: RollPass):
     return (self.in_profile.cross_section.area + 2 * self.out_profile.cross_section.area
             ) / 3 * self.length
```

### Comparing `pyroll_core-2.0.2/pyroll/core/rotator/hookimpls.py` & `pyroll_core-2.0.3/pyroll/core/rotator/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/rotator/rotator.py` & `pyroll_core-2.0.3/pyroll/core/rotator/rotator.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/sequence/sequence.py` & `pyroll_core-2.0.3/pyroll/core/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/transport/transport.py` & `pyroll_core-2.0.3/pyroll/core/transport/transport.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/unit/hookimpls.py` & `pyroll_core-2.0.3/pyroll/core/unit/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyroll/core/unit/unit.py` & `pyroll_core-2.0.3/pyroll/core/unit/unit.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/.gitignore` & `pyroll_core-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/LICENSE` & `pyroll_core-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/README.md` & `pyroll_core-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.2/pyproject.toml` & `pyroll_core-2.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -41,7 +41,15 @@
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://pyroll-project.github.io"
 Repository = "https://github.com/pyroll-project/pyroll-core"
 Documentation = "https://pyroll.readthedocs.io/en/latest"
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+    'ignore:Matplotlib is currently using:UserWarning',
+    'ignore:More than 20 figures have been opened:RuntimeWarning',
+]
+
```

### Comparing `pyroll_core-2.0.2/PKG-INFO` & `pyroll_core-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroll-core
-Version: 2.0.2
+Version: 2.0.3
 Summary: PyRoll rolling simulation framework - core library.
 Project-URL: Homepage, https://pyroll-project.github.io
 Project-URL: Repository, https://github.com/pyroll-project/pyroll-core
 Project-URL: Documentation, https://pyroll.readthedocs.io/en/latest
 Author-email: Max Weiner <max.weiner@imf.tu-freiberg.de>, Christoph Renzing <christoph.renzing@imf.tu-freiberg.de>, Matthias Schmidtchen <matthias.schmidtchen@imf.tu-freiberg.de>, Max Stirl <max.stirl@imf.tu-freiberg.de>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

