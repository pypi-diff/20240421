# Comparing `tmp/onnxscript-0.1.0.dev20240419.tar.gz` & `tmp/onnxscript-0.1.0.dev20240420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240419.tar", last modified: Fri Apr 19 00:01:34 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240420.tar", last modified: Sat Apr 20 00:02:18 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240419.tar` & `onnxscript-0.1.0.dev20240420.tar`

### file list

```diff
@@ -1,214 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.524758 onnxscript-0.1.0.dev20240419/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-19 00:01:34.524758 onnxscript-0.1.0.dev20240419/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.488758 onnxscript-0.1.0.dev20240419/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.492758 onnxscript-0.1.0.dev20240419/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.492758 onnxscript-0.1.0.dev20240419/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_legacy_ir/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6153 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_legacy_ir/protobuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.492758 onnxscript-0.1.0.dev20240419/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.492758 onnxscript-0.1.0.dev20240419/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.484758 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.496758 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.504758 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.484758 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.484758 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.504758 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.508758 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/_flags.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/graph_building.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.508758 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.512759 onnxscript-0.1.0.dev20240419/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2338 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    66691 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2525 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18800 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45188 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.512759 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.516759 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.520758 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.520758 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46294 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.520758 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.520758 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.520758 onnxscript-0.1.0.dev20240419/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.520758 onnxscript-0.1.0.dev20240419/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-19 00:01:34.524758 onnxscript-0.1.0.dev20240419/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-19 00:01:34.000000 onnxscript-0.1.0.dev20240419/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7995 2024-04-19 00:01:34.000000 onnxscript-0.1.0.dev20240419/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-19 00:01:34.000000 onnxscript-0.1.0.dev20240419/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-19 00:01:34.000000 onnxscript-0.1.0.dev20240419/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-19 00:01:34.000000 onnxscript-0.1.0.dev20240419/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-19 00:01:34.524758 onnxscript-0.1.0.dev20240419/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-19 00:01:04.000000 onnxscript-0.1.0.dev20240419/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.973299 onnxscript-0.1.0.dev20240420/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-20 00:02:18.969299 onnxscript-0.1.0.dev20240420/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.933298 onnxscript-0.1.0.dev20240420/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.937298 onnxscript-0.1.0.dev20240420/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.937298 onnxscript-0.1.0.dev20240420/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.937298 onnxscript-0.1.0.dev20240420/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.937298 onnxscript-0.1.0.dev20240420/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.925298 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.937298 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.949298 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.929298 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.929298 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.949298 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.949298 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.949298 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.953299 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.957299 onnxscript-0.1.0.dev20240420/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    73221 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19580 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46998 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.957299 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.961299 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.965299 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4316 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.969299 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1375 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2831 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6926 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2170 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8918 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36273 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.969299 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5746 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1922 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.969299 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1097 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42362 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.969299 onnxscript-0.1.0.dev20240420/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.969299 onnxscript-0.1.0.dev20240420/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 00:02:18.969299 onnxscript-0.1.0.dev20240420/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-20 00:02:18.000000 onnxscript-0.1.0.dev20240420/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8202 2024-04-20 00:02:18.000000 onnxscript-0.1.0.dev20240420/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-20 00:02:18.000000 onnxscript-0.1.0.dev20240420/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-20 00:02:18.000000 onnxscript-0.1.0.dev20240420/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-20 00:02:18.000000 onnxscript-0.1.0.dev20240420/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-20 00:02:18.973299 onnxscript-0.1.0.dev20240420/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-20 00:00:58.000000 onnxscript-0.1.0.dev20240420/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240419/LICENSE` & `onnxscript-0.1.0.dev20240420/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/PKG-INFO` & `onnxscript-0.1.0.dev20240420/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240419
+Version: 0.1.0.dev20240420
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240419/README.md` & `onnxscript-0.1.0.dev20240420/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_internal/runtime_typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """An internal wrapper for the beartype library.
 
 Decorate a function with `@runtime_typing.checked` to enable runtime
 type checking. The decorator is a no-op when the `beartype` library is not
 installed.
 """
 
+import typing
 import warnings
 
 __all__ = [
     "checked",
 ]
 
+T = typing.TypeVar("T", bound=typing.Callable[..., typing.Any])
+
 try:
     from beartype import beartype as checked
     from beartype import roar as _roar
 
     # Beartype warns when we import from typing because the types are deprecated
     # in Python 3.9. But there will be a long time until we can move to using
     # the native container types for type annotations (when 3.9 is the lowest
     # supported version). So we silence the warning.
     warnings.filterwarnings(
         "ignore",
         category=_roar.BeartypeDecorHintPep585DeprecationWarning,
     )
 except ImportError:
 
-    def checked(func):  # type: ignore[no-redef]
+    def checked(func: T) -> T:  # type: ignore[no-redef]
         return func
 
 except Exception as e:  # pylint: disable=broad-exception-caught
     # Warn errors that are not import errors (unexpected).
     warnings.warn(f"{e}", stacklevel=2)
 
-    def checked(func):  # type: ignore[no-redef]
+    def checked(func: T) -> T:  # type: ignore[no-redef]
         return func
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_legacy_ir/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -143,28 +143,28 @@
             return onnx.numpy_helper.to_array(self.value)
         return None
 
     def def_node(self) -> Node | None:
         return self.node
 
     def def_index(self) -> int:
-        return self.output_index
+        return self.output_index  # type: ignore[return-value]
 
     def is_same_as(self, other: StaticValueInfo) -> bool:
         """Returns true if this value represents the same IR object as the other value.
 
         This is *not* value-equality, but rather object-equality.
         """
         return self is other
 
     def __str__(self) -> str:
         shape = self.shape
         if shape is not None:
             shape = [str(dim) for dim in shape]
-            shape_str = f"[{', '.join(shape)}]"
+            shape_str = f"[{', '.join(shape)}]"  # type: ignore[arg-type]
         else:
             shape_str = "None"
         return (
             f"StaticValueInfo({self.name}, shape:{shape_str}, dtype:{self.element_type}, "
             f"{'has const value' if self.value is not unknown else 'no const value'}.)"
         )
 
@@ -232,16 +232,16 @@
     def output_names(self) -> list[str]:
         return [_.name for _ in self.original_graph_proto.output]
 
 
 class Function:
     def __init__(self, function_proto: onnx.FunctionProto):
         self.original_function_proto = function_proto
-        self.nodes = deque()
-        self.values = {}
+        self.nodes = deque()  # type: ignore[var-annotated]
+        self.values = {}  # type: ignore[var-annotated]
 
     @property
     def id(self) -> FunctionId:
         return (self.domain, self.name, self.overload)
 
     @property
     def domain(self) -> str:
@@ -289,16 +289,16 @@
         self.domain: str = node_proto.domain
         self.version: int | None = None
         self.op_type: str = node_proto.op_type
         if populate_io:
             self.inputs: list[Value | None] = [Value(i) for i in node_proto.input]
             self.outputs: list[Value | None] = [Value(i) for i in node_proto.output]
         else:
-            self.inputs: list[Value | None] = []
-            self.outputs: list[Value | None] = []
+            self.inputs: list[Value | None] = []  # type: ignore[no-redef]
+            self.outputs: list[Value | None] = []  # type: ignore[no-redef]
         # TODO: attributes are never populated.
         self.attributes: dict[str, int | float | RefAttr | Graph | list[Graph]] = {}
 
     def __repr__(self) -> str:
         return (
             f"{self.op_type}({','.join(self.original_node_proto.input)})"
             f"->{','.join(self.original_node_proto.output)}"
@@ -321,15 +321,15 @@
         return self.original_node_proto.attribute
 
     def set_version_if_custom_op(self, version_map: dict[str, int]) -> None:
         if self.domain != "" and self.domain in version_map:
             self.version = version_map[self.domain]
 
     def get_attribute(self, name: str) -> int | float | None:
-        return self.attributes.get(name, None)
+        return self.attributes.get(name, None)  # type: ignore[return-value]
 
     def __str__(self) -> str:
         return "\n".join(
             [
                 "Node",
                 f"OpType: {self.op_type}",
                 f"Inputs: {self.inputs}",
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_legacy_ir/visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             if len(splits) == 3:
                 overload = splits[2]
             function_id = (domain, function_name, overload)
         else:
             # Standard main graph value info format.
             function_id = None
             value_name = name
-        return function_id, ir.Value(value_name, type=value_info.type)
+        return function_id, ir.Value(name=value_name, type=value_info.type)
 
     def save_to_value_info(
         self, value: ir.Value, domain: str, function_name: str, overload: str
     ) -> onnx.ValueInfoProto | None:
         if overload != "":
             raise NotImplementedError("Overload is not supported yet.")
         function_id = f"{domain}::{function_name}"
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240420/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240420/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240420/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240420/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240420/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240420/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,7 +39,11 @@
     "TORCHLIB_EXPERIMENTAL_INITIALIZERS_AS_INPUTS",
     this_will="make initializers as inputs to the model graph",
 )
 EXPERIMENTAL_PREFER_TRACING: bool = _load_boolean_flag(
     "TORCHLIB_EXPERIMENTAL_PREFER_TRACING",
     this_will="trace all traceable functions to fold if branches and collapse constant expressions",
 )
+EXPERIMENTAL_USE_IR: bool = _load_boolean_flag(
+    "TORCHLIB_EXPERIMENTAL_USE_IR",
+    this_will="use the ONNX IR instead of the PyTorch Graph for graph building",
+)
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240420/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "AttrSparseTensor",
     "AttrSparseTensors",
     "AttrString",
     "AttrStrings",
     "AttrTensor",
     "AttrTensors",
     "AttrTypeProto",
-    "Dimension",
+    "SymbolicDim",
     "ExternalTensor",
     "Function",
     "Graph",
     "GraphView",
     "Input",
     "Model",
     "Node",
@@ -42,18 +42,19 @@
     "ArrayCompatible",
     "DLPackCompatible",
     "TensorProtocol",
     "ValueProtocol",
     "ModelProtocol",
     "NodeProtocol",
     "GraphProtocol",
+    "GraphViewProtocol",
     "AttributeProtocol",
     "ReferenceAttributeProtocol",
     "SparseTensorProtocol",
-    "DimensionProtocol",
+    "SymbolicDimProtocol",
     "ShapeProtocol",
     "TypeProtocol",
     "MapTypeProtocol",
     "FunctionProtocol",
     # Enums
     "AttributeType",
     "DataType",
@@ -73,46 +74,47 @@
     AttrSparseTensor,
     AttrSparseTensors,
     AttrString,
     AttrStrings,
     AttrTensor,
     AttrTensors,
     AttrTypeProto,
-    Dimension,
     ExternalTensor,
     Function,
     Graph,
     GraphView,
     Input,
     Model,
     Node,
     OptionalType,
     RefAttr,
     SequenceType,
     Shape,
     SparseTensorType,
+    SymbolicDim,
     Tensor,
     TensorType,
     Value,
 )
 from onnxscript.ir._enums import (
     AttributeType,
     DataType,
 )
 from onnxscript.ir._protocols import (
     ArrayCompatible,
     AttributeProtocol,
-    DimensionProtocol,
     DLPackCompatible,
     FunctionProtocol,
     GraphProtocol,
+    GraphViewProtocol,
     MapTypeProtocol,
     ModelProtocol,
     NodeProtocol,
     OperatorIdentifier,
     ReferenceAttributeProtocol,
     ShapeProtocol,
     SparseTensorProtocol,
+    SymbolicDimProtocol,
     TensorProtocol,
     TypeProtocol,
     ValueProtocol,
 )
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import mmap
 import os
 import sys
 import textwrap
 import typing
 from typing import (
     Any,
+    Collection,
     Generic,
     Iterable,
     Iterator,
     OrderedDict,
     Sequence,
     Union,
 )
@@ -100,15 +101,15 @@
 
     def display(self, *, page: bool | None = None) -> None:
         rich = _display.require_rich()
 
         if rich is None:
             status_manager = contextlib.nullcontext()
         else:
-            import rich.status  # pylint: disable=import-outside-toplevel
+            import rich.status  # type: ignore[import-not-found, no-redef]  # pylint: disable=import-outside-toplevel
 
             status_manager = rich.status.Status(f"Computing tensor stats for {self!r}")
 
         from onnxscript._thirdparty import (  # pylint: disable=import-outside-toplevel
             asciichartpy,
         )
 
@@ -144,51 +145,82 @@
             )
 
             text = "\n".join(lines)
 
         if rich is None:
             print(text)
         elif page:
-            import rich.console  # pylint: disable=import-outside-toplevel
+            import rich.console  # type: ignore[import-not-found, no-redef]  # pylint: disable=import-outside-toplevel
 
             console = rich.console.Console()
             with console.pager(styles=True):
                 console.print(text)
         else:
             rich.print(text)
 
 
 class Tensor(TensorBase, _protocols.TensorProtocol, Generic[TArrayCompatible]):
     """An immutable concrete value."""
 
-    __slots__ = ("_raw", "_dtype", "_shape", "name", "doc_string", "_metadata_props")
+    __slots__ = (
+        "_raw",
+        "_dtype",
+        "_shape",
+        "name",
+        "doc_string",
+        "_metadata_props",
+        "_metadata",
+    )
 
     def __init__(
         self,
         value: TArrayCompatible,
-        dtype: _enums.DataType,
+        dtype: _enums.DataType | None = None,
         *,
         shape: Shape | None = None,
         name: str = "",
         doc_string: str | None = None,
         metadata_props: dict[str, str] | None = None,
     ) -> None:
+        """Initialize a tensor.
+
+        Args:
+            value: The backing data of the tensor. It can be a numpy array or a DLPack compatible object.
+            dtype: The data type of the tensor. It can be None only when value is a numpy array.
+            shape: The shape of the tensor. If None, the shape is obtained from the value.
+            name: The name of the tensor.
+            doc_string: The documentation string.
+            metadata_props: The metadata properties.
+        """
         # NOTE: We should not do any copying here for performance reasons
         if not _compatible_with_numpy(value) and not _compatible_with_dlpack(value):
             raise TypeError(f"Expected an array compatible object, got {type(value)}")
-        if not hasattr(value, "shape") and shape is None:
-            raise ValueError(
-                f"Expected an object with a shape attribute, but {type(value)} does not have shape. "
-                "Please specify the shape explicitly."
-            )
+        if shape is None:
+            if not hasattr(value, "shape"):
+                raise ValueError(
+                    f"Expected an object with a shape attribute, but {type(value)} does not have shape. "
+                    "Please specify the shape explicitly."
+                )
+            self._shape = Shape(getattr(value, "shape"), frozen=True)  # noqa: B009
+        else:
+            self._shape = shape
+            self._shape._frozen = True
+        if dtype is None:
+            if isinstance(value, np.ndarray):
+                self._dtype = _enums.DataType.from_numpy(value.dtype)
+            else:
+                raise ValueError(
+                    "The dtype must be specified when the value is not a numpy array."
+                )
+        else:
+            self._dtype = dtype
         self._raw = value
-        self._dtype = dtype
-        self._shape = Shape(getattr(value, "shape"))  # noqa: B009
         self.name = name
         self.doc_string = doc_string
+        self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props = metadata_props
 
     def __array__(self, dtype: Any = None) -> np.ndarray:
         # TODO(justinchuby): Support numpy unsupported types
         if isinstance(self._raw, np.ndarray) or _compatible_with_numpy(self._raw):
             return self._raw.__array__(dtype)
         assert _compatible_with_dlpack(
@@ -197,14 +229,19 @@
         return np.from_dlpack(self._raw)
 
     def __dlpack__(self, *, stream: Any = None) -> Any:
         if _compatible_with_dlpack(self._raw):
             return self._raw.__dlpack__(stream=stream)
         return self.__array__().__dlpack__(stream=stream)
 
+    def __dlpack_device__(self) -> tuple[int, int]:
+        if _compatible_with_dlpack(self._raw):
+            return self._raw.__dlpack_device__()
+        return self.__array__().__dlpack_device__()
+
     def __repr__(self) -> str:
         return f"{self._repr_base()}({self._raw!r})"
 
     @property
     def dtype(self) -> _enums.DataType:
         """The data type of the tensor. Immutable."""
         return self._dtype
@@ -234,19 +271,31 @@
         """
         # TODO(justinchuby): Support DLPack
         array = self.numpy()
         if not IS_LITTLE_ENDIAN:
             return array.view(array.dtype.newbyteorder("<")).tobytes()
         return array.tobytes()
 
+    @property
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
             self._metadata_props = {}
         return self._metadata_props
 
+    @property
+    def meta(self) -> _metadata.MetadataStore:
+        """The metadata store for intermediate analysis.
+
+        Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
+        to the ONNX proto.
+        """
+        if self._metadata is None:
+            self._metadata = _metadata.MetadataStore()
+        return self._metadata
+
 
 class ExternalTensor(TensorBase, _protocols.TensorProtocol):
     """An immutable concrete tensor with its data store on disk.
 
     This class uses memory mapping to avoid loading the tensor into memory,
     when the data type is supported by numpy. Otherwise, the tensor is loaded
     into memory lazily when accessed.
@@ -278,14 +327,15 @@
         "_dtype",
         "_shape",
         "name",
         "doc_string",
         "_array",
         "raw",
         "_metadata_props",
+        "_metadata",
     )
 
     def __init__(
         self,
         path: os.PathLike | str,
         offset: int | None,
         length: int | None,
@@ -298,18 +348,20 @@
     ) -> None:
         self._path = path
         self._offset: int | None = offset
         self._length: int | None = length
         self._dtype: _enums.DataType = dtype
         self.name: str = name  # mutable
         self._shape: Shape = shape
+        self._shape._frozen = True
         self.doc_string: str | None = doc_string  # mutable
         self._array: np.ndarray | None = None
         self.raw: mmap.mmap | None = None
         self._metadata_props = metadata_props
+        self._metadata: _metadata.MetadataStore | None = None
 
     @property
     def path(self) -> str | os.PathLike:
         # Immutable
         return self._path
 
     @property
@@ -384,138 +436,167 @@
 
     @property
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
             self._metadata_props = {}
         return self._metadata_props
 
+    @property
+    def meta(self) -> _metadata.MetadataStore:
+        """The metadata store for intermediate analysis.
 
-class Dimension(_protocols.DimensionProtocol, _display.PrettyPrintable):
-    __slots__ = ("_value", "_denotation")
+        Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
+        to the ONNX proto.
+        """
+        if self._metadata is None:
+            self._metadata = _metadata.MetadataStore()
+        return self._metadata
 
-    def __init__(self, value: int | str | None, denotation: str | None = None) -> None:
-        self._value = value
-        self._denotation = denotation
 
-    def __int__(self) -> int:
-        if not isinstance(self.value, int):
-            raise TypeError(
-                f"The value of this Dimension is not int, but {type(self.value)} ({self.value})"
-            )
-        return self.value
+class SymbolicDim(_protocols.SymbolicDimProtocol, _display.PrettyPrintable):
+    __slots__ = ("_value",)
+
+    def __init__(self, value: str | None) -> None:
+        """Initialize a symbolic dimension.
 
-    def __index__(self) -> int:
-        return int(self)
+        Args:
+            value: The value of the dimension. It should not be an int.
+        """
+        if isinstance(value, int):
+            raise TypeError("The value of a SymbolicDim cannot be an int")
+        self._value = value
 
     def __eq__(self, other: object) -> bool:
-        if isinstance(other, (int, str)) or other is None:
+        if not isinstance(other, SymbolicDim):
             return self.value == other
-        if not isinstance(other, Dimension):
-            return False
         return self.value == other.value
 
-    def __ne__(self, value: object) -> bool:
-        return not self.__eq__(value)
-
-    def __lt__(self, other: object) -> bool:
-        if not isinstance(other, (int, Dimension)):
-            raise TypeError(f"Expected other to be Dimension or int, got {type(other)}")
-        return int(self) < int(other)
-
-    def __le__(self, other: object) -> bool:
-        if not isinstance(other, (int, Dimension)):
-            raise TypeError(f"Expected other to be Dimension or int, got {type(other)}")
-        return int(self) <= int(other)
-
-    def __gt__(self, other: object) -> bool:
-        if not isinstance(other, (int, Dimension)):
-            raise TypeError(f"Expected other to be Dimension or int, got {type(other)}")
-        return int(self) > int(other)
-
-    def __ge__(self, other: object) -> bool:
-        if not isinstance(other, (int, Dimension)):
-            raise TypeError(f"Expected other to be Dimension or int, got {type(other)}")
-        return int(self) >= int(other)
-
     def __hash__(self) -> int:
         return hash(self.value)
 
     @property
-    def value(self) -> int | str | None:
+    def value(self) -> str | None:
         return self._value
 
-    @property
-    def denotation(self) -> str | None:
-        return self._denotation
-
     def __str__(self) -> str:
         return f"{self._value}"
 
     def __repr__(self) -> str:
-        if self.denotation is not None:
-            denotation_text = f", denotation={self.denotation!r}"
-        else:
-            denotation_text = ""
-        return f"{self.__class__.__name__}({self._value}{denotation_text})"
+        return f"{self.__class__.__name__}({self._value})"
 
 
 class Shape(_protocols.ShapeProtocol, _display.PrettyPrintable):
-    __slots__ = ("_dims",)
+    __slots__ = ("_dims", "_frozen")
 
-    def __init__(self, dims: _protocols.SimpleShape | Sequence[Dimension]) -> None:
-        # TODO: Support symbolic shapes with expressions?
-        for dim in dims:
-            if dim is not None and not isinstance(dim, (int, str, Dimension)):
-                raise TypeError(f"Expected int, str, None or Dimension, got '{type(dim)}'")
-        self._dims: list[Dimension] = [
-            dim if isinstance(dim, Dimension) else Dimension(dim) for dim in dims
+    def __init__(
+        self,
+        dims: Iterable[int | SymbolicDim | str | None],
+        /,
+        denotations: Iterable[str | None] | None = None,
+        frozen: bool = False,
+    ) -> None:
+        """Initialize a shape.
+
+        Args:
+            dims: The dimensions of the shape. Each dimension can be an integer or a
+                SymbolicDim or any Python object. When a ``dim`` is not an integer or a
+                SymbolicDim, it is converted to a SymbolicDim.
+            denotations: The denotations of the dimensions. If None, the denotations are not set.
+                Standard denotation can optionally be used to denote tensor
+                dimensions with standard semantic descriptions to ensure
+                that operations are applied to the correct axis of a tensor.
+                Refer to https://github.com/onnx/onnx/blob/main/docs/DimensionDenotation.md#denotation-definition
+                for pre-defined dimension denotations.
+            frozen: If True, the shape is immutable and cannot be modified. This
+                is useful when the shape is initialized by a Tensor.
+        """
+        self._dims: list[int | SymbolicDim] = [
+            SymbolicDim(dim) if not isinstance(dim, (int, SymbolicDim)) else dim
+            for dim in dims
         ]
+        self._denotations: list[str | None] = (
+            list(denotations) if denotations is not None else [None] * len(self._dims)
+        )
+        if len(self._denotations) != len(self._dims):
+            raise ValueError(
+                "The number of denotations, when provided, must be equal to the number of dimensions."
+            )
+        self._frozen: bool = frozen
 
     @property
-    def dims(self) -> tuple[Dimension, ...]:
+    def dims(self) -> tuple[int | SymbolicDim, ...]:
         """All dimensions in the shape.
 
         This property is read-only. Use __getitem__ and __setitem__ to modify the shape or create a new shape.
         """
         return tuple(self._dims)
 
     def rank(self) -> int:
         """The rank of the shape."""
         return len(self._dims)
 
-    def simple(self) -> _protocols.SimpleShape:
-        return tuple(dim.value for dim in self._dims)
-
     def numpy(self) -> tuple[int, ...]:
-        if any(not isinstance(dim.value, int) for dim in self._dims):
+        if any(not isinstance(dim, int) for dim in self._dims):
             raise ValueError(f"Cannot convert the shape {self} to a tuple of ints")
-        return tuple(dim.value for dim in self._dims)  # type: ignore
+        return tuple(dim for dim in self._dims)  # type: ignore
 
     def __len__(self) -> int:
         return len(self._dims)
 
-    def __iter__(self) -> Iterator[Dimension]:
+    def __iter__(self) -> Iterator[int | SymbolicDim]:
         return iter(self._dims)
 
-    def __getitem__(self, index: int) -> Dimension:
-        return self._dims[index]
+    @typing.overload
+    def __getitem__(self, index: int) -> int | SymbolicDim: ...
 
-    def __setitem__(
-        self, index: int, value: _protocols.DimensionProtocol | int | str | None
-    ) -> None:
-        if isinstance(value, Dimension):
-            self._dims[index] = value
-            return
-        if isinstance(value, (int, str, type(None))):
-            self._dims[index] = Dimension(value)
-            return
+    @typing.overload
+    def __getitem__(self, index: slice) -> tuple[int | SymbolicDim, ...]: ...
 
-        raise TypeError(
-            f"Value must be int, str, None or DimensionProtocol. Got '{type(value)}'"
-        )
+    def __getitem__(self, index):
+        return tuple(self._dims)[index]
+
+    def __setitem__(self, index: int, value: int | SymbolicDim | str | None) -> None:
+        """Set the dimension at the index.
+
+        Args:
+            index: The index of the dimension.
+            value: The value of the dimension.
+
+        Raises:
+            TypeError: If the shape is frozen and cannot be modified.
+            TypeError: If the value is not an int or SymbolicDim.
+        """
+        if self._frozen:
+            raise TypeError("The shape is frozen and cannot be modified.")
+        if isinstance(value, str) or value is None:
+            value = SymbolicDim(value)
+        if not isinstance(value, (int, SymbolicDim)):
+            raise TypeError(f"Expected int, str, None or SymbolicDim, got '{type(value)}'")
+
+        self._dims[index] = value
+
+    def get_denotation(self, index: int) -> str | None:
+        """Return the denotation of the dimension at the index.
+
+        Args:
+            index: The index of the dimension.
+
+        Returns:
+            The denotation of the dimension.
+        """
+        return self._denotations[index]
+
+    def set_denotation(self, index: int, denotation: str | None) -> None:
+        """Set the denotation of the dimension at the index.
+
+        Args:
+            index: The index of the dimension.
+            denotation: The denotation of the dimension.
+        """
+        self._denotations[index] = denotation
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._dims!r})"
 
     def __str__(self) -> str:
         """Return a string representation of the shape.
 
@@ -528,15 +609,15 @@
 
         Two shapes are eqaul if all their dimensions are equal.
         """
         if isinstance(other, Shape):
             return self._dims == other._dims
         if not isinstance(other, Iterable):
             return False
-        return self.dims == tuple(other)
+        return self._dims == list(other)
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
 
 def _quoted(string: str) -> str:
     """Return a quoted string.
@@ -576,23 +657,24 @@
         "_graph",
     )
 
     def __init__(
         self,
         domain: str,
         op_type: str,
-        inputs: Sequence[Value | None],
-        attributes: Sequence[Attr | RefAttr] = (),
+        inputs: Iterable[Value | None],
+        attributes: Iterable[Attr | RefAttr] = (),
         *,
         overload: str = "",
         num_outputs: int = 1,
         version: int | None = None,
         graph: Graph | None = None,
         name: str | None = None,
         doc_string: str | None = None,
+        metadata_props: dict[str, str] | None = None,
     ):
         """Initialize a node and add it as a consumer of the input values.
 
         Args:
             domain: The domain of the operator. For onnx operators, this is an empty string.
             op_type: The name of the operator.
             inputs: The input values. When an input is None, it is an empty input.
@@ -600,34 +682,42 @@
             overload: The overload name when the node is invoking a function.
             num_outputs: The number of outputs of the node.
             version: The version of the operator. If None, the version is unspecified and will follow that of the graph.
             graph: The graph that the node belongs to. If None, the node is not added to any graph.
                 A `Node` must belong to zero or one graph.
             name: The name of the node. If None, the node is anonymous.
             doc_string: The documentation string.
+            metadata_props: The metadata properties.
         """
         self._name = name
         self._domain: str = domain
         self._op_type: str = op_type
         # NOTE: Make inputs immutable with the assumption that they are not mutated
         # very often. This way all mutations can be tracked.
         # If necessary, we can cache the inputs and outputs as tuples.
         self._inputs: tuple[Value | None, ...] = tuple(inputs)
         # Values belong to their defining nodes. The values list is immutable
         self._outputs: tuple[Value, ...] = tuple(
             Value(self, index=i) for i in range(num_outputs)
         )
+        attributes = tuple(attributes)
+        if attributes and not isinstance(attributes[0], (Attr, RefAttr)):
+            raise TypeError(
+                f"Expected the attributes to be Attr or RefAttr, got {type(attributes[0])}. "
+                "If you are copying the attributes from another node, make sure you call "
+                "node.attributes.values() because it is a dictionary."
+            )
         self._attributes: OrderedDict[str, Attr | RefAttr] = OrderedDict(
             (attr.name, attr) for attr in attributes
         )
         self._overload: str = overload
         # TODO(justinchuby): Potentially support a version range
         self._version: int | None = version
         self._metadata: _metadata.MetadataStore | None = None
-        self._metadata_props: dict[str, str] | None = None
+        self._metadata_props: dict[str, str] | None = metadata_props
         self._graph: Graph | None = graph
         self.doc_string = doc_string
 
         # Add the node as a consumer of the inputs
         for i, input_value in enumerate(self._inputs):
             if input_value is not None:
                 input_value._add_consumer(self, i)  # pylint: disable=protected-access
@@ -782,15 +872,19 @@
 
     @property
     def attributes(self) -> OrderedDict[str, Attr | RefAttr]:
         return self._attributes
 
     @property
     def meta(self) -> _metadata.MetadataStore:
-        """The metadata store for this node."""
+        """The metadata store for intermediate analysis.
+
+        Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
+        to the ONNX proto.
+        """
         if self._metadata is None:
             self._metadata = _metadata.MetadataStore()
         return self._metadata
 
     @property
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
@@ -966,15 +1060,16 @@
         self._shape: Shape | None = shape
         self._type: _protocols.TypeProtocol | None = type
         # TODO(justinchuby): Handle initialization when a const value is provided
         # We can get shape and type information from the const value
         self._const_value = const_value
         # Use a collection of (Node, int) to store consumers. This is needed
         # because a single consumer can use the same value multiple times.
-        self._consumers: set[tuple[Node, int]] = set()
+        # Use a dictionary to preserve insertion order so that the visiting order is deterministic
+        self._consumers: dict[tuple[Node, int], None] = {}
 
     def __repr__(self) -> str:
         value_name = self.name if self.name else "anonymous:" + str(id(self))
         producer = self.producer()
         producer_text = (
             producer.name or "anonymous_node:" + str(id(producer))
             if producer is not None
@@ -995,35 +1090,35 @@
         """The node that produces this value."""
         return self._producer
 
     def index(self) -> int | None:
         """The index of the output of the defining node."""
         return self._index
 
-    def consumers(self) -> frozenset[tuple[Node, int]]:
+    def consumers(self) -> Collection[tuple[Node, int]]:
         """Return a set of consumers of the value.
 
         The set contains tuples of ``(Node, index)`` where the index is the index of the input
         of the node. For example, if ``node.inputs[1] == value``, then the consumer is ``(node, 1)``.
         """
-        return frozenset(self._consumers)
+        return self._consumers.keys()
 
     def _add_consumer(self, consumer: Node, index: int) -> None:
         """Add a consumer node.
 
         This is an internal method. It should only be called by the Node class.
         """
-        self._consumers.add((consumer, index))
+        self._consumers[(consumer, index)] = None
 
     def _remove_consumer(self, consumer: Node, index: int) -> None:
         """Remove a node from the consumers of this value.
 
         This is an internal method. It should only be called by the Node class.
         """
-        self._consumers.remove((consumer, index))
+        self._consumers.pop((consumer, index))
 
     @property
     def name(self) -> str | None:
         return self._name
 
     @name.setter
     def name(self, value: str | None) -> None:
@@ -1064,22 +1159,22 @@
             self._type.dtype = value
 
     @property
     def shape(self) -> Shape | None:
         return self._shape
 
     @shape.setter
-    def shape(self, value: _protocols.SimpleShape | Shape | None) -> None:
+    def shape(self, value: Shape | None) -> None:
         if value is None:
             self._shape = None
             return
         if isinstance(value, Shape):
             self._shape = value
             return
-        self._shape = Shape(value)
+        raise TypeError(f"Expected value to be a Shape or None, got '{type(value)}'")
 
     @property
     def const_value(
         self,
     ) -> _protocols.TensorProtocol | Sequence[_protocols.TensorProtocol] | None:
         """A concrete value.
 
@@ -1110,20 +1205,21 @@
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
             self._metadata_props = {}
         return self._metadata_props
 
     def is_graph_output(self) -> bool:
         """Whether the value is an output of a graph."""
-        producer = self.producer()
-        if producer is None:
+        if (producer := self.producer()) is None:
             return False
-        if producer.graph is None:
+        if (graph := producer.graph) is None:
             return False
-        return self in producer.graph.outputs
+        # Cannot use `in` because __eq__ may be defined by subclasses, even though
+        # it is not recommended
+        return any(output is self for output in graph.outputs)
 
 
 class Input(Value):
     """Input of a Graph or a Function."""
 
     # Slots already defined in Value
     __slots__ = ()
@@ -1139,18 +1235,36 @@
         self._shape = shape
         self._type = type
 
 
 class Graph(_protocols.GraphProtocol, Sequence[Node], _display.PrettyPrintable):
     """IR Graph.
 
-    The graph can be used as a sequence of nodes::
+    Graph represents a computation graph. In addition to the ONNX specification
+    specified fields, it also contains a mapping of :attr:`opset_imports`. This
+    allows different subgraphs to import different opsets. It is the responsibility
+    of the deserializer to reconcile the different opsets.
+
+    The `nodes` are not guaranteed to be topologically sorted. But the
+    iteration order should be deterministic across different runs. It is the
+    responsibility of the user to maintain a topological order of the nodes.
+
+    Note that there is not a ``node`` attribute in the Graph. The Graph can be
+    seen as a Sequence of nodes and should be used as such. For example, to obtain
+    all nodes as a list, call ``list(graph)``.
 
-        for node in graph:
-            print(node)
+    Attributes:
+        name: The name of the graph.
+        inputs: The input values of the graph.
+        outputs: The output values of the graph.
+        initializers: The initializers in the graph.
+        doc_string: Documentation string.
+        opset_imports: Opsets imported by the graph.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     __slots__ = (
         "name",
         "_inputs",
         "_outputs",
         "_initializers",
@@ -1176,14 +1290,20 @@
     ):
         self.name = name
 
         # Private fields that are not to be accessed by any other classes
         self._inputs = list(inputs)
         self._outputs = list(outputs)
         for initializer in initializers:
+            if isinstance(initializer, str):
+                raise TypeError(
+                    "Initializer must be a TensorProtocol, not a string. "
+                    "If you are copying the initializers from another graph, "
+                    "make sure you call graph.initializers.values() because it is a dictionary."
+                )
             if initializer.name is None:
                 raise ValueError(f"Initializer must have a name: {initializer}")
         self._initializers = {tensor.name: tensor for tensor in initializers}
         self._doc_string = doc_string
         self._opset_imports = opset_imports or {}
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = metadata_props
@@ -1214,18 +1334,14 @@
     def doc_string(self, value: str | None) -> None:
         self._doc_string = value
 
     @property
     def opset_imports(self) -> dict[str, int]:
         return self._opset_imports
 
-    @property
-    def nodes(self) -> Sequence[Node]:
-        return tuple(self._nodes)
-
     def __getitem__(self, index: int) -> Node:
         return self._nodes[index]
 
     def __len__(self) -> int:
         return len(self._nodes)
 
     def __iter__(self) -> Iterator[Node]:
@@ -1365,15 +1481,15 @@
     ),
     outputs=({textwrap.indent(outputs_text, ' '*8)}
     ),{textwrap.indent(initializers_text, ' '*4)}
 )"""
     node_count = len(graph)
     number_width = len(str(node_count))
     node_lines = []
-    for i, node in enumerate(graph.nodes):
+    for i, node in enumerate(graph):
         node_name = node.name if node.name else f":anonymous_node:{id(node)}"
         node_text = f"# {node_name}\n{node}"
         indented_node_text = textwrap.indent(node_text, " " * (number_width + 4))
         # Remove the leading spaces
         indented_node_text = indented_node_text.strip()
         node_lines.append(f"{i:>{number_width}} |  {indented_node_text}")
     returns = ", ".join(str(x) for x in graph.outputs)
@@ -1429,19 +1545,19 @@
     will remain read-only as a GraphView. No copying will be done during the
     initialization process.
 
     Attributes:
         name: The name of the graph.
         inputs: The input values of the graph.
         outputs: The output values of the graph.
-        nodes: All nodes visible in this view. They do not have to be sorted.
         initializers: The initializers in the graph.
         doc_string: Documentation string.
         opset_imports: Opsets imported by the graph.
-        metadata_props: Metadata.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     __slots__ = (
         "name",
         "inputs",
         "outputs",
         "initializers",
@@ -1458,39 +1574,40 @@
         outputs: Sequence[Value],
         *,
         nodes: Iterable[Node],
         initializers: Sequence[_protocols.TensorProtocol] = (),
         doc_string: str | None = None,
         opset_imports: dict[str, int] | None = None,
         name: str | None = None,
+        metadata_props: dict[str, str] | None = None,
     ):
         self.name = name
         self.inputs = tuple(inputs)
         self.outputs = tuple(outputs)
         for initializer in initializers:
             if initializer.name is None:
                 raise ValueError(f"Initializer must have a name: {initializer}")
         self.initializers = {tensor.name: tensor for tensor in initializers}
         self.doc_string = doc_string
         self.opset_imports = opset_imports or {}
         self._metadata: _metadata.MetadataStore | None = None
-        self._metadata_props: dict[str, str] | None = None
-        self.nodes: tuple[Node, ...] = tuple(nodes)
+        self._metadata_props: dict[str, str] | None = metadata_props
+        self._nodes: tuple[Node, ...] = tuple(nodes)
 
     def __getitem__(self, index: int) -> Node:
-        return self.nodes[index]
+        return self._nodes[index]
 
     def __len__(self) -> int:
-        return len(self.nodes)
+        return len(self._nodes)
 
     def __iter__(self) -> Iterator[Node]:
-        return iter(self.nodes)
+        return iter(self._nodes)
 
     def __reversed__(self) -> Iterator[Node]:
-        return reversed(self.nodes)
+        return reversed(self._nodes)
 
     @property
     def meta(self) -> _metadata.MetadataStore:
         """The metadata store for intermediate analysis.
 
         Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
         to the ONNX proto.
@@ -1539,26 +1656,26 @@
         doc_string: Documentation string.
         functions: The functions defined in the model.
         metadata_props: Metadata.
     """
 
     def __init__(
         self,
-        graph: Graph | GraphView,
+        graph: Graph,
         *,
         ir_version: int,
         producer_name: str | None = None,
         producer_version: str | None = None,
         domain: str | None = None,
         model_version: int | None = None,
         doc_string: str | None = None,
         functions: Sequence[Function] = (),
         meta_data_props: dict[str, str] | None = None,
     ) -> None:
-        self.graph: Graph | GraphView = graph  # type: ignore[assignment]
+        self.graph: Graph = graph
         self.ir_version = ir_version
         self.producer_name = producer_name
         self.producer_version = producer_version
         self.domain = domain
         self.model_version = model_version
         self.doc_string = doc_string
         self._functions = {func.identifier(): func for func in functions}
@@ -1571,15 +1688,19 @@
 
     @property
     def opset_imports(self) -> dict[str, int]:
         return self.graph.opset_imports
 
     @property
     def meta(self) -> _metadata.MetadataStore:
-        """The metadata store for this node."""
+        """The metadata store for intermediate analysis.
+
+        Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
+        to the ONNX proto.
+        """
         if self._metadata is None:
             self._metadata = _metadata.MetadataStore()
         return self._metadata
 
     @property
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
@@ -1611,15 +1732,37 @@
     domain={self.domain!r},
     model_version={self.model_version!r},
     functions={self.functions!r},
     graph={textwrap.indent(repr(self.graph), ' ' * 4).strip()}
 )"""
 
 
-class Function(_protocols.FunctionProtocol, _display.PrettyPrintable):
+class Function(_protocols.FunctionProtocol, Sequence[Node], _display.PrettyPrintable):
+    """IR functions.
+
+    Like a graph, a function can have nodes that are not topologically sorted. It is
+    the responsibility of the user to maintain a topological order of the nodes.
+
+    Note that there is not a ``node`` attribute in the Function. The Function can be
+    seen as a Sequence of nodes and should be used as such. For example, to obtain
+    all nodes as a list, call ``list(function)``.
+
+    Attributes:
+        name: The function name.
+        domain: The domain this function is defined in.
+        overload: The overload name when the function is overloaded.
+        inputs: The input values of the function.
+        attributes: The attributes this function defines.
+        outputs: The output values of the function.
+        opset_imports: Opsets imported by the function.
+        doc_string: Documentation string.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
+    """
+
     __slots__ = (
         "_domain",
         "_name",
         "_overload",
         "_graph",
         "_attributes",
         "_metadata",
@@ -1681,18 +1824,14 @@
     def outputs(self) -> list[Value]:
         return self._graph.outputs
 
     @property
     def attributes(self) -> OrderedDict[str, Attr]:
         return self._attributes
 
-    @property
-    def nodes(self) -> Sequence[Node]:
-        return self._graph.nodes
-
     def __getitem__(self, index: int) -> Node:
         return self._graph.__getitem__(index)
 
     def __len__(self) -> int:
         return self._graph.__len__()
 
     def __iter__(self) -> Iterator[Node]:
@@ -1711,15 +1850,19 @@
 
     @property
     def opset_imports(self) -> dict[str, int]:
         return self._graph.opset_imports
 
     @property
     def meta(self) -> _metadata.MetadataStore:
-        """The metadata store for this node."""
+        """The metadata store for intermediate analysis.
+
+        Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
+        to the ONNX proto.
+        """
         if self._metadata is None:
             self._metadata = _metadata.MetadataStore()
         return self._metadata
 
     @property
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
@@ -1773,18 +1916,18 @@
     inputs=(
 {textwrap.indent(inputs_text, ' '*8)}
     ),{textwrap.indent(attributes_text, ' '*4)}
     outputs=(
 {textwrap.indent(outputs_text, ' '*8)}
     ),
 )"""
-        node_count = len(self.nodes)
+        node_count = len(self)
         number_width = len(str(node_count))
         node_lines = []
-        for i, node in enumerate(self.nodes):
+        for i, node in enumerate(self):
             node_name = node.name if node.name else f":anonymous_node:{id(node)}"
             node_text = f"# {node_name}\n{node}"
             indented_node_text = textwrap.indent(node_text, " " * (number_width + 4))
             # Remove the leading spaces
             indented_node_text = indented_node_text.strip()
             node_lines.append(f"{i:>{number_width}} |  {indented_node_text}")
         returns = ", ".join(str(x) for x in self.outputs)
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_enums.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,25 +3,21 @@
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 """ONNX IR enums that matches the ONNX spec."""
 
 from __future__ import annotations
 
 import enum
-import typing
 
-if typing.TYPE_CHECKING:
-    import numpy as np
+import numpy as np
 
 
 class AttributeType(enum.IntEnum):
     """Enum for the types of ONNX attributes."""
 
-    # TODO(justinchuby): Should we code gen this? We just need to get rid of protoc
-    # We can code gen with https://github.com/recap-build/proto-schema-parser/tree/main
     UNDEFINED = 0
     FLOAT = 1
     INT = 2
     STRING = 3
     TENSOR = 4
     GRAPH = 5
     FLOATS = 6
@@ -38,14 +34,18 @@
         return self.name
 
     def __str__(self) -> str:
         return self.__repr__()
 
 
 class DataType(enum.IntEnum):
+    """Enum for the data types of ONNX tensors, defined in ``onnx.TensorProto``."""
+
+    # NOTE: Naming: It is tempting to use shorter and more modern names like f32, i64,
+    # but we should stick to the names used in the ONNX spec for consistency.
     UNDEFINED = 0
     FLOAT = 1
     UINT8 = 2
     INT8 = 3
     UINT16 = 4
     INT16 = 5
     INT32 = 6
@@ -62,38 +62,48 @@
     FLOAT8E4M3FN = 17
     FLOAT8E4M3FNUZ = 18
     FLOAT8E5M2 = 19
     FLOAT8E5M2FNUZ = 20
     UINT4 = 21
     INT4 = 22
 
+    @classmethod
+    def from_numpy(cls, dtype: np.dtype) -> DataType:
+        """Returns the ONNX data type for the numpy dtype.
+
+        Raises:
+            TypeError: If the data type is not supported by ONNX.
+        """
+        if dtype not in _NP_TYPE_TO_DATA_TYPE:
+            raise TypeError(f"Unsupported numpy data type: {dtype}")
+        return cls(_NP_TYPE_TO_DATA_TYPE[dtype])
+
     @property
     def itemsize(self) -> float:
         """Returns the size of the data type in bytes."""
-        return ITEMSIZE_MAP[self]
+        return _ITEMSIZE_MAP[self]
 
     def numpy(self) -> np.dtype:
         """Returns the numpy dtype for the ONNX data type.
 
         Raises:
-            KeyError: If the data type is not supported by numpy.
+            TypeError: If the data type is not supported by numpy.
         """
-        import onnx.helper  # pylint: disable=import-outside-toplevel
-        # Import here to avoid bringing in the onnx protobuf dependencies to the module
-
-        return onnx.helper.tensor_dtype_to_np_dtype(self)
+        if self not in _DATA_TYPE_TO_NP_TYPE:
+            raise TypeError(f"Numpy does not support ONNX data type: {self}")
+        return _DATA_TYPE_TO_NP_TYPE[self]
 
     def __repr__(self) -> str:
         return self.name
 
     def __str__(self) -> str:
         return self.__repr__()
 
 
-ITEMSIZE_MAP = {
+_ITEMSIZE_MAP = {
     DataType.FLOAT: 4,
     DataType.UINT8: 1,
     DataType.INT8: 1,
     DataType.UINT16: 2,
     DataType.INT16: 2,
     DataType.INT32: 4,
     DataType.INT64: 8,
@@ -109,7 +119,30 @@
     DataType.FLOAT8E4M3FN: 1,
     DataType.FLOAT8E4M3FNUZ: 1,
     DataType.FLOAT8E5M2: 1,
     DataType.FLOAT8E5M2FNUZ: 1,
     DataType.UINT4: 0.5,
     DataType.INT4: 0.5,
 }
+
+
+_NP_TYPE_TO_DATA_TYPE = {
+    np.dtype("bool"): DataType.BOOL,
+    np.dtype("complex128"): DataType.COMPLEX128,
+    np.dtype("complex64"): DataType.COMPLEX64,
+    np.dtype("float16"): DataType.FLOAT16,
+    np.dtype("float32"): DataType.FLOAT,
+    np.dtype("float64"): DataType.DOUBLE,
+    np.dtype("int16"): DataType.INT16,
+    np.dtype("int32"): DataType.INT32,
+    np.dtype("int64"): DataType.INT64,
+    np.dtype("int8"): DataType.INT8,
+    np.dtype("object"): DataType.STRING,
+    np.dtype("uint16"): DataType.UINT16,
+    np.dtype("uint32"): DataType.UINT32,
+    np.dtype("uint64"): DataType.UINT64,
+    np.dtype("uint8"): DataType.UINT8,
+}
+
+# ONNX DataType to Numpy dtype. This mapping does not capture ONNX data
+# types that are not supported by numpy.
+_DATA_TYPE_TO_NP_TYPE = {v: k for k, v in _NP_TYPE_TO_DATA_TYPE.items()}
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,63 +2,36 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 """Class for storing metadata about the IR objects."""
 
 from __future__ import annotations
 
-from typing import Any, Iterator, Mapping
+import collections
+from typing import Any, Mapping
 
 
-class MetadataStore(Mapping[str, Any]):
+class MetadataStore(collections.UserDict):
     """Class for storing metadata about the IR objects.
 
     Metadata is stored as key-value pairs. The keys are strings and the values
     can be any Python object.
 
     The metadata store also supports marking keys as invalid. This is useful
     when a pass wants to mark a key that needs to be recomputed.
     """
 
-    __slots__ = ["_store", "_invalid_keys"]
-
-    def __init__(self) -> None:
-        self._store: dict[str, Any] = {}
+    def __init__(self, data: Mapping[str, Any] | None = None, /) -> None:
+        super().__init__(data)
         self._invalid_keys: set[str] = set()
 
-    def __getitem__(self, key: str) -> Any:
-        # We do not check validity here because we want to allow
-        # users to access invalid keys
-        return self._store[key]
-
-    def get(self, key: str, default: Any = None) -> Any:
-        return self._store.get(key, default)
-
-    def items(self):
-        return self._store.items()
-
-    def keys(self):
-        return self._store.keys()
-
-    def values(self):
-        return self._store.values()
-
-    def __iter__(self) -> Iterator[str]:
-        return self._store.__iter__()
-
-    def __len__(self) -> int:
-        return len(self._store)
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self._store[key] = value
+    def __setitem__(self, key: str, item: Any) -> None:
+        self.data[key] = item
         self._invalid_keys.discard(key)
 
-    def __contains__(self, key: str) -> bool:
-        return key in self._store
-
     def invalidate(self, key: str) -> None:
         self._invalid_keys.add(key)
 
     def is_valid(self, key: str) -> bool:
         """Returns whether the value is valid.
 
         Note that default values (None) are not necessarily invalid. For example,
@@ -66,12 +39,8 @@
         determined that the shape is unknown.
 
         Whether a value is valid is solely determined by the user that sets the value.
         """
         return key not in self._invalid_keys
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(store={self._store}, invalid_keys={self._invalid_keys})"
-
-    def to_metadata_props(self) -> dict[str, str]:
-        # TODO(justinchuby): Handle invalid keys
-        return {k: str(v) for k, v in self.items()}
+        return f"{self.__class__.__name__}({self.data!r}, invalid_keys={self._invalid_keys!r})"
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/_protocols.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,39 +10,33 @@
 tools.
 """
 
 from __future__ import annotations
 
 import typing
 from typing import (
-    AbstractSet,
     Any,
+    Collection,
     Iterable,
     Iterator,
     Mapping,
     MutableMapping,
     MutableSequence,
     OrderedDict,
     Protocol,
     Sequence,
     Tuple,
-    Union,
 )
 
 from onnxscript.ir import _enums
 
 if typing.TYPE_CHECKING:
     import numpy as np
     from typing_extensions import TypeAlias
 
-# Representation of a dimension. int is a known axis, str represents a dynamic axis, None is an unnamed dynamic axis.
-SimpleDim: TypeAlias = Union[int, str, None]
-# Representation of a shape. Each element is a simple dimension.
-SimpleShape: TypeAlias = Sequence[SimpleDim]
-
 # An identifier that will uniquely identify an operator. E.g (domain, op_type, overload)
 OperatorIdentifier: TypeAlias = Tuple[str, str, str]
 
 
 @typing.runtime_checkable
 class ArrayCompatible(Protocol):
     """Protocol for array-like objects.
@@ -63,14 +57,18 @@
     without copying the data.
     """
 
     def __dlpack__(self, *, stream: Any = ...) -> Any:
         """Return PyCapsule."""
         ...
 
+    def __dlpack_device__(self) -> Any:
+        """Return the device."""
+        ...
+
 
 @typing.runtime_checkable
 class TensorProtocol(ArrayCompatible, Protocol):
     """Concrete tensor backed by data.
 
     The protocol does not specify how the data is stored. That data is exposed
     through the :attr:`raw` attribute for examination, but accessing :attr:`raw`
@@ -87,22 +85,25 @@
         name: The name of the tensor.
         shape: The shape of the tensor.
         dtype: The data type of the elements of the tensor. It is an :class:`ir.DataType` enum.
         doc_string: Documentation string.
         raw: The raw data behind this tensor. It can be anything.
         size: The number of elements in the tensor.
         nbytes: The number of bytes in the tensor.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     name: str
     shape: ShapeProtocol
     dtype: _enums.DataType
     doc_string: str | None
     raw: Any
     metadata_props: MutableMapping[str, str]
+    meta: MutableMapping[str, Any]
 
     @property
     def size(self) -> int: ...
 
     @property
     def nbytes(self) -> int: ...
 
@@ -140,15 +141,16 @@
 
     To check if the value is an output of a graph, call :meth:`is_graph_output`.
 
     Attributes:
         name: The name of the value. A value is always named when it is part of a graph.
         shape: The shape of the value.
         type: The type of the value.
-        metadata_props: Metadata.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     name: str
     shape: ShapeProtocol | None
     type: TypeProtocol | None
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
@@ -157,15 +159,15 @@
         """The node that produces this value."""
         ...
 
     def index(self) -> int | None:
         """The index of the output of the node that produces this value."""
         ...
 
-    def consumers(self) -> AbstractSet[tuple[NodeProtocol, int]]:
+    def consumers(self) -> Collection[tuple[NodeProtocol, int]]:
         """The set of (node, input_index) with node being those that use this value as an input."""
         ...
 
     def is_graph_output(self) -> bool:
         """Whether this value is an output of a graph."""
         ...
 
@@ -203,15 +205,16 @@
         op_type: The operator name.
         overload: The overload name when the node is invoking a function.
         inputs: Input values.
         outputs: Output values.
         attributes: The attributes of the operator.
         version: The version of the operator.
         doc_string: Documentation string.
-        metadata_props: Metadata.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     name: str | None
     domain: str
     op_type: str
     overload: str
     inputs: Sequence[ValueProtocol]
@@ -232,37 +235,40 @@
     """Protocol for graphs.
 
     Graph represents a computation graph. In addition to the ONNX specification
     specified fields, it also contains a mapping of :attr:`opset_imports`. This
     allows different subgraphs to import different opsets. It is the responsibility
     of the deserializer to reconcile the different opsets.
 
-    The :attr:`nodes` are not guaranteed to be topologically sorted. But the
+    The nodes are not guaranteed to be topologically sorted. But the
     iteration order should be deterministic across different runs. It is the
     responsibility of the user to maintain a topological order of the nodes.
 
+    Note that there is not a ``node`` attribute in the Graph. The Graph can be
+    seen as a Sequence of nodes and should be used as such. For example, to obtain
+    all nodes as a list, call ``list(graph)``.
+
     Attributes:
         name: The name of the graph.
         inputs: The input values of the graph.
         outputs: The output values of the graph.
-        nodes: All nodes this graph directly owns. They do not have to be sorted.
         initializers: The initializers in the graph.
         doc_string: Documentation string.
         opset_imports: Opsets imported by the graph.
-        metadata_props: Metadata.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     # TODO(justinchuby): Support quantization_annotation
     name: str | None
     inputs: MutableSequence[ValueProtocol]
     outputs: MutableSequence[ValueProtocol]
-    nodes: Sequence[NodeProtocol]
-    initializers: Mapping[str, TensorProtocol]
+    initializers: MutableMapping[str, TensorProtocol]
     doc_string: str
-    opset_imports: Mapping[str, int]
+    opset_imports: MutableMapping[str, int]
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
 
     def __getitem__(self, index: int) -> NodeProtocol: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[NodeProtocol]: ...
     def __reversed__(self) -> Iterator[NodeProtocol]: ...
@@ -302,25 +308,24 @@
     change the ownership of the nodes, and so it is possible to create multiple
     GraphViews that contain the same nodes.
 
     Attributes:
         name: The name of the graph.
         inputs: The input values of the graph.
         outputs: The output values of the graph.
-        nodes: All nodes this graph directly owns. They do not have to be sorted.
         initializers: The initializers in the graph.
         doc_string: Documentation string.
         opset_imports: Opsets imported by the graph.
-        metadata_props: Metadata.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     name: str | None
     inputs: Sequence[ValueProtocol]
     outputs: Sequence[ValueProtocol]
-    nodes: Sequence[NodeProtocol]
     initializers: Mapping[str, TensorProtocol]
     doc_string: str
     opset_imports: Mapping[str, int]
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
 
     def __getitem__(self, index: int) -> NodeProtocol: ...
@@ -341,27 +346,28 @@
         ir_version: The version of the IR.
         producer_name: The name of the producer.
         producer_version: The version of the producer.
         domain: The domain of the model.
         model_version: The version of the model.
         doc_string: Documentation string.
         functions: The functions defined in the model.
-        metadata_props: Metadata.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     graph: GraphProtocol
     ir_version: int
     producer_name: str | None
     producer_version: str | None
     domain: str | None
     model_version: int | None
     doc_string: str | None
-    functions: Mapping[str, FunctionProtocol]
+    functions: MutableMapping[str, FunctionProtocol]
     # TODO(justinchuby): Add training_info
-    opset_imports: Mapping[str, int]
+    opset_imports: MutableMapping[str, int]
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
 
 
 @typing.runtime_checkable
 class AttributeProtocol(Protocol):
     """Protocol for ONNX attributes.
@@ -402,50 +408,51 @@
 class SparseTensorProtocol(Protocol):
     values: TensorProtocol
     indices: TensorProtocol
     dims: Sequence[int]
 
 
 @typing.runtime_checkable
-class DimensionProtocol(Protocol):
-    """Value of a single dimension in a shape.
+class SymbolicDimProtocol(Protocol):
+    """Value of a single symbolic/dynamic dimension in a shape.
 
     Attributes:
         value: The value of the dimension.
-        denotation: The denotation of the dimension.
-            Standard denotation can optionally be used to denote tensor
-            dimensions with standard semantic descriptions to ensure
-            that operations are applied to the correct axis of a tensor.
-            Refer to https://github.com/onnx/onnx/blob/main/docs/DimensionDenotation.md#denotation-definition
-            for pre-defined dimension denotations.
     """
 
-    value: int | str | None
-    denotation: str | None
+    value: str | None  # TODO(justinchuby): Maybe support sympy
 
 
 @typing.runtime_checkable
 class ShapeProtocol(Protocol):
     """Protocol for ONNX shapes.
 
     A shape is a sequence of dimensions.
 
     Attributes:
         dims: The dimensions of the shape.
     """
 
-    dims: Sequence[DimensionProtocol]
-
-    def __iter__(self) -> Iterator[DimensionProtocol]: ...
-
-    def __getitem__(self, index: int) -> DimensionProtocol: ...
-
-    def simple(self) -> SimpleShape: ...
+    dims: Sequence[int | SymbolicDimProtocol]
 
+    def __len__(self) -> int: ...
+    def __iter__(self) -> Iterator[int | SymbolicDimProtocol]: ...
+    @typing.overload
+    def __getitem__(self, index: int) -> int | SymbolicDimProtocol: ...
+    @typing.overload
+    def __getitem__(self, index: slice) -> tuple[int | SymbolicDimProtocol, ...]: ...
+    def __setitem__(
+        self, index: int, value: int | SymbolicDimProtocol | str | None
+    ) -> None: ...
+    def __eq__(self, other: object) -> bool: ...
+    def __ne__(self, value: object) -> bool: ...
+    def get_denotation(self, index: int) -> str | None: ...
+    def set_denotation(self, index: int, denotation: str | None) -> None: ...
     def numpy(self) -> Sequence[int]: ...
+    def rank(self) -> int: ...
 
 
 @typing.runtime_checkable
 class TypeProtocol(Protocol):
     """Protocol for ONNX tensors, Sequence tensors, Optional tensors and Sparse tensors.
 
     These three types of tensors share the same attribute "elem_type" so they are
@@ -494,36 +501,39 @@
 @typing.runtime_checkable
 class FunctionProtocol(Protocol):
     """Protocol for ONNX functions.
 
     Like a graph, a function can have nodes that are not topologically sorted. It is
     the responsibility of the user to maintain a topological order of the nodes.
 
+    Note that there is not a ``node`` attribute in the Function. The Function can be
+    seen as a Sequence of nodes and should be used as such. For example, to obtain
+    all nodes as a list, call ``list(function)``.
+
     Attributes:
         name: The function name.
         domain: The domain this function is defined in.
         overload: The overload name when the function is overloaded.
         inputs: The input values of the function.
         attributes: The attributes this function defines.
         outputs: The output values of the function.
         opset_imports: Opsets imported by the function.
         doc_string: Documentation string.
-        nodes: All nodes this function directly owns. They do not have to be sorted.
-        metadata_props: Metadata.
+        metadata_props: Metadata that will be serialized to the ONNX file.
+        meta: Metadata store for graph transform passes.
     """
 
     name: str
     domain: str
     overload: str
     inputs: Sequence[ValueProtocol]
     attributes: OrderedDict[str, AttributeProtocol]
     outputs: Sequence[ValueProtocol]
     doc_string: str
-    opset_imports: Mapping[str, int]
-    nodes: Sequence[NodeProtocol]
+    opset_imports: MutableMapping[str, int]
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
 
     def __getitem__(self, index: int) -> NodeProtocol: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[NodeProtocol]: ...
     def __reversed__(self) -> Iterator[NodeProtocol]: ...
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/convenience.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240420/onnxscript/ir/serde.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 import onnx
 import onnx.external_data_helper
 import onnx.numpy_helper
 
 from onnxscript.ir import (
     _core,
     _enums,
+    _metadata,
     _protocols,
 )
 
 if typing.TYPE_CHECKING:
     import google.protobuf.internal.containers as proto_containers
 
 logger = logging.getLogger(__name__)
@@ -82,23 +83,26 @@
 
 
 class TensorProtoTensor(_core.TensorBase):
     """A tensor initialized from a tensor proto."""
 
     def __init__(self, proto: onnx.TensorProto) -> None:
         self._proto = proto
-        self._metadata_props: dict[str, str] = deserialize_metadata_props(proto.metadata_props)
+        self._metadata_props: dict[str, str] | None = deserialize_metadata_props(
+            proto.metadata_props
+        )
+        self._metadata: _metadata.MetadataStore | None = None
 
     @property
     def name(self) -> str:
         return self._proto.name
 
     @property
     def shape(self) -> _core.Shape:
-        return _core.Shape(self._proto.dims)
+        return _core.Shape(self._proto.dims, frozen=True)
 
     @property
     def dtype(self) -> _enums.DataType:
         return _enums.DataType(self._proto.data_type)
 
     @property
     def doc_string(self) -> str:
@@ -124,15 +128,28 @@
         if not self._proto.HasField("raw_data"):
             raise ValueError(
                 "Cannot convert non-raw tensor to bytes. Use a specialized tensor class like FloatDataTensor instead."
             )
         return self._proto.raw_data
 
     @property
+    def meta(self) -> _metadata.MetadataStore:
+        """The metadata store for intermediate analysis.
+
+        Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
+        to the ONNX proto.
+        """
+        if self._metadata is None:
+            self._metadata = _metadata.MetadataStore()
+        return self._metadata
+
+    @property
     def metadata_props(self) -> dict[str, str]:
+        if self._metadata_props is None:
+            self._metadata_props = {}
         return self._metadata_props
 
 
 class FloatDataTensor(TensorProtoTensor):  # pylint: disable=too-many-ancestors
     """Specialized tensor for float data.
 
     When serializing, the data can be stored in the float_data field.
@@ -336,28 +353,28 @@
         function_domain, function_name, value_name = parsed
         function_overload = ""
         # TODO(justinchuby): Create a constructor for OperatorIdentifier so we don't create tuples manually
         function_id = (function_domain, function_name, function_overload)
         function = functions.get(function_id)
         if function is None:
             # Function not found
-            logger.warning(
+            logger.debug(
                 "Function with ID '%s' not found in model functions. Value info '%s' will be ignored.",
                 function_id,
                 value_info_proto.name,
             )
             continue
         function_value_value_info_mapping[function_id][value_name] = value_info_proto
     for function_id, function in functions.items():
         for input in function.inputs:
             if input.name in function_value_value_info_mapping[function_id]:
                 deserialize_value_info_proto(
                     function_value_value_info_mapping[function_id][input.name], input
                 )
-        for node in function.nodes:
+        for node in function:
             for output in node.outputs:
                 if output.name in function_value_value_info_mapping[function_id]:
                     deserialize_value_info_proto(
                         function_value_value_info_mapping[function_id][output.name],
                         output,
                     )
             # The function outputs are handled as well because they are also node outputs
@@ -466,30 +483,42 @@
     proto: onnx.ValueInfoProto, value: _core.Value | None
 ) -> _core.Value:
     if value is None:
         value = _core.Value(None, index=None)
         value.name = proto.name
     value.shape = deserialize_type_proto_for_shape(proto.type)
     value.type = deserialize_type_proto_for_type(proto.type)
-    value.metadata_props.update(deserialize_metadata_props(proto.metadata_props))
+    metadata_props = deserialize_metadata_props(proto.metadata_props)
+    if metadata_props is not None:
+        value.metadata_props.update(metadata_props)
     return value
 
 
 def deserialize_type_proto_for_shape(proto: onnx.TypeProto) -> _core.Shape | None:
     if proto.HasField("tensor_type"):
         if (shape_proto := _get_field(proto.tensor_type, "shape")) is None:
             return None
         # This logic handles when the shape is [] as well
         dim_protos = shape_proto.dim
-        return _core.Shape([deserialize_dimension(d) for d in dim_protos])
+        deserialized_dim_denotations = [
+            deserialize_dimension(dim_proto) for dim_proto in dim_protos
+        ]
+        dims = [dim for dim, _ in deserialized_dim_denotations]
+        denotations = [denotation for _, denotation in deserialized_dim_denotations]
+        return _core.Shape(dims, denotations=denotations, frozen=True)
     if proto.HasField("sparse_tensor_type"):
         if (shape_proto := _get_field(proto.sparse_tensor_type, "shape")) is None:
             return None
         dim_protos = shape_proto.dim
-        return _core.Shape([deserialize_dimension(d) for d in dim_protos])
+        deserialized_dim_denotations = [
+            deserialize_dimension(dim_proto) for dim_proto in dim_protos
+        ]
+        dims = [dim for dim, _ in deserialized_dim_denotations]
+        denotations = [denotation for _, denotation in deserialized_dim_denotations]
+        return _core.Shape(dims, denotations=denotations, frozen=True)
     if proto.HasField("sequence_type"):
         if (elem_type := _get_field(proto.sequence_type, "elem_type")) is None:
             return None
         return deserialize_type_proto_for_shape(elem_type)
     if proto.HasField("optional_type"):
         if (elem_type := _get_field(proto.optional_type, "elem_type")) is None:
             return None
@@ -532,20 +561,34 @@
     if proto.HasField("map_type"):
         # TODO(justinchuby): Do we need to support map types?
         raise NotImplementedError("Map types are not supported yet")
 
     return None
 
 
-def deserialize_dimension(proto: onnx.TensorShapeProto.Dimension) -> _core.Dimension:
+def deserialize_dimension(
+    proto: onnx.TensorShapeProto.Dimension,
+) -> tuple[int | _core.SymbolicDim, str | None]:
+    """Deserialize a dimension proto into (dimension, denotation).
+
+    Args:
+        proto: The dimension proto to deserialize.
+
+    Returns:
+        A tuple of the dimension and its denotation.
+    """
     value_field = proto.WhichOneof("value")
     denotation = _get_field(proto, "denotation")
     if value_field is not None:
-        return _core.Dimension(getattr(proto, value_field), denotation=denotation)
-    return _core.Dimension(None)
+        value = getattr(proto, value_field)
+        if value_field == "dim_value":
+            return value, denotation
+        if value_field == "dim_param":
+            return _core.SymbolicDim(value), denotation
+    return _core.SymbolicDim(None), denotation
 
 
 def deserialize_tensor(
     proto: onnx.TensorProto, base_path: str | os.PathLike = ""
 ) -> _protocols.TensorProtocol:
     # TODO: Sanitize base_path
     if proto.data_location == onnx.TensorProto.EXTERNAL:
@@ -576,15 +619,20 @@
     if proto.data_type in UInt64DataTensor.compatible_types:
         return UInt64DataTensor(proto)
     raise ValueError(
         f"TensorProto(name={proto.name}) does not have any data fields set and is not an external tensor."
     )
 
 
-def deserialize_metadata_props(proto: Sequence[onnx.StringStringEntryProto]) -> dict[str, str]:
+def deserialize_metadata_props(
+    proto: Sequence[onnx.StringStringEntryProto],
+) -> dict[str, str] | None:
+    if len(proto) == 0:
+        # Avoid creating an empty dictionary to save memory
+        return None
     return {entry.key: entry.value for entry in proto}
 
 
 def deserialize_attribute(proto: onnx.AttributeProto) -> _core.Attr | _core.RefAttr:
     return _deserialize_attribute(proto, [])
 
 
@@ -665,30 +713,31 @@
         proto.domain,
         proto.op_type,
         node_inputs,
         [_deserialize_attribute(a, scoped_values) for a in proto.attribute],
         overload=getattr(proto, "overload", ""),
         num_outputs=len(proto.output),
         name=proto.name,
+        doc_string=_get_field(proto, "doc_string"),
+        metadata_props=deserialize_metadata_props(proto.metadata_props),
     )
 
     for output, value in zip(proto.output, node.outputs):
         value.name = output
         if output in value_info:
             deserialize_value_info_proto(value_info[output], value)
         else:
             logger.debug(
                 "ValueInfoProto not found for output '%s' in node '%s' of type '%s'",
                 output,
                 proto.name,
                 proto.op_type,
             )
         scoped_values[-1][output] = value
-    for prop in getattr(proto, "metadata_props", []):
-        node.metadata_props[prop.key] = prop.value
+
     return node
 
 
 # Serialization
 
 
 def serialize_model(model: _protocols.ModelProtocol) -> onnx.ModelProto:
@@ -772,15 +821,15 @@
                 input,
             )
             continue
         if not _should_create_value_info_for_value(input):
             # No need to serialize value info if it is not set
             continue
         serialize_value_into(graph_proto.value_info.add(), input, name=format_name(input.name))
-    for node in function.nodes:
+    for node in function:
         for node_output in node.outputs:
             if not node_output.name:
                 logging.warning(
                     "Function '%s': Value name not set for node output: %s",
                     function_qualified_name,
                     node_output,
                 )
@@ -844,15 +893,15 @@
     if from_.doc_string:
         graph_proto.doc_string = from_.doc_string
     for input_ in from_.inputs:
         serialize_value_into(graph_proto.input.add(), input_)
     # TODO(justinchuby): Support sparse_initializer
     for initializer in from_.initializers.values():
         serialize_tensor_into(graph_proto.initializer.add(), from_=initializer)
-    for node in from_.nodes:
+    for node in from_:
         serialize_node_into(graph_proto.node.add(), from_=node)
         for node_output in node.outputs:
             if not _should_create_value_info_for_value(node_output):
                 # No need to serialize value info if it is not set
                 continue
             if node_output.is_graph_output():
                 # No need to serialize value info for these outputs because they are also graph outputs
@@ -924,15 +973,15 @@
         else:
             # ONNX does not record type information if the attribute does not have a default
             function_proto.attribute.append(attr.name)
     for func_output in from_.outputs:
         function_proto.output.append(func_output.name)
         # No need to serialize value info for function outputs because they are
         # also node outputs
-    for node in from_.nodes:
+    for node in from_:
         serialize_node_into(function_proto.node.add(), from_=node)
         # Record value info for outputs
         for node_output in node.outputs:
             if not _should_create_value_info_for_value(node_output):
                 # No need to serialize value info if it is not set
                 continue
             if not create_value_info:
@@ -1142,21 +1191,23 @@
         raise TypeError(f"Unsupported type: {from_}")
 
 
 def serialize_shape_into(type_proto: onnx.TypeProto, from_: _protocols.ShapeProtocol) -> None:
     tensor_type_proto = type_proto.tensor_type
     # When from is empty, we still need to set the shape field to an empty list by touching it
     tensor_type_proto.shape.ClearField("dim")
-    for dim in from_:
-        serialize_dimension_into(tensor_type_proto.shape.dim.add(), from_=dim)
+    for i, dim in enumerate(from_):
+        denotation = from_.get_denotation(i)
+        serialize_dimension_into(tensor_type_proto.shape.dim.add(), dim, denotation)
 
 
 def serialize_dimension_into(
-    dim_proto: onnx.TensorShapeProto.Dimension, from_: _protocols.DimensionProtocol
+    dim_proto: onnx.TensorShapeProto.Dimension,
+    dim: int | _protocols.SymbolicDimProtocol,
+    denotation: str | None = None,
 ) -> None:
-    value = from_.value
-    if from_.denotation:
-        dim_proto.denotation = from_.denotation
-    if isinstance(value, int):
-        dim_proto.dim_value = value
-    elif isinstance(value, str):
-        dim_proto.dim_param = value
+    if denotation:
+        dim_proto.denotation = denotation
+    if isinstance(dim, int):
+        dim_proto.dim_value = dim
+    elif isinstance(dim, (_core.SymbolicDim, _protocols.SymbolicDimProtocol)):
+        dim_proto.dim_param = str(dim.value)
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240420/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/main.py` & `onnxscript-0.1.0.dev20240420/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240420/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/optimizer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import Any
 
 import onnx
+import onnx.shape_inference
 
 from onnxscript import rewriter
 from onnxscript.optimizer.constant_folding import fold_constants
 from onnxscript.optimizer.copy_propagation import (
     do_copy_propagation,
     do_sequence_simplification,
 )
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240420/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240420/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240420/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240420/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240420/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240420/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240420/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 from __future__ import annotations
 
 from typing import Sequence
 
 __all__ = [
     # Modules
-    "irbuilder",
-    "protobuilder",
     "function_rule",
     "pattern",
     # Functions
     "rewrite",
 ]
 
 import onnx
 
-from onnxscript._legacy_ir import irbuilder, protobuilder
+from onnxscript import ir
 from onnxscript.optimizer import remove_unused, remove_unused_function
 from onnxscript.rewriter import function_rule, pattern
 
 PatternRewriteRule = pattern.RewriteRule
 FunctionRewriteRule = function_rule.FunctionRewriteRule
 
 
 def rewrite(
     model: onnx.ModelProto,
     function_rewrite_rules: Sequence[type[FunctionRewriteRule]] = (),
     pattern_rewrite_rules: Sequence[PatternRewriteRule] = (),
 ) -> onnx.ModelProto:
+    print(f"len(value_info): {len(model.graph.value_info)}")
+    model_ir = ir.serde.deserialize_model(model)
     if function_rewrite_rules:
-        model_ir = irbuilder.build_ir(model)
         for rule_cls in function_rewrite_rules:
-            rule_cls().apply_to_model(model_ir)
-        model = model_ir.original_model_proto
+            count, model_ir = rule_cls().apply_to_model(model_ir)
+            print(f"Applied {count} of onnxruntime specific function rewrite rules.")
     if pattern_rewrite_rules:
-        model_ir = irbuilder.build_ir(model)
         count = pattern.RewriteRuleSet(pattern_rewrite_rules).apply_to_model(model_ir)
-        print(f"Applied {count} pattern rewrite rules.")
-        model = protobuilder.build_model_proto(model_ir)
-    # TODO: Does it make more sense we run DCE after each rewrite rule applied?
-    # If so, we need IR to support DCE.
+        print(f"Applied {count} of general pattern rewrite rules.")
+    model = ir.serde.serialize_model(model_ir)
     remove_unused.remove_unused_nodes(model)
     remove_unused_function.remove_unused_functions(model)
+    print(f"len(value_info): {len(model.graph.value_info)}")
     return model
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import numpy as np
 
-import onnxscript._legacy_ir as ir
-from onnxscript.rewriter import pattern
+from onnxscript import ir
+from onnxscript.rewriter import _ir_utils, pattern
 
 op = pattern.onnxop
 logger = logging.getLogger(__name__)
 
 
 # condition to check if we need to replace the pattern
 def check_if_need_reshape(match_bindings: dict[str, ir.Value | Any]) -> bool:
@@ -27,15 +27,17 @@
 
     Returns:
         bool: True if we need to replace the pattern, False otherwise.
 
     """
     input_a_shape = match_bindings["input_a"].shape
     input_b_shape = match_bindings["input_b"].shape
-    shape_c = match_bindings["shape_c"].value_as_np_array
+    # TODO: Get a helper func to get const_value
+    shape_c_value = _ir_utils.propagate_const_value(match_bindings["shape_c"])
+    shape_c = shape_c_value.const_value.numpy()  # type: ignore[union-attr]
     if shape_c is None:
         return False
     if not isinstance(shape_c, np.ndarray):
         logger.info("Unexpected shape_c value. Expected np.ndarray, got %s", type(shape_c))
         return False
     if len(shape_c.shape) != 1:
         logger.info(
@@ -46,14 +48,16 @@
     shape_c = shape_c.tolist()
 
     # NOTE: When there is a subset match with a pattern. The MatchResult won't have the shape
     # information. So, we need to check if the shape is None and return False.
     if input_a_shape is None or input_b_shape is None or shape_c is None:
         logger.info("Shape information is not available for the inputs and outputs.")
         return False
+    input_a_shape = list(input_a_shape)
+    input_b_shape = list(input_b_shape)
 
     dim_a = len(input_a_shape)
     dim_b = len(input_b_shape)
 
     # 1. Check if input shapes are broadcastable
     # 1.a. If the first input is 1-D, check whether
     # the dim matches the last second dim of the second input.
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import logging
 from typing import Any, Sequence
 
 import numpy as np
-import onnx
 
-import onnxscript._legacy_ir as ir
+from onnxscript import ir
 from onnxscript.rewriter import pattern
 
 op = pattern.onnxop
 logger = logging.getLogger(__name__)
 
 
 def cast_constant_of_shape(
@@ -26,17 +25,16 @@
 def fused_cast_constant_of_shape(
     shape: Sequence[int], t: Any, dtype: int, match_bindings: dict[str, ir.Value | Any]
 ) -> pattern.OpPattern:
     del dtype  # unused
     del t  # unused
     v_dtype = match_bindings["dtype"]
     v_t = match_bindings["t"]
-    casted_val = onnx.numpy_helper.to_array(v_t).astype(  # type: ignore[arg-type]
-        dtype=onnx.helper.tensor_dtype_to_np_dtype(v_dtype)  # type: ignore[arg-type]
-    )
+    v_dtype = ir.DataType(v_dtype.value).numpy()  # type: ignore[union-attr]
+    casted_val = ir.Tensor(v_t.value.numpy().astype(v_dtype))  # type: ignore[union-attr]
     return op.ConstantOfShape(shape, value=casted_val)
 
 
 def cast_constant_of_shape_without_value(
     shape: Sequence[int],
     dtype: int,
     match_bindings: dict[str, ir.Value | Any] | None = None,
@@ -47,15 +45,16 @@
 
 
 def fused_cast_constant_of_shape_without_value(
     shape: Sequence[int], dtype: int, match_bindings: dict[str, ir.Value | Any]
 ) -> pattern.OpPattern:
     del dtype  # Unused
     v_dtype = match_bindings["dtype"]
-    val = np.zeros(1, dtype=onnx.helper.tensor_dtype_to_np_dtype(v_dtype))  # type: ignore
+    v_dtype = ir.DataType(v_dtype.value).numpy()  # type: ignore[union-attr]
+    val = ir.Tensor(np.zeros(1, dtype=v_dtype))
     return op.ConstantOfShape(shape, value=val)
 
 
 cast_constant_of_shape_rule = pattern.RewriteRule(
     cast_constant_of_shape,
     pattern.ReplacementPatternFunction(fused_cast_constant_of_shape, delay_run=True),
 )
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/function_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import functools
 import logging
 
 import onnx
 from packaging import version
 
 import onnxscript
-import onnxscript._legacy_ir as ir
+from onnxscript import ir
 from onnxscript._legacy_ir import visitor
 from onnxscript.rewriter import pattern
 
 logger = logging.getLogger(__name__)
 
 
 class FunctionRewriteError(RuntimeError): ...
@@ -208,35 +208,37 @@
 
         del function.node[:]
         function.node.extend(nodes)
         for new_opset in opset_imports:
             function.opset_import.append(new_opset)
             if new_opset.domain not in self._opset_imports:
                 model.opset_import.append(new_opset)
-
         return True
 
     def try_rewrite(self, model: ir.Model, value) -> bool:
         raise NotImplementedError(
             "Use `try_rewrite_function` instead for function based rewrites."
         )
 
     def lookup(self, function: onnx.FunctionProto, value_name: str) -> ir.Value | None:
         return self._function_shape_env.lookup(function, value_name)
 
-    def apply_to_model(self, model: ir.Model, *, commute: bool = False) -> int:
+    def apply_to_model(
+        self, model: ir.Model, *, commute: bool = False
+    ) -> tuple[int, ir.Model]:
         del commute  # unused
-        model_proto: onnx.ModelProto = model.original_model_proto
+        model_proto: onnx.ModelProto = ir.serde.serialize_model(model)
         self._function_shape_env = visitor.FunctionShapeEnv()
-        self._function_shape_env.load_from_model_proto(model.original_model_proto)
+        self._function_shape_env.load_from_model_proto(model_proto)
         self._opset_imports = {x.domain: x.version for x in model_proto.opset_import}
 
         rewrite_count = 0
         for function in model_proto.functions:
             rewrite_count += self.try_rewrite_function(function, model_proto)
-        return rewrite_count
+        model = ir.serde.deserialize_model(model_proto)
+        return rewrite_count, model
 
     def count_matches(self, model, *, commute: bool = False) -> int:
         raise NotImplementedError()
 
     def commute(self) -> list[pattern.RewriteRule]:
         raise NotImplementedError()
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/pattern.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1228 +1,1131 @@
 from __future__ import annotations
 
-import collections
 import inspect
-import os
-import textwrap
-import typing
+import itertools
+import math
+from typing import Any, Callable, Sequence
 
+import numpy as np
 import onnx
-import onnx.helper as oh
+import onnx.numpy_helper
+import onnx.printer
 
-import onnxscript
-import onnxscript._legacy_ir as oir
-import onnxscript.rewriter.pattern as orp
+from onnxscript import ir
+from onnxscript.rewriter import _ir_utils
 
+# Overview of the pattern module: The classes below are used to define both
+# patterns (that we search for) and replacements for rewrite rules.
+# The matches() method of a pattern is used to check if an IR component
+# matches the pattern.
+# The to_ir() method of a pattern is used to create a new IR component
+# TODO: Ensure that all matches() methods have same type signature (where
+# appropriate) and that all to_ir() methods have same type signature (where
+# appropriate).
+
+
+class PythonPattern:
+    def __init__(self, value: int | str | Sequence, name: str | None = None) -> None:
+        self._value = value
+        self._name = name
 
-def enumerate_subgraphs(
-    node: oir.Node,
-) -> typing.Iterator[tuple[typing.Any, ...]]:
-    """Returns the subgraphs inside a graph."""
-    for att in node.attribute:
-        if att.type == onnx.AttributeProto.GRAPH and att.g:
-            this = node, att.name, att.g
-            yield this
+    @property
+    def value(self) -> int | str | Sequence:
+        return self._value
 
-            for no in att.g.node:
-                for tu in enumerate_subgraphs(no):
-                    yield this + tu
+    @property
+    def name(self) -> str | None:
+        return self._name
 
+    def matches(self, value: int | str | Sequence) -> bool:
+        return value == self.value
 
-class _GraphStructureAPI:
-    """Common accessors to predecessors and successors."""
+    def to_ir(self, model, bindings=None) -> int | str | Sequence:
+        return self.value
 
-    def __init__(self):
-        self.predecessors_: dict[str, int] = {}
-        self.successors_: dict[str, list[int]] = {}
-        self.nodes_: dict[int, oir.Node] = {}
 
-    def node_before(self, name: str) -> oir.Node | None:
-        """
-        Returns the node producing this output.
+class StringConstantPattern:
+    def __init__(self, value: str, name: str) -> None:
+        self._value = value
+        self._name = name
 
-        Returns None if it is an input or an initializer.
-        """
-        if name not in self.predecessors_:
-            return None
-        predecessor = self.predecessors_[name]
-        return self.nodes_[predecessor]
-
-    def next_nodes(self, name: str) -> list[oir.Node] | None:
-        """Returns the node consuming the given results."""
-        if name not in self.successors_:
-            return []
-        return [self.nodes_[i] for i in self.successors_[name]]
+    @property
+    def value(self) -> str:
+        return self._value
+
+    @property
+    def name(self) -> str:
+        return self._name
 
+    def matches(self, attr: ir.AttrString) -> bool:
+        return attr.value == self.value
 
-class BuilderWithGraphStructure(_GraphStructureAPI):
-    """Very concise graph builder.
+    def to_ir(self, model, bindings=None) -> ir.AttrString:
+        return ir.AttrString(value=self.value, name=self.name)
 
-    It wraps an ONNX graph
-    and builds successors and predecessors on top of it.
-    """
 
-    def __init__(self, bridge: ModelWithGraphStructure):
-        super().__init__()
-        self.bridge: ModelWithGraphStructure = bridge
-        self.input_names: list[str] = []
-        self.output_names: list[str] = []
-        self.nodes: list[oir.Node] = []
-
-    def _build(self) -> None:
-        self.predecessors_: dict[str, int] = {}
-        self.successors_: dict[str, list[int]] = {}
-        self.nodes_: dict[int, oir.Node] = {}
-
-        self.outputs_ = set(self.output_names)
-        for node in self.nodes:
-            self.nodes_[id(node)] = node
-
-        for k, v in self.nodes_.items():
-            assert isinstance(v, oir.Node), f"Unexpected type {type(v)} for node {k}"
-            for o in v.output_names:
-                self.predecessors_[o] = k
-            for i in v.input_names:
-                if i not in self.successors_:
-                    self.successors_[i] = []
-                self.successors_[i].append(k)
-
-    def make_input(self, name: str) -> None:
-        self.input_names.append(name)
-
-    def make_output(self, name: str) -> None:
-        self.output_names.append(name)
-
-    def __getattr__(self, name: str) -> typing.Any:
-        if name in self.__dict__:
-            return self.__dict__[name]
-
-        # unknown name
-        assert (
-            name[0].upper() == name[0]
-        ), f"A node type must starts with an upper letter but it is {name!r}"
-        return lambda *args, _name=name, **kwargs: self._make_node(_name, *args, **kwargs)
+class IntConstantPattern:
+    def __init__(self, value: int, name: str) -> None:
+        self._value = value
+        self._name = name
 
-    def _make_node(
-        self,
-        op_type: str,
-        *args: str,
-        output_names: list[str] | int | None = None,
-        **kwargs: typing.Any,
-    ) -> str | tuple[str]:
-        if output_names is None:
-            # We assume there is only one outputs, we could also check into the schema.
-            output_names = 1
-        return self.make_node(op_type, *args, output_names=output_names, **kwargs)
-
-    def make_node_with_proto(self, node_proto: onnx.NodeProto) -> tuple[str] | str:
-        node = oir.Node(node_proto, True)
-        self.nodes.append(node)
-        assert node.output_names, f"No output in node {node}. This can't be true."
-        if len(node.output_names) == 1:
-            return node.output_names[0]
-        return tuple(node.output_names)
+    @property
+    def value(self) -> int:
+        return self._value
 
-    def make_node(
-        self,
-        op_type: str,
-        *input_names: str,
-        output_names: int | list[str] | str | None = None,
-        domain: str = "",
-        name: str | None = None,
-        **kwargs: typing.Any,
-    ) -> str | tuple[str]:
-        node = oir.Node(
-            self.bridge.make_node(
-                op_type, input_names, output_names, domain=domain, name=name, **kwargs
-            ),
-            True,
+    @property
+    def name(self) -> str:
+        return self._name
+
+    def matches(self, attr: ir.AttrInt64) -> bool:
+        return attr.value == self.value
+
+    def to_ir(self, model, bindings=None) -> ir.AttrInt64:
+        return ir.AttrInt64(value=self.value, name=self.name)
+
+
+class ListConstantPattern:
+    def __init__(self, value: Sequence[int | str | float], name: str) -> None:
+        self._value = value
+        self._name = name
+
+    @property
+    def value(self) -> Sequence[int | str | float]:
+        return self._value
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    def matches(self, attr: ir.AttrFloat32s | ir.AttrInt64s | ir.AttrStrings) -> bool:
+        # TODO: Need more data points to determine if this is the right way to compare lists.
+        return attr.value == self.value
+
+    def to_ir(self, model, bindings=None) -> ir.AttrFloat32s | ir.AttrInt64s | ir.AttrStrings:
+        the_first_non_none_item = next((item for item in self.value if item is not None), None)
+        if isinstance(the_first_non_none_item, int):
+            return ir.AttrInt64s(value=self.value, name=self.name)  # type: ignore
+        if isinstance(the_first_non_none_item, str):
+            return ir.AttrStrings(value=self.value, name=self.name)  # type: ignore
+        if isinstance(the_first_non_none_item, float):
+            return ir.AttrFloat32s(value=self.value, name=self.name)  # type: ignore
+        raise TypeError(
+            f"Cannot convert list of {type(the_first_non_none_item)} to ConstantPattern"
         )
-        self.nodes.append(node)
-        assert node.output_names, f"No output in node {node}. This can't be true."
-        if len(node.output_names) == 1:
-            return node.output_names[0]
-        return tuple(node.output_names)
 
 
-class ModelWithGraphStructure(oir.Model, _GraphStructureAPI):
-    """Implements all the necessary API it needs to work.
+class PrefixPattern:
+    """This pattern is used to simplify submodule opset pattern matching."""
 
-    Wraps a :class:`Model` and builds successors and predecessors on
-    top of it.
-    """
+    def __init__(self, value: str) -> None:
+        self._value = value
 
-    def __init__(self, model: oir.Model, verbose: int = 0):
-        oir.Model.__init__(self)
-        _GraphStructureAPI.__init__(self)
-        self.model = model
-        if hasattr(self.model, "graph"):
-            self.nodes = list(model.graph.nodes)
-            self.input_names = list(model.graph.input_names)
-            self.output_names = list(model.graph.output_names)
-            self._build()
-        else:
-            # empty graph
-            self._unique_names: set = set()
-            self._unique_node_names: set = set()
-        self.verbose = verbose
-
-    def _build(self) -> None:
-        """Builds successor and predecessor."""
-        self.nodes_ = {}
-        self.outputs_ = set(self.output_names)
-        self._unique_node_names = set()
-        for node in self.nodes:
-            self.nodes_[id(node)] = node
-            if node.name:
-                self._unique_node_names.add(node.name)
-
-        self.predecessors_: dict = {}
-        self.successors_: dict = {}
-        # TODO: # initiliazer are missing
-        self._unique_names = set(self.input_names) | set(self.output_names)
-        for k, v in self.nodes_.items():
-            assert isinstance(v, oir.Node), f"Unexpected type {type(v)} for node {k}"
-            for o in v.output_names:
-                self.predecessors_[o] = k
-            for i in v.input_names:
-                if i not in self.successors_:
-                    self.successors_[i] = []
-                self.successors_[i].append(k)
-
-            for sub in enumerate_subgraphs(v):
-                g = sub[-1]
-                sub_knowns = set()
-                for n in g.input:
-                    sub_knowns.add(n.name)
-                for n in g.initializer:
-                    sub_knowns.add(n.name)
-                for n in g.sparse_initializer:
-                    sub_knowns.add(n.name)
-                for n in g.node:
-                    for i in n.input:
-                        if i not in sub_knowns:
-                            # an input coming from the parent
-                            self._unique_names.add(i)
-                    for i in n.output:
-                        sub_knowns.add(i)
+    @property
+    def value(self) -> str:
+        return self._value
 
-    def unique_name(self, prefix: str) -> str:
-        """Generates a unique result name.
+    def matches(self, value: str) -> bool:
+        return value.startswith(self.value)
 
-        That excludes existing names as well.
-        """
-        if prefix in self._unique_names:
-            i = 2
-            sug = f"{prefix}2"
-            while sug in self._unique_names:
-                i += 1
-                sug = f"{prefix}{i}"
-            self._unique_names.add(sug)
-            return sug
-        self._unique_names.add(prefix)
-        return prefix
-
-    def unique_node_name(self, name: str | None) -> str:
-        """Creates a unique node name."""
-        name = name or ""
-        if name in self._unique_node_names:
-            i = 2
-            sug = f"{name}2"
-            while sug in self._unique_node_names:
-                i += 1
-                sug = f"{name}{i}"
-            self._unique_node_names.add(sug)
-            return sug
-        self._unique_node_names.add(name)
-        return name
+    def to_ir(self, model, bindings=None) -> str:
+        raise NotImplementedError("PrefixPattern should not be converted to IR")
 
-    def make_opset(self) -> BuilderWithGraphStructure:
-        return BuilderWithGraphStructure(self)
+
+class FloatConstantPattern:
+    def __init__(
+        self, value: float, name: str, rel_tol: float = 1e-5, abs_tol: float = 1e-8
+    ) -> None:
+        self._value = value
+        self._name = name
+        self._rel_tol = rel_tol
+        self._abs_tol = abs_tol
 
     @property
-    def opsets(self) -> dict:
-        """Property."""
-        return self.model.version_map
+    def value(self):
+        return self._value
 
-    def make_node(
-        self,
-        op_type: str,
-        input_names: str | typing.Sequence[str] | None,
-        output_names: int | typing.Sequence[str] | str | None = 1,
-        domain: str = "",
-        attributes: list[onnx.AttributeProto] | None = None,
-        name: str | None = None,
-        **kwargs: typing.Any,
-    ) -> onnx.NodeProto:
-        """
-        Creates a node without adding it to the graph.
+    @property
+    def name(self):
+        return self._name
 
-        :param op_type: operator type
-        :param input_names: input names
-        :param output_names: outputs names, if one integer, creates n unique names,
-            if str, creates one unique names, if a list, use the name
-        :param domain: node domain
-        :param attributes: list of attributes
-        :param name: node name
-        :param kwargs: other attributes
-        :return: a node
-        """
-        name = self.unique_node_name(name)
-        if isinstance(output_names, int):
-            if output_names == 1:
-                output_names = [self.unique_name(f"{op_type.lower()}")]
-            else:
-                output_names = [
-                    self.unique_name(f"{op_type.lower()}-{i}") for i in range(output_names)
-                ]
-        elif isinstance(output_names, str):
-            output_names = [self.unique_name(output_names)]
-
-        proto = oh.make_node(
-            op_type,
-            (
-                input_names
-                if isinstance(input_names, (list, tuple))
-                else ([input_names] if isinstance(input_names, str) else None)
-            ),
-            output_names,
-            domain=domain,
-            name=name,
-            **kwargs,
+    def matches(self, attr: ir.AttrFloat32):
+        return math.isclose(
+            attr.value, self.value, rel_tol=self._rel_tol, abs_tol=self._abs_tol
         )
-        if attributes:
-            proto.attribute.extend(attributes)
-        return proto
-
-
-class PatternMatchResult:
-    """Stores information about a match if a match was successful.
-
-    * pattern: the instance of :class:`GenericPattern` which found this result
-    * model_nodes: matched nodes coming from the model
-    * pattern_nodes: corresponding nodes coming from the pattern
-    * pattern_input_names: input names of the pattern
-    * pattern_ouptut_names: output names of the pattern
-    * kwargs: additional attributes the user may add through the method
-        :meth:`PatternMatchResult.add_kwargs`
-
-    The class creates one attributes `matched_pattern_to_model_name`,
-    which maps every result name from the pattern to the corresponding
-    result name in the model.
-    """
 
-    def __init__(
-        self,
-        pattern: GenericPattern,
-        model_nodes: typing.Sequence[oir.Node],
-        pattern_nodes: typing.Sequence[oir.Node],
-        pattern_input_names: typing.Sequence[str],
-        pattern_output_names: typing.Sequence[str],
-    ):
-        assert len(model_nodes) == len(pattern_nodes)
-        self.pattern = pattern
-        self.model_nodes = model_nodes
-        self.pattern_nodes = pattern_nodes
-        self.pattern_input_names = pattern_input_names
-        self.pattern_output_names = pattern_output_names
-        self.kwargs = {}
-
-        matched_pattern_to_model_name: dict[str, str] = {}
-        for gn, pn in zip(model_nodes, pattern_nodes):
-            assert (
-                gn.op_type == pn.op_type
-            ), f"Unexpected type mismatch {gn.op_type!r} != {pn.op_type!r}"
-            assert len(gn.input_names) == len(
-                pn.input_names
-            ), f"Unexpected number of inputs for type {gn.op_type}"
-            for a, b in zip(gn.input_names, pn.input_names):
-                if b == "":
-                    # optional input or not an interesting input
-                    continue
-                if b in matched_pattern_to_model_name:
-                    assert matched_pattern_to_model_name[b] == a, (
-                        f"Ambiguities, pattern name {b!r} means "
-                        f"{a!r} or {matched_pattern_to_model_name[b]}"
-                    )
-                else:
-                    matched_pattern_to_model_name[b] = a
+    def to_ir(self, model, bindings=None) -> ir.AttrFloat32:
+        return ir.AttrFloat32(self.name, self.value)
 
-            assert len(gn.output_names) == len(
-                pn.output_names
-            ), f"Unexpected number of outputs for type {gn.op_type}"
-            for a, b in zip(gn.output_names, pn.output_names):
-                if b == "":
-                    # Only final outputs are interesting.
-                    continue
-                assert a != "", f"{a!r} cannot be optional"
-                if b in matched_pattern_to_model_name:
-                    assert matched_pattern_to_model_name[b] == a, (
-                        f"Ambiguities, pattern name {b!r} means "
-                        f"{a!r} or {matched_pattern_to_model_name[b]}"
-                    )
-                else:
-                    matched_pattern_to_model_name[b] = a
 
-        self.matched_pattern_to_model_name = matched_pattern_to_model_name
+class TensorConstantPattern:
+    def __init__(
+        self, value: ir.TensorProtocol, name, rel_tol: float = 1e-3, abs_tol: float = 1e-3
+    ) -> None:
+        self._value = value
+        self._name = name
+        self._rel_tol = rel_tol
+        self._abs_tol = abs_tol
 
-    def add_kwargs(self, name: str, value: typing.Any):
-        """Adds an attribute, it can be done when the match is being validated,
-        this attribute can be used when building the replacement nodes.
-        """
-        self.kwargs[name] = value
+    @property
+    def value(self):
+        return self._value
 
-    def __repr__(self) -> str:
+    @property
+    def name(self):
+        return self._name
+
+    def matches(self, attr: ir.AttrTensor):
         return (
-            f"{self.__class__.__name__}([{self.pattern.__class__.__name__}], "
-            f"... {len(self.model_nodes)} nodes ..., {self.pattern_input_names}, "
-            f"{self.pattern_output_names})"
+            attr.value.dtype == self._value.dtype
+            and attr.value.shape == self._value.shape
+            and np.allclose(
+                attr.value,
+                self._value,
+                rtol=self._rel_tol,
+                atol=self._abs_tol,
+            )
         )
 
+    def to_ir(self, model, bindings=None) -> ir.AttrTensor:
+        return ir.AttrTensor(self.name, self.value)
 
-class GenericRewriteRule(orp.RewriteRule):
-    """
-    Defines a rewriting rule.
 
-    :param pattern: a pattern defines by :class:`GenericPattern`.
+def _make_constant_pattern(
+    value: float | int | Sequence | ir.TensorProtocol, name: str
+) -> (
+    IntConstantPattern
+    | FloatConstantPattern
+    | TensorConstantPattern
+    | StringConstantPattern
+    | ListConstantPattern
+):
+    """Convert an attrbute value to a ConstantPattern."""
+    if isinstance(value, float):
+        return FloatConstantPattern(value, name)
+    if isinstance(value, int):
+        return IntConstantPattern(value, name)
+    if isinstance(value, str):
+        return StringConstantPattern(value, name)
+    if isinstance(value, Sequence):
+        return ListConstantPattern(value, name)
+    if isinstance(value, ir.TensorProtocol):
+        return TensorConstantPattern(value, name)
+    raise TypeError(f"Cannot convert {type(value)} to ConstantPattern")
+
+
+class AnyPattern:
+    def matches(self, value) -> bool:
+        return True
+
+
+class AttrPattern:
+    def __init__(
+        self, value: Var | int | float | Sequence | ir.TensorProtocol, name: str
+    ) -> None:
+        if isinstance(value, Var):
+            self.value_pattern = value
+        elif isinstance(value, (int, float, Sequence, ir.TensorProtocol)):
+            self.value_pattern = _make_constant_pattern(value, name)  # type: ignore[assignment]
+        else:
+            raise TypeError(f"Cannot convert {type(value)} to AttrPattern")
+
+    def matches(
+        self,
+        attr_val: int | float | Sequence | Var | ir.TensorProtocol | ir.Value,
+        model: ir.Model,
+    ) -> MatchResult:
+        if isinstance(self.value_pattern, Var):
+            return self.value_pattern.matches(attr_val, model)  # type: ignore[arg-type]
+        return self.value_pattern.matches(attr_val)
+
+    def to_ir(self, model: ir.Model, rewrite_cache: RewriteCache, bindings=None) -> ir.Value:
+        if isinstance(self.value_pattern, Var):
+            val, nodes = self.value_pattern.to_ir(
+                model, bindings, 1, rewrite_cache
+            )  # TODO: handle multiple outputs
+            return val
+        # constant pattern
+        return self.value_pattern.to_ir(model, bindings)
+
+
+class OpsetPattern:
+    """Represents an opset pattern.
+
+    It is used primarily to create a NodePattern (via OpPattern).
+    Example usage:
+    ::
+
+        z = op.Matmul(x, y)
+
+    Here, `op` is an instance of OpsetPattern and `op.Matmul` is an instance
+    of OpPattern, and  `op.Matmul(x, y)` is an instance of NodePattern.
+
+    An opset pattern is also matched against the actual opset used in the
+    input model. Typically, we match against an ONNX opset (ignoring the
+    version), but we can match against a specific version of the opset too.
+    However, it is preferable that version-dependences are handled at the
+    level of a rewrite rule, rather than at the level of a pattern.
+
     """
 
-    def __init__(self, pattern: GenericPattern):
-        self.pattern = pattern
+    def __init__(
+        self,
+        domain_pattern: PythonPattern | PrefixPattern,
+        version_pattern: PythonPattern | AnyPattern,
+    ) -> None:
+        self.domain_pattern = domain_pattern
+        self.version_pattern = version_pattern
 
-    def matches(self, node: oir.Node, model: oir.Model) -> orp.MatchResult:
-        del model
-        del node
-        raise RuntimeError(f"This pattern {self} is meant to replace not to only match.")
+    @classmethod
+    def singleton(cls, domain: str, version: int) -> OpsetPattern:
+        return cls(PythonPattern(domain), PythonPattern(version))
 
-    def try_rewrite(
-        self, model: oir.Model, node: oir.Node
-    ) -> tuple[int, list[oir.Node], list[oir.Node]] | None:
-        """See :meth:`RewriteRule.try_rewrite`."""
-        if isinstance(model, ModelWithGraphStructure):
-            bridge = model
-        else:
-            bridge = ModelWithGraphStructure(model)
-        deleted_nodes = []
-        added_nodes = []
-        marked = set()
-        matched = 0
-        for match_result in self.pattern.enumerate_matches(bridge, node):
-            conflict = False
-            for node in match_result.model_nodes:
-                if id(node) in marked:
-                    conflict = True
-                    break
-            if conflict:
-                # Some nodes are already marked as rewritten.
-                continue
-
-            # Let's build the new nodes
-            if not self.pattern.validate_mapping(bridge, match_result):
-                match_result._hint(
-                    "validate_mapping", "The pattern was rejected by the validation function."
-                )
-                continue
+    @classmethod
+    def domain(cls, domain: str) -> OpsetPattern:
+        return cls(PythonPattern(domain), AnyPattern())
 
-            new_nodes = self.pattern.apply(bridge, match_result)
-            assert all(
-                isinstance(i, oir.Node) for i in new_nodes
-            ), f"Unexpected types {[type(n) for n in new_nodes]}"
-
-            # Everything is good.
-            marked |= set(map(id, match_result.model_nodes))
-            added_nodes.extend(new_nodes)
-            deleted_nodes.extend(match_result.model_nodes)
-            matched += 1
+    @classmethod
+    def domain_prefix(cls, domain: str) -> OpsetPattern:
+        return cls(PrefixPattern(domain), AnyPattern())
 
-        if matched > 0:
-            return matched, deleted_nodes, added_nodes
-        return None
+    def matches(self, opset):
+        domain, version = opset
+        return self.domain_pattern.matches(domain) and self.version_pattern.matches(version)
 
-    def count_matches(self, model: oir.Model, *, commute: bool = False) -> int:
-        """See :meth:`RewriteRule.count_matches`."""
-        raise NotImplementedError("Not supported yet.")
+    def to_ir(self, model, bindings=None) -> str:
+        domain = self.domain_pattern.to_ir(model, bindings)
+        assert isinstance(domain, str), f"Expected str, got {type(domain)}"
+        # TODO: Should we ban other custom domains?
+        if domain not in model.opset_imports:
+            assert isinstance(
+                self.version_pattern, PythonPattern
+            ), f"custom domain {domain} needs to have a specific version."
+            model.opset_imports[self.domain_pattern.value] = self.version_pattern.value
+        return domain
 
-    def commute(self) -> list[orp.RewriteRule]:
-        """See :meth:`RewriteRule.commute`."""
-        raise RuntimeError("Not supported (yet?). It could lead to many patterns.")
+    def __getattr__(self, name: str) -> Any:
+        return OpPattern(self, PythonPattern(name))
 
-    def apply_to_model(self, model: oir.Model, *, commute: bool = False) -> int:
-        """See :meth:`RewriteRule.apply_to_model`."""
-        return orp.RewriteRuleSet([self], commute=commute).apply_to_model(model)
+    def submodule(self, name: str) -> Any:
+        """This method is used to match against submodule ops with prefix."""
+        return OpPattern(self, PrefixPattern(name))
 
 
-class GenericPattern:
-    """
-    Implements a pattern optimization for quick experimentation.
+opset17 = OpsetPattern.singleton("", 17)
 
-    Current limitation:
+onnxop = OpsetPattern.domain("")
 
-    * The current implementation does match on domain name (easy fix).
-    * It does not compares attributes either (easy fix as well).
-    """
+msft_op = OpsetPattern.singleton("com.microsoft", 1)
 
-    def __init__(self, verbose: int = 0):
-        self.verbose = verbose
-        self._cache: dict = {}
-
-    def validate_mapping(self, g: oir.Model, match_result: PatternMatchResult) -> bool:
-        """Evaluates the consistency of the replacements."""
-        raise NotImplementedError(
-            "This method could return True but it is better to let you know "
-            "that it exists. You need to overwrite it to return True."
-        )
+torch_module_op = OpsetPattern.domain_prefix("pkg.torch")
 
-    def enumerate_matches(
-        self, g: ModelWithGraphStructure, node: oir.Node | None = None
-    ) -> typing.Iterator:
-        """Enumerates all the matches."""
-        if node is None:
-            matched = []
-            for node in g.nodes:
-                res = self.match(g, node)
-                if res:
-                    matched.append(res)
-                    yield res
-        else:
-            res = self.match(g, node)
-            if res:
-                yield res
 
-    def none(
+class OpPattern:
+    """A utility class to build a NodePattern.
+
+    It is used primarily to create a NodePattern.
+    Example usage:
+    ::
+
+        z = op.Matmul(x, y)
+
+    Here, `op` is an instance of OpsetPattern and `op.Matmul` is an instance
+    of OpPattern, and  `op.Matmul(x, y)` is an instance of NodePattern.
+
+    """
+
+    def __init__(
         self,
-        node: oir.Node | None = None,
-        lineno: int | None = None,
-        msg: str = "",
+        opset_pattern: OpsetPattern,
+        op_name_pattern: PythonPattern | PrefixPattern,
     ) -> None:
-        """Must be called every time a match fails to trace it.
+        self.opset_pattern = opset_pattern
+        self.op_name_pattern = op_name_pattern
 
-        It may be useful which reason made a pattern matching fail.
-        Instead of returning None, method *match* can return the following
-        expression:
-
-        ::
-
-            return self.none(node, inspect.currentframe().f_lineno)
-
-        By setting the verbosity (see next Section), the user may then know
-        which lines in the code returned None and which condition failed.
-        If logs are fully enabled, it shows informations about matched none
-        and the line deciding the matched failed.
-        For example, this tells the matching failed at line 601 in ``generic_pattern.py``.
-        It happens when propagating the match in the backward directions.
-        The unmatched types are Mul, MatMul and below,
-        it shows the matched nodes. The first one was Cast.
-        And the failure happened at iteration 5.
-        ``139774002356544-139774000632672`` is the pair of ids used in container ``marked``.
-        ``id(node)`` is used as a unique identifiers of the nodes.
-
-        ::
-
-            [RotaryEmbeddingPattern.match] NONE - line: 601:__main__, op_type=Cast
-                --hint--: BACKWARD: different node types
-                --pattern
-                Mul(pos_ids, cast) -> (mul)
-                -- model
-                MatMul(/_original_modu...Expand_output_0, /_original_modu...b/Cast_output_0) -> (/_original_modu...MatMul_output_0)
-                iteration=5
-                --marked-- #6
-                Cast(/_original_modu...mb/Cos_output_0) ~ Cast(cos) [139774002356544-139774000632672]
-                Cos(/_original_modu...ncat_1_output_0) ~ Cos(concattraining-transpose-0) [139774002356448-139774000632048]
-                ConcatTraining(/_original_modu...nspose_output_0,/_original_modu...nspose_output_0) ~ ConcatTraining(transpose,transpose) [139774002356352-139774000631712]
-                Transpose(/_original_modu...MatMul_output_0) ~ Transpose(mul) [139774002356256-139774000631184]
-                Sin(/_original_modu...ncat_1_output_0) ~ Sin(concattraining-transpose-0) [139774002358512-139774000631568]
-                Cast(/_original_modu...mb/Sin_output_0) ~ Cast(sin) [139774002358608-139774000632384]
-                len(stacked)=0:[]
+    def __call__(self, *args, **kwargs):
+        if "_num_outputs" in kwargs:
+            num_outputs = kwargs["_num_outputs"]
+            del kwargs["_num_outputs"]
+        else:
+            num_outputs = 1
+        attributes = {
+            name: AttrPattern(value=value, name=name) for (name, value) in kwargs.items()
+        }
+        node_pattern = NodePattern(self.opset_pattern, self.op_name_pattern, args, attributes)
+        if num_outputs == 1:
+            return NodeOutputPattern(node_pattern, 0)
+        else:
+            return [NodeOutputPattern(node_pattern, i) for i in range(num_outputs)]
 
-        'hints' are not added everywhere. More can easily be added with method ``_hint``.
-        """
-        if node and self.verbose:
-            if self.verbose >= 10:
-                if hasattr(self, "_debug"):
-                    msg2 = self._debug_print()
-                    if msg2:
-                        msg2 = f"\n{textwrap.indent(msg2, '    ')}"
-                else:
-                    msg2 = ""
-                print(
-                    f"[{self.__class__.__name__}.match] NONE - line: {lineno}:"
-                    f"{os.path.split(self.__class__.__module__)[-1]}, "
-                    f"op_type={node.op_type}{msg}{msg2}"
-                )
+
+def _to_value_pattern(
+    x: ValuePattern | int | float,
+) -> NodeOutputPattern | Constant | Var | ValuePattern:
+    """Promotes an input-value used to construct a NodePattern to a ValuePattern.
+
+    Example usage:
+    ::
+        x = op.MatMul(a, b)
+        z = op.Add(x, 0)
+
+    In this example, `a, `b`, and `x` are ValuePatterns used to construct a NodePattern.
+    `0` is a constant (int) value, and is automatically promoted to a ValuePattern.
+
+    Note that this is a shorthand for creating a Constant pattern. The user can more
+    explicitly write this as:
+    ::
+        z = op.Add(x, op.Constant(0))
+    """
+    if isinstance(x, ValuePattern):
+        return x
+    if isinstance(x, (int, float, Sequence)):
+        return Constant(x)
+    # TODO(titaiwang): Could this be wrapped Constant?
+    raise TypeError(f"Cannot convert {type(x)} to ValuePattern")
+
+
+class MatchResult:
+    """Represents the result of a match operation.
+
+    A match can either succeed or fail.
+    If it succeeds, it returns a list of IR values that matched the pattern
+    and a set of bindings for the variables in the pattern.
+
+    Example:
+    ::
+        def pattern(x, shape1, shape2):
+            t1 = op.Reshape(x, shape1)
+            t2 = op.Reshape(t1, shape2)
+            return t2
+    The above pattern matches a sequence of two Reshape ops.
+    The matched_values will contain the values representing the (output of)
+    the two Reshape ops, and the bindings will contain the values that
+    are bound to the variables `x`, `shape1`, and `shape2`.
+    """
+
+    def __init__(
+        self, matched_values=None, bindings: dict[str, ir.Value | Any] | None = None
+    ) -> None:
+        assert matched_values is None or isinstance(matched_values, list)
+        self.success: bool = matched_values is not None
+        # For a successful match, matched_values is a list of values that matched the pattern.
+        # These include the internal nodes of the pattern that were matched, but not
+        # the leaves (sub-trees) that match against the variables in the pattern.
+        # These represent the values that will be replaced by the replacement pattern.
+        self.matched_values: Sequence[Any] | None = matched_values
+        # For a successful match, bindings is a dictionary of mapping pattern-variable-names
+        # to values.
+        self.bindings: dict[str, Any] = bindings if bindings is not None else {}
+
+    def __bool__(self):
+        return self.success
 
     @classmethod
-    def match_pattern(
-        cls,
-        g: ModelWithGraphStructure,
-        *args: str,
-        **kwargs: typing.Any,
-    ) -> list[oir.Node] | None:
-        """Builds the pattern to match."""
-        raise NotImplementedError(
-            f"Class {cls.__name__!r} must overwrite method match_pattern."
-        )
+    def FAIL(cls):
+        return cls(None)
+
+    @property
+    def values(self) -> Sequence[Any] | None:
+        return self.matched_values
+
+    def fail(self):
+        self.success = False
+        self.matched_values = None
+        self.bindings = {}
+
+    def extend(self, other: MatchResult | bool, model):
+        del model  # Unused
+        if not self.success:
+            return
+        if not other:
+            self.fail()
+            return
+        if isinstance(other, bool):
+            return
+        for var, val in other.bindings.items():
+            if var in self.bindings:
+                # TODO: handle attribute var bindings
+                if self.bindings[var] != val:
+                    self.fail()
+                    return
+            else:
+                self.bindings[var] = val
+        assert self.matched_values is not None, "matched_values should not be None."
+        self.matched_values.extend(other.matched_values)  # type: ignore[attr-defined]
+
+
+class ValuePattern:
+    """Base class for all patterns that match against IR values.
+
+    This is used primarily to provide operator overloadings for arithmetic
+    operations, so that we can write patterns like `x + 1` and `1 + x`.
+    """
+
+    def __init__(self) -> None:
+        pass
+
+    def __add__(self, other):
+        return onnxop.Add(self, other)
+
+    def __radd__(self, other):
+        return onnxop.Add(other, self)
+
+    def __sub__(self, other):
+        return onnxop.Sub(self, other)
+
+    def __rsub__(self, other):
+        return onnxop.Sub(other, self)
 
-    def _build_pattern(
+    def __mul__(self, other):
+        return onnxop.Mul(self, other)
+
+    def __rmul__(self, other):
+        return onnxop.Mul(other, self)
+
+    def __truediv__(self, other):
+        return onnxop.Div(self, other)
+
+    def __rtruediv__(self, other):
+        return onnxop.Div(other, self)
+
+    def __pow__(self, other):
+        return onnxop.Pow(self, other)
+
+
+class NodePattern:
+    """Represents a pattern that matches against a Node.
+
+    This differs from a NodeOutputPattern in that it matches against a node (which
+    may produce 1 or more outputs), whereas a NodeOutputPattern matches against
+    a specific output of a node.
+    """
+
+    def __init__(
         self,
-        g: ModelWithGraphStructure,
-        fct: typing.Callable | None = None,
-        match: bool = True,
-        kwargs: dict[str, typing.Any] | None = None,
-    ) -> BuilderWithGraphStructure:
-        del match
-        assert fct, f"Not implemented if fct is None in class {self.__class__.__name__}"
-        assert not kwargs, (
-            f"Not implemented when kwargs is not empty but {kwargs} "
-            f"in class {self.__class__.__name__}"
+        domain: OpsetPattern,
+        op: PythonPattern | PrefixPattern,
+        inputs: Sequence[int | float | ValuePattern],
+        attributes: dict[str, AttrPattern],
+    ):
+        self.domain = domain
+        self.op = op
+        self.inputs = [_to_value_pattern(x) for x in inputs]
+        self.attributes = attributes
+        self.bound_value = None
+
+    def matches(self, value: ir.Value, model: ir.Model):
+        if self.bound_value is not None:
+            # DAG-matching, not Tree-matching.
+            if self.bound_value.is_same_as(value):
+                return MatchResult([])
+            else:
+                return MatchResult.FAIL()
+        node = value.producer()
+        if node is None:
+            # Eg., value could be an input parameter, which will not match a value
+            # computed by the op in this pattern.
+            return MatchResult.FAIL()
+        return self.matches_node(node, model)
+
+    def matches_node(self, node: ir.Node, model: ir.Model) -> MatchResult:
+        """Examine if the IR node matches the self pattern."""
+        node_version = model.graph.opset_imports.get(node.domain, 0)
+        if not self.domain.matches((node.domain, node_version)):
+            return MatchResult.FAIL()
+        if not self.op.matches(node.op_type):
+            return MatchResult.FAIL()
+        match = MatchResult([])
+        # TODO: We should add filtered logging starting from here to emit why
+        # matching failed. This should cut a lot of noises compared to logging everything,
+        # because at least the starting node op_type is already matched.
+        for arg_value, previous_node_output_pattern in zip(node.inputs, self.inputs):
+            # previous_node_output_pattern could be a Var, if it's the original arg.
+            sub_match = previous_node_output_pattern.matches(arg_value, model)  # type: ignore[attr-defined]
+            match.extend(sub_match, model)
+            if not match:  # If sub-match failed,
+                return match
+        # Sub-graphs not handled yet.
+        for name, attr_pattern in self.attributes.items():
+            attr_value = node.attributes.get(name)
+            if attr_value is None:
+                return MatchResult.FAIL()
+            sub_match = attr_pattern.matches(attr_value, model)  # type: ignore[arg-type]
+            if not sub_match:
+                return MatchResult.FAIL()
+            match.extend(sub_match, model)
+        for name in node.attributes:
+            # TODO: Support matching default values for attributes.
+            if name not in self.attributes:
+                return MatchResult.FAIL()
+        assert match.values is not None, "Matched values should not be None."
+        match.values.append(node)  #  type: ignore[attr-defined]
+        return match
+
+    def to_ir(
+        self,
+        model: ir.Model,
+        bindings: dict[str, ir.Value | Any],
+        num_outputs: int,
+        rewrite_cache: RewriteCache,
+    ) -> tuple[Sequence[ir.Value], Sequence[ir.Node]]:
+        domain = self.domain.to_ir(model)
+        op = self.op.to_ir(model)
+        assert isinstance(op, str), f"Expected str, got {type(op)}"
+        inputs = []
+        nodes: list[ir.Node] = []
+        for val_pattern in self.inputs:
+            if (
+                value_and_node := rewrite_cache.get_node_output_pattern(val_pattern)  # type: ignore[arg-type]
+            ) is not None:
+                val, n = value_and_node
+            else:
+                val, n = val_pattern.to_ir(model, bindings, 1, rewrite_cache)  # type: ignore[attr-defined]
+                rewrite_cache.set_node_output_pattern_with_ir(val_pattern, val, n)  # type: ignore[arg-type]
+                nodes.extend(n)  # type: ignore[arg-type]
+            # If one of the inputs was a the output of a previous node,
+            # unpack the new output ir value that is created for that node
+            if isinstance(val, tuple):
+                # TODO: Move implementation of output_index to NodeOutputPatter.to_ir
+                inputs.append(val[val_pattern.output_index])
+            else:
+                inputs.append(val)
+        attributes = (
+            attr_pattern.to_ir(model, rewrite_cache, bindings)
+            for attr_pattern in self.attributes.values()
         )
-        kwargs = {}
-        args = []
+        new_node = ir.Node(
+            domain=domain,
+            op_type=op,
+            inputs=inputs,
+            attributes=attributes,  # type: ignore[arg-type]
+            num_outputs=num_outputs,
+        )
+        nodes.append(new_node)
+        return new_node.outputs, nodes
+
+    def commute(self) -> Sequence[NodePattern]:
+        list_of_lists = [pattern.commute() for pattern in self.inputs]  # type: ignore[attr-defined]
 
-        # There should be a better way.
-        sig = inspect.signature(fct)
-        for i, p in enumerate(sig.parameters.values()):
-            if i == 0:
-                continue
-            if p.default is not inspect._empty:
-                # an attribute
-                kwargs[p.name] = p.default
+        def enumerate_inputs(inputs, index):
+            if index >= len(inputs):
+                yield []
             else:
-                args.append(p.name)
+                for pattern in inputs[index]:
+                    for rest in enumerate_inputs(inputs, index + 1):
+                        yield [pattern, *rest]
+
+        inputs = list(enumerate_inputs(list_of_lists, 0))
+        if self.domain.matches(("", None)) and (
+            self.op.matches("Add") or self.op.matches("Mul")
+        ):
+            # TODO: handle cases where number of inputs is not 2.
+            swapped = [[x[1], x[0]] for x in inputs]
+            inputs.extend(swapped)
+        return [NodePattern(self.domain, self.op, input, self.attributes) for input in inputs]
 
-        assert len(kwargs) == 0, f"Attributes are not supported yet but kwargs={kwargs}"
 
-        g2 = g.make_opset()
-        for name in args:
-            g2.make_input(name)
-        output = fct(g2, *args, **kwargs)
-        if isinstance(output, str):
-            g2.make_output(output)
-        else:
-            for name in output:
-                g2.make_output(name)
-        g2._build()
-        return g2
-
-    def _get_match_pattern(self, g: ModelWithGraphStructure) -> BuilderWithGraphStructure:
-        cache_key = 0, tuple(sorted(g.opsets.items()))
-        if cache_key in self._cache:
-            return self._cache[cache_key]
-
-        pat = self._build_pattern(g, fct=self.match_pattern, match=True)
-        self._cache[cache_key] = pat
-        return pat
-
-    def _get_apply_pattern(self, g: ModelWithGraphStructure) -> BuilderWithGraphStructure:
-        cache_key = 1, tuple(sorted(g.opsets.items()))
-        if cache_key in self._cache:
-            return self._cache[cache_key]
-
-        pat = self._build_pattern(g, fct=self.apply_pattern, match=False)
-        self._cache[cache_key] = pat
-        return pat
-
-    def print_match(self, n1: oir.Node, n2: oir.Node) -> str:
-        s1 = f"{n1.op_type}({','.join(n1.input_names)})"
-        s2 = f"{n2.op_type}({','.join(n2.input_names)})"
-        return f"match {s1} with {s2} (pattern)"
-
-    def _debug_print(self) -> str:
-        if not hasattr(self, "_debug"):
-            return ""
-
-        def _s(s: str) -> str:
-            if len(s) <= 30:
-                return s
-            return f"{s[:15]}...{s[-15:]}"
-
-        def _p(n: oir.Node, full: bool = False) -> str:
-            if isinstance(n, (oir.Node, onnx.NodeProto)):
-                if full:
-                    return (
-                        f"{n.op_type}({', '.join(map(_s, n.input_names))}) "
-                        f"-> ({', '.join(map(_s, n.output_names))})"
-                    )
-                return f"{n.op_type}({','.join(map(_s, n.input_names))})"
-            return str(n)
+class NodeOutputPattern(ValuePattern):
+    """Represents a pattern that matches against a specific output of a Node.
+
+    This is the primary pattern used to match against computed values, that
+    is values computed using a specific op.
+    """
 
-        rows = []
-        for k, v in sorted(self._debug.items()):
-            if k == "stacked":
-                rows.append(f"len({k})={len(v)}:{v}")
-                continue
-            if k == "iteration":
-                rows.append(f"{k}={v}")
-                continue
-            if k == "marked":
-                rows.append(f"--marked-- #{len(v)}")
-                for i, tu in v.items():
-                    rows.append(f"  {_p(tu[0])} ~ {_p(tu[1])} [{id(tu[0])}-{i}]")
-                continue
-            if k == "hint":
-                rows.append(f"--hint--: {v[0]}")
-                for i in v[1:]:
-                    rows.append("  " + _p(i, full=True))
-                continue
-            if k in {"node", "pattern", "pattern_node", "pattern_nodes"}:
-                continue
-            rows.append(f"-- not shown {k}")
-
-        return "\n".join(rows)
-
-    def _hint(self, *args: typing.Any) -> None:
-        """Add debugging information to help users."""
-        self._debug["hint"] = args
+    def __init__(self, node_pattern: NodePattern, output_index: int) -> None:
+        self.node_pattern = node_pattern
+        self.output_index = output_index
+
+    def matches(self, value: ir.Value, model: ir.Model):
+        """Match the StaticValueInfo from IR with the `matches_node()` in node pattern."""
+        node = value.producer()
+        if node is None:
+            return MatchResult.FAIL()
+        if value.index() != self.output_index:
+            return MatchResult.FAIL()
+        return self.node_pattern.matches_node(node, model)
 
-    def _match_backward(
+    def to_ir(
         self,
-        g: ModelWithGraphStructure,
-        node: oir.Node,
-        pat: ModelWithGraphStructure,
-        marked: dict[int, tuple[oir.Node, oir.Node]],
-        stacked: list[int],
-        n: oir.Node,
-        pn: oir.Node,
-    ) -> int | None:
-        """
-        Matches backward.
+        model: ir.Model,
+        bindings: dict[str, ir.Value | Any],
+        num_outputs: int,
+        rewrite_cache: RewriteCache,
+    ) -> tuple[Sequence[ir.Value], Sequence[ir.Node]]:
+        assert self.output_index == 0, "TODO: handle multiple outputs"
+        return self.node_pattern.to_ir(model, bindings, num_outputs, rewrite_cache)
 
