# Comparing `tmp/flask_openapi3-3.1.0.tar.gz` & `tmp/flask_openapi3-3.1.1.tar.gz`

## Comparing `flask_openapi3-3.1.0.tar` & `flask_openapi3-3.1.1.tar`

### file list

```diff
@@ -1,119 +1,120 @@
--rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/api_blueprint_demo.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/api_view_demo.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/async_demo.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/custom_ui_templates_demo.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/enum_demo.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/header_demo.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/image_demo.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/init_oauth_demo.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/just_flask.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/nested_apiblueprint_demo.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/openapi_extensions.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/openapi_extra.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/orjson_demo.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/pydantic_custom_root_types.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/raw_request_demo.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/response_demo.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/rest_demo.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/servers_demo.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/simple_demo.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/examples/upload_file_demo.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/__version__.py
--rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/blueprint.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/commands.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/markdown.py
--rw-r--r--   0        0        0    18986 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/openapi.py
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/request.py
--rw-r--r--   0        0        0    17791 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/scaffold.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/types.py
--rw-r--r--   0        0        0    21294 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/utils.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/view.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/callback.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/components.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/contact.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/data_type.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/discriminator.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/encoding.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/example.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/external_documentation.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/file.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/header.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/info.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/license.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/link.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/media_type.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/oauth_flow.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/oauth_flows.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/operation.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/parameter.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/parameter_in_type.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/path_item.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/paths.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/reference.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/request_body.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/response.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/responses.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/schema.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/security_requirement.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/security_scheme.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/security_scheme_in_type.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/server.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/server_variable.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/style_values.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/tag.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/validation_error.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/models/xml.py
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/__init__.py
--rw-r--r--   0        0        0   152042 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/css/swagger-ui.css
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/images/apidoc.svg
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/images/rapidoc.svg
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/images/redoc.svg
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/images/swagger.svg
--rw-r--r--   0        0        0   662202 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/js/rapidoc-min.js
--rw-r--r--   0        0        0   870152 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/js/redoc.standalone.js
--rw-r--r--   0        0        0  1415333 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/js/swagger-ui-bundle.js
--rw-r--r--   0        0        0   230777 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/requirements/build.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/requirements/doc.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/requirements/flake8.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/requirements/mypy.txt
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/requirements/test.txt
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_api_blueprint.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_api_view.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_api_view_args.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_async.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_custom_ui_templates_demo.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_default_query.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_empty_body.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_enum.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_fixed_externaldocs_support.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_form.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_model_config.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_multi_decorator.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_nested_apiblueprint.py
--rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_openapi.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_openapi_extensions.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_options_in_viewfunc.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_pydantic_calculated_fields.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_pydantic_custom_root_types.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_request.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_response.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_restapi.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_restapi_with_doc_prefix.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_security.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_str_body.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_summary.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_swagger_config.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_tags.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_trail_slash.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/tests/test_validation_error.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/LICENSE.rst
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/README.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 flask_openapi3-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/api_blueprint_demo.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/api_view_demo.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/async_demo.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/custom_ui_templates_demo.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/enum_demo.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/header_demo.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/image_demo.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/init_oauth_demo.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/just_flask.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/nested_apiblueprint_demo.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/openapi_extensions.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/openapi_extra.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/orjson_demo.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/pydantic_custom_root_types.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/raw_request_demo.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/response_demo.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/rest_demo.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/servers_demo.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/simple_demo.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/upload_file_demo.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/__version__.py
+-rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/blueprint.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/commands.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/markdown.py
+-rw-r--r--   0        0        0    18986 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/openapi.py
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/request.py
+-rw-r--r--   0        0        0    17791 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/scaffold.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/types.py
+-rw-r--r--   0        0        0    21294 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/utils.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/view.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/callback.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/components.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/contact.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/data_type.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/discriminator.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/encoding.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/example.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/external_documentation.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/file.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/header.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/info.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/license.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/link.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/media_type.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/oauth_flow.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/oauth_flows.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/operation.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/parameter.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/parameter_in_type.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/path_item.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/paths.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/reference.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/request_body.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/response.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/responses.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/schema.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/security_requirement.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/security_scheme.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/security_scheme_in_type.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/server.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/server_variable.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/style_values.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/tag.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/validation_error.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/xml.py
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/__init__.py
+-rw-r--r--   0        0        0   152042 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/css/swagger-ui.css
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/images/apidoc.svg
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/images/rapidoc.svg
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/images/redoc.svg
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/images/swagger.svg
+-rw-r--r--   0        0        0   662202 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/js/rapidoc-min.js
+-rw-r--r--   0        0        0   870152 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/js/redoc.standalone.js
+-rw-r--r--   0        0        0  1415333 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/js/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   230777 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/build.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/doc.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/flake8.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/mypy.txt
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/test.txt
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_api_blueprint.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_api_view.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_api_view_args.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_async.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_custom_ui_templates_demo.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_default_query.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_empty_body.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_enum.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_fixed_externaldocs_support.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_form.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_model_config.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_multi_decorator.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_nested_apiblueprint.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_number_constraints.py
+-rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_openapi.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_openapi_extensions.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_options_in_viewfunc.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_pydantic_calculated_fields.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_pydantic_custom_root_types.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_request.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_response.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_restapi.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_restapi_with_doc_prefix.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_security.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_str_body.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_summary.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_swagger_config.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_tags.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_trail_slash.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_validation_error.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/LICENSE.rst
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/README.md
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/PKG-INFO
```

