# Comparing `tmp/pykiso-0.22.2.tar.gz` & `tmp/pykiso-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykiso-0.22.2.tar", max compression
+gzip compressed data, was "pykiso-0.23.0.tar", max compression
```

## Comparing `pykiso-0.22.2.tar` & `pykiso-0.23.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0    14194 2023-06-21 06:36:48.823367 pykiso-0.22.2/LICENSE
--rw-r--r--   0        0        0     6028 2023-06-21 06:36:48.824367 pykiso-0.22.2/README.md
--rw-r--r--   0        0        0     4365 2023-06-21 06:36:49.015364 pykiso-0.22.2/pyproject.toml
--rw-r--r--   0        0        0     1972 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/__init__.py
--rw-r--r--   0        0        0      642 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/__main__.py
--rw-r--r--   0        0        0     9480 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/auxiliary.py
--rw-r--r--   0        0        0     7920 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/cli.py
--rw-r--r--   0        0        0    11837 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/config_parser.py
--rw-r--r--   0        0        0     5559 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/connector.py
--rw-r--r--   0        0        0     2436 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/exceptions.py
--rw-r--r--   0        0        0     4509 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/global_config.py
--rw-r--r--   0        0        0      410 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/interfaces/__init__.py
--rw-r--r--   0        0        0    13651 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/interfaces/dt_auxiliary.py
--rw-r--r--   0        0        0     8975 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/interfaces/mp_auxiliary.py
--rw-r--r--   0        0        0     4318 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/interfaces/simple_auxiliary.py
--rw-r--r--   0        0        0     8665 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/interfaces/thread_auxiliary.py
--rw-r--r--   0        0        0      516 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/__init__.py
--rw-r--r--   0        0        0      552 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/__init__.py
--rw-r--r--   0        0        0     8415 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/acroname_auxiliary.py
--rw-r--r--   0        0        0     7916 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/communication_auxiliary.py
--rw-r--r--   0        0        0    12655 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/dut_auxiliary.py
--rw-r--r--   0        0        0     2014 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py
--rw-r--r--   0        0        0    10145 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py
--rw-r--r--   0        0        0    19216 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py
--rw-r--r--   0        0        0     5029 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py
--rw-r--r--   0        0        0    16676 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py
--rw-r--r--   0        0        0    14219 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py
--rw-r--r--   0        0        0    14149 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/proxy_auxiliary.py
--rw-r--r--   0        0        0    17111 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/record_auxiliary.py
--rw-r--r--   0        0        0     2645 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py
--rw-r--r--   0        0        0     6511 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py
--rw-r--r--   0        0        0    14146 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py
--rw-r--r--   0        0        0     3889 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py
--rw-r--r--   0        0        0     4288 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py
--rw-r--r--   0        0        0      718 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/__init__.py
--rw-r--r--   0        0        0      599 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py
--rw-r--r--   0        0        0     3913 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py
--rw-r--r--   0        0        0     5299 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py
--rw-r--r--   0        0        0    12896 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py
--rw-r--r--   0        0        0     1517 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py
--rw-r--r--   0        0        0     1570 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py
--rw-r--r--   0        0        0     2664 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py
--rw-r--r--   0        0        0     1404 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py
--rw-r--r--   0        0        0    12764 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py
--rw-r--r--   0        0        0    17074 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py
--rw-r--r--   0        0        0    13528 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/ykush_auxiliary.py
--rw-r--r--   0        0        0      548 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/connectors/__init__.py
--rw-r--r--   0        0        0     3999 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_example.py
--rw-r--r--   0        0        0    13274 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_fdx_lauterbach.py
--rw-r--r--   0        0        0     1446 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_flasher_example.py
--rw-r--r--   0        0        0     4966 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_mp_proxy.py
--rw-r--r--   0        0        0    19995 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_pcan_can.py
--rw-r--r--   0        0        0    11002 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_process.py
--rw-r--r--   0        0        0     5697 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_proxy.py
--rw-r--r--   0        0        0     2048 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_raw_loopback.py
--rw-r--r--   0        0        0    14178 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_rtt_segger.py
--rw-r--r--   0        0        0     7584 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_serial.py
--rw-r--r--   0        0        0      538 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/__init__.py
--rw-r--r--   0        0        0     7361 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py
--rw-r--r--   0        0        0     8065 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py
--rw-r--r--   0        0        0     3215 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_tcp_ip.py
--rw-r--r--   0        0        0     5893 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_uart.py
--rw-r--r--   0        0        0     2981 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_udp.py
--rw-r--r--   0        0        0     3425 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_udp_server.py
--rw-r--r--   0        0        0     2440 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_usb.py
--rw-r--r--   0        0        0     7378 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_vector_can.py
--rw-r--r--   0        0        0     7194 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_visa.py
--rw-r--r--   0        0        0     4085 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/flash_jlink.py
--rw-r--r--   0        0        0     8380 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/flash_lauterbach.py
--rw-r--r--   0        0        0      530 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/robot_framework/__init__.py
--rw-r--r--   0        0        0     4193 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/acroname_auxiliary.py
--rw-r--r--   0        0        0     2380 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/aux_interface.py
--rw-r--r--   0        0        0     3361 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/communication_auxiliary.py
--rw-r--r--   0        0        0     3639 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/dut_auxiliary.py
--rw-r--r--   0        0        0    16126 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py
--rw-r--r--   0        0        0     3599 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/loader.py
--rw-r--r--   0        0        0     2321 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/proxy_auxiliary.py
--rw-r--r--   0        0        0     6606 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/lib/robot_framework/record_auxiliary.py
--rw-r--r--   0        0        0     6840 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/lib/robot_framework/uds_auxiliary.py
--rw-r--r--   0        0        0     7770 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/logging_initializer.py
--rw-r--r--   0        0        0    11744 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/message.py
--rw-r--r--   0        0        0      766 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/__init__.py
--rw-r--r--   0        0        0    12366 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/collection.py
--rw-r--r--   0        0        0     2436 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/commandline.py
--rw-r--r--   0        0        0     1449 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/hooks.py
--rw-r--r--   0        0        0     2376 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/logging.py
--rw-r--r--   0        0        0      988 2023-06-21 06:36:49.108363 pykiso-0.22.2/src/pykiso/pytest_plugin/markers.py
--rw-r--r--   0        0        0     1503 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/pytest_plugin/reporting.py
--rw-r--r--   0        0        0     1685 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/pytest_plugin/utils.py
--rw-r--r--   0        0        0      410 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/test_coordinator/__init__.py
--rw-r--r--   0        0        0    12735 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/test_coordinator/test_case.py
--rw-r--r--   0        0        0    16129 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/test_coordinator/test_execution.py
--rw-r--r--   0        0        0     5480 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/test_coordinator/test_message_handler.py
--rw-r--r--   0        0        0    16859 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_coordinator/test_suite.py
--rw-r--r--   0        0        0      515 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/__init__.py
--rw-r--r--   0        0        0    17429 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/assert_step_report.py
--rw-r--r--   0        0        0     8391 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/multi_result.py
--rw-r--r--   0        0        0     1971 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/templates/report_template.css
--rw-r--r--   0        0        0     6250 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/templates/report_template.html.j2
--rw-r--r--   0        0        0     3182 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_result/templates/report_template_script.js
--rw-r--r--   0        0        0     9917 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_result/text_result.py
--rw-r--r--   0        0        0     5663 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_result/xml_result.py
--rw-r--r--   0        0        0      410 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_setup/__init__.py
--rw-r--r--   0        0        0     9799 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_setup/config_registry.py
--rw-r--r--   0        0        0    14160 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_setup/dynamic_loader.py
--rw-r--r--   0        0        0      410 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/__init__.py
--rw-r--r--   0        0        0      410 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/__init__.py
--rw-r--r--   0        0        0     5577 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/cli.py
--rw-r--r--   0        0        0     3114 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2
--rw-r--r--   0        0        0    11816 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/show_tag.py
--rw-r--r--   0        0        0      410 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/testrail/__init__.py
--rw-r--r--   0        0        0    12414 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/testrail/api.py
--rw-r--r--   0        0        0     7728 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/testrail/cli.py
--rw-r--r--   0        0        0     5195 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/testrail/console.py
--rw-r--r--   0        0        0     8545 2023-06-21 06:36:49.113362 pykiso-0.22.2/src/pykiso/tool/testrail/containers.py
--rw-r--r--   0        0        0     5075 2023-06-21 06:36:49.113362 pykiso-0.22.2/src/pykiso/tool/testrail/extraction.py
--rw-r--r--   0        0        0    12851 2023-06-21 06:36:49.113362 pykiso-0.22.2/src/pykiso/tool/testrail/testrail.py
--rw-r--r--   0        0        0     1794 2023-06-21 06:36:49.113362 pykiso-0.22.2/src/pykiso/types.py
--rw-r--r--   0        0        0     9449 1970-01-01 00:00:00.000000 pykiso-0.22.2/setup.py
--rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 pykiso-0.22.2/PKG-INFO
+-rw-r--r--   0        0        0    14194 2023-07-05 09:55:02.789015 pykiso-0.23.0/LICENSE
+-rw-r--r--   0        0        0     6241 2023-07-05 09:55:02.789015 pykiso-0.23.0/README.md
+-rw-r--r--   0        0        0     4451 2023-07-05 09:55:02.986011 pykiso-0.23.0/pyproject.toml
+-rw-r--r--   0        0        0     1972 2023-07-05 09:55:02.986011 pykiso-0.23.0/src/pykiso/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-05 09:55:02.987011 pykiso-0.23.0/src/pykiso/__main__.py
+-rw-r--r--   0        0        0     9480 2023-07-05 09:55:02.987011 pykiso-0.23.0/src/pykiso/auxiliary.py
+-rw-r--r--   0        0        0     8232 2023-07-05 09:55:02.987011 pykiso-0.23.0/src/pykiso/cli.py
+-rw-r--r--   0        0        0    11993 2023-07-05 09:55:02.987011 pykiso-0.23.0/src/pykiso/config_parser.py
+-rw-r--r--   0        0        0     5686 2023-07-05 09:55:02.987011 pykiso-0.23.0/src/pykiso/connector.py
+-rw-r--r--   0        0        0     2436 2023-07-05 09:55:02.987011 pykiso-0.23.0/src/pykiso/exceptions.py
+-rw-r--r--   0        0        0     4509 2023-07-05 09:55:02.987011 pykiso-0.23.0/src/pykiso/global_config.py
+-rw-r--r--   0        0        0      410 2023-07-05 09:55:02.988011 pykiso-0.23.0/src/pykiso/interfaces/__init__.py
+-rw-r--r--   0        0        0    13958 2023-07-05 09:55:02.988011 pykiso-0.23.0/src/pykiso/interfaces/dt_auxiliary.py
+-rw-r--r--   0        0        0     8975 2023-07-05 09:55:02.988011 pykiso-0.23.0/src/pykiso/interfaces/mp_auxiliary.py
+-rw-r--r--   0        0        0     4318 2023-07-05 09:55:02.988011 pykiso-0.23.0/src/pykiso/interfaces/simple_auxiliary.py
+-rw-r--r--   0        0        0     8665 2023-07-05 09:55:02.988011 pykiso-0.23.0/src/pykiso/interfaces/thread_auxiliary.py
+-rw-r--r--   0        0        0      516 2023-07-05 09:55:02.989011 pykiso-0.23.0/src/pykiso/lib/__init__.py
+-rw-r--r--   0        0        0      552 2023-07-05 09:55:02.989011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/__init__.py
+-rw-r--r--   0        0        0     8415 2023-07-05 09:55:02.989011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/acroname_auxiliary.py
+-rw-r--r--   0        0        0     7916 2023-07-05 09:55:02.989011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/communication_auxiliary.py
+-rw-r--r--   0        0        0    12655 2023-07-05 09:55:02.989011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/dut_auxiliary.py
+-rw-r--r--   0        0        0     2014 2023-07-05 09:55:02.989011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py
+-rw-r--r--   0        0        0    10145 2023-07-05 09:55:02.989011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py
+-rw-r--r--   0        0        0    19216 2023-07-05 09:55:02.990011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py
+-rw-r--r--   0        0        0     5029 2023-07-05 09:55:02.990011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py
+-rw-r--r--   0        0        0    16676 2023-07-05 09:55:02.990011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py
+-rw-r--r--   0        0        0    14219 2023-07-05 09:55:02.990011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py
+-rw-r--r--   0        0        0    14819 2023-07-05 09:55:02.990011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/proxy_auxiliary.py
+-rw-r--r--   0        0        0    17134 2023-07-05 09:55:02.991011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/record_auxiliary.py
+-rw-r--r--   0        0        0     2645 2023-07-05 09:55:02.991011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py
+-rw-r--r--   0        0        0     6511 2023-07-05 09:55:02.991011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py
+-rw-r--r--   0        0        0    14146 2023-07-05 09:55:02.991011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py
+-rw-r--r--   0        0        0     3889 2023-07-05 09:55:02.991011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py
+-rw-r--r--   0        0        0     4288 2023-07-05 09:55:02.991011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py
+-rw-r--r--   0        0        0      718 2023-07-05 09:55:02.991011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-05 09:55:02.992011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py
+-rw-r--r--   0        0        0     3992 2023-07-05 09:55:02.992011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py
+-rw-r--r--   0        0        0     5299 2023-07-05 09:55:02.992011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py
+-rw-r--r--   0        0        0    12896 2023-07-05 09:55:02.992011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py
+-rw-r--r--   0        0        0     1517 2023-07-05 09:55:02.992011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py
+-rw-r--r--   0        0        0     1570 2023-07-05 09:55:02.992011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py
+-rw-r--r--   0        0        0     2664 2023-07-05 09:55:02.992011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py
+-rw-r--r--   0        0        0     1404 2023-07-05 09:55:02.992011 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py
+-rw-r--r--   0        0        0    12764 2023-07-05 09:55:03.080009 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py
+-rw-r--r--   0        0        0    17074 2023-07-05 09:55:03.081009 pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py
+-rw-r--r--   0        0        0    13528 2023-07-05 09:55:03.081009 pykiso-0.23.0/src/pykiso/lib/auxiliaries/ykush_auxiliary.py
+-rw-r--r--   0        0        0      548 2023-07-05 09:55:03.081009 pykiso-0.23.0/src/pykiso/lib/connectors/__init__.py
+-rw-r--r--   0        0        0     3999 2023-07-05 09:55:03.081009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_example.py
+-rw-r--r--   0        0        0    13274 2023-07-05 09:55:03.081009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_fdx_lauterbach.py
+-rw-r--r--   0        0        0     1446 2023-07-05 09:55:03.081009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_flasher_example.py
+-rw-r--r--   0        0        0     4966 2023-07-05 09:55:03.082009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_mp_proxy.py
+-rw-r--r--   0        0        0    20177 2023-07-05 09:55:03.082009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_pcan_can.py
+-rw-r--r--   0        0        0    11148 2023-07-05 09:55:03.082009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_process.py
+-rw-r--r--   0        0        0     5688 2023-07-05 09:55:03.082009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_proxy.py
+-rw-r--r--   0        0        0     2048 2023-07-05 09:55:03.082009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_raw_loopback.py
+-rw-r--r--   0        0        0    14178 2023-07-05 09:55:03.082009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_rtt_segger.py
+-rw-r--r--   0        0        0     8393 2023-07-05 09:55:03.082009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_serial.py
+-rw-r--r--   0        0        0      538 2023-07-05 09:55:03.083009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_socket_can/__init__.py
+-rw-r--r--   0        0        0     7361 2023-07-05 09:55:03.083009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py
+-rw-r--r--   0        0        0     8065 2023-07-05 09:55:03.083009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py
+-rw-r--r--   0        0        0     3215 2023-07-05 09:55:03.083009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_tcp_ip.py
+-rw-r--r--   0        0        0     5893 2023-07-05 09:55:03.083009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_uart.py
+-rw-r--r--   0        0        0     2981 2023-07-05 09:55:03.083009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_udp.py
+-rw-r--r--   0        0        0     3425 2023-07-05 09:55:03.083009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_udp_server.py
+-rw-r--r--   0        0        0     2440 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_usb.py
+-rw-r--r--   0        0        0     7378 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_vector_can.py
+-rw-r--r--   0        0        0     7194 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/connectors/cc_visa.py
+-rw-r--r--   0        0        0     4085 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/connectors/flash_jlink.py
+-rw-r--r--   0        0        0     8380 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/connectors/flash_lauterbach.py
+-rw-r--r--   0        0        0      530 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/robot_framework/__init__.py
+-rw-r--r--   0        0        0     4193 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/robot_framework/acroname_auxiliary.py
+-rw-r--r--   0        0        0     2380 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/robot_framework/aux_interface.py
+-rw-r--r--   0        0        0     3361 2023-07-05 09:55:03.084009 pykiso-0.23.0/src/pykiso/lib/robot_framework/communication_auxiliary.py
+-rw-r--r--   0        0        0     3639 2023-07-05 09:55:03.085009 pykiso-0.23.0/src/pykiso/lib/robot_framework/dut_auxiliary.py
+-rw-r--r--   0        0        0    16126 2023-07-05 09:55:03.085009 pykiso-0.23.0/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py
+-rw-r--r--   0        0        0     3599 2023-07-05 09:55:03.085009 pykiso-0.23.0/src/pykiso/lib/robot_framework/loader.py
+-rw-r--r--   0        0        0     2321 2023-07-05 09:55:03.085009 pykiso-0.23.0/src/pykiso/lib/robot_framework/proxy_auxiliary.py
+-rw-r--r--   0        0        0     6606 2023-07-05 09:55:03.085009 pykiso-0.23.0/src/pykiso/lib/robot_framework/record_auxiliary.py
+-rw-r--r--   0        0        0     6840 2023-07-05 09:55:03.085009 pykiso-0.23.0/src/pykiso/lib/robot_framework/uds_auxiliary.py
+-rw-r--r--   0        0        0    11244 2023-07-05 09:55:03.085009 pykiso-0.23.0/src/pykiso/logging_initializer.py
+-rw-r--r--   0        0        0    11744 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/message.py
+-rw-r--r--   0        0        0      766 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0    12366 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/pytest_plugin/collection.py
+-rw-r--r--   0        0        0     2436 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/pytest_plugin/commandline.py
+-rw-r--r--   0        0        0     1449 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/pytest_plugin/hooks.py
+-rw-r--r--   0        0        0     2376 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/pytest_plugin/logging.py
+-rw-r--r--   0        0        0      988 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/pytest_plugin/markers.py
+-rw-r--r--   0        0        0     1503 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/pytest_plugin/reporting.py
+-rw-r--r--   0        0        0     1685 2023-07-05 09:55:03.086009 pykiso-0.23.0/src/pykiso/pytest_plugin/utils.py
+-rw-r--r--   0        0        0      410 2023-07-05 09:55:03.087009 pykiso-0.23.0/src/pykiso/test_coordinator/__init__.py
+-rw-r--r--   0        0        0    13472 2023-07-05 09:55:03.087009 pykiso-0.23.0/src/pykiso/test_coordinator/test_case.py
+-rw-r--r--   0        0        0    16129 2023-07-05 09:55:03.087009 pykiso-0.23.0/src/pykiso/test_coordinator/test_execution.py
+-rw-r--r--   0        0        0     5479 2023-07-05 09:55:03.087009 pykiso-0.23.0/src/pykiso/test_coordinator/test_message_handler.py
+-rw-r--r--   0        0        0    16859 2023-07-05 09:55:03.087009 pykiso-0.23.0/src/pykiso/test_coordinator/test_suite.py
+-rw-r--r--   0        0        0      515 2023-07-05 09:55:03.088008 pykiso-0.23.0/src/pykiso/test_result/__init__.py
+-rw-r--r--   0        0        0    18907 2023-07-05 09:55:03.088008 pykiso-0.23.0/src/pykiso/test_result/assert_step_report.py
+-rw-r--r--   0        0        0     8391 2023-07-05 09:55:03.088008 pykiso-0.23.0/src/pykiso/test_result/multi_result.py
+-rw-r--r--   0        0        0     1971 2023-07-05 09:55:03.088008 pykiso-0.23.0/src/pykiso/test_result/templates/report_template.css
+-rw-r--r--   0        0        0     7883 2023-07-05 09:55:03.088008 pykiso-0.23.0/src/pykiso/test_result/templates/report_template.html.j2
+-rw-r--r--   0        0        0     3255 2023-07-05 09:55:03.088008 pykiso-0.23.0/src/pykiso/test_result/templates/report_template_script.js
+-rw-r--r--   0        0        0     9917 2023-07-05 09:55:03.088008 pykiso-0.23.0/src/pykiso/test_result/text_result.py
+-rw-r--r--   0        0        0     5663 2023-07-05 09:55:03.089009 pykiso-0.23.0/src/pykiso/test_result/xml_result.py
+-rw-r--r--   0        0        0      410 2023-07-05 09:55:03.089009 pykiso-0.23.0/src/pykiso/test_setup/__init__.py
+-rw-r--r--   0        0        0     9799 2023-07-05 09:55:03.089009 pykiso-0.23.0/src/pykiso/test_setup/config_registry.py
+-rw-r--r--   0        0        0    14160 2023-07-05 09:55:03.089009 pykiso-0.23.0/src/pykiso/test_setup/dynamic_loader.py
+-rw-r--r--   0        0        0      410 2023-07-05 09:55:03.089009 pykiso-0.23.0/src/pykiso/tool/__init__.py
+-rw-r--r--   0        0        0      410 2023-07-05 09:55:03.089009 pykiso-0.23.0/src/pykiso/tool/pykiso_to_pytest/__init__.py
+-rw-r--r--   0        0        0     5877 2023-07-05 09:55:03.089009 pykiso-0.23.0/src/pykiso/tool/pykiso_to_pytest/cli.py
+-rw-r--r--   0        0        0     3114 2023-07-05 09:55:03.090009 pykiso-0.23.0/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2
+-rw-r--r--   0        0        0    11816 2023-07-05 09:55:03.090009 pykiso-0.23.0/src/pykiso/tool/show_tag.py
+-rw-r--r--   0        0        0      410 2023-07-05 09:55:03.090009 pykiso-0.23.0/src/pykiso/tool/testrail/__init__.py
+-rw-r--r--   0        0        0    12414 2023-07-05 09:55:03.090009 pykiso-0.23.0/src/pykiso/tool/testrail/api.py
+-rw-r--r--   0        0        0     7728 2023-07-05 09:55:03.090009 pykiso-0.23.0/src/pykiso/tool/testrail/cli.py
+-rw-r--r--   0        0        0     5195 2023-07-05 09:55:03.090009 pykiso-0.23.0/src/pykiso/tool/testrail/console.py
+-rw-r--r--   0        0        0     8545 2023-07-05 09:55:03.090009 pykiso-0.23.0/src/pykiso/tool/testrail/containers.py
+-rw-r--r--   0        0        0     5067 2023-07-05 09:55:03.091009 pykiso-0.23.0/src/pykiso/tool/testrail/extraction.py
+-rw-r--r--   0        0        0    12851 2023-07-05 09:55:03.091009 pykiso-0.23.0/src/pykiso/tool/testrail/testrail.py
+-rw-r--r--   0        0        0     1794 2023-07-05 09:55:03.091009 pykiso-0.23.0/src/pykiso/types.py
+-rw-r--r--   0        0        0     9696 1970-01-01 00:00:00.000000 pykiso-0.23.0/setup.py
+-rw-r--r--   0        0        0     9516 1970-01-01 00:00:00.000000 pykiso-0.23.0/PKG-INFO
```

### Comparing `pykiso-0.22.2/LICENSE` & `pykiso-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/README.md` & `pykiso-0.23.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,17 @@
                                   failure
   -v, --verbose                   activate the internal framework logs
   -p, --pattern TEXT              test filter pattern, e.g. 'test_suite_1.py'
                                   or 'test_*.py'. Or even more granularly
                                   'test_suite_1.py::test_class::test_name'
   --version                       Show the version and exit.
   -h, --help                      Show this message and exit.