-        :param g: graph
-        :param node: root node (the node the matched begain with,
-            used only for debugging)
-        :param pat: pattern
-        :param marked: nodes of the pattern marked as already matched
-        :param stacked: next node to look into
-        :param n: node coming from the graph
-        :param pn: node coming from the pattern
-        :return: number of matched nodes, None or False to indicate a failed match
-        """
-        res = 0
 
-        # predecessors
-        if len(n.input_names) != len(pn.input_names):
-            # not the same number of inputs
-            self._hint(
-                "BACKWARD: not the same number of inputs",
-                "-- pattern",
-                pn,
-                "-- model",
-                n,
-            )
-            return self.none(node, inspect.currentframe().f_lineno)
-        for i, pi in zip(n.input_names, pn.input_names):
-            ppred = pat.node_before(pi)
-            if ppred is None:
-                # ppred is None means the pattern ends here.
-                continue
-            pred = g.node_before(i)
-            if pred is None:
-                # No node in the graph.
-                return self.none(node, inspect.currentframe().f_lineno)
-            if pred.op_type != ppred.op_type:
-                self._hint(
-                    "BACKWARD: different node types",
-                    "--pattern",
-                    ppred,
-                    "-- model",
-                    pred,
-                )
-                return self.none(node, inspect.currentframe().f_lineno)
-            # matching backward
-            key = id(ppred)
-            if key not in marked:
-                if self.verbose >= 10:
-                    print(f"[GenericPattern._match_backward] {self.print_match(pred, ppred)}")
-                marked[key] = pred, ppred
-                stacked.append(key)
-                res += 1
-        if self.verbose > 5 and res > 0:
-            print(f"[GenericPattern._match_backward] add {res} nodes")
-        return res
+class Var(ValuePattern):
+    """Represents a pattern variable."""
+
+    def __init__(self, name: str) -> None:
+        self.pattern_var_name = name
+        self.bound_value = None
+
+    def __repr__(self) -> str:
+        return f"Var({self.pattern_var_name!r})"
 
-    def _match_forward(
+    def matches(self, value: ir.Value, model: ir.Model):
+        return MatchResult([], {self.pattern_var_name: value})
+
+    def to_ir(
         self,
-        g: ModelWithGraphStructure,
-        node: oir.Node,
-        pat: ModelWithGraphStructure,
-        marked: dict[int, tuple[oir.Node, oir.Node]],
-        stacked: list[int],
-        n: oir.Node,
-        pn: oir.Node,
-    ) -> int | None:
-        """
-        Matches forward.
+        model: ir.Model,
+        bindings: dict[str, ir.Value | Any],
+        num_outputs: int,
+        rewrite_cache: RewriteCache,
+    ) -> tuple[ir.Value, Sequence]:
+        del model  # Unused
+        del num_outputs  # Unused
+        del rewrite_cache  # Unused
+        return bindings[self.pattern_var_name], []
 
