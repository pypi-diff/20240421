# Comparing `tmp/airbyte-source-yahoo-finance-price-0.2.0.tar.gz` & `tmp/airbyte_source_yahoo_finance_price-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-yahoo-finance-price-0.2.0.tar", last modified: Thu Feb  1 09:44:01 2024, max compression
+gzip compressed data, was "airbyte_source_yahoo_finance_price-0.2.4.tar", max compression
```

## Comparing `airbyte-source-yahoo-finance-price-0.2.0.tar` & `airbyte_source_yahoo_finance_price-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,7 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:01.373325 airbyte-source-yahoo-finance-price-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     5594 2024-02-01 09:44:01.373325 airbyte-source-yahoo-finance-price-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5559 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:01.369325 airbyte-source-yahoo-finance-price-0.2.0/airbyte_source_yahoo_finance_price.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5594 2024-02-01 09:44:01.000000 airbyte-source-yahoo-finance-price-0.2.0/airbyte_source_yahoo_finance_price.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2024-02-01 09:44:01.000000 airbyte-source-yahoo-finance-price-0.2.0/airbyte_source_yahoo_finance_price.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 09:44:01.000000 airbyte-source-yahoo-finance-price-0.2.0/airbyte_source_yahoo_finance_price.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-02-01 09:44:01.000000 airbyte-source-yahoo-finance-price-0.2.0/airbyte_source_yahoo_finance_price.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-02-01 09:44:01.000000 airbyte-source-yahoo-finance-price-0.2.0/airbyte_source_yahoo_finance_price.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-02-01 09:44:01.000000 airbyte-source-yahoo-finance-price-0.2.0/airbyte_source_yahoo_finance_price.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:01.369325 airbyte-source-yahoo-finance-price-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      459 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)      459 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       62 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       60 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     5474 2024-02-01 09:44:01.373325 airbyte-source-yahoo-finance-price-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      960 2024-02-01 09:43:59.000000 airbyte-source-yahoo-finance-price-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:44:01.369325 airbyte-source-yahoo-finance-price-0.2.0/source_yahoo_finance_price/
--rw-r--r--   0 root         (0) root         (0)      146 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/source_yahoo_finance_price/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8651 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/source_yahoo_finance_price/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      265 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/source_yahoo_finance_price/run.py
--rw-r--r--   0 root         (0) root         (0)      486 2024-02-01 09:38:30.000000 airbyte-source-yahoo-finance-price-0.2.0/source_yahoo_finance_price/source.py
+-rw-r--r--   0        0        0     4730 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/README.md
+-rw-r--r--   0        0        0      821 2024-04-21 00:10:15.542645 airbyte_source_yahoo_finance_price-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/__init__.py
+-rw-r--r--   0        0        0    15036 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/manifest.yaml
+-rw-r--r--   0        0        0      265 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/run.py
+-rw-r--r--   0        0        0      486 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/source.py
+-rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 airbyte_source_yahoo_finance_price-0.2.4/PKG-INFO
```

### Comparing `airbyte-source-yahoo-finance-price-0.2.0/PKG-INFO` & `airbyte_source_yahoo_finance_price-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-yahoo-finance-price
-Version: 0.2.0
+Version: 0.2.4
 Summary: Source implementation for Yahoo Finance Price.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/yahoo-finance-price
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Yahoo Finance Source
+# Yahoo-Finance-Price source connector
 
-This is the repository for the Yahoo Finance source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/yahoo-finance-price).
 
+This is the repository for the Yahoo-Finance-Price source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/yahoo-finance-price).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/yahoo-finance-price)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_yahoo_finance_price/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/yahoo-finance-price)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_yahoo_finance_price/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source yahoo-finance-price test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-yahoo-finance-price spec
+poetry run source-yahoo-finance-price check --config secrets/config.json
+poetry run source-yahoo-finance-price discover --config secrets/config.json
+poetry run source-yahoo-finance-price read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-yahoo-finance-price build
 ```
 
-An image will be built with the tag `airbyte/source-yahoo-finance-price:dev`.
+An image will be available on your host with the tag `airbyte/source-yahoo-finance-price:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-yahoo-finance-price:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-yahoo-finance-price:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-yahoo-finance-price:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-yahoo-finance-price:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-yahoo-finance-price:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-yahoo-finance-price test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-yahoo-finance-price test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/yahoo-finance-price.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/yahoo-finance-price.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-yahoo-finance-price-0.2.0/README.md` & `airbyte_source_yahoo_finance_price-0.2.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,91 @@
-# Yahoo Finance Source
+# Yahoo-Finance-Price source connector
 
-This is the repository for the Yahoo Finance source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/yahoo-finance-price).
+
+This is the repository for the Yahoo-Finance-Price source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/yahoo-finance-price).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
-
-#### Minimum Python version required `= 3.7.0`
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/yahoo-finance-price)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_yahoo_finance_price/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/yahoo-finance-price)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_yahoo_finance_price/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source yahoo-finance-price test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-yahoo-finance-price spec
+poetry run source-yahoo-finance-price check --config secrets/config.json
+poetry run source-yahoo-finance-price discover --config secrets/config.json
+poetry run source-yahoo-finance-price read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Locally running the connector docker image
-
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-yahoo-finance-price build
 ```
 
-An image will be built with the tag `airbyte/source-yahoo-finance-price:dev`.
+An image will be available on your host with the tag `airbyte/source-yahoo-finance-price:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-yahoo-finance-price:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-yahoo-finance-price:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-yahoo-finance-price:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-yahoo-finance-price:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-yahoo-finance-price:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-yahoo-finance-price test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
-### Publishing a new version of the connector
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-yahoo-finance-price test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/yahoo-finance-price.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/yahoo-finance-price.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