### Comparing `flask_openapi3-3.1.0/CHANGELOG.md` & `flask_openapi3-3.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## v3.1.1 2024-04-21
+
+- Wrong types of exclusiveMinimum & exclusiveMaximum fields in Schema class by @Lavertis in #149
+
 ## v3.1.0 2024-03-24
 
 - Add the swagger_config parameter to configure the swagger ui by @luolingchun in #146
 - Use full links in Swagger and RapiDoc
 - Upgrade Redoc to 2.1.3
 - Upgrade Swagger to 5.12.0
```

### Comparing `flask_openapi3-3.1.0/CONTRIBUTING.md` & `flask_openapi3-3.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/api_blueprint_demo.py` & `flask_openapi3-3.1.1/examples/api_blueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/api_view_demo.py` & `flask_openapi3-3.1.1/examples/api_view_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/async_demo.py` & `flask_openapi3-3.1.1/examples/async_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/custom_ui_templates_demo.py` & `flask_openapi3-3.1.1/examples/custom_ui_templates_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/enum_demo.py` & `flask_openapi3-3.1.1/examples/enum_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/header_demo.py` & `flask_openapi3-3.1.1/examples/header_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/init_oauth_demo.py` & `flask_openapi3-3.1.1/examples/init_oauth_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/nested_apiblueprint_demo.py` & `flask_openapi3-3.1.1/examples/nested_apiblueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/openapi_extensions.py` & `flask_openapi3-3.1.1/examples/openapi_extensions.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/openapi_extra.py` & `flask_openapi3-3.1.1/examples/openapi_extra.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/orjson_demo.py` & `flask_openapi3-3.1.1/examples/orjson_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/pydantic_custom_root_types.py` & `flask_openapi3-3.1.1/examples/pydantic_custom_root_types.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/response_demo.py` & `flask_openapi3-3.1.1/examples/response_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/rest_demo.py` & `flask_openapi3-3.1.1/examples/rest_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/servers_demo.py` & `flask_openapi3-3.1.1/examples/servers_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/simple_demo.py` & `flask_openapi3-3.1.1/examples/simple_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/examples/upload_file_demo.py` & `flask_openapi3-3.1.1/examples/upload_file_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/__init__.py` & `flask_openapi3-3.1.1/flask_openapi3/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/blueprint.py` & `flask_openapi3-3.1.1/flask_openapi3/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/commands.py` & `flask_openapi3-3.1.1/flask_openapi3/commands.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/markdown.py` & `flask_openapi3-3.1.1/flask_openapi3/markdown.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/openapi.py` & `flask_openapi3-3.1.1/flask_openapi3/openapi.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/request.py` & `flask_openapi3-3.1.1/flask_openapi3/request.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/scaffold.py` & `flask_openapi3-3.1.1/flask_openapi3/scaffold.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/types.py` & `flask_openapi3-3.1.1/flask_openapi3/types.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/utils.py` & `flask_openapi3-3.1.1/flask_openapi3/utils.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/view.py` & `flask_openapi3-3.1.1/flask_openapi3/view.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/__init__.py` & `flask_openapi3-3.1.1/flask_openapi3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/callback.py` & `flask_openapi3-3.1.1/flask_openapi3/models/callback.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/components.py` & `flask_openapi3-3.1.1/flask_openapi3/models/components.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/encoding.py` & `flask_openapi3-3.1.1/flask_openapi3/models/encoding.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/file.py` & `flask_openapi3-3.1.1/flask_openapi3/models/file.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/info.py` & `flask_openapi3-3.1.1/flask_openapi3/models/info.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/link.py` & `flask_openapi3-3.1.1/flask_openapi3/models/link.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/media_type.py` & `flask_openapi3-3.1.1/flask_openapi3/models/media_type.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/operation.py` & `flask_openapi3-3.1.1/flask_openapi3/models/operation.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/parameter.py` & `flask_openapi3-3.1.1/flask_openapi3/models/parameter.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/path_item.py` & `flask_openapi3-3.1.1/flask_openapi3/models/path_item.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/response.py` & `flask_openapi3-3.1.1/flask_openapi3/models/response.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/schema.py` & `flask_openapi3-3.1.1/flask_openapi3/models/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     """
     https://spec.openapis.org/oas/v3.1.0#schema-object
     """
     ref: Optional[str] = Field(alias="$ref", default=None)
     title: Optional[str] = None
     multipleOf: Optional[float] = Field(default=None, gt=0.0)
     maximum: Optional[float] = None