-        :param g: graph
-        :param node: root node (the node the matched begain with,
-            used only for debugging)
-        :param pat: pattern
-        :param marked: nodes of the pattern marked as already matched
-        :param stacked: next node to look into
-        :param n: node coming from the graph
-        :param ns: node coming from the pattern
-        :return: number of matched nodes to continue, None or False to indicate a failed match
-        """
-        res = 0
+    def commute(self) -> Sequence[ValuePattern]:
+        return [self]
 
-        # successors
-        if len(n.output_names) != len(pn.output_names):
-            # not the same number of outputs
-            self._hint(
-                "FORWARD: not the same number of output_names",
-                "-- pattern",
-                pn,
-                "-- model",
-                n,
-            )
-            return self.none(node, inspect.currentframe().f_lineno)
 
-        for o, op in zip(n.output_names, pn.output_names):
-            ns = g.next_nodes(o)
-            pns = pat.next_nodes(op)
-            if len(pns) == 0:
-                # The pattern has no node forward, the matching stops.
-                continue
-            if len(ns) < len(pns):
-                # Not enough node in the graph to match the pattern,
-                # the result is known.
-                return self.none(node, inspect.currentframe().f_lineno)
-
-            # Here comes the fun part, there is the same number of successors or more
-            # nodes in the graph to match with the pattern.
-            # And we have to handle the nodes already marked as found.
-            # Hopefully, there is only one option.
-
-            if len(ns) == len(pns) == 1:
-                # Let's deal with the simple case
-                if ns[0].op_type != pns[0].op_type:
-                    return self.none(node, inspect.currentframe().f_lineno)
-
-                key = id(pns[0])
-                if key not in marked:
-                    if self.verbose >= 10:
-                        print(
-                            f"[GenericPattern._match_forward]{self.print_match(ns[0], pns[0])}"
-                        )
-                    marked[key] = ns[0], pns[0]
-                    stacked.append(key)
-                    res += 1
-                continue
-
-            # Let's remove the nodes already marked.
-            p_marked = [_ for _ in pns if id(_) not in marked]
-            id_marked = [id(marked[id(_)][0]) for _ in pns if id(_) in marked]
-            assert len(id_marked) + len(p_marked) == len(pns), (
-                f"Unexpected, id_marked={id_marked}, "
-                f"id_p_marked={set(map(id, p_marked))}, "
-                f"pns_ids={set(map(id, pns))}, "
-                f"ns_ids={set(map(id, ns))}, o={o!r}, op={op!r}, "
-                f"n.op_type={n.op_type!r}, "
-                f"n.output={n.output}, np.output={pn.output}, "
-                f"ns_types={ {_.op_type for _ in ns} }, "
-                f"pns_types={ {_.op_type for _ in pns} }"
-            )
-            free = [_ for _ in ns if id(_) not in id_marked]
-            if len(p_marked) == 0:
-                # Everything is already marked.
-                continue
-            if len(free) < len(p_marked):
-                # Not enough successors to match the remaining patterns.
-                return self.none(node, inspect.currentframe().f_lineno)
-            if len(p_marked) == len(free) == 1:
-                # Only one option again.
-                if p_marked[0].op_type != free[0].op_type:
-                    return self.none(node, inspect.currentframe().f_lineno)
-
-                key = id(p_marked[0])
-                if key not in marked:
-                    if self.verbose >= 10:
-                        print(
-                            f"[GenericPattern._match_forward] {self.print_match(free[0], p_marked[0])}"
-                        )
-                    marked[key] = free[0], p_marked[0]
-                    stacked.append(key)
-                    res += 1
-                continue
-
-            # And now another fun part, let's try to handle the case when
-            # there is only one option, matching on node type only returns one
-            # option.
-            expected_op_type = [_.op_type for _ in p_marked]
-            got_op_type = [_.op_type for _ in free]
-
-            ec = collections.Counter(expected_op_type)
-            gc = collections.Counter(got_op_type)
-            if len(ec) != len(gc) or set(ec) != set(gc):
-                # unique operator types is different.
-                self._hint(
-                    "FORWARD: unique operator types are different",
-                    "-- pattern",
-                    ec,
-                    pn,
-                    "-- model",
-                    gc,
-                    n,
-                    "-- model-marked",
-                    id_marked,
-                )
-                return self.none(node, inspect.currentframe().f_lineno)
-            for k, v in ec.items():
-                if gc[k] < v:
-                    # Not enough types to match.
-                    return self.none(node, inspect.currentframe().f_lineno)
-
-            # At this stage, we know matching the types is possible.
-            # We first mark whatever is possible.
-            ptype_to_node = {_.op_type: _ for _ in p_marked}
-            gtype_to_node = {_.op_type: _ for _ in got_op_type}
-            missing = []
-            for k, v in ec.items():
-                if gc[k] == v == 1:
-                    key = id(ptype_to_node[k])
-                    if key not in marked:
-                        if self.verbose >= 10:
-                            print(
-                                f"[GenericPattern._match_forward] match "
-                                f"{self.print_match(gtype_to_node[k], ptype_to_node[k])}"
-                            )
-                        marked[key] = gtype_to_node[k], ptype_to_node[k]
-                        stacked.append(key)
-                        res += 1
-                else:
-                    missing.append(k)
-
-            if not missing:
-                continue
-
-            # At this stage, there are mutiple options for matching. We can:
-            # 1. make assumptions and continue
-            # 2. mark the node as incomplete matching, we could end up stuck anyway.
-            raise AssertionError(
-                f"There are more than one option, this will be implemented later, "
-                f"ec={ec}, gc={gc}"
-            )
-        if self.verbose > 5 and res > 0:
-            print(f"[GenericPattern._match_forward] add {res} nodes")
-        return res
+class Constant(ValuePattern):
+    """Represents a pattern that matches against a scalar constant value."""
 
-    def match(
-        self,
-        g: ModelWithGraphStructure,
-        node: oir.Node,
-    ) -> PatternMatchResult | None:
-        self._debug = {}
-
-        pat = self._get_match_pattern(g)
-
-        # Let's match the last node.
-        # Then we need to match successors and predecessors.
-        p_node = pat.nodes[-1]  # the last one
-        if node.op_type != p_node.op_type:
-            # The last node does not have the same type.
-            return self.none()
-
-        check_ids = {id(n) for n in pat.nodes}
-        if self.verbose > 5:
-            print(
-                f"[GenericPattern.match] starts with "
-                f"{node.op_type}({', '.join(node.input_names)})"
-            )
-            if self.verbose >= 10:
-                print(f"[GenericPattern.match] match pattern {self!r}")
+    def __init__(
+        self, value: int | float, rel_tol: float = 1e-5, abs_tol: float = 1e-8
+    ) -> None:
+        self.value = value
+        self.rel_tol = rel_tol
+        self.abs_tol = abs_tol
+
+    def match_scalar(self, scalar_value, return_value: Sequence[ir.Node]):
+        if math.isclose(scalar_value, self.value, rel_tol=self.rel_tol, abs_tol=self.abs_tol):
+            return MatchResult(return_value)
+        return MatchResult.FAIL()
+
+    def matches(self, value: ir.Value, model: ir.Model):
+        value = _ir_utils.propagate_const_value(value)
+        constant_value = _ir_utils.get_numpy_from_ir_value(value)
+        if constant_value is None:
+            return MatchResult.FAIL()
+
+        # TODO (rama): allow users to specify shape requirement, if desired.
+        if constant_value.size != 1:
+            return MatchResult.FAIL()
+
+        return_value: list[ir.Node] = []
+        # Note: If the value is produced by a Constant node, we could include
+        # the Constant node in the return_value list. However, we don't do that.
+        # Instead, we will rely on DCE to remove the constant node if it is not
+        # used elsewhere.
+
+        return self.match_scalar(constant_value.item(), return_value)
+
+    def commute(self) -> list[ValuePattern]:
+        return [self]
+
+
+def _handle_pattern_return_value(
+    node_output_pattern: NodeOutputPattern | list[NodeOutputPattern],
+) -> tuple[NodePattern, int]:
+    """This checks and cleans up the return value of a pattern-construction function.
+
+    A pattern-construction function will return values as below:
+    ::
+        def pattern(x, shape1, shape2):
+            ...
+            return op.SomeOp(...)
+    However, `SomeOp` may represent an ONNX op that produces multiple outputs.
+    This function validates that the return values represent the outputs of
+    a single NodePattern. It returns the node_pattern and the number of outputs.
+
+    This follows an important restriction of the pattern-matcher algorithm: it
+    only matches against subgraphs that end in a single terminal node. If we
+    permit two terminal nodes, then we would have to match against all possible
+    pairs of nodes in the graph, which produces an extra quadratic factor in the
+    complexity of the pattern-matching algorithm. In general, the complexity becomes
+    exponential in the number of terminal nodes.
 