+  --logger                        Change the logger class used in pykiso, value
+                                  is the import path to the logger class, example
+                                  'logging.Logger'
 ```
 
 Suitable config files are available in the `examples` folder.
 
 ### Demo using example config ##
 
 ```bash
```

### Comparing `pykiso-0.22.2/pyproject.toml` & `pykiso-0.23.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykiso"
-version = "0.22.2"
+version = "0.23.0"
 description = "Embedded integration testing framework."
 authors = ["Sebastian Fischer <sebastian.fischer@de.bosch.com>"]
 license = "Eclipse Public License - v 2.0"
 readme = "README.md"
 homepage = "https://pypi.org/project/pykiso/"
 repository = "https://github.com/eclipse/kiso-testing"
 documentation = "https://kiso-testing.readthedocs.io/en/latest/"
@@ -57,14 +57,15 @@
 black = {version = "22.10.0",optional = true}
 pylink-square = {version = ">=0.12,<0.15", optional = true}
 pykiso-python-uds = {version = "~3.0.2", optional = true}
 pyserial = {version = "^3.0", optional = true}
 PyVISA = {version = "^1.12.0", optional = true}
 PyVISA-py = {version = "~0.5.3", optional = true}
 python-can = {version = "^4.0.0", optional = true, extras = ["pcan,vector"]}