-    exclusiveMaximum: Optional[bool] = None
+    exclusiveMaximum: Optional[float] = None
     minimum: Optional[float] = None
-    exclusiveMinimum: Optional[bool] = None
+    exclusiveMinimum: Optional[float] = None
     maxLength: Optional[int] = Field(default=None, ge=0)
     minLength: Optional[int] = Field(default=None, ge=0)
     pattern: Optional[str] = None
     maxItems: Optional[int] = Field(default=None, ge=0)
     minItems: Optional[int] = Field(default=None, ge=0)
     uniqueItems: Optional[bool] = None
     maxProperties: Optional[int] = Field(default=None, ge=0)
```

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/security_scheme.py` & `flask_openapi3-3.1.1/flask_openapi3/models/security_scheme.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/models/validation_error.py` & `flask_openapi3-3.1.1/flask_openapi3/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/__init__.py` & `flask_openapi3-3.1.1/flask_openapi3/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/css/swagger-ui.css` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/css/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/images/apidoc.svg` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/images/apidoc.svg`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/images/rapidoc.svg` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/images/rapidoc.svg`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/images/redoc.svg` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/images/redoc.svg`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/images/swagger.svg` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/images/swagger.svg`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/js/rapidoc-min.js` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/js/rapidoc-min.js`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/js/redoc.standalone.js` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/js/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/js/swagger-ui-bundle.js` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/js/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js` & `flask_openapi3-3.1.1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_api_blueprint.py` & `flask_openapi3-3.1.1/tests/test_api_blueprint.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_api_view.py` & `flask_openapi3-3.1.1/tests/test_api_view.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_api_view_args.py` & `flask_openapi3-3.1.1/tests/test_api_view_args.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_async.py` & `flask_openapi3-3.1.1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_custom_ui_templates_demo.py` & `flask_openapi3-3.1.1/tests/test_custom_ui_templates_demo.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_default_query.py` & `flask_openapi3-3.1.1/tests/test_default_query.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_empty_body.py` & `flask_openapi3-3.1.1/tests/test_empty_body.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_enum.py` & `flask_openapi3-3.1.1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_fixed_externaldocs_support.py` & `flask_openapi3-3.1.1/tests/test_fixed_externaldocs_support.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_form.py` & `flask_openapi3-3.1.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_model_config.py` & `flask_openapi3-3.1.1/tests/test_model_config.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_multi_decorator.py` & `flask_openapi3-3.1.1/tests/test_multi_decorator.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_nested_apiblueprint.py` & `flask_openapi3-3.1.1/tests/test_nested_apiblueprint.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_openapi.py` & `flask_openapi3-3.1.1/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_openapi_extensions.py` & `flask_openapi3-3.1.1/tests/test_openapi_extensions.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_options_in_viewfunc.py` & `flask_openapi3-3.1.1/tests/test_options_in_viewfunc.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_pydantic_calculated_fields.py` & `flask_openapi3-3.1.1/tests/test_pydantic_calculated_fields.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_pydantic_custom_root_types.py` & `flask_openapi3-3.1.1/tests/test_pydantic_custom_root_types.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_request.py` & `flask_openapi3-3.1.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_response.py` & `flask_openapi3-3.1.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_restapi.py` & `flask_openapi3-3.1.1/tests/test_restapi.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_restapi_with_doc_prefix.py` & `flask_openapi3-3.1.1/tests/test_restapi_with_doc_prefix.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_security.py` & `flask_openapi3-3.1.1/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_str_body.py` & `flask_openapi3-3.1.1/tests/test_str_body.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_summary.py` & `flask_openapi3-3.1.1/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_swagger_config.py` & `flask_openapi3-3.1.1/tests/test_swagger_config.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_tags.py` & `flask_openapi3-3.1.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_trail_slash.py` & `flask_openapi3-3.1.1/tests/test_trail_slash.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/tests/test_validation_error.py` & `flask_openapi3-3.1.1/tests/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/.gitignore` & `flask_openapi3-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/LICENSE.rst` & `flask_openapi3-3.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/README.md` & `flask_openapi3-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/pyproject.toml` & `flask_openapi3-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_openapi3-3.1.0/PKG-INFO` & `flask_openapi3-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flask-openapi3
-Version: 3.1.0
+Version: 3.1.1
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Project-URL: Homepage, https://github.com/luolingchun/flask-openapi3
 Project-URL: Documentation, https://luolingchun.github.io/flask-openapi3
 Maintainer-email: llc <luolingchun@outlook.com>
 License: MIT
 License-File: LICENSE.rst
 Classifier: Development Status :: 5 - Production/Stable
```