-        marked = {id(p_node): (node, p_node)}
-        stacked = [id(p_node)]
-        iteration = 0
-
-        if self.verbose > 5:
-            self._debug = dict(
-                pattern=pat,
-                marked=marked,
-                stacked=stacked,
-                iteration=iteration,
-                node=node,
-                pattern_node=p_node,
-                pattern_nodes=pat.nodes,
-            )
+    Args:
+        node_output_pattern: NodeOutputPattern | Sequence[NodeOutputPattern]
 
-        max_iter = len(pat.nodes) * 2
-        while stacked and iteration < max_iter:
-            assert all(id(b[1]) in check_ids for b in marked.values()), (
-                f"At least one id is not part of the pattern ids={check_ids}, "
-                f"marked={ {id(b[1]) for b in marked.values()} }"
-            )
+    Returns:
+        tuple[NodePattern, int]: The last node_pattern, num_outputs
+    """
+    if isinstance(node_output_pattern, NodeOutputPattern):
+        node_pattern = node_output_pattern.node_pattern
+        num_outputs = 1
+    elif isinstance(node_output_pattern, Sequence):
+        node_pattern = node_output_pattern[0].node_pattern
+        num_outputs = len(node_output_pattern)
+        for i, p in enumerate(node_output_pattern):
+            assert isinstance(p, NodeOutputPattern)
+            assert p.node_pattern is node_pattern
+            assert p.output_index == i
+    else:
+        raise TypeError(f"Invalid type {type(node_output_pattern)} for pattern")
+    return node_pattern, num_outputs
 
-            iteration += 1
-            if self.verbose > 5:
-                print(
-                    f"[GenericPattern.match] iteration={iteration} "
-                    f"n_marked={len(marked)}, n_stacked={len(stacked)}, "
-                    f"marked_types={collections.Counter(_[1].op_type for _ in marked.values())}"
-                )
-            idn = stacked.pop()
-            n, pn = marked[idn]
 
-            res = self._match_backward(g, node, pat, marked, stacked, n, pn)
-            if res is None:
-                if self.verbose > 5:
-                    print("[GenericPattern.match] done. backward failed.")
-                return res
-
-            assert all(id(b[1]) in check_ids for b in marked.values()), (
-                f"At least one id is not part of the pattern ids={check_ids}, "
-                f"marked={ {id(b[1]) for b in marked.values()} }"
-            )
+# Currently, the replacement graph function is the same as the pattern function.
+# This may change in the future.
+_handle_replacement_return_value = _handle_pattern_return_value
+
+
+def _valid_to_replace(matched_nodes: Sequence[Any]) -> bool:
+    """Check that values computed by the matched_nodes, except for the last one, are used only by the matched_nodes."""
+    # * Must check that all values matched by pattern are used only by pattern,
+    # except for the value that is replaced.
+    # * Must ensure that replacement subgraph does not use any of the deleted
+    # (intermediate) values. (Not necessary for now. Guaranteed.)
+    deleted_nodes = matched_nodes[:-1]
+    for n in deleted_nodes:
+        for v in n.outputs:
+            if v.is_graph_output():
+                # value is an output-value of the graph/function.
+                return False
+            for consumer, _ in v.consumers():
+                if consumer not in matched_nodes:
+                    return False
+    return True
 
-            res = self._match_forward(g, node, pat, marked, stacked, n, pn)
-            if res is None:
-                if self.verbose > 5:
-                    print("[GenericPattern.match] done. forward failed.")
-                return res
-
-            assert all(id(b[1]) in check_ids for b in marked.values()), (
-                f"At least one id is not part of the pattern ids={check_ids}, "
-                f"marked={ {id(b[1]) for b in marked.values()} }"
-            )
 
-            if self.verbose > 5:
-                self._debug["iteration"] = iteration
+class TargetPatternFunction:
+    """The targeted pattern that will be replaced by the replacement pattern.
 