+defusedxml = "^0.7.1"
 
 [tool.poetry.extras]
 plugins = [
     "pylink-square",
     "pykiso-python-uds",
     "python-can",
     "pyserial",
@@ -135,14 +136,16 @@
 [tool.pytest.ini_options]
 testpaths = [
     "./tests"
 ]
 addopts = """\
     --verbose \
     --log-level=INFO \
+    -p no:pytest_kiso \
+    --junitxml=reports/testReport.xml \
     --cov=./src \
     --cov-report=html \
     --cov-report html:./tests/coverage_report.html \
     --ignore=tests/test_acroname_usb_auxiliary.py \
     --ignore=tests/test_robot_acroname.py \
 """
```

### Comparing `pykiso-0.22.2/src/pykiso/__init__.py` & `pykiso-0.23.0/src/pykiso/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/__main__.py` & `pykiso-0.23.0/src/pykiso/__main__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/auxiliary.py` & `pykiso-0.23.0/src/pykiso/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/cli.py` & `pykiso-0.23.0/src/pykiso/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from typing import Dict, List, Optional, Tuple
 
 import click
 
 from . import __version__
 from .config_parser import parse_config
 from .global_config import Grabber
-from .logging_initializer import initialize_logging
+from .logging_initializer import change_logger_class, initialize_logging
 from .test_coordinator import test_execution
 from .test_setup.config_registry import ConfigRegistry
 from .types import PathType
 
 
 def eval_user_tags(click_context: click.Context) -> Dict[str, List[str]]:
     """Evaluate commandline args for user tags and raise exceptions for invalid
@@ -162,27 +162,34 @@
 @click.option(
     "-p",
     "--pattern",
     type=click.STRING,
     required=False,
     help="test filter pattern, e.g. 'test_suite_1.py' or 'test_*.py'. Or even more granularly 'test_suite_1.py::TestClass::test_name'",
 )
+@click.option(
+    "--logger",
+    type=click.STRING,
+    required=False,
+    help="use the specified logger class in pykiso",
+)
 @click.version_option(__version__)
 @Grabber.grab_cli_config
 @click.pass_context
 def main(
     click_context: click.Context,
     test_configuration_file: Tuple[PathType],
     log_path: Tuple[PathType] = None,
     log_level: str = "INFO",
     report_type: str = "text",
     step_report: Optional[PathType] = None,
     pattern: Optional[str] = None,
     failfast: bool = False,
     verbose: bool = False,
+    logger: Optional[str] = None,
 ):
     """Embedded Integration Test Framework - CLI Entry Point.
 
     TAG Filters: any additional option to be passed to the test as tag through
     the pykiso call. Multiple values must be separated with a comma.
 
     For example: pykiso -c your_config.yaml --branch-level dev,master --variant delta
@@ -195,43 +202,45 @@
     :param report_type: if "test", the standard report, if "junit", a junit report is generated
     :param variant: allow the user to execute a subset of tests based on variants
     :param branch_level: allow the user to execute a subset of tests based on branch levels
     :param step_report: file path for the step report or None
     :param pattern: overwrite the pattern from the YAML file for easier test development
     :param failfast: stop the test run on the first error or failure
     :param verbose: activate logging for the whole framework
+    :param logger: class of the logger that will be used in the tests
     """
+    if logger:
+        change_logger_class(log_level, verbose, logger)
 
     for idx, config_file in enumerate(test_configuration_file):
-
         yaml_name = Path(config_file).stem
         # Set the logging
         if log_path:
             # Put all logs in one file
             if len(log_path) == 1:
-                logger = initialize_logging(
+                log = initialize_logging(
                     log_path[0], log_level, verbose, report_type, yaml_name
                 )
             # Log in different files for each yaml
             elif len(log_path) == len(test_configuration_file):
-                logger = initialize_logging(
+                log = initialize_logging(
                     log_path[idx], log_level, verbose, report_type, yaml_name
                 )
             else:
                 raise click.UsageError(
                     f"Mismatch: {len(test_configuration_file)} yaml config files provided but {len(log_path)} log files"
                 )
         else:
             log_path = None
-            logger = initialize_logging(log_path, log_level, verbose, report_type)
-
+            log = initialize_logging(log_path, log_level, verbose, report_type)
         # Get YAML configuration
+
         cfg_dict = parse_config(config_file)
         # Run tests
-        logger.debug("cfg_dict:\n{}".format(pprint.pformat(cfg_dict)))
+        log.debug("cfg_dict:\n{}".format(pprint.pformat(cfg_dict)))
 
         ConfigRegistry.register_aux_con(cfg_dict)
 
         user_tags = eval_user_tags(click_context)
 
         exit_code = test_execution.execute(
             cfg_dict, report_type, yaml_name, user_tags, step_report, pattern, failfast
```

### Comparing `pykiso-0.22.2/src/pykiso/config_parser.py` & `pykiso-0.23.0/src/pykiso/config_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,17 @@
         """Return the content of a yaml file identified by !include tag.
 
         :param node: ScalarNode currently in use
 
         :return: included yaml file's content
         """
         nested_yaml = (self._base_dir / Path(node.value)).resolve()
-        nested_cfg = yaml.load(nested_yaml, Loader=YamlLoader)
+        nested_cfg = yaml.load(
+            nested_yaml, Loader=YamlLoader
+        )  # nosec B506 YamlLoader inherits from yaml.SafeLoader.
         return nested_cfg
 
     def resolve_path(self, node: yaml.nodes.ScalarNode) -> str:
         """Resolve a path relative to the config file's location.
 
         :param node: ScalarNode currently in use
 
@@ -308,15 +310,17 @@
         * Including the sub-YAML files marked by the !include tag.
 
     :param file_name: path to the config file
 
     :return: config dict with resolved paths where needed
     """
     with open(file_name, "r") as f:
-        cfg = yaml.load(f, Loader=YamlLoader)
+        cfg = yaml.load(
+            f, Loader=YamlLoader
+        )  # nosec B506 YamlLoader inherits from yaml.SafeLoader.
 
     # Check requirements
     requirements = cfg.get("requirements")
     if requirements:
         check_requirements(requirements)
 
     if "connectors" not in cfg:
```

### Comparing `pykiso-0.22.2/src/pykiso/connector.py` & `pykiso-0.23.0/src/pykiso/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,18 @@
             self._cc_open()
 
     def close(self) -> None:
         """Close a thread-safe channel."""
         with self._lock:
             self._cc_close()
 
+    def shutdown(self) -> None:
+        """Unitialize channel. Will be called at the end of the test session."""
+        pass
+
     def cc_send(self, msg: MsgType, *args, **kwargs) -> None:
         """Send a thread-safe message on the channel and wait for an acknowledgement.
 
         :param msg: message to send
         :param kwargs: named arguments
         """
         if ("raw" in kwargs) or args:
```

### Comparing `pykiso-0.22.2/src/pykiso/exceptions.py` & `pykiso-0.23.0/src/pykiso/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/global_config.py` & `pykiso-0.23.0/src/pykiso/global_config.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/interfaces/dt_auxiliary.py` & `pykiso-0.23.0/src/pykiso/interfaces/dt_auxiliary.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         :raises AuxiliaryCreationError: if instance creation failed
         """
         log.internal_info(f"Creating instance of auxiliary {self.name}")
 
         with self.lock:
             # if the current aux is alive don't try to create it again
             if self.is_instance:
+                log.internal_info(f"Auxiliary {self.name} is already created")
                 return True
 
             is_created = self._create_auxiliary_instance()
 
             if not is_created:
                 raise AuxiliaryCreationError(self.name)
 
@@ -162,14 +163,15 @@
         log.internal_info(f"Deleting instance of auxiliary {self.name}")
 
         with self.lock:
 
             # if the current aux is not alive don't try to delete it
             # again
             if not self.is_instance:
+                log.internal_info(f"Auxiliary {self.name} is already deleted")
                 return True
 
             # stop each auxiliary's tasks
             self._stop_tx_task()
             self._stop_rx_task()
 
             is_deleted = self._delete_auxiliary_instance()
@@ -184,48 +186,46 @@
 
     def _start_tx_task(self) -> None:
         """Start transmission task."""
         if self.tx_task_on is False:
             log.internal_debug("transmit task is not needed, don't start it")
             return
 
-        log.internal_debug(f"start transmit task {self.name}_tx")
-        self.tx_thread = threading.Thread(
-            name=f"{self.name}_tx", target=self._transmit_task
-        )
+        task_name = f"{self.name}_tx"
+        log.internal_debug("start transmit task %s", task_name)
+        self.tx_thread = threading.Thread(name=task_name, target=self._transmit_task)
         self.tx_thread.start()
 
     def _start_rx_task(self) -> None:
         """Start reception task."""
         if self.rx_task_on is False:
             log.internal_debug("reception task is not needed, don't start it")
             return
 
-        log.internal_debug(f"start reception task {self.name}_rx")
-        self.rx_thread = threading.Thread(
-            name=f"{self.name}_rx", target=self._reception_task
-        )
+        task_name = f"{self.name}_rx"
+        log.internal_debug("start reception task %s", task_name)
+        self.rx_thread = threading.Thread(name=task_name, target=self._reception_task)
         self.rx_thread.start()
 
     def _stop_tx_task(self) -> None:
         """Stop transmission task."""
         if self.tx_task_on is False:
-            log.internal_debug("transmit task was not started, so no need to stop it")
+            log.internal_debug("transmit task was not started, no need to stop it")
             return
 
         log.internal_debug(f"stop transmit task {self.name}_tx")
         self.queue_in.put((AuxCommand.DELETE_AUXILIARY, None))
         self.stop_tx.set()
         self.tx_thread.join()
         self.stop_tx.clear()
 
     def _stop_rx_task(self) -> None:
         """Stop reception task."""
         if self.rx_task_on is False:
-            log.internal_debug("recpetion task was not started, so no need t stop it")
+            log.internal_debug("reception task was not started, no need to stop it")
             return
 
         log.internal_debug(f"stop reception task {self.name}_rx")
         self.stop_rx.set()
         self.rx_thread.join()
         self.stop_rx.clear()
 
@@ -299,14 +299,18 @@
         :return: data contained in the auxiliary's queue_out
         """
         try:
             return self.queue_out.get(blocking, timeout_in_s)
         except queue.Empty:
             return None
 
+    def shutdown(self):
+        """Uninitialize method. Will be called at the end of the test session."""
+        pass
+
     @abc.abstractmethod
     def _create_auxiliary_instance(self) -> bool:
         """Common interface call at auxiliary creation.
 
         This method could be used to e.g initiate the communication
         using the attached connector.
 
@@ -383,16 +387,17 @@
         :param args: positional arguments
         :param kwargs: named arguments
 
         :return: True if everything was successful otherwise False
         """
         log.internal_info("Close channel")
         try:
+            ret = func(self, *arg, **kwargs)
             self.channel.close()
-            return func(self, *arg, **kwargs)
+            return ret
         except Exception:
             log.exception("Unable to close channel communication")
             return False
 
     return inner_close
```

### Comparing `pykiso-0.22.2/src/pykiso/interfaces/mp_auxiliary.py` & `pykiso-0.23.0/src/pykiso/interfaces/mp_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/interfaces/simple_auxiliary.py` & `pykiso-0.23.0/src/pykiso/interfaces/simple_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/interfaces/thread_auxiliary.py` & `pykiso-0.23.0/src/pykiso/interfaces/thread_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/acroname_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/acroname_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/communication_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/communication_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/dut_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/dut_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/proxy_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/proxy_auxiliary.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     |_____________________________________________|
 
 .. currentmodule:: proxy_auxiliary
 
 """
 
 import logging
+import queue
 import sys
 import time
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 from pykiso import AuxiliaryInterface, CChannel
 from pykiso.interfaces.dt_auxiliary import (
@@ -92,14 +93,27 @@
             is_proxy_capable=True, tx_task_on=False, rx_task_on=True, **kwargs
         )
         self.channel = com
         self._open_count = 0
         self.logger = self._init_trace(activate_trace, trace_dir, trace_name)
         self.proxy_channels = self.get_proxy_con(aux_list)
 
+    def _count_open_proxy_channels(self) -> int:
+        """
+        Get the number of proxy channels connected to this auxiliary
+        that are currently open.
+        """
+        return len(
+            [
+                ccproxy
+                for ccproxy in self.proxy_channels
+                if isinstance(ccproxy.queue_out, queue.Queue)
+            ]
+        )
+
     @property
     def _open_connections(self) -> int:
         """A counter monitoring the number of attached running auxiliaries.
 
         .. warning::
             Do not set this manually as it can easily result in unexpected behaviours.
 
@@ -116,23 +130,27 @@
         with self.lock:
             return self._open_count
 
     @_open_connections.setter
     def _open_connections(self, value: int):
         # locking shouldn't be necessary but we're never too paranoid
         with self.lock:
+            # on the original proxy setup, the auxiliaries are created before the proxy
+            # therefore, when the first auxiliary will be stopped, the counter value will be -1
+            if value < 0:
+                value = self._count_open_proxy_channels()
             last_connection_closed = value == 0 and self._open_count == 1
             first_connection_opened = value == 1 and self._open_count == 0
-            # prevent negative values on invalid initialization
-            if value >= 0:
-                self._open_count = value
-            if last_connection_closed and self.is_instance:
-                self.delete_instance()
-            elif first_connection_opened and not self.is_instance:
-                self.create_instance()
+            self._open_count = value
+        # stop proxy if the last attached auxiliary was stopped
+        if last_connection_closed and self.is_instance:
+            self.delete_instance()
+        # start proxy if the first attached auxiliary is started
+        elif first_connection_opened and not self.is_instance:
+            self.create_instance()
 
     @staticmethod
     def _init_trace(
         activate: bool, t_dir: Optional[str] = None, t_name: Optional[str] = None
     ) -> logging.Logger:
         """Initialize the logging trace for proxy auxiliary received
         message recording.
```

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/record_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/record_auxiliary.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,20 +217,20 @@
         :param data: data to be decoded
 
         :return: data decoded
         """
         # decode
         try:
             return data.decode()
-        except UnicodeDecodeError:
+        except (UnicodeDecodeError, AttributeError):
             pass
         # get Hex values
         try:
             return data.hex()
-        except Exception:
+        except AttributeError:
             pass
 
         # Fail decoding, parse RAW data in string (avoid losing it)
         log.error(f"Could not parse the received data: {data}")
         return str(data)
 
     def clear_buffer(self) -> None:
```

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 """
 from __future__ import annotations
 
 import logging
 from enum import Enum
 from pathlib import Path
 from typing import List
-from xml.etree import ElementTree
 from xml.etree.ElementTree import Element
 
+# Use defusedxml, as xml is not secure against maliciously constructed data.
+from defusedxml import ElementTree
+
 log = logging.getLogger(__name__)
 
 
 class OdxParser:
     """Used to parse ODX files to configure a Uds server"""
 
     class RefType(Enum):
```

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/auxiliaries/ykush_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/auxiliaries/ykush_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_example.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_example.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_fdx_lauterbach.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_fdx_lauterbach.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_flasher_example.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_flasher_example.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_mp_proxy.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_mp_proxy.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_pcan_can.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_pcan_can.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 .. currentmodule:: cc_pcan_can
 
 """
 
 import logging
 import os
+import shutil
 import sys
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 try:
     import can
     import can.bus
@@ -369,15 +370,17 @@
                 log.internal_debug(
                     f"received CAN Message: {frame_id}, {payload}, {timestamp}"
                 )
                 return {"msg": payload, "remote_id": frame_id, "timestamp": timestamp}
             else:
                 return {"msg": None}
         except can.CanError as can_error:
-            log.internal_debug(f"encountered can error: {can_error}")
+            log.internal_info(
+                f"encountered CAN error while receiving message: {can_error}"
+            )
             return {"msg": None}
         except Exception:
             log.exception(f"encountered error while receiving message via {self}")
             return {"msg": None}
 
     # TODO: refactor to use trc reader when new version of python can is release
     def _merge_trc(self) -> None:
@@ -394,15 +397,18 @@
         try:
             if self.trace_name is None:
                 # If a log file is not provided, take the fist trace created as result file
                 result_trace = list_of_traces[0]
             else:
                 # Else write the first trace content in the log file and then remove it
                 result_trace = Path(self.trace_path / self.trace_name)
-                list_of_traces[0] = list_of_traces[0].rename(result_trace)
+                list_of_traces[0] = shutil.move(
+                    str(list_of_traces[0]), str(result_trace)
+                )
+                list_of_traces[0] = Path(list_of_traces[0])
 
             # End of the trace header
             first_message_line = 33
 
             # Get start time of the first trc file
             with list_of_traces[0].open("r") as trc:
                 data = trc.read().splitlines(True)
@@ -499,11 +505,11 @@
                 millisecond.
 
         :return: start time of the trc file in ms since the start of the day
         """
         ms_in_a_day = 86400000
         return (start_time % 1) * ms_in_a_day
 
-    def __del__(self) -> None:
+    def shutdown(self) -> None:
         """Destructor method."""
         if self.logging_activated:
             self._merge_trc()
```

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_process.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             stdout=subprocess.PIPE if self._pipe_stdout else None,
             stdin=subprocess.PIPE if self._pipe_stdin else None,
             shell=self._shell,
             text=self._text,
             encoding=self._encoding,
             cwd=self._cwd,
             env=self._env,
-        )
+        )  # nosec B602 Since we only provide an interface to the user to popen, we accept the risk of a vulnerablility to various shell injection attacks.
 
         if self._pipe_stdout:
             self._stdout_thread = self._start_read_thread(
                 self._process.stdout, "stdout"
             )
         if self._pipe_stderr:
             self._stderr_thread = self._start_read_thread(
```

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_proxy.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         """Open proxy channel."""
         log.internal_info("Open proxy channel")
         self.queue_out = queue.Queue()
 
     def _cc_close(self) -> None:
         """Close proxy channel."""
         log.internal_debug("Close proxy channel")
-        self.queue_out = queue.Queue()
+        self.queue_out = None
 
     def _cc_send(self, *args: Any, **kwargs: Any) -> None:
         """Call the attached ProxyAuxiliary's transmission callback
         with the provided arguments.
 
         :param args: positionnal arguments to pass to the callback
         :param kwargs: named arguments to pass to the callback
```

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_raw_loopback.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_raw_loopback.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_rtt_segger.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_rtt_segger.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_serial.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_serial.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 class CCSerial(connector.CChannel):
     """Connector for serial devices"""
 
     def __init__(
         self,
         port: Optional[str] = None,
+        serial_number: Optional[str] = None,
         vid: Optional[int] = None,
         pid: Optional[int] = None,
         baudrate: int = 9600,
         bytesize: ByteSize = ByteSize.EIGHT_BITS,
         parity: Parity = Parity.PARITY_NONE,
         stopbits: StopBits = StopBits.STOPBITS_ONE,
         timeout: Optional[float] = None,
@@ -81,14 +82,17 @@
         inter_byte_timeout: Optional[float] = None,
         exclusive: Optional[bool] = None,
         **kwargs,
     ):
         """Init Serial settings
 
         :param port: Device name (e.g. "COM1" for Windows or "/dev/ttyACM0" for Linux)
+        :param serial_number: serial number
+        :param vid: vendor id
+        :param pid: product id
         :param baudrate: Baud rate such as 9600 or 115200 etc, defaults to 9600
         :param bytesize: Number of data bits. Possible values:
           FIVEBITS, SIXBITS, SEVENBITS, EIGHTBITS, defaults to EIGHTBITS
         :param parity: Enable parity checking. Possible values:
           PARITY_NONE, PARITY_EVEN, PARITY_ODD PARITY_MARK, PARITY_SPACE,
           defaults to PARITY_NONE
         :param stopbits:  Number of stop bits. Possible values:
@@ -121,58 +125,77 @@
             write_timeout=write_timeout,
             dsrdtr=dsrdtr,
             inter_byte_timeout=inter_byte_timeout,
             exclusive=exclusive,
         )
 
         self.current_write_timeout = write_timeout
-        self.serial.port = self._get_port(port=port, vid=vid, pid=pid)
+        self.serial.port = self._get_port(
+            port=port, vid=vid, pid=pid, serial_number=serial_number
+        )
 
     @staticmethod
-    def _find_device(vid: int, pid: int) -> str:
-        """Return the device which matches pid and vid.
+    def _find_device(vid: int, pid: int, serial_number: str) -> str:
+        """Return the device which matches the given pid/vid or serial_number.
 
         :param vid: vendor id
         :param pid: product id
+        :param serial_number: serial number
 
         :return: com port for the found device. I.e. "COM4" or "/dev/tty1"
         """
 
         attached_com_devices = serial.tools.list_ports.comports()
-        found_devices = [
-            port for port in attached_com_devices if port.pid == pid and port.vid == vid
-        ]
+        found_devices = []
+        if pid and vid:
+            found_devices.extend(
+                [
+                    port
+                    for port in attached_com_devices
+                    if port.pid == pid and port.vid == vid
+                ]
+            )
+
+        if serial_number:
+            found_devices.extend(
+                [
+                    port
+                    for port in attached_com_devices
+                    if port.serial_number == serial_number
+                ]
+            )
+
         if not found_devices:
             raise ConnectionError(
-                f"Failed to detect connected USB device with IDs {vid:04X}:{pid:04x}."
+                f"Failed to detect connected USB device with IDs {vid:04X}:{pid:04x} or serial_number {serial_number}."
             )
 
         found_devices = [
             port.name if not sys.platform.startswith("win") else port.device
             for port in found_devices
         ]
         if len(found_devices) > 1:
             log.internal_warning(
-                f"Found multiple devices, {found_devices}, with matching IDs {vid:04X}:{pid:04x}. Select first device {found_devices[0]}."
+                f"Found multiple devices, {found_devices}, with matching IDs {vid:04X}:{pid:04X} or serial_number {serial_number}. Select first device {found_devices[0]}."
             )
         return found_devices[0]
 
-    def _get_port(self, port: str, vid: int, pid: int) -> str:
+    def _get_port(self, port: str, vid: int, pid: int, serial_number: str) -> str:
         """Returns com port depending on the given port argument.
-        If port set to auto, the device will be searched for,
-        using the pid and vid, else the port argument will be returned.
+        If port is None, the device will be searched for,
+        using the pid/vid and serial_number, else the port argument will be returned.
 
         :param port: port  I.e. "COM4" or "/dev/tty1"
         :param vid: vendor id
         :param pid: product id
 
         :return: com ports of given or found device. I.e. "COM4" or "/dev/tty1"
         """
         if port is None:
-            return CCSerial._find_device(vid=vid, pid=pid)
+            return CCSerial._find_device(vid=vid, pid=pid, serial_number=serial_number)
         else:
             return port
 
     def _cc_open(self) -> None:
         """Open serial port"""
         self.serial.open()
```

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_socket_can/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_tcp_ip.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_tcp_ip.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_uart.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_uart.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_udp.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_udp.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_udp_server.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_udp_server.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_usb.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_usb.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_vector_can.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_vector_can.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/cc_visa.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/cc_visa.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/flash_jlink.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/flash_jlink.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/connectors/flash_lauterbach.py` & `pykiso-0.23.0/src/pykiso/lib/connectors/flash_lauterbach.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/__init__.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/acroname_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/acroname_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/aux_interface.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/aux_interface.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/communication_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/communication_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/dut_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/dut_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/loader.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/loader.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/proxy_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/record_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/record_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/lib/robot_framework/uds_auxiliary.py` & `pykiso-0.23.0/src/pykiso/lib/robot_framework/uds_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/logging_initializer.py` & `pykiso-0.23.0/src/pykiso/logging_initializer.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,35 +14,61 @@
 :module: logging
 
 :synopsis: Handles initialization of the loggers and cutom logging levels.
 
 .. currentmodule:: logging
 
 """
+import importlib
 import logging
+import re
 import sys
 import time
+from ast import literal_eval
+from functools import partialmethod
 from pathlib import Path
-from typing import List, NamedTuple, Optional
+from typing import List, NamedTuple, Optional, Union
 
 from .test_setup.dynamic_loader import PACKAGE
 from .types import PathType
 
+LEVELS = {
+    "DEBUG": logging.DEBUG,
+    "INFO": logging.INFO,
+    "WARNING": logging.WARNING,
+    "ERROR": logging.ERROR,
+}
+
 
 class LogOptions(NamedTuple):
     """
     Namedtuple containing the available options for logging configuration.
     """
 
-    log_path: PathType
+    log_path: Optional[PathType]
     log_level: str
     report_type: str
     verbose: bool
 
 
+class InternalLogsFilter(logging.Filter):
+    def filter(self, record: logging.LogRecord) -> bool:
+        """Filters internal log levels
+
+        :param record: event being logged
+
+        :return: False if internal logging, True otherwise
+        """
+        return record.levelno not in (
+            logging.INTERNAL_WARNING,
+            logging.INTERNAL_INFO,
+            logging.INTERNAL_DEBUG,
+        )
+
+
 # used to store the selected logging options
 log_options: Optional[LogOptions] = None
 
 # used to store the loggers that shouldn't be silenced
 active_loggers = set()
 
 
@@ -59,15 +85,15 @@
     if not hasattr(logging, "INTERNAL_WARNING"):
         add_logging_level("INTERNAL_WARNING", logging.WARNING + 1)
         add_logging_level("INTERNAL_INFO", logging.INFO + 1)
         add_logging_level("INTERNAL_DEBUG", logging.DEBUG + 1)
 
 
 def initialize_logging(
-    log_path: PathType,
+    log_path: Optional[PathType],
     log_level: str,
     verbose: bool,
     report_type: str = None,
     yaml_name: str = None,
 ) -> logging.Logger:
     """Initialize the logging.
 
@@ -82,53 +108,33 @@
 
     :returns: configured Logger
     """
     root_logger = logging.getLogger()
     log_format = logging.Formatter(
         "%(asctime)s [%(levelname)s] %(module)s:%(lineno)d: %(message)s"
     )
-    levels = {
-        "DEBUG": logging.DEBUG,
-        "INFO": logging.INFO,
-        "WARNING": logging.WARNING,
-        "ERROR": logging.ERROR,
-    }
     # add internal kiso log levels
     add_internal_log_levels()
 
-    # update logging options
-    global log_options
-    log_options = LogOptions(log_path, log_level, report_type, verbose)
-
-    class InternalLogsFilter(logging.Filter):
-        def filter(self, record):
-            """Filters internal log levels
-
-            :param record: event being logged
-
-            :return: False if internal logging, True otherwise
-            """
-            return record.levelno not in (
-                logging.INTERNAL_WARNING,
-                logging.INTERNAL_INFO,
-                logging.INTERNAL_DEBUG,
-            )
-
     # if log_path is given create a file handler
     if log_path is not None:
         log_path = Path(log_path)
         if log_path.suffix == "":
             log_path.mkdir(parents=True, exist_ok=True)
             fname = time.strftime(f"%Y-%m-%d_%H-%M-{yaml_name}.log")
             log_path = log_path / fname
         file_handler = logging.FileHandler(log_path, "a+")
         file_handler.setFormatter(log_format)
-        file_handler.setLevel(levels[log_level])
+        file_handler.setLevel(LEVELS[log_level])
         root_logger.addHandler(file_handler)
 
+    # update logging options after having modified the log path
+    global log_options
+    log_options = LogOptions(log_path, log_level, report_type, verbose)
+
     # if report_type is junit use sys.stdout as stream
     if report_type == "junit":
         stream = sys.stdout
         # flush all StreamHandlers
         for handler in root_logger.handlers:
             if isinstance(handler, logging.StreamHandler):
                 handler.flush()
@@ -141,21 +147,21 @@
     # report type is not junit just instanciate a StreamHandler that prints to stderr
     else:
         stream = sys.stderr
 
     # for all report types add a StreamHandler
     stream_handler = logging.StreamHandler(stream)
     stream_handler.setFormatter(log_format)
-    stream_handler.setLevel(levels[log_level])
+    stream_handler.setLevel(LEVELS[log_level])
     if not verbose:
         # filter internal log levels
         stream_handler.addFilter(InternalLogsFilter())
     root_logger.addHandler(stream_handler)
 
-    root_logger.setLevel(levels[log_level])
+    root_logger.setLevel(LEVELS[log_level])
 
     return logging.getLogger(__name__)
 
 
 def add_logging_level(level_name: str, level_num: int):
     """
     Comprehensively adds a new logging level to the `logging` module and the
@@ -230,7 +236,102 @@
     # store previous loggers to keep active (union of previous and current loggers)
     active_loggers |= set(loggers)
 
     # set the loggers that are not part of active_loggers to level WARNING
     loggers_to_deactivate = set(relevant_loggers) - set(active_loggers)
     for logger_name in loggers_to_deactivate:
         logging.getLogger(logger_name).setLevel(logging.WARNING)
+
+
+def import_object(path: str) -> Union[None, logging.Logger]:
+    """return the object based on the path.
+        For example : logging.Logger will return Logger
+
+    :param path: path to the object
+
+    :return: object based on the path
+    """
+    if path:
+        components = path.split(".")
+        mod = importlib.import_module(".".join(components[:-1]))
+        obj = getattr(mod, components[-1])
+        if not issubclass(obj, logging.Logger):
+            raise TypeError(f"{obj} is not derived from logging.Logger.")
+        return obj
+    else:
+        return None
+
+
+def add_filter_to_handler(func):
+    """Decorator function that will add a filter to all the handlers
+        of a logger after a function.
+
+    :param func: function to execute
+    """
+
+    def wrapper(self, *arg, **kwargs):
+        func(self, *arg, **kwargs)
+        for handler in self.handlers:
+            handler.addFilter(InternalLogsFilter())
+
+    return wrapper
+
+
+def remove_handler_from_logger(func):
+    """Decorator that will remove all handlers of a logger after
+        executing a function.
+
+    :param func: function to execute
+    """
+
+    def wrapper(self, *arg, **kwargs):
+        func(self, *arg, **kwargs)
+        for handler in self.handlers:
+            self.removeHandler(handler)
+
+    return wrapper
+
+
+def change_logger_class(log_level: str, verbose: bool, logger: str):
+    """Change the class of all the logger of pykiso.
+
+    :param log_level: level of the log
+    :param logger: str of the path to the logger class
+    """
+    # Get the argument to initialize the logger if needed
+    kwargs_log = {}
+    # Search if the str has the following pattern name.name(name_arg=arg) or name.name
+    arg_match = re.match(r"([^(]*)\(([^\)]+)\)", logger)
+    if arg_match:
+        logger_class = arg_match.group(1)
+        arg_logger = arg_match.group(2).split(",")
+        kwargs_log = {
+            arg.split("=")[0]: literal_eval(arg.split("=")[1]) for arg in arg_logger
+        }
+    else:
+        logger_class = logger
+
+    # Import the logger class
+    logger_class = import_object(logger_class)
+    # We modify the init function so that the logger only need the name to be initialized
+    if kwargs_log:
+        logger_class.__init__ = partialmethod(
+            logger_class.__init__, level=LEVELS[log_level], **kwargs_log
+        )
+    # If the verbose is not specified, the filter is added to the handler of the logger
+    if not verbose:
+        logger_class.__init__ = add_filter_to_handler(logger_class.__init__)
+    # Change logging.root since test can use logging.info for example
+    logging.root = logger_class(name="root", level=LEVELS[log_level])
+    # Remove the handler from the new logger else the handler will be called twice with the handler from the root
+    logger_class.__init__ = remove_handler_from_logger(logger_class.__init__)
+
+    # Replace already existing logger with the new class and change the parent
+    for name, module in sys.modules.items():
+        if name.startswith("pykiso"):
+            if getattr(module, "log", None):
+                module.log = logger_class(name=module.log.name, level=LEVELS[log_level])
+                module.log.parent = logging.root
+
+    # Setup the future logger class as the new class for the manager
+    logging.Logger.manager.root = logging.root
+    logging.setLoggerClass(logger_class)
```

### Comparing `pykiso-0.22.2/src/pykiso/message.py` & `pykiso-0.23.0/src/pykiso/message.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/pytest_plugin/__init__.py` & `pykiso-0.23.0/src/pykiso/pytest_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/pytest_plugin/collection.py` & `pykiso-0.23.0/src/pykiso/pytest_plugin/collection.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/pytest_plugin/commandline.py` & `pykiso-0.23.0/src/pykiso/pytest_plugin/commandline.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/pytest_plugin/hooks.py` & `pykiso-0.23.0/src/pykiso/pytest_plugin/hooks.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/pytest_plugin/logging.py` & `pykiso-0.23.0/src/pykiso/pytest_plugin/logging.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/pytest_plugin/markers.py` & `pykiso-0.23.0/src/pykiso/pytest_plugin/markers.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/pytest_plugin/reporting.py` & `pykiso-0.23.0/src/pykiso/pytest_plugin/reporting.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/pytest_plugin/utils.py` & `pykiso-0.23.0/src/pykiso/pytest_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_coordinator/test_case.py` & `pykiso-0.23.0/src/pykiso/test_coordinator/test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from __future__ import annotations
 
 import functools
 import logging
 import unittest
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union
 
+import pykiso.test_result.assert_step_report as step_report
+
 from .. import message
 from ..interfaces.thread_auxiliary import AuxiliaryInterface
 from ..logging_initializer import get_logging_options, initialize_logging
 from .test_message_handler import test_app_interaction
 
 if TYPE_CHECKING:
     from .test_suite import BaseTestSuite
@@ -290,14 +292,19 @@
     """
 
     def decorator(func):
         @functools.wraps(func)
         def func_wrapper(self: BasicTest) -> None:
             # track the current execution for logging
             current_execution = None
+            test_class_name = type(self).__name__
+            # Prepare report for the current test so we can get the current result for the class
+            if getattr(self, "step_report", False) and self.step_report.header:
+                step_report._prepare_report(self, self._testMethodName)
+                result_test = step_report.ALL_STEP_REPORT[test_class_name]["succeed"]
 
             for retry_nb in range(1, max_try + 1):
                 try:
                     # by the 2nd attempt, end the test with the teardown and start with setUp
                     if retry_nb > 1:
                         if rerun_teardown:
                             current_execution = self.tearDown
@@ -325,14 +332,20 @@
 
                     # raise the exception that occurred during the latest attempt
                     if retry_nb == max_try or stability_test:
                         log.error(
                             f">>>>>>>>>> Test {retry_nb}/{max_try} failed <<<<<<<<<<"
                         )
                         raise e
+                    elif (
+                        getattr(self, "step_report", False) and self.step_report.header
+                    ):
+                        step_report.add_retry_information(
+                            self, result_test, retry_nb, max_try, e
+                        )
 
                     # print counter only after failing test to avoid spamming the console
                     log.info(f">>>>>>>>>> Attempt: {retry_nb +1}/{max_try} <<<<<<<<<<")
 
         return func_wrapper
 
     return decorator
```

### Comparing `pykiso-0.22.2/src/pykiso/test_coordinator/test_execution.py` & `pykiso-0.23.0/src/pykiso/test_coordinator/test_execution.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_coordinator/test_message_handler.py` & `pykiso-0.23.0/src/pykiso/test_coordinator/test_message_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,14 @@
                     f"--------------- TEARDOWN: {self.test_suite_id}, {self.test_case_id} ---------------"
                 )
                 timeout_resp = self.teardown_timeout
 
             # for all configured auxiliaries just send the associated
             # command and evaluate return test results
             for aux in self.test_auxiliary_list:
-
                 cmd = message.Message(
                     msg_type=message.MessageType.COMMAND,
                     sub_type=message_type,
                     test_suite=self.test_suite_id,
                     test_case=self.test_case_id,
                 )
                 is_ack = aux.send_fixture_command(command=cmd, timeout=timeout_cmd)
```

### Comparing `pykiso-0.22.2/src/pykiso/test_coordinator/test_suite.py` & `pykiso-0.23.0/src/pykiso/test_coordinator/test_suite.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_result/__init__.py` & `pykiso-0.23.0/src/pykiso/test_result/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_result/assert_step_report.py` & `pykiso-0.23.0/src/pykiso/test_result/assert_step_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,26 +26,29 @@
 """
 import functools
 import inspect
 import linecache
 import logging
 import re
 import sys
+import traceback
 import types
 import typing
 import unittest
 from collections import OrderedDict
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
-from typing import List, Union
+from typing import Dict, List, Union
 from unittest.case import TestCase, _SubTest
 
 import jinja2
 
+from pykiso.test_coordinator.test_case import BasicTest
+
 from .text_result import BannerTestResult
 from .xml_result import TestInfo, XmlTestResult
 
 log = logging.getLogger(__name__)
 
 
 # Global variables
@@ -213,32 +216,35 @@
         # Store the tests list
         ALL_STEP_REPORT[test_class_name]["test_list"] = OrderedDict()
 
     # Create the current test step storage
     if not ALL_STEP_REPORT[test_class_name]["test_list"].get(test_name):
         test_method = getattr(test, test_name, None)
         test_description = test_method.__doc__ or ""
-        ALL_STEP_REPORT[test_class_name]["test_list"][test_name] = {
+        ALL_STEP_REPORT[test_class_name]["test_list"][test_name]: Dict[
+            str,
+            Union[str, List[List[Dict[str, Union[str, bool]]]], List[List[str]]],
+        ] = {
             "description": test_description,
-            "steps": [],
-            "unexpected_errors": [],
+            "steps": [[]],
+            "unexpected_errors": [[]],
         }
 
 
 def _add_step(
     test_class_name: str,
     test_name: str,
     message: str,
     var_name: str,
     expected: typing.Any,
     received: typing.Any,
 ):
     global ALL_STEP_REPORT, REPORT_KEYS
 
-    ALL_STEP_REPORT[test_class_name]["test_list"][test_name]["steps"].append(
+    ALL_STEP_REPORT[test_class_name]["test_list"][test_name]["steps"][-1].append(
         dict(zip(REPORT_KEYS, [message, var_name, expected, received, True]))
     )
 
 
 def determine_parent_test_function(test_name: str) -> str:
     """Determine the parent test function.
 
@@ -359,17 +365,17 @@
         # Run the assert method and mark the test as failed if the AssertionError is raised
         try:
             return assert_method(*args, **kwargs)
         except test_case_inst.failureException as e:
             log.error(f"Assert step exception: {e}")
             test_case_inst.step_report.last_error_message = f"{e}"
             if parent_method:
-                ALL_STEP_REPORT[test_class_name]["test_list"][test_name][-1][
-                    "succeed"
-                ] = False
+                ALL_STEP_REPORT[test_class_name]["test_list"][test_name]["steps"][-1][
+                    -1
+                ]["succeed"] = False
                 ALL_STEP_REPORT[test_class_name]["succeed"] = False
 
             test_case_inst.step_report.success = False
 
             # repeat the assertion failure as first element in the traceback
             frame = currentframe.f_back
             tb = types.TracebackType(None, frame, frame.f_lasti, frame.f_lineno)
@@ -392,16 +398,17 @@
 def is_test_success(test: dict) -> bool:
     """Check if test was successful.
 
     :param tests: test
     :return: True if each step in a test was successful and no unexpected error
         was raised else False
     """
-    return all([step["succeed"] for step in test["steps"]]) and not test.get(
-        "unexpected_errors"
+    return (
+        all([step["succeed"] for step in test["steps"][-1]])
+        and not test.get("unexpected_errors")[-1]
     )
 
 
 jinja_template_functions = {
     "is_test_success": is_test_success,
 }
 
@@ -458,21 +465,52 @@
             ALL_STEP_REPORT[class_name]["time_result"]["End Time"] = stop_time
             ALL_STEP_REPORT[class_name]["time_result"]["Elapsed Time"] = round(
                 elapsed_time, 2
             )
             if test_case in test_result.errors:
                 ALL_STEP_REPORT[class_name]["test_list"][test_method_name][
                     "unexpected_errors"
-                ].append(test_case[1])
-
+                ][-1].append(test_case[1])
                 ALL_STEP_REPORT[class_name]["succeed"] = False
+
     # Render the source template
-    render_environment = jinja2.Environment(loader=jinja2.FileSystemLoader(SCRIPT_PATH))
+    render_environment = jinja2.Environment(
+        loader=jinja2.FileSystemLoader(SCRIPT_PATH), autoescape=True
+    )
     template = render_environment.get_template(REPORT_TEMPLATE)
     template.globals.update(jinja_template_functions)
     output_text = template.render({"ALL_STEP_REPORT": ALL_STEP_REPORT})
 
     output_file = Path(output_file).resolve()
     output_file.parent.mkdir(parents=True, exist_ok=True)
     # Write the output into the output file
     with output_file.open("w") as report_file:
         report_file.write(output_text)
+
+
+def add_retry_information(
+    test: BasicTest, result_test: bool, retry_nb: int, max_try: int, exc: Exception
+) -> None:
+    """Add information in the step report if a test fails and is retried.
+
+    :param test: test failed
+    :param result_test: result of the tests of the class before the retry
+    :param retry_nb: number of the current try
+    :param max_try: maximum tries that will be done
+    :param exc: exception caught
+    """
+    global ALL_STEP_REPORT
+    test_class_name = type(test).__name__
+    test_information = ALL_STEP_REPORT[test_class_name]["test_list"][
+        test._testMethodName
+    ]
+    # Add information about the number of try
+    test_information["number_try"] = retry_nb + 1
+    test_information["max_try"] = max_try
+    # Add another list to steps to differentiate the try
+    test_information["steps"].append([])
+    # We add the error raised if it was not an assertion error
+    if not isinstance(exc, AssertionError):
+        test_information["unexpected_errors"][-1].append(traceback.format_exc())
+    test_information["unexpected_errors"].append([])
+    # Go back to the state before executing the test
+    ALL_STEP_REPORT[test_class_name]["succeed"] = result_test
```

### Comparing `pykiso-0.22.2/src/pykiso/test_result/multi_result.py` & `pykiso-0.23.0/src/pykiso/test_result/multi_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_result/templates/report_template.css` & `pykiso-0.23.0/src/pykiso/test_result/templates/report_template.css`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_result/templates/report_template.html.j2` & `pykiso-0.23.0/src/pykiso/test_result/templates/report_template.html.j2`

 * *Files 18% similar despite different names*

```diff
@@ -35,74 +35,103 @@
                 {%- endfor %}
             {%- endfor %}
             </p>
             {#- For each test (setUp, run, tearDown) -#}
             {% for test_name, test_content in class_content["test_list"].items() %}
                 {% set test_success = is_test_success(test_content) -%}
                 <details {% if not test_success %}open class="failed-test-details"{% endif %}><summary><h3>{{test_name}}
-                {% if test_success -%}<span style="color:green;">Success</span>
-                {% else %}<span style="color:red;">Fail</span>
-                {%- endif %}</h3></summary>
+                {% if test_success -%}
+                    <span style="color:green;">Success
+                    {% if test_content.get("number_try") -%}
+                        (attempt: {{test_content.get("number_try")}}/{{test_content.get("max_try")}})
+                    {%- endif %}
+                    </span>
+                {% else %}
+                    <span style="color:red;">Fail
+                    {% if test_content.get("number_try") -%}
+                        ({{test_content.get("number_try")}} attempts made)
+                    {%- endif %}
+                    </span>
+                {%- endif %}
+                </h3></summary>
                 <p>{{test_content["description"] | replace("\n", "<br/>\n") }}</p>
-                <table>
-                    <thead>
-                        <tr>
-                            {# Set Columns name from the first row, excluding succeed flag -#}
-                            <th scope="col" style="width: 3%">Step</th>
-                            {% for column_name in test_content["steps"][0].keys() if column_name != "succeed" -%}
-                                <th scope="col">{{column_name}}</th>
-                            {%- endfor %}
-                        </tr>
-                    </thead>
-                    <tbody>
-                        {#- Loop over each assert method called (step-report) -#}
-                        {% for row in test_content["steps"] -%}
-                            {# Set cell color variable according to the assert result and emptiness -#}
-                            {% if row.pop("succeed") -%}
-                                {% set color_cell = "background-color: rgb(196, 243, 196);" -%}
-                                {% set color_empty_cell = "background-color: rgb(250, 250, 128);" -%}
-                            {% else -%}
-                                {% set color_cell = "background-color: rgb(236, 160, 160);" -%}
-                                {% set color_empty_cell = "background-color: rgb(236, 160, 160);" -%}
-                            {%- endif %}
-                            {# Needed for setting unique class per row in html in inner loop -#}
-                            {% set row_index = loop.index -%}
+                {# Loop over the number of try of a test -#}
+                {% for index in range(test_content["steps"] |length) -%}
+                    {# Check if we are in a case of a retry -#}
+                    {% if test_content["steps"] | length >1 and index == 0 -%}
+                       <details><summary><b>Attempt details</b></summary>
+                    {%- endif %}
+                    {% if test_content["steps"] | length >1 -%}
+                        <b>Attempt {{index+1}} :</b>
+                        <br>
+                    {%- endif %}
+                    <table>
+                        <thead>
                             <tr>
-                                <th scope="row" style="{{color_cell}}" >{{loop.index}}</th>
-                                {#- Loop over each cell of the row -#}
-                                {% for col_value in row.values() -%}
-                                    {#- Set the value and apply colors to the cell #}
-                                    <td {% if (col_value or col_value == False) %} style="{{color_cell}}" {% else %} style="{{color_empty_cell}}" {% endif %}>
-                                        {# Use a <details> if content is too long for better results overview and synchronize toggling them per row -#}
-                                        {% if col_value | string | length > 100 -%}
-                                        <details class="{{class_name}}{{test_name}}row_{{row_index}}" ontoggle="toggleDetailsInRow(this, '{{class_name}}{{test_name}}row_{{row_index}}')">
-                                            <summary>{{col_value | string | truncate(53, true, leeway = 0)}}</summary>
-                                            <br>
+                                {% if test_content["steps"][index] | length >0 -%}
+                                    {# Set Columns name from the first row, excluding succeed flag -#}
+                                    <th scope="col" style="width: 3%">Step</th>
+                                    {% for column_name in test_content["steps"][index][0].keys() if column_name != "succeed" -%}
+                                        <th scope="col">{{column_name}}</th>
+                                    {%- endfor %}
+                                {%- endif %}
+                            </tr>
+                        </thead>
+                        <tbody>
+                            {#- Loop over each assert method called (step-report) -#}
+                            {% for row in test_content["steps"][index] -%}
+                                {# Set cell color variable according to the assert result and emptiness -#}
+                                {% if row.pop("succeed") == true -%}
+                                    {% set color_cell = "background-color: rgb(196, 243, 196);" -%}
+                                    {% set color_empty_cell = "background-color: rgb(250, 250, 128);" -%}
+                                {% else -%}
+                                    {% set color_cell = "background-color: rgb(236, 160, 160);" -%}
+                                    {% set color_empty_cell = "background-color: rgb(236, 160, 160);" -%}
+                                {%- endif %}
+                                {# Needed for setting unique class per row in html in inner loop -#}
+                                {% set row_index = loop.index -%}
+                                <tr>
+                                    <th scope="row" style="{{color_cell}}" >{{loop.index}}</th>
+                                    {#- Loop over each cell of the row -#}
+                                    {% for col_value in row.values() -%}
+                                        {#- Set the value and apply colors to the cell #}
+                                        <td {% if (col_value or col_value == False) %} style="{{color_cell}}" {% else %} style="{{color_empty_cell}}" {% endif %}>
+                                            {# Use a <details> if content is too long for better results overview and synchronize toggling them per row -#}
+                                            {% if col_value | string | length > 100 -%}
+                                            <details class="{{class_name}}{{test_name}}row_{{row_index}}" ontoggle="toggleDetailsInRow(this, '{{class_name}}{{test_name}}row_{{row_index}}')">
+                                                <summary>{{col_value | string | truncate(53, true, leeway = 0)}}</summary>
+                                                <br>
+                                                <div>
+                                                    {{col_value}}
+                                                </div>
+                                            </details>
+                                            {%- else -%}
                                             <div>
                                                 {{col_value}}
                                             </div>
-                                        </details>
-                                        {%- else -%}
-                                        <div>
-                                            {{col_value}}
-                                        </div>
-                                        {%- endif %}
-                                    </td>
-                                {%- endfor %}
-                            </tr>
-                        {%- endfor %}
-                    </tbody>
-                </table>
-                {% if test_content.get("unexpected_errors") -%}
+                                            {%- endif %}
+                                        </td>
+                                    {%- endfor %}
+                                </tr>
+                            {%- endfor %}
+
+                        </tbody>
+                    </table>
+                    {% if test_content["unexpected_errors"][index] -%}
                     <b style='color:red;'><strong>Unexpected errors happened :</strong> <br></b>
-                        {% for error in test_content.get("unexpected_errors") -%}
+                        {% for error in test_content.get("unexpected_errors")[index] -%}
                             <pre>{{error}}</pre>
                         {%- endfor %}
 
-                {%- endif %}
+                    {%- endif %}
+                    {% if (test_content["steps"] | length >1 and (index+2 == (test_content["steps"] | length))) -%}
+                            </details>
+                    {%- endif %}
+                {%- endfor %}
+
                 </details>
             {%- endfor %}
 
         </details>
     {%- endfor %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -14,18 +14,29 @@
 {# Add additional information from header key -#} {% for data in [class_content
 ["time_result"], class_content["header"]] -%} {% for key, value in data.items()
 -%} {{key}}: {{value}} {%- endfor %} {%- endfor %}
 {#- For each test (setUp, run, tearDown) -#} {% for test_name, test_content in
 class_content["test_list"].items() %} {% set test_success = is_test_success
 (test_content) -%}
 % if not test_success %}open class="failed-test-details"{% endif %}>
-**** {{test_name}} {% if test_success -%}Success {% else %}Fail {%- endif %}
-****
+**** {{test_name}} {% if test_success -%} Success {% if test_content.get
+("number_try") -%} (attempt: {{test_content.get("number_try")}}/{
+{test_content.get("max_try")}}) {%- endif %}  {% else %} Fail {% if
+test_content.get("number_try") -%} ({{test_content.get("number_try")}} attempts
+made) {%- endif %}  {%- endif %} ****
 {{test_content["description"] | replace("\n", "
 \n") }}
+{# Loop over the number of try of a test -#} {% for index in range(test_content
+["steps"] |length) -%} {# Check if we are in a case of a retry -#} {% if
+test_content["steps"] | length >1 and index == 0 -%} Attempt details {%- endif
+%} {% if test_content["steps"] | length >1 -%} Attempt {{index+1}} :
+{%- endif %}
 Step           {{column_name}}
 {{loop.index}}
-{% if test_content.get("unexpected_errors") -%} Unexpected errors happened :
- {% for error in test_content.get("unexpected_errors") -%}
+{% if test_content["unexpected_errors"][index] -%} Unexpected errors happened :
+
+ {% for error in test_content.get("unexpected_errors")[index] -%}
 {{error}}
-{%- endfor %} {%- endif %}  {%- endfor %}  {%- endfor %}
+{%- endfor %} {%- endif %} {% if (test_content["steps"] | length >1 and
+(index+2 == (test_content["steps"] | length))) -%}  {%- endif %} {%- endfor %}
+{%- endfor %}  {%- endfor %}
```

### Comparing `pykiso-0.22.2/src/pykiso/test_result/templates/report_template_script.js` & `pykiso-0.23.0/src/pykiso/test_result/templates/report_template_script.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,16 @@
     element.scrollIntoView();
     const isOpen = element.hasAttribute("open");
     const detailsElements = document.getElementsByClassName(className);
     for (details of detailsElements) {
         details.open = isOpen;
         isOpen ? setSummary("Click to minimize", details) : setTruncatedSummary(details);
     }
-}
+} // no-unused-vars function is used (false positive),eslint-disable-line
+
 
 document.addEventListener("DOMContentLoaded", function() {
     var failButton = document.getElementById("failButton");
     failButton.addEventListener("click", function() {
         var failedDetailElements = document.querySelectorAll(".failed-test-details");
         failedDetailElements.forEach(function(details) {
             toggleFailDetails(details);
```

### Comparing `pykiso-0.22.2/src/pykiso/test_result/text_result.py` & `pykiso-0.23.0/src/pykiso/test_result/text_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_result/xml_result.py` & `pykiso-0.23.0/src/pykiso/test_result/xml_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_setup/config_registry.py` & `pykiso-0.23.0/src/pykiso/test_setup/config_registry.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/test_setup/dynamic_loader.py` & `pykiso-0.23.0/src/pykiso/test_setup/dynamic_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,18 +228,18 @@
         )
         inst = self.modules[name](name=name, **self.configs[name])
         self.instances[name] = inst
         log.internal_debug(f"instantiated {name}")
         return inst
 
     def delete_all_instances(self) -> None:
-        """Call custom del method if it exists"""
+        """Call shutdown method if it exists"""
         for instance in self.instances.values():
-            if callable(getattr(instance, "__del__", None)):
-                instance.__del__()
+            if callable(getattr(instance, "shutdown", None)):
+                instance.shutdown()
 
 
 class AuxiliaryCache(ModuleCache):
     """A ModuleCache that specifically provides Auxiliaries.
 
     This has the additional functionality that if an auxiliary has any defined connectors,
     these will be provided automatically.
```

### Comparing `pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/cli.py` & `pykiso-0.23.0/src/pykiso/tool/pykiso_to_pytest/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,17 @@
 
     :param filename: pykiso yaml file to convert
     :param destination: destination file path
     """
     pykiso_config = config_parser.parse_config(filename)
 
     template_loader = FileSystemLoader(searchpath=str(ROOT_PATH / "templates"))
-    template_env = Environment(loader=template_loader)
+    # The issue B701 wants autoescape to be set to true in order to filter input strings to escape any HTML content submitted via template variables.
+    # Autoescape needs to be switched off, since executable python code is included which falsely triggers the issue.
+    template_env = Environment(loader=template_loader, autoescape=False)  # nosec B701
     template_env.filters["format_value"] = format_value
     template = template_env.get_template("conftest_template.jinja2")
 
     # Grab import information -> Channels and Auxiliaries
     yaml_config_folder = pathlib.Path(filename).resolve().parent
 
     import_info = set()
```

### Comparing `pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2` & `pykiso-0.23.0/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/tool/show_tag.py` & `pykiso-0.23.0/src/pykiso/tool/show_tag.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/tool/testrail/api.py` & `pykiso-0.23.0/src/pykiso/tool/testrail/api.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/tool/testrail/cli.py` & `pykiso-0.23.0/src/pykiso/tool/testrail/cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/tool/testrail/console.py` & `pykiso-0.23.0/src/pykiso/tool/testrail/console.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/tool/testrail/containers.py` & `pykiso-0.23.0/src/pykiso/tool/testrail/containers.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/tool/testrail/extraction.py` & `pykiso-0.23.0/src/pykiso/tool/testrail/extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 .. currentmodule:: extraction
 """
 
 import enum
 import json
 import xml
 from pathlib import Path
-from typing import List, Optional
-from xml.etree import ElementTree as etree
+from typing import List
+
+from defusedxml import ElementTree as etree
 
 
 class Status(enum.IntEnum):
     """All possible status on TestRail."""
 
     PASSED = 1
     TEST_EXECUTION_BLOCKED = 2
```

### Comparing `pykiso-0.22.2/src/pykiso/tool/testrail/testrail.py` & `pykiso-0.23.0/src/pykiso/tool/testrail/testrail.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/src/pykiso/types.py` & `pykiso-0.23.0/src/pykiso/types.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.2/setup.py` & `pykiso-0.23.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 install_requires = \
 ['Jinja2>=2.11.0,<4.0.0',
  'MarkupSafe>=2.0.1,<2.1.0',
  'PyYAML>=6.0,<7.0',
  'brainstem',
  'click>=7.0.0,<9.0.0',
+ 'defusedxml>=0.7.1,<0.8.0',
  'hidapi>=0.12.0.post2,<0.13.0',
  'robotframework==3.2.2',
  'tabulate>=0.8.9,<0.10.0',
  'unittest-xml-reporting>=3.2.0,<4.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.12,<6.0'],
@@ -74,17 +75,17 @@
                      'pykiso-tags = pykiso.tool.show_tag:main',
                      'pykitest = pykiso.tool.pykiso_to_pytest.cli:main',
                      'testrail = pykiso.tool.testrail.cli:cli_testrail'],
  'pytest11': ['pytest_kiso = pykiso.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'pykiso',
-    'version': '0.22.2',
+    'version': '0.23.0',
     'description': 'Embedded integration testing framework.',
-    'long_description': '[![License](https://img.shields.io/badge/Licence-Eclipse%20Public%20License%202.0-lightgrey)](https://opensource.org/licenses/EPL-2.0)\n[![Platforms](https://img.shields.io/badge/Platforms-win64%20linux64%20osx64-lightgrey)]()\n[![Supported python version](https://img.shields.io/pypi/pyversions/pykiso)]()\n[![Build status](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![Documentation Status](https://readthedocs.org/projects/kiso-testing/badge/?version=latest)](https://kiso-testing.readthedocs.io/en/latest/?badge=latest)\n[![Test results](https://img.shields.io/jenkins/tests?compact_message&failed_label=failed&jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F&passed_label=passed&skipped_label=skipped)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![codecov](https://codecov.io/gh/eclipse/kiso-testing/branch/master/graph/badge.svg?token=IBKQ700ABS)](https://codecov.io/gh/eclipse/kiso-testing)\n[![CodeFactor](https://www.codefactor.io/repository/github/eclipse/kiso-testing/badge)](https://www.codefactor.io/repository/github/eclipse/kiso-testing)\n[![Last commit](https://img.shields.io/github/last-commit/eclipse/kiso-testing)]()\n[![Commits since latest version](https://img.shields.io/github/commits-since/eclipse/kiso-testing/latest/master)]()\n\n# PyKiso\n\n![Optional Text](./docs/images/pykiso_logo.png)\n\n## Introduction ##\n\n**pykiso** is an integration test framework. With it, it is possible to write\n* Whitebox integration tests directly on my target device\n* Graybox integration tests to make sure the communication-link with my target device is working as expected\n* Blackbox integration tests to make sure my external device interfaces are working as expected\n\nThe project will contain:\n* The core python framework (this repository)\n* Framework plugins that are generic enough to be integrated as "native" (this repository)\n* Additional "testApps" for different targets platforms (e.g. stm32, ...) or languages (C, C++, ...) . It could be pure SW or also HW (other repositories)\n\n## Link to Eclipse Project\nhttps://projects.eclipse.org/projects/iot.kiso-testing\n\n## Requirements ##\n\n* Python 3.7+\n* pip/poetry (used to get the rest of the requirements)\n\n## Install ##\n\n```bash\npip install pykiso # Core framework\npip install pykiso[plugins] # For installing all plugins\npip install pykiso[all] # For installing all what we have to offer\n```\n\n[Poetry](https://python-poetry.org/) is more appropriate for developers as it automatically creates virtual environments.\n\n```bash\ncd kiso-testing\npoetry install --all-extras\npoetry shell\n```\n\n### Pre-Commit\n\nTo improve code-quality, a configuration of [pre-commit](https://pre-commit.com/) hooks are available.\nThe following pre-commit hooks are used:\n\n- black\n- flake8\n- isort\n- trailing-whitespace\n- end-of-file-fixer\n- check-docstring-first\n- check-json\n- check-added-large-files\n- check-yaml\n- debug-statements\n\nIf you don\'t have pre-commit installed, you can get it using pip:\n\n```bash\npip install pre-commit\n```\n\nStart using the hooks with\n\n```bash\npre-commit install\n```\n\n## Commit message convention\n\nCommits are sorted into multiple categories based on keywords that can occur at any position as part of the commit message.\n[Category] Keywords\n* [BREAKING CHANGES] BREAKING CHANGE\n* [Features] feat:\n* [Fixes] fix:\n* [Docs] docs:\n* [Styles] style:\n* [Refactors] refactor!:\n* [Performances] perf:\n* [Tests] test:\n* [Build] build:\n* [Ci] ci:\nEach commit is considered only once according to the order of the categories listed above. Merge commits are ignored.\n\nThe tool commitizen can help you to create commits which follows these standards.\n```bash\n# if not yet installed:\npip install -U commitizen==2.20.4\n# helps you to create a commit:\ncz commit\n# or use equivalent short variant:\ncz c\n```\n\n## Generate Changelog\n\nAfter you installed the dev dependencies from the pipfile you are able to\nautogenerate the Changelog.\n\n```bash\ninvoke changelog\n```\n\n## Usage ##\n\nOnce installed the application is bound to `pykiso`, it can be called with the following arguments:\n\n```bash\nUsage: pykiso [OPTIONS]\n\n  Embedded Integration Test Framework - CLI Entry Point.\n\n  TAG Filters: any additional option to be passed to the test as tag through\n  the pykiso call. Multiple values must be separated with a comma.\n\n  For example: pykiso -c your_config.yaml --branch-level dev,master --variant\n  delta\n\nOptions:\n  -c, --test-configuration-file FILE\n                                  path to the test configuration file (in YAML\n                                  format)  [required]\n  -l, --log-path PATH             path to log-file or folder. If not set will\n                                  log to STDOUT\n  --log-level [DEBUG|INFO|WARNING|ERROR]\n                                  set the verbosity of the logging\n  --junit                         enables the generation of a junit report\n  --text                          default, test results are only displayed in\n                                  the console\n  --step-report PATH              generate the step report at the specified\n                                  path\n  --failfast                      stop the test run on the first error or\n                                  failure\n  -v, --verbose                   activate the internal framework logs\n  -p, --pattern TEXT              test filter pattern, e.g. \'test_suite_1.py\'\n                                  or \'test_*.py\'. Or even more granularly\n                                  \'test_suite_1.py::test_class::test_name\'\n  --version                       Show the version and exit.\n  -h, --help                      Show this message and exit.\n```\n\nSuitable config files are available in the `examples` folder.\n\n### Demo using example config ##\n\n```bash\ninvoke run\n```\n\n### Running the Tests ##\n\n```bash\ninvoke test\n```\n\nor\n\n```bash\npytest\n```\n',
+    'long_description': '[![License](https://img.shields.io/badge/Licence-Eclipse%20Public%20License%202.0-lightgrey)](https://opensource.org/licenses/EPL-2.0)\n[![Platforms](https://img.shields.io/badge/Platforms-win64%20linux64%20osx64-lightgrey)]()\n[![Supported python version](https://img.shields.io/pypi/pyversions/pykiso)]()\n[![Build status](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![Documentation Status](https://readthedocs.org/projects/kiso-testing/badge/?version=latest)](https://kiso-testing.readthedocs.io/en/latest/?badge=latest)\n[![Test results](https://img.shields.io/jenkins/tests?compact_message&failed_label=failed&jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F&passed_label=passed&skipped_label=skipped)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![codecov](https://codecov.io/gh/eclipse/kiso-testing/branch/master/graph/badge.svg?token=IBKQ700ABS)](https://codecov.io/gh/eclipse/kiso-testing)\n[![CodeFactor](https://www.codefactor.io/repository/github/eclipse/kiso-testing/badge)](https://www.codefactor.io/repository/github/eclipse/kiso-testing)\n[![Last commit](https://img.shields.io/github/last-commit/eclipse/kiso-testing)]()\n[![Commits since latest version](https://img.shields.io/github/commits-since/eclipse/kiso-testing/latest/master)]()\n\n# PyKiso\n\n![Optional Text](./docs/images/pykiso_logo.png)\n\n## Introduction ##\n\n**pykiso** is an integration test framework. With it, it is possible to write\n* Whitebox integration tests directly on my target device\n* Graybox integration tests to make sure the communication-link with my target device is working as expected\n* Blackbox integration tests to make sure my external device interfaces are working as expected\n\nThe project will contain:\n* The core python framework (this repository)\n* Framework plugins that are generic enough to be integrated as "native" (this repository)\n* Additional "testApps" for different targets platforms (e.g. stm32, ...) or languages (C, C++, ...) . It could be pure SW or also HW (other repositories)\n\n## Link to Eclipse Project\nhttps://projects.eclipse.org/projects/iot.kiso-testing\n\n## Requirements ##\n\n* Python 3.7+\n* pip/poetry (used to get the rest of the requirements)\n\n## Install ##\n\n```bash\npip install pykiso # Core framework\npip install pykiso[plugins] # For installing all plugins\npip install pykiso[all] # For installing all what we have to offer\n```\n\n[Poetry](https://python-poetry.org/) is more appropriate for developers as it automatically creates virtual environments.\n\n```bash\ncd kiso-testing\npoetry install --all-extras\npoetry shell\n```\n\n### Pre-Commit\n\nTo improve code-quality, a configuration of [pre-commit](https://pre-commit.com/) hooks are available.\nThe following pre-commit hooks are used:\n\n- black\n- flake8\n- isort\n- trailing-whitespace\n- end-of-file-fixer\n- check-docstring-first\n- check-json\n- check-added-large-files\n- check-yaml\n- debug-statements\n\nIf you don\'t have pre-commit installed, you can get it using pip:\n\n```bash\npip install pre-commit\n```\n\nStart using the hooks with\n\n```bash\npre-commit install\n```\n\n## Commit message convention\n\nCommits are sorted into multiple categories based on keywords that can occur at any position as part of the commit message.\n[Category] Keywords\n* [BREAKING CHANGES] BREAKING CHANGE\n* [Features] feat:\n* [Fixes] fix:\n* [Docs] docs:\n* [Styles] style:\n* [Refactors] refactor!:\n* [Performances] perf:\n* [Tests] test:\n* [Build] build:\n* [Ci] ci:\nEach commit is considered only once according to the order of the categories listed above. Merge commits are ignored.\n\nThe tool commitizen can help you to create commits which follows these standards.\n```bash\n# if not yet installed:\npip install -U commitizen==2.20.4\n# helps you to create a commit:\ncz commit\n# or use equivalent short variant:\ncz c\n```\n\n## Generate Changelog\n\nAfter you installed the dev dependencies from the pipfile you are able to\nautogenerate the Changelog.\n\n```bash\ninvoke changelog\n```\n\n## Usage ##\n\nOnce installed the application is bound to `pykiso`, it can be called with the following arguments:\n\n```bash\nUsage: pykiso [OPTIONS]\n\n  Embedded Integration Test Framework - CLI Entry Point.\n\n  TAG Filters: any additional option to be passed to the test as tag through\n  the pykiso call. Multiple values must be separated with a comma.\n\n  For example: pykiso -c your_config.yaml --branch-level dev,master --variant\n  delta\n\nOptions:\n  -c, --test-configuration-file FILE\n                                  path to the test configuration file (in YAML\n                                  format)  [required]\n  -l, --log-path PATH             path to log-file or folder. If not set will\n                                  log to STDOUT\n  --log-level [DEBUG|INFO|WARNING|ERROR]\n                                  set the verbosity of the logging\n  --junit                         enables the generation of a junit report\n  --text                          default, test results are only displayed in\n                                  the console\n  --step-report PATH              generate the step report at the specified\n                                  path\n  --failfast                      stop the test run on the first error or\n                                  failure\n  -v, --verbose                   activate the internal framework logs\n  -p, --pattern TEXT              test filter pattern, e.g. \'test_suite_1.py\'\n                                  or \'test_*.py\'. Or even more granularly\n                                  \'test_suite_1.py::test_class::test_name\'\n  --version                       Show the version and exit.\n  -h, --help                      Show this message and exit.\n  --logger                        Change the logger class used in pykiso, value\n                                  is the import path to the logger class, example\n                                  \'logging.Logger\'\n```\n\nSuitable config files are available in the `examples` folder.\n\n### Demo using example config ##\n\n```bash\ninvoke run\n```\n\n### Running the Tests ##\n\n```bash\ninvoke test\n```\n\nor\n\n```bash\npytest\n```\n',
     'author': 'Sebastian Fischer',
     'author_email': 'sebastian.fischer@de.bosch.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/pykiso/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pykiso-0.22.2/PKG-INFO` & `pykiso-0.23.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykiso
-Version: 0.22.2
+Version: 0.23.0
 Summary: Embedded integration testing framework.
 Home-page: https://pypi.org/project/pykiso/
 License: Eclipse Public License - v 2.0
 Keywords: testing,integration testing,framework,testing framework
 Author: Sebastian Fischer
 Author-email: sebastian.fischer@de.bosch.com
 Requires-Python: >=3.7,<4.0
@@ -41,14 +41,15 @@
 Requires-Dist: MarkupSafe (>=2.0.1,<2.1.0)
 Requires-Dist: PyVISA (>=1.12.0,<2.0.0) ; extra == "plugins" or extra == "instrument" or extra == "all"
 Requires-Dist: PyVISA-py (>=0.5.3,<0.6.0) ; extra == "plugins" or extra == "instrument" or extra == "all"
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: black (==22.10.0) ; extra == "pykitest" or extra == "all"
 Requires-Dist: brainstem
 Requires-Dist: click (>=7.0.0,<9.0.0)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: hidapi (>=0.12.0.post2,<0.13.0)
 Requires-Dist: importlib-metadata (>=4.12,<6.0) ; python_version < "3.8"
 Requires-Dist: isort (>=5.11.4) ; extra == "pykitest" or extra == "all"
 Requires-Dist: pykiso-python-uds (>=3.0.2,<3.1.0) ; extra == "plugins" or extra == "can" or extra == "all"
 Requires-Dist: pylink-square (>=0.12,<0.15) ; extra == "plugins" or extra == "debugger" or extra == "all"
 Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) ; python_version >= "3.5" and python_version < "4.0"
 Requires-Dist: pyserial (>=3.0,<4.0) ; extra == "plugins" or extra == "serial" or extra == "all"
@@ -208,14 +209,17 @@
                                   failure
   -v, --verbose                   activate the internal framework logs
   -p, --pattern TEXT              test filter pattern, e.g. 'test_suite_1.py'
                                   or 'test_*.py'. Or even more granularly
                                   'test_suite_1.py::test_class::test_name'
   --version                       Show the version and exit.
   -h, --help                      Show this message and exit.
+  --logger                        Change the logger class used in pykiso, value
+                                  is the import path to the logger class, example
+                                  'logging.Logger'
 ```
 
 Suitable config files are available in the `examples` folder.
 
 ### Demo using example config ##
 
 ```bash
```