-        if iteration >= max_iter and stacked:
-            self._hint("reached {iteration}>={max_iter} iterations")
-            return self.none(node, inspect.currentframe().f_lineno)
-
-        if self.verbose > 5:
-            print(f"[GenericPattern.match] done. {len(marked)} marked nodes")
-
-        # At this point, the pattern is matched but let's make sure.
-        assert len(marked) == len(pat.nodes), (
-            f"Number of marked nodes is different, {len(marked)} marked nodes, "
-            f"and {len(pat.nodes)} nodes in the pattern, marked is {marked}"
-        )
-        assert len(stacked) == 0, f"There are still {len(stacked)} nodes to explore."
+    Attributes:
+        function (Callable): The pattern function that will be matched against the IR.
+    """
 
-        # We order the matched nodes in the same order than the pattern
-        # to let next functions to be able to build the matching again.
-        matched_nodes = [marked[id(n)][0] for i, n in enumerate(pat.nodes)]
-        return PatternMatchResult(
-            self, matched_nodes, pat.nodes, pat.input_names, pat.output_names
-        )
+    def __init__(self, function: Callable) -> None:
+        self._function = function
 
-    @classmethod
-    def apply_pattern(
-        cls,
-        g: ModelWithGraphStructure,
-        *args: typing.Any,
-        **kwargs: typing.Any,
-    ) -> list[oir.Node]:
-        """Applies the replacement."""
-        raise NotImplementedError(
-            f"Class {cls.__name__!r} must overwrite method 'apply_pattern'."
-        )
+    @property
+    def function(self) -> Callable:
+        return self._function
+
+    def get_pattern(self, *variables: Sequence[Var]) -> tuple[NodePattern, int]:
+        node_output_pattern = self._function(*variables)
+        return _handle_pattern_return_value(node_output_pattern)
+
+
+class ReplacementPatternFunction:
+    """The replacement pattern that will replace the targeted pattern.
+
+    Attributes:
+        function (Callable): The replacement function that will be used to replace the matched pattern.
+        delay_run (bool): If True, the replacement function will not be run until the matched pattern is found.
+            This is useful when we want to extract certain metavalue from the matched pattern and use it in the
+            replacement pattern.
+    """
+
+    def __init__(self, function, *, delay_run: bool = False):
+        self._function = function
+        self._delay_run = delay_run
+
+    @property
+    def function(self) -> Callable:
+        return self._function
+
+    @property
+    def delay_run(self) -> bool:
+        return self._delay_run
 
-    def apply(
+    # TODO: How do we merge it with to_ir function?
+    def get_pattern(
         self,
-        g: ModelWithGraphStructure,
-        match_result: PatternMatchResult,
-    ) -> list[oir.Node]:
-        assert isinstance(match_result, PatternMatchResult)
-        new_pat = self._build_pattern(
-            g, fct=self.apply_pattern, kwargs=match_result.kwargs, match=False
-        )
-        assert len(new_pat.input_names) == len(match_result.pattern_input_names), (
-            f"Not the same number of inputs, "
-            f"matched inputs={len(new_pat.input_names)}, "
-            f"got {len(match_result.pattern_input_names)} in the applied pattern."
-        )
-        assert len(new_pat.output_names) == len(match_result.pattern_output_names), (
-            f"Not the same number of outputs, matched "
-            f"outputs={match_result.pattern_output_names}, "
-            f"got {new_pat.output_names} in the applied pattern."
+        *vars: Sequence[Var],
+        match_bindings: dict[str, ir.Value | Any] | None = None,
+    ) -> tuple[NodePattern | None, int | None]:
+        if self._delay_run:
+            if match_bindings is None:
+                return None, None
+            node_output_pattern = self._function(*vars, match_bindings)
+        else:
+            node_output_pattern = self._function(*vars)
+        return _handle_pattern_return_value(node_output_pattern)
+
+
+class RewriteCache:
+    def __init__(self):
+        self._node_output_pattern_to_ir: dict[NodeOutputPattern, tuple[ir.Value, ir.Node]] = (
+            dict()
         )
 
-        if g.verbose > 5:
-            print(
-                f"[GenericPattern.apply] replace {len(match_result.model_nodes)} nodes, "
-                f"applied {self.display_pattern(g, self.apply_pattern)}"
-            )
+    def get_node_output_pattern(
+        self, node_output_pattern: NodeOutputPattern
+    ) -> tuple[ir.Value, ir.Node] | None:
+        return self._node_output_pattern_to_ir.get(node_output_pattern, None)
+
+    def set_node_output_pattern_with_ir(
+        self, node_output_pattern: NodeOutputPattern, value: ir.Value, node: ir.Node
+    ) -> None:
+        self._node_output_pattern_to_ir[node_output_pattern] = (value, node)
 
-        # TODO: handle initializers here
-        # for name, init in pattern.initializers.items():
-        #   # We add them to the graph, they will be removed if unused.
-        #   new_name = g.make_initializer(name, init)
-        #   replacements[new_name] = name
-
-        applied_pattern_to_match_pattern = {}
-        for i, j in zip(match_result.pattern_input_names, new_pat.input_names):
-            applied_pattern_to_match_pattern[j] = i
-        for i, j in zip(match_result.pattern_output_names, new_pat.output_names):
-            applied_pattern_to_match_pattern[j] = i
-
-        replacements = {}
-        for k, v in applied_pattern_to_match_pattern.items():
-            replacements[k] = match_result.matched_pattern_to_model_name[v]
-
-        # Creation of the new node.
-        new_nodes = []
-        for node in new_pat.nodes:
-            new_inputs = []
-            for i in node.input_names:
-                assert i in replacements, f"Unable to find {i!r} in {replacements}"
-                ni = replacements[i]
-                new_inputs.append(ni)
-            new_outputs = []
-            for o in node.output_names:
-                if o in replacements:
-                    new_outputs.append(replacements[o])
-                else:
-                    # We give it a new name.
-                    n = g.unique_name(o)
-                    replacements[o] = n
-                    new_outputs.append(n)
-            new_node = g.make_node(node.op_type, new_inputs, new_outputs, domain=node.domain)
-            new_node.attribute.extend(node.original_node_proto.attribute)
-            new_nodes.append(oir.Node(new_node, True))
-
-        if g.verbose > 5:
-            print(f"[GenericPattern.apply] done with {len(new_nodes)} nodes")
-
-        return new_nodes
-
-    def make_rule(self) -> orp.RewriteRule:
-        """Creates the corresponding rule for this pattern."""
-        return GenericRewriteRule(self)
-
-
-class OnnxGenericPattern(GenericPattern):
-    """An instance of GenericPattern taking onnx model.
-
-    It defines the matching pattern and its replacement.
-
-    :param match_proto: the onnx function defining the matching pattern
-    :param apply_proto: the onnx function defining the new pattern
-    :param validate_mapping: the function used to validate a pattern
-    :param use_onnxscript: tells if the apply_proto is an onnxscript function or
-        a regular function returning a FunctionProto
-    :param opsets: opset to consider when converting the function into ONNX,
-        if not specified, it is opset 18 for the main opset, and opset 1
-        for domain com.microsoft.
-    :param verbose: in [0, 10], increase the verbosity to understand why a pattern
-        does not match
-    """
 
+class RewriteRule:
     def __init__(
         self,
-        match_proto: onnx.FunctionProto,
-        apply_proto: onnx.FunctionProto | typing.Callable,
-        validate_mapping: typing.Callable,
-        use_onnxscript: bool = True,
-        opsets: dict[str, onnxscript.values.Opset] | None = None,
-        verbose: int = 0,
-    ):
-        super().__init__(verbose=verbose)
-        self.match_proto = match_proto
-        self._validate_mapping = validate_mapping
-        self.apply_proto = apply_proto
-        self.use_onnxscript = use_onnxscript
-        self.opsets = opsets
-        self._cache = {}
-
-    def validate_mapping(self, g: oir.Model, match_result: PatternMatchResult) -> bool:
-        """Evaluates the consistency of the replacements."""
-        return self._validate_mapping(g, match_result)
+        target_pattern: TargetPatternFunction | Callable | None = None,
+        replacement_pattern: ReplacementPatternFunction | Callable | None = None,
+        condition_function: Callable | None = None,
+    ) -> None:
+        """Create a rewrite rule.
 
-    def _build_pattern(
-        self,
-        g: ModelWithGraphStructure,
-        fct: typing.Callable | None = None,
-        kwargs: dict[str, typing.Any] | None = None,
-        match: bool = True,
-    ) -> BuilderWithGraphStructure:
-        del fct
-        if match:
-            key = id(g), match, str(kwargs)
-        else:
-            key = id(g), match, str(kwargs)
-            assert not callable(self.apply_proto) or isinstance(kwargs, dict)
-        if key in self._cache:
-            return self._cache[key]
+        Args:
+            target_pattern: The pattern function that will be
+                matched against the IR.
+            replacement_pattern: The replacement function that
+                will be used to replace the matched pattern.
+            condition_function: The condition function that
+                will be used to check if the pattern matches the IR with ir.Values
+                constraints in consideration.
+
+        """
+        if target_pattern is None:
+            # NOTE: commute() generated rules will have target_pattern as None
+            # ReplacementPatternFunction is still needed in try_rewrite
+            assert replacement_pattern is None
+            assert condition_function is None
+            self._replacement_pattern = ReplacementPatternFunction(replacement_pattern)
+            return
+        elif replacement_pattern is None:
+            raise ValueError(
+                "replacement_pattern must be provided if target_pattern is provided"
+            )
+        # TODO: Do we want to tolerate Callable inputs?
+        if callable(target_pattern):
+            target_pattern = TargetPatternFunction(target_pattern)
+        if callable(replacement_pattern):
+            replacement_pattern = ReplacementPatternFunction(replacement_pattern)
+
+        self._target_pattern = target_pattern
+        self._replacement_pattern = replacement_pattern
+        self._condition_function = condition_function
+
+        _pattern_vars = inspect.signature(self._target_pattern.function).parameters
+        _replacement_vars = inspect.signature(self._replacement_pattern.function).parameters
+        # TODO: accept _replacement_vars being subset of _pattern_vars?
+        assert len(_pattern_vars) == len(_replacement_vars)
+
+        self._vars = [Var(v) for v in _pattern_vars]
+        # Get the last node pattern and number of outputs from the pattern function
+        self._target_node_pattern, self._target_num_outputs = self._target_pattern.get_pattern(
+            *self._vars  # type: ignore[arg-type]
+        )
+        # NOTE: Return Nones if the replacement pattern is delayed running
+        self._replace_node_pattern, _replacement_num_outputs = replacement_pattern.get_pattern(
+            *self._vars  # type: ignore[arg-type]
+        )
+        if _replacement_num_outputs is not None:
+            assert self._target_num_outputs == _replacement_num_outputs
+
+    def matches(self, node: ir.Node, model: ir.Model) -> MatchResult:
+        """Check if the node from IR matches the pattern."""
+        if len(node.outputs) != self._target_num_outputs:
+            return MatchResult.FAIL()
+        match = self._target_node_pattern.matches_node(node, model)
+        if (
+            self._condition_function is not None
+            and match
+            and not self._condition_function(match.bindings)
+        ):
+            return MatchResult.FAIL()
+        return match
 
+    def try_rewrite(
+        self, model: ir.Model, node: ir.Node
+    ) -> tuple[Sequence[Any], Sequence[ir.Node]] | None:
+        """If the node matches the pattern, then replace the node with the replacement pattern."""
+        match = self.matches(node, model)
         if match:
-            onx = self.match_proto
-        elif callable(self.apply_proto):
-            if self.use_onnxscript:
-                onx = onnxscript.script(**self.opsets)(self.apply_proto).to_function_proto()
-            else:
-                sig = inspect.signature(self.apply_proto)
-                args = []
-                for p in sig.parameters.values():
-                    if p.default is not inspect._empty:
-                        continue
-                    args.append(p.name)
-                onx = self.apply_proto(*args, **kwargs)
-        self._cache[key] = onx
-
-        g2 = g.make_opset()
-        for name in onx.input:
-            g2.make_input(name)
-        for node in onx.node:
-            g2.make_node_with_proto(node)
-        for name in onx.output:
-            g2.make_output(name)
-        g2._build()
-        self._cache[key] = g2
-        return g2
-
-
-def make_pattern_rule(
-    match_pattern: typing.Callable | onnx.FunctionProto,
-    apply_pattern: typing.Callable | onnx.FunctionProto,
-    validate_mapping: typing.Callable | None = None,
-    verbose: int = 0,
-    use_onnxscript: bool = True,
-    opsets: dict[str, onnxscript.values.Opset] | None = None,
-) -> orp.RewriteRule:
-    """
-    Creates a rewriting rule.
+            assert match.values is not None, "Matched values should not be None."
+            if _valid_to_replace(match.values):
+                # NOTE: delayed running as the replacement pattern needs bindings
+                if self._replacement_pattern.delay_run:
+                    # bindings will be consumed by the replacement function
+                    self._replace_node_pattern, _replacement_num_outputs = (
+                        self._replacement_pattern.get_pattern(
+                            *self._vars[:-1],  # type: ignore[arg-type]
+                            match_bindings=match.bindings,
+                        )
+                    )
+                    assert self._target_num_outputs == _replacement_num_outputs
+                rewrite_cache = RewriteCache()
+                assert self._replace_node_pattern is not None, "Replacement pattern is None."
+                _, _to_insert = self._replace_node_pattern.to_ir(
+                    model, match.bindings, self._target_num_outputs, rewrite_cache
+                )
 
-    :param match_pattern: a function interpreted by onnx-script
-        and converted into an onnx model, this model defines the
-        nodes to be replaced
-    :param apply_pattern: a function interpreted by onnx-script and
-        converted into an onnx model, this model defines the new nodes
-        replacing the matched nodes
-    :param validate_mapping: a function validating the matching once
-        it has happened, it is not valid, the pattern is not applied,
-        if not specified, the function always return True
-    :param opsets: opset to consider when converting the function into ONNX,
-        if not specified, it is opset 18 for the main opset, and opset 1
-        for domain com.microsoft.
-    :param use_onnxscript: tells if the apply_proto is an onnxscript function or
-        a regular function returning a FunctionProto
-    :return: the rewriting rule
+                return (match.values, _to_insert)  # type: ignore[return-value]
+        return None
+
+    def apply_to_model(self, model: ir.Model, *, commute: bool = False):
+        # TODO(titaiwang): Why do we need RewriteRuleSet?
+        return RewriteRuleSet([self], commute=commute).apply_to_model(model)
+
+    def count_matches(self, model: ir.Model, *, commute: bool = False):
+        return RewriteRuleSet([self], commute=commute).count_matches(model)
+
+    def commute(self) -> Sequence[RewriteRule]:
+        def replace_pattern(new_pattern):
+            """Return a shallow copy of self with node_pattern replaced by new_pattern."""
+            rule = RewriteRule()
+            rule._condition_function = self._condition_function
+            rule._target_node_pattern = new_pattern
+            rule._target_num_outputs = self._target_num_outputs
+            rule._replace_node_pattern = self._replace_node_pattern
+            return rule
+
+        return [replace_pattern(p) for p in self._target_node_pattern.commute()]
+
+
+def _apply_deltas(
+    graph_or_function: ir.Graph | ir.Function,
+    # TODO(jutinchuby): Use a more descriptive data structure to store deltas
+    deltas: Sequence[tuple[int, tuple[Sequence[ir.Node], Sequence[ir.Node]]]],
+):
+    """Applies deltas.
+
+    This code is valid is the considered pattern has only one output.
+    In case of multi output replacements, there is not need to rename
+    the outputs.
+
+    In case of multi-output design, the nodes may not be necessary inserted
+    all at the same position. To be convinced, you can take a pattern
+    producing two outputs, but the second one needs the first one and
+    another input appeared after the first outputs. What could be
+    the right place to inserted all of the node.
+
+    The current implementation insert all the nodes at the same position
+    but checks there is not inconsistency. In that case, it fails.
+    We could reorder (long) or do more clever changes.
+    The reordering would probably happen not very often.
     """
-    import onnxscript
+    existing_ids = {id(n): (i, n) for i, n in enumerate(graph_or_function)}
+    to_delete: set[ir.Node] = set()
+    to_insert: list[tuple[ir.Node, list[ir.Node]]] = []
+
+    for i, delta in reversed(deltas):
+        if len(delta) == 3:
+            # multi-outut strategy
+            n_matches, deleted_nodes, inserted_nodes = delta
+            for d in deleted_nodes:
+                assert id(d) in existing_ids
+                to_delete.add(d)
+
+            # the position to insert must be chosen.
+            # we'll try position i
+            assert i not in to_insert  # conflicts should avoid that case
+            to_insert.append((graph_or_function[i], inserted_nodes))
+        else:
+            deleted_nodes, inserted_nodes = delta
+            # Replace deleted nodes with inserted nodes.
+            # However, we merge the last deleted node and last inserted node
+            # to avoid replacing the values produced by the last deleted node
+            # in all places where they are used. So, we reuse the output
+            # values from the last deleted node and replace the node itself
+            # TODO: simplify this
+            last_deleted = deleted_nodes[-1]
+            last_inserted = inserted_nodes[-1]
+            assert len(last_deleted.outputs) == len(last_inserted.outputs)
+            # Reconnect the users of the deleted node to use the new outputs
+            for last_deleted_output, last_inserted_output in zip(
+                last_deleted.outputs, last_inserted.outputs
+            ):
+                for node, index in tuple(last_deleted_output.consumers()):
+                    # Fix consumers because we are mutating consumers in the loop
+                    node.replace_input_with(index, last_inserted_output)
+
+                # Update graph/function outputs if the node generates output
+                for old_output, new_output in zip(last_deleted.outputs, last_inserted.outputs):
+                    for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
+                        if graph_or_function_output is old_output:
+                            graph_or_function.outputs[idx] = new_output
+
+            # insert new nodes after the index node
+            # TODO(justinchuby): Do not access by index [i]
+            graph_or_function.insert_after(graph_or_function[i], inserted_nodes)
+
+            for old_node in deleted_nodes:
+                graph_or_function.remove(old_node)
+
+    for replaced_node, inserted_nodes in to_insert:
+        graph_or_function.insert_after(replaced_node, inserted_nodes)
+        # TODO: improve this
+        # This is updating the graph/function outputs to use the new outputs
+        for inserted_node in inserted_nodes:
+            for new_output in inserted_node.outputs:
+                if (index := new_output.meta.get(_ir_utils.GRAPH_OUTPUT_META_KEY)) is not None:  # type: ignore[assignment]
+                    graph_or_function.outputs[index] = new_output
+
+    for n in to_delete:
+        graph_or_function.remove(n)
+
+
+class RewriteRuleSet:
+    def __init__(self, rules: Sequence[RewriteRule], *, commute: bool = False) -> None:
+        if commute:
+            rules = list(itertools.chain.from_iterable([rule.commute() for rule in rules]))
+        self.rules = rules
 
-    if opsets is None:
-        opsets = dict(
-            op=onnxscript.opset18, msft_op=onnxscript.values.Opset("com.microsoft", 1)
-        )
+    def _apply_to_graph_or_function(
+        self,
+        model: ir.Model,
+        graph_or_function: ir.Graph | ir.Function,
+    ) -> int:
+        count = 0
+        marked = set()
+        # NOTE: Rules should be prioritized in the order they are added to the RewriteRuleSet.
+        # And the graph is applied in order.
+        for rule in self.rules:
+            deltas = []
+            for i, node in enumerate(graph_or_function):
+                delta = rule.try_rewrite(model, node)
 
-    if verbose > 5:
-        print(f"[make_pattern_rule] Converting {match_pattern} into ONNX.")
+                if delta is None:
+                    continue
 
-    if isinstance(match_pattern, onnx.FunctionProto):
-        match = match_pattern
-    else:
-        match = onnxscript.script(**opsets)(match_pattern).to_function_proto()
-    assert match.node, f"The match pattern has no node, function={match_pattern}."
+                matched_nodes, _ = delta[-2:]
+
+                conflict = False
+                for n in matched_nodes:
+                    if id(n) in marked:
+                        # The same node cannot be matched twice with different patterns.
+                        conflict = True
+                        break
+
+                if conflict:
+                    # Some nodes are already marked as rewritten.
+                    continue
 
-    pat = OnnxGenericPattern(
-        match,
-        apply_pattern,
-        validate_mapping or (lambda *_, **__: True),
-        verbose=verbose,
-        use_onnxscript=use_onnxscript,
-        opsets=opsets,
-    )
-    return pat.make_rule()
+                marked |= set(map(id, matched_nodes))
+
+                deltas.append((i, delta))
+                count += 1
+
+            _apply_deltas(graph_or_function, deltas)
+        return count
+
+    def apply_to_model(self, model: ir.Model) -> int:
+        assert isinstance(model, ir.Model)
+        count = self._apply_to_graph_or_function(model, model.graph)
+        for function in model.functions.values():
+            count += self._apply_to_graph_or_function(model, function)
+        return count
+
+    def _count_matches_in_graph_or_function(
+        self, model: ir.Model, graph_or_function: ir.Graph | ir.Function
+    ) -> int:
+        count = 0
+        for node in graph_or_function:
+            for rule in self.rules:
+                if rule.matches(node, model):
+                    count += 1
+                    break
+        return count
+
+    def count_matches(self, model: onnx.ModelProto | ir.Model):
+        if isinstance(model, onnx.ModelProto):
+            model = ir.serde.deserialize_model(model)
+        else:
+            assert isinstance(model, ir.Model)
+        count = self._count_matches_in_graph_or_function(model, model.graph)
+        for function in model.functions.values():
+            count += self._count_matches_in_graph_or_function(model, function)
+        return count
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import onnx
 
-from onnxscript._legacy_ir import irbuilder, protobuilder
+from onnxscript import ir
 from onnxscript.optimizer import remove_unused, remove_unused_function
 from onnxscript.rewriter import function_rule, pattern
 from onnxscript.rewriter.onnxruntime import (
     group_normalization_merge_silu,
     instance_to_group_normalization,
     softmax,
     transformers,
@@ -19,41 +19,39 @@
     *instance_to_group_normalization.rules.rules,
     # NOTE: group normalization merge silu should be applied after instance to group normalization
     *group_normalization_merge_silu.rules.rules,
 ]
 
 
 def rewrite(
-    model: onnx.ModelProto,
+    model_proto: onnx.ModelProto,
+    /,
     function_rules: list[type[function_rule.FunctionRewriteRule]] | None = None,
     pattern_rules: list[pattern.RewriteRule] | None = None,
 ) -> onnx.ModelProto:
     """Rewrite the model using the given rules.
 
     Args:
-        model: The model to rewrite.
+        model_proto: The model to rewrite.
         function_rules: The function rewrite rules to apply. If None, the default rules
             for onnxruntime are used.
         pattern_rules: The pattern rewrite rules to apply. If None, the default rules
             for onnxruntime are used.
 
     Returns:
         The rewritten model.
     """
     function_rules = function_rules or ORT_FUNCTION_REWRITE_RULES
     pattern_rules = pattern_rules or ORT_PATTERN_REWRITE_RULES
-    # TODO: Function rules first, or pattern rules first?
+    model = ir.serde.deserialize_model(model_proto)
+    # TODO(bowenbao): Function rules first, or pattern rules first?
     if function_rules:
-        model_ir = irbuilder.build_ir(model)
         for rule_cls in function_rules:
-            rule_cls().apply_to_model(model_ir)
-        model = model_ir.original_model_proto
+            count, model = rule_cls().apply_to_model(model)
+            print(f"Applied {count} of onnxruntime specific function rewrite rules.")
     if pattern_rules:
-        model_ir = irbuilder.build_ir(model)
-        count = pattern.RewriteRuleSet(pattern_rules).apply_to_model(model_ir)
-        print(f"Applied {count} pattern rewrite rules.")
-        model = protobuilder.build_model_proto(model_ir)
-    # TODO: Does it make more sense we run DCE after each rewrite rule applied?
-    # If so, we need IR to support DCE.
-    remove_unused.remove_unused_nodes(model)
-    remove_unused_function.remove_unused_functions(model)
-    return model
+        count = pattern.RewriteRuleSet(pattern_rules).apply_to_model(model)
+        print(f"Applied {count} of onnxruntime specific pattern rewrite rules.")
+    model_proto = ir.serde.serialize_model(model)
+    remove_unused.remove_unused_nodes(model_proto)
+    remove_unused_function.remove_unused_functions(model_proto)
+    return model_proto
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import logging
 from typing import Any
 
 import numpy as np
 import onnx
 
-import onnxscript._legacy_ir as ir
-from onnxscript.rewriter import pattern
+from onnxscript import ir
+from onnxscript.rewriter import _ir_utils, pattern
 
 op = pattern.onnxop
 msft_op = pattern.msft_op
 torch_module_op = pattern.torch_module_op
 
 logger = logging.getLogger(__name__)
 
@@ -22,17 +22,23 @@
     original_input_shape,
     weight_for_norm,
     bias_for_norm,
     weight_full,
     bias_full,
     **kwargs,
 ) -> bool:
-    if not np.all(weight_for_norm.value_as_np_array == 1):
+    weight_for_norm = _ir_utils.propagate_const_value(weight_for_norm)
+    weight_for_norm = _ir_utils.get_numpy_from_ir_value(weight_for_norm)
+
+    bias_for_norm = _ir_utils.propagate_const_value(bias_for_norm)
+    bias_for_norm = _ir_utils.get_numpy_from_ir_value(bias_for_norm)
+
+    if not np.all(weight_for_norm == 1):
         return False
-    if not np.all(bias_for_norm.value_as_np_array == 0):
+    if not np.all(bias_for_norm == 0):
         return False
 
     input_rank_minus_one = len(input_x.shape) - 1
     weight_full_rank = len(weight_full.shape)
     bias_full_rank = len(bias_full.shape)
     if weight_full_rank != input_rank_minus_one or bias_full_rank != input_rank_minus_one:
         return False
@@ -44,21 +50,24 @@
     weight_full_shape = weight_full.shape
     if not all(dim == 1 for dim in weight_full_shape[1:]):
         return False
     bias_full_shape = bias_full.shape
     if not all(dim == 1 for dim in bias_full_shape[1:]):
         return False
 
-    adjusted_input_shape = adjusted_input_shape.value_as_np_array
+    adjusted_input_shape = _ir_utils.propagate_const_value(adjusted_input_shape)
+    adjusted_input_shape = _ir_utils.get_numpy_from_ir_value(adjusted_input_shape)
+
     g = weight_for_norm.shape[0]
     if adjusted_input_shape is None or adjusted_input_shape.tolist() != [0, g, -1]:
         return False
 
     # NOTE: Restrict the rule to only support constant shape
-    original_input_shape = original_input_shape.value_as_np_array
+    original_input_shape = _ir_utils.propagate_const_value(original_input_shape)
+    original_input_shape = _ir_utils.get_numpy_from_ir_value(original_input_shape)
     if original_input_shape is None or original_input_shape.tolist() != input_x.shape:
         return False
 
     return True
 
 
 def check_if_simulated_instance_norm_is_used(
@@ -112,25 +121,29 @@
     adjusted_input_shape,
     original_input_shape,
     weight_for_norm,
     bias_for_norm,
     weight_full,
     bias_full,
     epsilon,
-    match_bindings: dict[str, ir.Value | Any] | None = None,
+    match_bindings: dict[str, ir.Value],
 ):
     # com.microsoft.GroupNorm only supports NHWC for now
     nhwc_input = op.Transpose(input_x, perm=[0, 2, 3, 1])
     # com.microsoft.GroupNorm only supports gamma and beta as float type
     weight_full = op.Cast(weight_full, to=onnx.TensorProto.FLOAT)
     reshape_to_1d = op.Constant(value_ints=[-1])
     weight_full = op.Reshape(weight_full, reshape_to_1d)
     bias_full = op.Cast(bias_full, to=onnx.TensorProto.FLOAT)
     bias_full = op.Reshape(bias_full, reshape_to_1d)
     # re-obtain attribute groups
+    if "weight_for_norm" not in match_bindings:
+        raise ValueError("weight_for_norm is not found in match_bindings")
+    if match_bindings["weight_for_norm"].shape is None:
+        raise ValueError("weight_for_norm shape not known")
     groups = match_bindings["weight_for_norm"].shape[0]
     output = msft_op.GroupNorm(
         nhwc_input,
         weight_full,
         bias_full,
         activation=0,
         channels_last=1,
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import onnx
 
-import onnxscript._legacy_ir as ir
+from onnxscript import ir
 from onnxscript.rewriter import pattern
 
 op = pattern.onnxop
 logger = logging.getLogger(__name__)
 
 
 def softmax_with_fp32_upcast(input, axis):
@@ -36,15 +36,15 @@
     input_val = match_bindings.get("input")
     if input_val is None:
         logger.warning(
             "Cannot perform softmax upcast removal: "
             "cannot retrieve match_bindings for 'input' for dtype validation."
         )
         return False
-    return input_val.element_type == onnx.TensorProto.FLOAT16
+    return input_val.dtype == ir.DataType.FLOAT16
 
 
 # pylint: disable=pointless-string-statement
 """
 This is an onnxruntime specific pattern. Softmax upcast is a common
 pattern observed in transformers models to prevent overflow. However
 this is not required since onnxruntime implementation already takes
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240420/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240420/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240420/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240420/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240420/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240420/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240420/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240420/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript/values.py` & `onnxscript-0.1.0.dev20240420/onnxscript/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,15 +532,15 @@
 
         # NOTE: We generate the parameter schemas from the function_ir instead
         # of relying on the auto generated OpSchema because we need to preserve the keyword
         # argument order from the Python function definition, which is lost in OpSchema.
         self._param_schemas = param_schemas_from_function_ir(self.function_ir)
         return self._param_schemas
 
-    def to_function_proto(self):
+    def to_function_proto(self) -> onnx.FunctionProto:
         """Converts the function into :class:`onnx.FunctionProto`."""
         return self.function_ir.to_function_proto()
 
     def to_model_proto(self, **kwargs):
         """Converts the function into :class:`onnx.ModelProto`."""
         if self.function_ir.attrs and any(
             not attr.has_default for attr in self.function_ir.attrs
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240420/onnxscript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240419
+Version: 0.1.0.dev20240420
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240419/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240420/onnxscript.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 onnxscript/_internal/autocast.py
 onnxscript/_internal/deprecation.py
 onnxscript/_internal/param_manipulation.py
 onnxscript/_internal/runtime_typing.py
 onnxscript/_internal/utils.py
 onnxscript/_internal/version_utils.py
 onnxscript/_legacy_ir/__init__.py
-onnxscript/_legacy_ir/irbuilder.py
-onnxscript/_legacy_ir/protobuilder.py
 onnxscript/_legacy_ir/visitor.py
 onnxscript/_thirdparty/asciichartpy.py
 onnxscript/backend/__init__.py
 onnxscript/backend/onnx_backend.py
 onnxscript/backend/onnx_export.py
 onnxscript/diagnostics/infra/__init__.py
 onnxscript/diagnostics/infra/_infra.py
@@ -100,17 +98,19 @@
 onnxscript/diagnostics/infra/sarif/version.py
 onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
 onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
 onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
 onnxscript/function_libs/torch_lib/__init__.py
 onnxscript/function_libs/torch_lib/_constants.py
 onnxscript/function_libs/torch_lib/_flags.py
-onnxscript/function_libs/torch_lib/graph_building.py
 onnxscript/function_libs/torch_lib/registration.py
 onnxscript/function_libs/torch_lib/tensor_typing.py
+onnxscript/function_libs/torch_lib/graph_building/__init__.py
+onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
 onnxscript/function_libs/torch_lib/ops/__init__.py
 onnxscript/function_libs/torch_lib/ops/common.py
 onnxscript/function_libs/torch_lib/ops/core.py
 onnxscript/function_libs/torch_lib/ops/fft.py
 onnxscript/function_libs/torch_lib/ops/linalg.py
 onnxscript/function_libs/torch_lib/ops/nested.py
 onnxscript/function_libs/torch_lib/ops/nn.py
@@ -161,27 +161,30 @@
 onnxscript/optimizer/copy_propagation.py
 onnxscript/optimizer/evaluator.py
 onnxscript/optimizer/fold_constants_v0.py
 onnxscript/optimizer/remove_unused.py
 onnxscript/optimizer/remove_unused_function.py
 onnxscript/optimizer/simple_function_folding.py
 onnxscript/rewriter/__init__.py
+onnxscript/rewriter/_ir_utils.py
+onnxscript/rewriter/_tape.py
 onnxscript/rewriter/broadcast_to_matmul.py
 onnxscript/rewriter/cast_constant_of_shape.py
 onnxscript/rewriter/erfgelu.py
 onnxscript/rewriter/function_rule.py
 onnxscript/rewriter/gemm_to_matmul_add.py
 onnxscript/rewriter/generic_pattern.py
 onnxscript/rewriter/no_op.py
 onnxscript/rewriter/pattern.py
 onnxscript/rewriter/onnxruntime/__init__.py
 onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
 onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
 onnxscript/rewriter/onnxruntime/softmax.py
 onnxscript/rewriter/onnxruntime/transformers/__init__.py
+onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
 onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
 onnxscript/rewriter/onnxruntime/transformers/layernorm.py
 onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
 onnxscript/testing/__init__.py
 onnxscript/utils/__init__.py
 onnxscript/utils/evaluation_utils.py
 onnxscript/utils/timing_utils.py
```

### Comparing `onnxscript-0.1.0.dev20240419/pyproject.toml` & `onnxscript-0.1.0.dev20240420/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240419/setup.py` & `onnxscript-0.1.0.dev20240420/setup.py`

 * *Files identical despite different names*

