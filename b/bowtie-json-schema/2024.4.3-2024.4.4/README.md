# Comparing `tmp/bowtie_json_schema-2024.4.3.tar.gz` & `tmp/bowtie_json_schema-2024.4.4.tar.gz`

## Comparing `bowtie_json_schema-2024.4.3.tar` & `bowtie_json_schema-2024.4.4.tar`

### file list

```diff
@@ -1,236 +1,237 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.gitpod.Dockerfile
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.prettierrc.json
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/action.yml
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/noxfile.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/test-requirements.in
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/test-requirements.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.devcontainer/Containerfile
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/__main__.py
--rw-r--r--   0        0        0    44741 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/_cli.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/_commands.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/_containers.py
--rw-r--r--   0        0        0    21220 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/_core.py
--rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/_report.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/exceptions.py
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/py.typed
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/Makefile
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/cli.rst
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/github-actions.rst
--rw-r--r--   0        0        0    36245 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/index.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/motd.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/requirements.in
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/index.html
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/package.json
--rw-r--r--   0        0        0   152698 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/global.css
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/conftest.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/test_cli.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/test_github.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/test_implementation.py
--rw-r--r--   0        0        0    64093 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/test_integration.py
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/test_report.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/hatch_build.py
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/pyproject.toml
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.3/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.prettierrc.json
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/action.yml
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/noxfile.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/test-requirements.in
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/test-requirements.txt
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/__main__.py
+-rw-r--r--   0        0        0    49511 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_cli.py
+-rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_commands.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_containers.py
+-rw-r--r--   0        0        0    21271 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_core.py
+-rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_report.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/py.typed
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/Makefile
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/cli.rst
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/index.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/motd.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/requirements.in
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/index.html
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/package.json
+-rw-r--r--   0        0        0   165892 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/global.css
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/conftest.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_cli.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_github.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_implementation.py
+-rw-r--r--   0        0        0    64095 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_integration.py
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_report.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/hatch_build.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.4.4/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.4.3/.gitpod.yml` & `bowtie_json_schema-2024.4.4/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/.pre-commit-config.yaml` & `bowtie_json_schema-2024.4.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 ci:
   skip:
     - clippy # doesn't seem to run in pre-commit.ci
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-ast
       - id: check-json
       - id: check-toml
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.5"
+    rev: "v0.3.7"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.1
+    rev: 0.28.2
     hooks:
       - name: ensure bowtie's own schemas are valid
         id: check-metaschema
         files: ^bowtie/schemas/.*\.json$
   - repo: local
     hooks:
       - id: check-dependabot
@@ -38,15 +38,15 @@
         additional_dependencies: [pyyaml]
       - id: check-lintsonschema
         name: check lintsonschema for drift
         language: python
         pass_filenames: false
         entry: .pre-commit-hooks/check-lintsonschema-schema
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.0
     hooks:
       - name: black (python implementations & bowtie internals)
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
@@ -102,15 +102,15 @@
     rev: v0.20.0
     hooks:
       - name: stylua (lua implementations)
         id: stylua
         exclude: .*/json.lua
         args: ["--config-path", "implementations/lua-jsonschema/stylua.toml"]
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v18.1.2
+    rev: v18.1.3
     hooks:
       - name: clang-format (c/c++/c#/java implementations)
         id: clang-format
         types_or: [c++, c, c#, java, objective-c]
   - repo: https://github.com/dustinsand/pre-commit-jvm
     rev: v0.11.0
     hooks:
```

### Comparing `bowtie_json_schema-2024.4.3/CONTRIBUTING.rst` & `bowtie_json_schema-2024.4.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/action.yml` & `bowtie_json_schema-2024.4.4/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/noxfile.py` & `bowtie_json_schema-2024.4.4/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 ]
 
 
 # aiohttp / aiodocker don't support 3.12
 SUPPORTED = ["pypy3.10", "3.11", "3.12"]
 LATEST = SUPPORTED[-1]
 
+nox.options.default_venv_backend = "uv|virtualenv"
 nox.options.sessions = []
 
 
 def session(default=True, python=LATEST, **kwargs):  # noqa: D103
     def _session(fn):
         if default:
             nox.options.sessions.append(kwargs.get("name", fn.__name__))
@@ -357,24 +358,22 @@
 
 
 @session(default=False)
 def requirements(session):
     """
     Update bowtie's requirements.txt files.
     """
-    session.install("pip-tools")
+    if session.venv_backend == "uv":
+        cmd = ["uv", "pip", "compile"]
+    else:
+        session.install("pip-tools")
+        cmd = ["pip-compile", "--resolver", "backtracking", "--strip-extras"]
+
     for each in REQUIREMENTS_IN:
-        session.run(
-            "pip-compile",
-            "--resolver",
-            "backtracking",
-            "--strip-extras",
-            "-U",
-            each.relative_to(ROOT),
-        )
+        session.run(*cmd, "-U", each.relative_to(ROOT))
 
 
 @session(default=False, python=False)
 def ui(session):
     """
     Run a local development UI.
```

### Comparing `bowtie_json_schema-2024.4.3/requirements.txt` & `bowtie_json_schema-2024.4.4/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile --strip-extras pyproject.toml
 #
 aiodocker==0.21.0
     # via bowtie-json-schema (pyproject.toml)
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   bowtie-json-schema (pyproject.toml)
@@ -19,28 +19,28 @@
 certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
-    # via bowtie-json-schema (pyproject.toml)
+    # via rich-click
 cryptography==42.0.5
     # via pyjwt
-diagnostic==2.0.0
+diagnostic==2.1.0
     # via bowtie-json-schema (pyproject.toml)
-docutils==0.20.1
+docutils==0.21.1
     # via diagnostic
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 github3-py==4.0.1
     # via bowtie-json-schema (pyproject.toml)
-idna==3.6
+idna==3.7
     # via
     #   requests
     #   yarl
 jsonschema==4.21.1
     # via bowtie-json-schema (pyproject.toml)
 jsonschema-lexer==0.2.1
     # via bowtie-json-schema (pyproject.toml)
@@ -76,25 +76,30 @@
     # via bowtie-json-schema (pyproject.toml)
 requests==2.31.0
     # via github3-py
 rich==13.7.1
     # via
     #   bowtie-json-schema (pyproject.toml)
     #   diagnostic
+    #   rich-click
+rich-click==1.8.0.dev6
+    # via bowtie-json-schema (pyproject.toml)
 rpds-py==0.18.0
     # via
     #   bowtie-json-schema (pyproject.toml)
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 structlog==24.1.0
     # via bowtie-json-schema (pyproject.toml)
-typing-extensions==4.10.0
-    # via aiodocker
+typing-extensions==4.11.0
+    # via
+    #   aiodocker
+    #   rich-click
 uritemplate==4.1.1
     # via github3-py
 url-py==0.10.0
     # via bowtie-json-schema (pyproject.toml)
 urllib3==2.2.1
     # via requests
 yarl==1.9.4
```

### Comparing `bowtie_json_schema-2024.4.3/test-requirements.txt` & `bowtie_json_schema-2024.4.4/test-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --strip-extras test-requirements.in
 #
 aiodocker==0.21.0
     # via
     #   -r requirements.txt
     #   bowtie-json-schema
-aiohttp==3.9.3
+aiohttp==3.9.4
     # via
     #   -r requirements.txt
     #   aiodocker
 aiosignal==1.3.1
     # via
     #   -r requirements.txt
     #   aiohttp
@@ -37,41 +37,41 @@
 charset-normalizer==3.3.2
     # via
     #   -r requirements.txt
     #   requests
 click==8.1.7
     # via
     #   -r requirements.txt
-    #   bowtie-json-schema
+    #   rich-click
 cryptography==42.0.5
     # via
     #   -r requirements.txt
     #   pyjwt
-diagnostic==2.0.0
+diagnostic==2.1.0
     # via
     #   -r requirements.txt
     #   bowtie-json-schema
-docutils==0.20.1
+docutils==0.21.1
     # via
     #   -r requirements.txt
     #   diagnostic
 frozenlist==1.4.1
     # via
     #   -r requirements.txt
     #   aiohttp
     #   aiosignal
 github3-py==4.0.1
     # via
     #   -r requirements.txt
     #   bowtie-json-schema
-hypothesis==6.99.13
+hypothesis==6.100.1
     # via -r test-requirements.in
 icdiff==2.0.7
     # via pytest-icdiff
-idna==3.6
+idna==3.7
     # via
     #   -r requirements.txt
     #   requests
     #   yarl
 iniconfig==2.0.0
     # via pytest
 jsonschema==4.21.1
@@ -108,15 +108,15 @@
     # via -r test-requirements.in
 pluggy==1.4.0
     # via pytest
 pprintpp==0.4.0
     # via pytest-icdiff
 ptyprocess==0.7.0
     # via pexpect
-pycparser==2.21
+pycparser==2.22
     # via
     #   -r requirements.txt
     #   cffi
 pygments==2.17.2
     # via
     #   -r requirements.txt
     #   jsonschema-lexer
@@ -154,14 +154,19 @@
     #   -r requirements.txt
     #   github3-py
 rich==13.7.1
     # via
     #   -r requirements.txt
     #   bowtie-json-schema
     #   diagnostic
+    #   rich-click
+rich-click==1.8.0.dev6
+    # via
+    #   -r requirements.txt
+    #   bowtie-json-schema
 rpds-py==0.18.0
     # via
     #   -r requirements.txt
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 six==1.16.0
@@ -170,18 +175,19 @@
     #   python-dateutil
 sortedcontainers==2.4.0
     # via hypothesis
 structlog==24.1.0
     # via
     #   -r requirements.txt
     #   bowtie-json-schema
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   -r requirements.txt
     #   aiodocker
+    #   rich-click
 uritemplate==4.1.1
     # via
     #   -r requirements.txt
     #   github3-py
 url-py==0.10.0
     # via
     #   -r requirements.txt
```

### Comparing `bowtie_json_schema-2024.4.3/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.4.4/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.4.4/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/_cli.py` & `bowtie_json_schema-2024.4.4/bowtie/_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections.abc import Callable, Iterable
 from contextlib import AsyncExitStack, asynccontextmanager
 from fnmatch import fnmatch
 from functools import cache, wraps
 from importlib.resources import files
 from pathlib import Path
 from pprint import pformat
+from textwrap import dedent
 from typing import TYPE_CHECKING, Literal, ParamSpec, Protocol
 import asyncio
 import json
 import logging
 import os
 import sys
 
@@ -23,17 +24,18 @@
     JsonLexer,
 )
 from referencing.jsonschema import EMPTY_REGISTRY
 from rich import box, console, panel
 from rich.syntax import Syntax
 from rich.table import Column, Table
 from rich.text import Text
+from rich_click.utils import CommandGroupDict, OptionGroupDict
 from url import URL, RelativeURLWithoutBase
-import click
 import referencing_loaders
+import rich_click as click
 import structlog
 import structlog.typing
 
 from bowtie import _containers, _report, _suite
 from bowtie._commands import SeqCase, Unsuccessful
 from bowtie._core import (
     Dialect,
@@ -57,14 +59,15 @@
 
     from click.decorators import FC
     from referencing.jsonschema import Schema, SchemaRegistry, SchemaResource
 
     from bowtie._commands import AnyTestResult, ImplementationId
     from bowtie._core import DialectRunner, ImplementationInfo, MakeValidator
 
+
 # Windows fallbacks...
 _EX_CONFIG = getattr(os, "EX_CONFIG", 1)
 _EX_DATAERR = getattr(os, "EX_DATAERR", 1)
 _EX_NOINPUT = getattr(os, "EX_NOINPUT", 1)
 
 STDERR = console.Console(stderr=True)
 
@@ -79,24 +82,192 @@
     default=lambda: "pretty" if sys.stdout.isatty() else "json",
     show_default="pretty if stdout is a tty, otherwise JSON",
     type=click.Choice(["json", "pretty", "markdown"]),
 )
 _F = Literal["json", "pretty", "markdown"]
 
 
+def option_group(name: str, *options: str, **kwargs: Any):
+    return OptionGroupDict(
+        name=name,
+        options=[f"--{option}" for option in options],
+        **kwargs,
+    )
+
+
+# rich-click's CommandGroupDict seems to be missing some covariance, as using a
+# regular dict here makes pyright complain.
+_COMMAND_GROUPS = dict(
+    bowtie=[
+        CommandGroupDict(
+            name="Basic Commands",
+            commands=["validate", "suite", "summary", "info"],
+        ),
+        CommandGroupDict(
+            name="Advanced Usage",
+            commands=["filter-dialects", "filter-implementations", "run"],
+        ),
+        CommandGroupDict(
+            name="Plumbing Commands",
+            commands=["badges", "smoke"],
+        ),
+    ],
+)
+_OPTION_GROUPS = {
+    "bowtie validate": [
+        option_group(
+            "Required",
+            "implementation",
+        ),
+        option_group(
+            "Schema Behavior Options",
+            "dialect",
+            "set-schema",
+        ),
+        option_group(
+            "Validation Metadata Options",
+            "description",
+            "expect",
+        ),
+        option_group(
+            "Connection & Communication Options",
+            "read-timeout",
+            "validate-implementations",
+        ),
+        option_group("Help", "help"),
+    ],
+    "bowtie suite": [
+        option_group(
+            "Required",
+            "implementation",
+        ),
+        option_group(
+            "Test Run Options",
+            "fail-fast",
+            "filter",
+            "max-error",
+            "max-fail",
+        ),
+        option_group(
+            "Test Modification Options",
+            "set-schema",
+        ),
+        option_group(
+            "Connection & Communication Options",
+            "read-timeout",
+            "validate-implementations",
+        ),
+        option_group("Help", "help"),
+    ],
+    "bowtie info": [
+        option_group(
+            "Basic Options",
+            "implementation",
+            "format",
+        ),
+        option_group(
+            "Connection & Communication Options",
+            "read-timeout",
+        ),
+        option_group("Help", "help"),
+    ],
+    "bowtie smoke": [
+        option_group(
+            "Basic Options",
+            "implementation",
+            "quiet",
+            "format",
+        ),
+        option_group(
+            "Connection & Communication Options",
+            "read-timeout",
+        ),
+        option_group("Help", "help"),
+    ],
+    "bowtie filter-dialects": [
+        option_group(
+            "Required",
+            "implementation",
+        ),
+        option_group(
+            "Filters",
+            "dialect",
+            "latest",
+            "boolean-schemas",
+        ),
+        option_group(
+            "Connection & Communication Options",
+            "read-timeout",
+        ),
+        option_group("Help", "help"),
+    ],
+    "bowtie filter-implementations": [
+        option_group(
+            "Required",
+            "implementation",
+        ),
+        option_group(
+            "Filters",
+            "supports-dialect",
+            "language",
+        ),
+        option_group(
+            "Connection & Communication Options",
+            "read-timeout",
+        ),
+        option_group("Help", "help"),
+    ],
+    "bowtie run": [
+        option_group(
+            "Required",
+            "implementation",
+        ),
+        option_group(
+            "Schema Behavior Options",
+            "dialect",
+            "set-schema",
+        ),
+        option_group(
+            "Test Run Options",
+            "fail-fast",
+            "filter",
+            "max-error",
+            "max-fail",
+        ),
+        option_group(
+            "Connection & Communication Options",
+            "read-timeout",
+            "validate-implementations",
+        ),
+        option_group("Help", "help"),
+    ],
+}
+
+
+@click.rich_config(
+    help_config=click.RichHelpConfiguration(
+        command_groups=_COMMAND_GROUPS,
+        option_groups=_OPTION_GROUPS,
+        style_commands_table_column_width_ratio=(1, 3),
+        # Otherwise there's an uncomfortable amount of internal whitespace.
+        max_width=120,
+    ),
+)
 @click.group(
     context_settings=dict(help_option_names=["--help", "-h"]),
-    epilog="""
-    If you don't know where to begin, `bowtie validate` (for checking
-    what any given implementations think of your schema) or `bowtie suite`
-    (for running the official test suite against implementations) are likely
-    good places to start.
+    # needing to explicitly dedent here, as well as the extra newline
+    # before "Full documentation" both seem like rich-click bugs.
+    epilog=dedent(
+        """
+        If you don't know where to begin, `bowtie validate --help` or
+        `bowtie suite --help` are likely good places to start.
 
-    Full documentation can also be found at https://docs.bowtie.report
-    """,
+        Full documentation can also be found at https://docs.bowtie.report
+        """,
+    ),
 )
 @click.version_option(prog_name="bowtie", package_name="bowtie-json-schema")
 @click.option(
     "--log-level",
     "-L",
     help="How verbose should Bowtie be?",
     default="warning",
@@ -111,19 +282,19 @@
         ],
     ),
 )
 def main(log_level: str):
     """
     A meta-validator for the JSON Schema specifications.
 
-    Bowtie gives you access to JSON Schema across every programming
-    language and implementation.
+    Bowtie gives you access to the JSON Schema ecosystem across every
+    programming language and implementation.
 
-    It lets you compare implementations to each other, or to known correct
-    results from the JSON Schema test suite.
+    It lets you compare implementations either to each other or to known
+    correct results from the official JSON Schema test suite.
     """
     _redirect_structlog(log_level=getattr(logging, log_level.upper()))
 
 
 P = ParamSpec("P")
 
 
@@ -241,15 +412,15 @@
     help=(
         "The path to a previously generated collection of reports, "
         "used to generate the badges."
     ),
 )
 def badges(site: Path):
     """
-    Generate Bowtie badges from previous runs.
+    Generate Bowtie badges for implementations using a previous Bowtie run.
 
     Will generate badges for any existing dialects, and ignore any for which a
     report was not generated.
     """
     outdir = site / "badges"
     try:
         outdir.mkdir()
@@ -938,15 +1109,19 @@
 def run(
     input: Iterable[str],
     filter: CaseTransform,
     dialect: Dialect,
     **kwargs: Any,
 ):
     """
-    Run test cases written in Bowtie's test format.
+    Run test cases written directly in Bowtie's testing format.
+
+    This is generally useful if you wish to hand-author which schemas to
+    include in the schema registry, or otherwise exactly control the contents
+    of a test case.
     """
     cases = filter(
         TestCase.from_dict(dialect=dialect, **json.loads(line))
         for line in input
     )
     return asyncio.run(_run(**kwargs, cases=cases, dialect=dialect))
 
@@ -984,15 +1159,15 @@
     schema: Any,
     instances: Iterable[TextIO],
     expect: str,
     description: str,
     **kwargs: Any,
 ):
     """
-    Validate instances across any implementation.
+    Validate instances under a schema across any supported implementation.
     """
     if not instances:
         return _EX_NOINPUT
 
     case = TestCase(
         description=description,
         schema=schema,
@@ -1054,15 +1229,18 @@
 async def filter_implementations(
     ctx: click.Context,
     start: Callable[[], AsyncIterator[Implementation]],
     dialects: Sequence[Dialect],
     languages: Set[str],
 ):
     """
-    Output implementations matching a given criteria.
+    Output implementations which match the given criteria.
+
+    Useful for piping or otherwise using the resulting output for further
+    Bowtie commands.
     """
     if not dialects and languages == KNOWN_LANGUAGES:
         for implementation in ctx.params.get("image_names", ()):
             click.echo(implementation.removeprefix(f"{IMAGE_REPOSITORY}/"))
         return
 
     async for each in start():
@@ -1091,15 +1269,15 @@
 )
 @click.option(
     "--boolean-schemas/--no-boolean-schemas",
     "-b/-B",
     "booleans",
     default=None,
     help=(
-        "If provided, show only dialects which do (or do not)"
+        "If provided, show only dialects which do (or do not) "
         "support boolean schemas. Otherwise show either kind."
     ),
 )
 async def filter_dialects(
     start: Callable[[], AsyncIterator[Implementation]],
     dialects: Iterable[Dialect],
     latest: bool,
@@ -1194,15 +1372,15 @@
 @FORMAT
 async def smoke(
     start: Callable[[], AsyncIterator[Implementation]],
     format: _F,
     echo: Callable[..., None],
 ) -> int:
     """
-    Smoke test implementations for basic correctness.
+    Smoke test implementations for basic correctness against Bowtie's protocol.
     """
     exit_code = 0
 
     async for implementation in start():
         echo(f"Testing {implementation.name!r}...\n", file=sys.stderr)
         serializable: list[dict[str, Any]] = []
         implementation_exit_code = 0
@@ -1262,15 +1440,15 @@
 @click.argument("input", type=_suite.ClickParam())
 def suite(
     input: tuple[Iterable[TestCase], Dialect, dict[str, Any]],
     filter: CaseTransform,
     **kwargs: Any,
 ):
     """
-    Run tests from the official JSON Schema suite.
+    Run the official JSON Schema test suite against any implementation.
 
     Supports a number of possible inputs:
 
         * file paths found on the local file system containing tests, e.g.:
 
             - ``{PATH}/tests/draft7`` to run the draft 7 version's tests out of a local checkout of the test suite
```

### Comparing `bowtie_json_schema-2024.4.3/bowtie/_commands.py` & `bowtie_json_schema-2024.4.4/bowtie/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,22 +210,14 @@
     issue_url: str | None = field(default=None)
 
     errored = False
     skipped: bool = field(init=False, default=True)
 
     description = "skipped"
 
-    @property
-    def reason(self) -> str:
-        if self.message is not None:
-            return self.message
-        if self.issue_url is not None:
-            return self.issue_url
-        return "skipped"
-
     @classmethod
     def in_skipped_case(cls):
         """
         A skipped test which mentions it is part of an entirely skipped case.
         """
         return cls(message="All tests in this test case were skipped.")
 
@@ -235,21 +227,14 @@
     context: dict[str, Any] = field(factory=dict)
 
     errored: bool = field(init=False, default=True)
     skipped: bool = False
 
     description = "error"
 
-    @property
-    def reason(self) -> str:
-        message = self.context.get("message")
-        if message:
-            return message
-        return "Encountered an error."
-
     @classmethod
     def in_errored_case(cls):
         """
         A errored test which mentions it is part of an entirely errored case.
         """
         return cls(
             context=dict(message="All tests in this test case errored."),
```

### Comparing `bowtie_json_schema-2024.4.3/bowtie/_containers.py` & `bowtie_json_schema-2024.4.4/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/_core.py` & `bowtie_json_schema-2024.4.4/bowtie/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from contextlib import asynccontextmanager
 from datetime import date
 from functools import cache
 from importlib.resources import files
 from pathlib import Path
-from typing import TYPE_CHECKING, Protocol, TypeVar
+from typing import TYPE_CHECKING, Protocol, TypeVar, cast
 from uuid import uuid4
 import json
 
 from attrs import asdict, evolve, field, frozen, mutable
 from diagnostic import DiagnosticError
 from referencing.jsonschema import (
     EMPTY_REGISTRY,
@@ -64,15 +64,18 @@
     A dialect of JSON Schema.
     """
 
     pretty_name: str
     uri: URL = field(repr=False)
     short_name: str = field(repr=False)
     first_publication_date: date = field(repr=False)
-    aliases: Set[str] = field(default=frozenset(), repr=False)
+    aliases: Set[str] = field(
+        default=cast(frozenset[str], frozenset()),
+        repr=False,
+    )
     has_boolean_schemas: bool = field(default=True, repr=False)
 
     def __lt__(self, other: Any):
         if other.__class__ is not Dialect:
             return NotImplemented
         return self.first_publication_date < other.first_publication_date
```

### Comparing `bowtie_json_schema-2024.4.3/bowtie/_report.py` & `bowtie_json_schema-2024.4.4/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/_suite.py` & `bowtie_json_schema-2024.4.4/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/exceptions.py` & `bowtie_json_schema-2024.4.4/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/hypothesis.py` & `bowtie_json_schema-2024.4.4/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.4.4/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.4.4/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.4.4/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.4.4/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.4.4/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.4.4/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/data/dialects.json` & `bowtie_json_schema-2024.4.4/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/docs/Makefile` & `bowtie_json_schema-2024.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/docs/cli.rst` & `bowtie_json_schema-2024.4.4/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/docs/conf.py` & `bowtie_json_schema-2024.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/docs/contributing.rst` & `bowtie_json_schema-2024.4.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/docs/github-actions.rst` & `bowtie_json_schema-2024.4.4/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/docs/implementers.rst` & `bowtie_json_schema-2024.4.4/docs/implementers.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,25 @@
 
 The purpose of `Bowtie` is to support passing :term:`instances <instance>` and :term:`schemas <schema>` through a large number of JSON Schema implementations, collecting their output for comparison.
 
 If you've written or used an implementation of JSON Schema which isn't already supported, let's see how you can add support for it to Bowtie.
 
 Bowtie orchestrates running a number of containers, passing JSON Schema test cases to each one of them, and then collecting and comparing results across implementations.
 Any JSON Schema implementation will have some way of getting schemas and instances "into" it for processing.
-We'll wrap this implementation-specific API inside a small harness which accepts input from Bowtie over standard input and writes results to standard output in the format Bowtie expects.
+We'll wrap this implementation-specific API inside a small harness which accepts input from Bowtie over standard input and writes results to standard output in the format Bowtie expects, as shown below:
+
+.. image:: _static/bowtie_diagram_light.svg
+    :class: only-light
+    :width: 80 %
+    :align: center
+
+.. image:: _static/bowtie_diagram_dark.svg
+    :class: only-dark
+    :width: 80 %
+    :align: center
 
 As a last step before we get into details, let's summarize some terminology (which you can also skip and refer back to if needed):
 
 .. glossary::
 
     implementation
         a library or program which implements the JSON Schema specification
```

### Comparing `bowtie_json_schema-2024.4.3/docs/index.rst` & `bowtie_json_schema-2024.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/docs/motd.txt` & `bowtie_json_schema-2024.4.4/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/docs/requirements.txt` & `bowtie_json_schema-2024.4.4/docs/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile --strip-extras docs/requirements.in
 #
 aiodocker==0.21.0
     # via bowtie-json-schema
-aiohttp==3.9.3
+aiohttp==3.9.4
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
 attrs==23.2.0
     # via
@@ -28,19 +28,19 @@
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
-    #   bowtie-json-schema
+    #   rich-click
     #   sphinx-click
 cryptography==42.0.5
     # via pyjwt
-diagnostic==2.0.0
+diagnostic==2.1.0
     # via bowtie-json-schema
 docutils==0.20.1
     # via
     #   diagnostic
     #   sphinx
     #   sphinx-click
     #   sphinx-prompt
@@ -50,29 +50,29 @@
     # via
     #   aiohttp
     #   aiosignal
 furo==2024.1.29
     # via -r docs/requirements.in
 github3-py==4.0.1
     # via bowtie-json-schema
-idna==3.6
+idna==3.7
     # via
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.3
     # via sphinx
 jsonschema==4.21.1
     # via bowtie-json-schema
 jsonschema-lexer==0.2.1
     # via bowtie-json-schema
 jsonschema-specifications==2023.12.1
     # via jsonschema
-lxml==5.1.0
+lxml==5.2.1
     # via sphinx-json-schema-spec
 markdown-it-py==3.0.0
     # via
     #   diagnostic
     #   rich
 markupsafe==2.1.5
     # via jinja2
@@ -80,15 +80,15 @@
     # via markdown-it-py
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 packaging==24.0
     # via sphinx
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
 pygments==2.17.2
     # via
     #   furo
     #   jsonschema-lexer
@@ -115,14 +115,17 @@
     # via
     #   github3-py
     #   sphinx
 rich==13.7.1
     # via
     #   bowtie-json-schema
     #   diagnostic
+    #   rich-click
+rich-click==1.8.0.dev6
+    # via bowtie-json-schema
 rpds-py==0.18.0
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
@@ -171,16 +174,18 @@
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r docs/requirements.in
 sphinxext-opengraph==0.9.1
     # via -r docs/requirements.in
 structlog==24.1.0
     # via bowtie-json-schema
-typing-extensions==4.10.0
-    # via aiodocker
+typing-extensions==4.11.0
+    # via
+    #   aiodocker
+    #   rich-click
 uritemplate==4.1.1
     # via github3-py
 url-py==0.10.0
     # via
     #   -r docs/requirements.in
     #   bowtie-json-schema
 urllib3==2.2.1
```

### Comparing `bowtie_json_schema-2024.4.3/docs/_static/logo.svg` & `bowtie_json_schema-2024.4.4/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/package.json` & `bowtie_json_schema-2024.4.4/frontend/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9796783625730996%*

 * *Differences: {"'dependencies'": "{'bootstrap': '^5.3.3', 'react-bootstrap': '^2.10.2', 'react-bootstrap-icons': "*

 * *                   "'^1.11.4', 'react-router-dom': '^6.22.3'}",*

 * * "'devDependencies'": "{'@types/react': '^18.2.79', '@types/react-dom': '^18.2.25', 'eslint': "*

 * *                      "'8.57.0', 'eslint-plugin-react': '7.34.1', 'typescript': '^5.4.4', 'vite': "*

 * *                      "'^5.2.10', 'vitest': '^1.5.0'}"}*

```diff
@@ -1,40 +1,40 @@
 {
     "dependencies": {
-        "bootstrap": "^5.3.2",
+        "bootstrap": "^5.3.3",
         "dayjs": "^1.11.10",
         "react": "^18.2.0",
-        "react-bootstrap": "^2.10.1",
-        "react-bootstrap-icons": "^1.11.3",
+        "react-bootstrap": "^2.10.2",
+        "react-bootstrap-icons": "^1.11.4",
         "react-dom": "^18.2.0",
-        "react-router-dom": "^6.22.1",
+        "react-router-dom": "^6.22.3",
         "react-syntax-highlighter": "^15.5.0",
         "urijs": "^1.19.11"
     },
     "description": "The UI displays the outcomes generated by Bowtie, which serves as a meta-validator for the JSON Schema specification",
     "devDependencies": {
-        "@types/react": "^18.2.56",
-        "@types/react-dom": "^18.2.19",
+        "@types/react": "^18.2.79",
+        "@types/react-dom": "^18.2.25",
         "@types/react-syntax-highlighter": "^15.5.11",
         "@types/react-test-renderer": "^18.0.7",
         "@types/urijs": "^1.19.25",
         "@typescript-eslint/eslint-plugin": "^7.0.0",
         "@typescript-eslint/parser": "^6.21.0",
         "@vitejs/plugin-react": "^4.2.1",
-        "eslint": "8.56.0",
-        "eslint-plugin-react": "7.33.2",
+        "eslint": "8.57.0",
+        "eslint-plugin-react": "7.34.1",
         "eslint-plugin-react-hooks": "4.6.0",
         "jsdom": "^24.0.0",
         "react-test-renderer": "^18.2.0",
         "ts-loader": "^9.5.1",
         "ts-node": "^10.9.2",
-        "typescript": "^5.3.3",
-        "vite": "^5.1.7",
+        "typescript": "^5.4.4",
+        "vite": "^5.2.10",
         "vite-bundle-visualizer": "^1.1.0",
-        "vitest": "^1.3.1"
+        "vitest": "^1.5.0"
     },
     "engines": {
         "node": ">=21.0.0"
     },
     "eslintConfig": {
         "env": {
             "browser": true,
```

### Comparing `bowtie_json_schema-2024.4.3/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.4.4/frontend/pnpm-lock.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -2,99 +2,99 @@
 
 settings:
   autoInstallPeers: true
   excludeLinksFromLockfile: false
 
 dependencies:
   bootstrap:
-    specifier: ^5.3.2
-    version: 5.3.2(@popperjs/core@2.11.8)
+    specifier: ^5.3.3
+    version: 5.3.3(@popperjs/core@2.11.8)
   dayjs:
     specifier: ^1.11.10
     version: 1.11.10
   react:
     specifier: ^18.2.0
     version: 18.2.0
   react-bootstrap:
-    specifier: ^2.10.1
-    version: 2.10.1(@types/react@18.2.56)(react-dom@18.2.0)(react@18.2.0)
+    specifier: ^2.10.2
+    version: 2.10.2(@types/react@18.2.79)(react-dom@18.2.0)(react@18.2.0)
   react-bootstrap-icons:
-    specifier: ^1.11.3
-    version: 1.11.3(react@18.2.0)
+    specifier: ^1.11.4
+    version: 1.11.4(react@18.2.0)
   react-dom:
     specifier: ^18.2.0
     version: 18.2.0(react@18.2.0)
   react-router-dom:
-    specifier: ^6.22.1
-    version: 6.22.1(react-dom@18.2.0)(react@18.2.0)
+    specifier: ^6.22.3
+    version: 6.22.3(react-dom@18.2.0)(react@18.2.0)
   react-syntax-highlighter:
     specifier: ^15.5.0
     version: 15.5.0(react@18.2.0)
   urijs:
     specifier: ^1.19.11
     version: 1.19.11
 
 devDependencies:
   '@types/react':
-    specifier: ^18.2.56
-    version: 18.2.56
+    specifier: ^18.2.79
+    version: 18.2.79
   '@types/react-dom':
-    specifier: ^18.2.19
-    version: 18.2.19
+    specifier: ^18.2.25
+    version: 18.2.25
   '@types/react-syntax-highlighter':
     specifier: ^15.5.11
     version: 15.5.11
   '@types/react-test-renderer':
     specifier: ^18.0.7
     version: 18.0.7
   '@types/urijs':
     specifier: ^1.19.25
     version: 1.19.25
   '@typescript-eslint/eslint-plugin':
     specifier: ^7.0.0
-    version: 7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.56.0)(typescript@5.3.3)
+    version: 7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.57.0)(typescript@5.4.4)
   '@typescript-eslint/parser':
     specifier: ^6.21.0
-    version: 6.21.0(eslint@8.56.0)(typescript@5.3.3)
+    version: 6.21.0(eslint@8.57.0)(typescript@5.4.4)
   '@vitejs/plugin-react':
     specifier: ^4.2.1
-    version: 4.2.1(vite@5.1.7)
+    version: 4.2.1(vite@5.2.10)
   eslint:
-    specifier: 8.56.0
-    version: 8.56.0
+    specifier: 8.57.0
+    version: 8.57.0
   eslint-plugin-react:
-    specifier: 7.33.2
-    version: 7.33.2(eslint@8.56.0)
+    specifier: 7.34.1
+    version: 7.34.1(eslint@8.57.0)
   eslint-plugin-react-hooks:
     specifier: 4.6.0
-    version: 4.6.0(eslint@8.56.0)
+    version: 4.6.0(eslint@8.57.0)
   jsdom:
     specifier: ^24.0.0
     version: 24.0.0
   react-test-renderer:
     specifier: ^18.2.0
     version: 18.2.0(react@18.2.0)
   ts-loader:
     specifier: ^9.5.1
-    version: 9.5.1(typescript@5.3.3)(webpack@5.89.0)
+    version: 9.5.1(typescript@5.4.4)(webpack@5.89.0)
   ts-node:
     specifier: ^10.9.2
-    version: 10.9.2(@types/node@20.11.5)(typescript@5.3.3)
+    version: 10.9.2(@types/node@20.11.5)(typescript@5.4.4)
   typescript:
-    specifier: ^5.3.3
-    version: 5.3.3
+    specifier: ^5.4.4
+    version: 5.4.4
   vite:
-    specifier: ^5.1.7
-    version: 5.1.7(@types/node@20.11.5)
+    specifier: ^5.2.10
+    version: 5.2.10(@types/node@20.11.5)
   vite-bundle-visualizer:
     specifier: ^1.1.0
     version: 1.1.0
   vitest:
-    specifier: ^1.3.1
-    version: 1.3.1(@types/node@20.11.5)(jsdom@24.0.0)
+    specifier: ^1.5.0
+    version: 1.5.0(@types/node@20.11.5)(jsdom@24.0.0)
 
 packages:
 
   /@aashutoshrathi/word-wrap@1.2.6:
     resolution: {integrity: sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==}
     engines: {node: '>=0.10.0'}
     dev: true
@@ -333,228 +333,228 @@
   /@cspotcode/source-map-support@0.8.1:
     resolution: {integrity: sha512-IchNf6dN4tHoMFIn/7OE8LWZ19Y6q/67Bmf6vnGREv8RSbBVb9LPJxEcnwrcwX6ixSvaiGoomAUvu4YSxXrVgw==}
     engines: {node: '>=12'}
     dependencies:
       '@jridgewell/trace-mapping': 0.3.9
     dev: true
 
-  /@esbuild/aix-ppc64@0.19.11:
-    resolution: {integrity: sha512-FnzU0LyE3ySQk7UntJO4+qIiQgI7KoODnZg5xzXIrFJlKd2P2gwHsHY4927xj9y5PJmJSzULiUCWmv7iWnNa7g==}
+  /@esbuild/aix-ppc64@0.20.2:
+    resolution: {integrity: sha512-D+EBOJHXdNZcLJRBkhENNG8Wji2kgc9AZ9KiPr1JuZjsNtyHzrsfLRrY0tk2H2aoFu6RANO1y1iPPUCDYWkb5g==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [aix]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/android-arm64@0.19.11:
-    resolution: {integrity: sha512-aiu7K/5JnLj//KOnOfEZ0D90obUkRzDMyqd/wNAUQ34m4YUPVhRZpnqKV9uqDGxT7cToSDnIHsGooyIczu9T+Q==}
+  /@esbuild/android-arm64@0.20.2:
+    resolution: {integrity: sha512-mRzjLacRtl/tWU0SvD8lUEwb61yP9cqQo6noDZP/O8VkwafSYwZ4yWy24kan8jE/IMERpYncRt2dw438LP3Xmg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/android-arm@0.19.11:
-    resolution: {integrity: sha512-5OVapq0ClabvKvQ58Bws8+wkLCV+Rxg7tUVbo9xu034Nm536QTII4YzhaFriQ7rMrorfnFKUsArD2lqKbFY4vw==}
+  /@esbuild/android-arm@0.20.2:
+    resolution: {integrity: sha512-t98Ra6pw2VaDhqNWO2Oph2LXbz/EJcnLmKLGBJwEwXX/JAN83Fym1rU8l0JUWK6HkIbWONCSSatf4sf2NBRx/w==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/android-x64@0.19.11:
-    resolution: {integrity: sha512-eccxjlfGw43WYoY9QgB82SgGgDbibcqyDTlk3l3C0jOVHKxrjdc9CTwDUQd0vkvYg5um0OH+GpxYvp39r+IPOg==}
+  /@esbuild/android-x64@0.20.2:
+    resolution: {integrity: sha512-btzExgV+/lMGDDa194CcUQm53ncxzeBrWJcncOBxuC6ndBkKxnHdFJn86mCIgTELsooUmwUm9FkhSp5HYu00Rg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/darwin-arm64@0.19.11:
-    resolution: {integrity: sha512-ETp87DRWuSt9KdDVkqSoKoLFHYTrkyz2+65fj9nfXsaV3bMhTCjtQfw3y+um88vGRKRiF7erPrh/ZuIdLUIVxQ==}
+  /@esbuild/darwin-arm64@0.20.2:
+    resolution: {integrity: sha512-4J6IRT+10J3aJH3l1yzEg9y3wkTDgDk7TSDFX+wKFiWjqWp/iCfLIYzGyasx9l0SAFPT1HwSCR+0w/h1ES/MjA==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/darwin-x64@0.19.11:
-    resolution: {integrity: sha512-fkFUiS6IUK9WYUO/+22omwetaSNl5/A8giXvQlcinLIjVkxwTLSktbF5f/kJMftM2MJp9+fXqZ5ezS7+SALp4g==}
+  /@esbuild/darwin-x64@0.20.2:
+    resolution: {integrity: sha512-tBcXp9KNphnNH0dfhv8KYkZhjc+H3XBkF5DKtswJblV7KlT9EI2+jeA8DgBjp908WEuYll6pF+UStUCfEpdysA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/freebsd-arm64@0.19.11:
-    resolution: {integrity: sha512-lhoSp5K6bxKRNdXUtHoNc5HhbXVCS8V0iZmDvyWvYq9S5WSfTIHU2UGjcGt7UeS6iEYp9eeymIl5mJBn0yiuxA==}
+  /@esbuild/freebsd-arm64@0.20.2:
+    resolution: {integrity: sha512-d3qI41G4SuLiCGCFGUrKsSeTXyWG6yem1KcGZVS+3FYlYhtNoNgYrWcvkOoaqMhwXSMrZRl69ArHsGJ9mYdbbw==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/freebsd-x64@0.19.11:
-    resolution: {integrity: sha512-JkUqn44AffGXitVI6/AbQdoYAq0TEullFdqcMY/PCUZ36xJ9ZJRtQabzMA+Vi7r78+25ZIBosLTOKnUXBSi1Kw==}
+  /@esbuild/freebsd-x64@0.20.2:
+    resolution: {integrity: sha512-d+DipyvHRuqEeM5zDivKV1KuXn9WeRX6vqSqIDgwIfPQtwMP4jaDsQsDncjTDDsExT4lR/91OLjRo8bmC1e+Cw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-arm64@0.19.11:
-    resolution: {integrity: sha512-LneLg3ypEeveBSMuoa0kwMpCGmpu8XQUh+mL8XXwoYZ6Be2qBnVtcDI5azSvh7vioMDhoJFZzp9GWp9IWpYoUg==}
+  /@esbuild/linux-arm64@0.20.2:
+    resolution: {integrity: sha512-9pb6rBjGvTFNira2FLIWqDk/uaf42sSyLE8j1rnUpuzsODBq7FvpwHYZxQ/It/8b+QOS1RYfqgGFNLRI+qlq2A==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-arm@0.19.11:
-    resolution: {integrity: sha512-3CRkr9+vCV2XJbjwgzjPtO8T0SZUmRZla+UL1jw+XqHZPkPgZiyWvbDvl9rqAN8Zl7qJF0O/9ycMtjU67HN9/Q==}
+  /@esbuild/linux-arm@0.20.2:
+    resolution: {integrity: sha512-VhLPeR8HTMPccbuWWcEUD1Az68TqaTYyj6nfE4QByZIQEQVWBB8vup8PpR7y1QHL3CpcF6xd5WVBU/+SBEvGTg==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-ia32@0.19.11:
-    resolution: {integrity: sha512-caHy++CsD8Bgq2V5CodbJjFPEiDPq8JJmBdeyZ8GWVQMjRD0sU548nNdwPNvKjVpamYYVL40AORekgfIubwHoA==}
+  /@esbuild/linux-ia32@0.20.2:
+    resolution: {integrity: sha512-o10utieEkNPFDZFQm9CoP7Tvb33UutoJqg3qKf1PWVeeJhJw0Q347PxMvBgVVFgouYLGIhFYG0UGdBumROyiig==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-loong64@0.19.11:
-    resolution: {integrity: sha512-ppZSSLVpPrwHccvC6nQVZaSHlFsvCQyjnvirnVjbKSHuE5N24Yl8F3UwYUUR1UEPaFObGD2tSvVKbvR+uT1Nrg==}
+  /@esbuild/linux-loong64@0.20.2:
+    resolution: {integrity: sha512-PR7sp6R/UC4CFVomVINKJ80pMFlfDfMQMYynX7t1tNTeivQ6XdX5r2XovMmha/VjR1YN/HgHWsVcTRIMkymrgQ==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-mips64el@0.19.11:
-    resolution: {integrity: sha512-B5x9j0OgjG+v1dF2DkH34lr+7Gmv0kzX6/V0afF41FkPMMqaQ77pH7CrhWeR22aEeHKaeZVtZ6yFwlxOKPVFyg==}
+  /@esbuild/linux-mips64el@0.20.2:
+    resolution: {integrity: sha512-4BlTqeutE/KnOiTG5Y6Sb/Hw6hsBOZapOVF6njAESHInhlQAghVVZL1ZpIctBOoTFbQyGW+LsVYZ8lSSB3wkjA==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-ppc64@0.19.11:
-    resolution: {integrity: sha512-MHrZYLeCG8vXblMetWyttkdVRjQlQUb/oMgBNurVEnhj4YWOr4G5lmBfZjHYQHHN0g6yDmCAQRR8MUHldvvRDA==}
+  /@esbuild/linux-ppc64@0.20.2:
+    resolution: {integrity: sha512-rD3KsaDprDcfajSKdn25ooz5J5/fWBylaaXkuotBDGnMnDP1Uv5DLAN/45qfnf3JDYyJv/ytGHQaziHUdyzaAg==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-riscv64@0.19.11:
-    resolution: {integrity: sha512-f3DY++t94uVg141dozDu4CCUkYW+09rWtaWfnb3bqe4w5NqmZd6nPVBm+qbz7WaHZCoqXqHz5p6CM6qv3qnSSQ==}
+  /@esbuild/linux-riscv64@0.20.2:
+    resolution: {integrity: sha512-snwmBKacKmwTMmhLlz/3aH1Q9T8v45bKYGE3j26TsaOVtjIag4wLfWSiZykXzXuE1kbCE+zJRmwp+ZbIHinnVg==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-s390x@0.19.11:
-    resolution: {integrity: sha512-A5xdUoyWJHMMlcSMcPGVLzYzpcY8QP1RtYzX5/bS4dvjBGVxdhuiYyFwp7z74ocV7WDc0n1harxmpq2ePOjI0Q==}
+  /@esbuild/linux-s390x@0.20.2:
+    resolution: {integrity: sha512-wcWISOobRWNm3cezm5HOZcYz1sKoHLd8VL1dl309DiixxVFoFe/o8HnwuIwn6sXre88Nwj+VwZUvJf4AFxkyrQ==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-x64@0.19.11:
-    resolution: {integrity: sha512-grbyMlVCvJSfxFQUndw5mCtWs5LO1gUlwP4CDi4iJBbVpZcqLVT29FxgGuBJGSzyOxotFG4LoO5X+M1350zmPA==}
+  /@esbuild/linux-x64@0.20.2:
+    resolution: {integrity: sha512-1MdwI6OOTsfQfek8sLwgyjOXAu+wKhLEoaOLTjbijk6E2WONYpH9ZU2mNtR+lZ2B4uwr+usqGuVfFT9tMtGvGw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/netbsd-x64@0.19.11:
-    resolution: {integrity: sha512-13jvrQZJc3P230OhU8xgwUnDeuC/9egsjTkXN49b3GcS5BKvJqZn86aGM8W9pd14Kd+u7HuFBMVtrNGhh6fHEQ==}
+  /@esbuild/netbsd-x64@0.20.2:
+    resolution: {integrity: sha512-K8/DhBxcVQkzYc43yJXDSyjlFeHQJBiowJ0uVL6Tor3jGQfSGHNNJcWxNbOI8v5k82prYqzPuwkzHt3J1T1iZQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/openbsd-x64@0.19.11:
-    resolution: {integrity: sha512-ysyOGZuTp6SNKPE11INDUeFVVQFrhcNDVUgSQVDzqsqX38DjhPEPATpid04LCoUr2WXhQTEZ8ct/EgJCUDpyNw==}
+  /@esbuild/openbsd-x64@0.20.2:
+    resolution: {integrity: sha512-eMpKlV0SThJmmJgiVyN9jTPJ2VBPquf6Kt/nAoo6DgHAoN57K15ZghiHaMvqjCye/uU4X5u3YSMgVBI1h3vKrQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/sunos-x64@0.19.11:
-    resolution: {integrity: sha512-Hf+Sad9nVwvtxy4DXCZQqLpgmRTQqyFyhT3bZ4F2XlJCjxGmRFF0Shwn9rzhOYRB61w9VMXUkxlBy56dk9JJiQ==}
+  /@esbuild/sunos-x64@0.20.2:
+    resolution: {integrity: sha512-2UyFtRC6cXLyejf/YEld4Hajo7UHILetzE1vsRcGL3earZEW77JxrFjH4Ez2qaTiEfMgAXxfAZCm1fvM/G/o8w==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-arm64@0.19.11:
-    resolution: {integrity: sha512-0P58Sbi0LctOMOQbpEOvOL44Ne0sqbS0XWHMvvrg6NE5jQ1xguCSSw9jQeUk2lfrXYsKDdOe6K+oZiwKPilYPQ==}
+  /@esbuild/win32-arm64@0.20.2:
+    resolution: {integrity: sha512-GRibxoawM9ZCnDxnP3usoUDO9vUkpAxIIZ6GQI+IlVmr5kP3zUq+l17xELTHMWTWzjxa2guPNyrpq1GWmPvcGQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-ia32@0.19.11:
-    resolution: {integrity: sha512-6YOrWS+sDJDmshdBIQU+Uoyh7pQKrdykdefC1avn76ss5c+RN6gut3LZA4E2cH5xUEp5/cA0+YxRaVtRAb0xBg==}
+  /@esbuild/win32-ia32@0.20.2:
+    resolution: {integrity: sha512-HfLOfn9YWmkSKRQqovpnITazdtquEW8/SoHW7pWpuEeguaZI4QnCRW6b+oZTztdBnZOS2hqJ6im/D5cPzBTTlQ==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-x64@0.19.11:
-    resolution: {integrity: sha512-vfkhltrjCAb603XaFhqhAF4LGDi2M4OrCRrFusyQ+iTLQ/o60QQXxc9cZC/FFpihBI9N1Grn6SMKVJ4KP7Fuiw==}
+  /@esbuild/win32-x64@0.20.2:
+    resolution: {integrity: sha512-N49X4lJX27+l9jbLKSqZ6bKNjzQvHaT8IIFUy+YIqmXQdjYCToGWwOItDrfby14c78aDd5NHQl29xingXfCdLQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@eslint-community/eslint-utils@4.4.0(eslint@8.56.0):
+  /@eslint-community/eslint-utils@4.4.0(eslint@8.57.0):
     resolution: {integrity: sha512-1/sA4dwrzBAyeUoQ6oxahHKmrZvsnLCg4RfxW3ZFGGmQkSNQPFNLV9CUEFQP1x9EYXHTo5p6xdhZM1Ne9p/AfA==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     peerDependencies:
       eslint: ^6.0.0 || ^7.0.0 || >=8.0.0
     dependencies:
-      eslint: 8.56.0
+      eslint: 8.57.0
       eslint-visitor-keys: 3.4.3
     dev: true
 
   /@eslint-community/regexpp@4.10.0:
     resolution: {integrity: sha512-Cu96Sd2By9mCNTx2iyKOmq10v22jUVQv0lQnlGNy16oE9589yE+QADPbrMGCkA51cKZSg3Pu/aTJVTGfL/qjUA==}
     engines: {node: ^12.0.0 || ^14.0.0 || >=16.0.0}
     dev: true
@@ -572,16 +572,16 @@
       js-yaml: 4.1.0
       minimatch: 3.1.2
       strip-json-comments: 3.1.1
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@eslint/js@8.56.0:
-    resolution: {integrity: sha512-gMsVel9D7f2HLkBma9VbtzZRehRogVRfbr++f06nL2vnCGCNlzOD+/MUov/F4p8myyAHspEhVobgjpX64q5m6A==}
+  /@eslint/js@8.57.0:
+    resolution: {integrity: sha512-Ys+3g2TaW7gADOJzPt83SJtCDhMjndcDMFVQ/Tj9iA1BfJzFKD9mAUXT3OenpuPHbI6P/myECxRJrofUsDx/5g==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     dev: true
 
   /@humanwhocodes/config-array@0.11.14:
     resolution: {integrity: sha512-3T8LkOmg45BV5FICb15QQMsyUSWrQ8AygVfC7ZG32zOalnqrilm018ZVCw0eapXux8FtA33q8PSRSstjee3jSg==}
     engines: {node: '>=10.10.0'}
     dependencies:
@@ -683,30 +683,30 @@
     peerDependencies:
       react: ^16.8.0 || ^17.0.0-rc.1 || ^18.0.0
     dependencies:
       '@swc/helpers': 0.5.3
       react: 18.2.0
     dev: false
 
-  /@remix-run/router@1.15.1:
-    resolution: {integrity: sha512-zcU0gM3z+3iqj8UX45AmWY810l3oUmXM7uH4dt5xtzvMhRtYVhKGOmgOd1877dOPPepfCjUv57w+syamWIYe7w==}
+  /@remix-run/router@1.15.3:
+    resolution: {integrity: sha512-Oy8rmScVrVxWZVOpEF57ovlnhpZ8CCPlnIIumVcV9nFdiSIrus99+Lw78ekXyGvVDlIsFJbSfmSovJUhCWYV3w==}
     engines: {node: '>=14.0.0'}
     dev: false
 
   /@restart/hooks@0.4.15(react@18.2.0):
     resolution: {integrity: sha512-cZFXYTxbpzYcieq/mBwSyXgqnGMHoBVh3J7MU0CCoIB4NRZxV9/TuwTBAaLMqpNhC3zTPMCgkQ5Ey07L02Xmcw==}
     peerDependencies:
       react: '>=16.8.0'
     dependencies:
       dequal: 2.0.3
       react: 18.2.0
     dev: false
 
-  /@restart/ui@1.6.6(react-dom@18.2.0)(react@18.2.0):
-    resolution: {integrity: sha512-eC3puKuWE1SRYbojWHXnvCNHGgf3uzHCb6JOhnF4OXPibOIPEkR1sqDSkL643ydigxwh+ruCa1CmYHlzk7ikKA==}
+  /@restart/ui@1.6.8(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-6ndCv3oZ7r9vuP1Ok9KH55TM1/UkdBnP/fSraW0DFDMbPMzWKhVKeFAIEUCRCSdzayjZDcFYK6xbMlipN9dmMA==}
     peerDependencies:
       react: '>=16.14.0'
       react-dom: '>=16.14.0'
     dependencies:
       '@babel/runtime': 7.23.8
       '@popperjs/core': 2.11.8
       '@react-aria/ssr': 3.9.1(react@18.2.0)
@@ -716,112 +716,128 @@
       dom-helpers: 5.2.1
       react: 18.2.0
       react-dom: 18.2.0(react@18.2.0)
       uncontrollable: 8.0.4(react@18.2.0)
       warning: 4.0.3
     dev: false
 
-  /@rollup/rollup-android-arm-eabi@4.9.6:
-    resolution: {integrity: sha512-MVNXSSYN6QXOulbHpLMKYi60ppyO13W9my1qogeiAqtjb2yR4LSmfU2+POvDkLzhjYLXz9Rf9+9a3zFHW1Lecg==}
+  /@rollup/rollup-android-arm-eabi@4.14.2:
+    resolution: {integrity: sha512-ahxSgCkAEk+P/AVO0vYr7DxOD3CwAQrT0Go9BJyGQ9Ef0QxVOfjDZMiF4Y2s3mLyPrjonchIMH/tbWHucJMykQ==}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-android-arm64@4.9.6:
-    resolution: {integrity: sha512-T14aNLpqJ5wzKNf5jEDpv5zgyIqcpn1MlwCrUXLrwoADr2RkWA0vOWP4XxbO9aiO3dvMCQICZdKeDrFl7UMClw==}
+  /@rollup/rollup-android-arm64@4.14.2:
+    resolution: {integrity: sha512-lAarIdxZWbFSHFSDao9+I/F5jDaKyCqAPMq5HqnfpBw8dKDiCaaqM0lq5h1pQTLeIqueeay4PieGR5jGZMWprw==}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-darwin-arm64@4.9.6:
-    resolution: {integrity: sha512-CqNNAyhRkTbo8VVZ5R85X73H3R5NX9ONnKbXuHisGWC0qRbTTxnF1U4V9NafzJbgGM0sHZpdO83pLPzq8uOZFw==}
+  /@rollup/rollup-darwin-arm64@4.14.2:
+    resolution: {integrity: sha512-SWsr8zEUk82KSqquIMgZEg2GE5mCSfr9sE/thDROkX6pb3QQWPp8Vw8zOq2GyxZ2t0XoSIUlvHDkrf5Gmf7x3Q==}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-darwin-x64@4.9.6:
-    resolution: {integrity: sha512-zRDtdJuRvA1dc9Mp6BWYqAsU5oeLixdfUvkTHuiYOHwqYuQ4YgSmi6+/lPvSsqc/I0Omw3DdICx4Tfacdzmhog==}
+  /@rollup/rollup-darwin-x64@4.14.2:
+    resolution: {integrity: sha512-o/HAIrQq0jIxJAhgtIvV5FWviYK4WB0WwV91SLUnsliw1lSAoLsmgEEgRWzDguAFeUEUUoIWXiJrPqU7vGiVkA==}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-linux-arm-gnueabihf@4.9.6:
-    resolution: {integrity: sha512-oNk8YXDDnNyG4qlNb6is1ojTOGL/tRhbbKeE/YuccItzerEZT68Z9gHrY3ROh7axDc974+zYAPxK5SH0j/G+QQ==}
+  /@rollup/rollup-linux-arm-gnueabihf@4.14.2:
+    resolution: {integrity: sha512-nwlJ65UY9eGq91cBi6VyDfArUJSKOYt5dJQBq8xyLhvS23qO+4Nr/RreibFHjP6t+5ap2ohZrUJcHv5zk5ju/g==}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-linux-arm64-gnu@4.9.6:
-    resolution: {integrity: sha512-Z3O60yxPtuCYobrtzjo0wlmvDdx2qZfeAWTyfOjEDqd08kthDKexLpV97KfAeUXPosENKd8uyJMRDfFMxcYkDQ==}
+  /@rollup/rollup-linux-arm64-gnu@4.14.2:
+    resolution: {integrity: sha512-Pg5TxxO2IVlMj79+c/9G0LREC9SY3HM+pfAwX7zj5/cAuwrbfj2Wv9JbMHIdPCfQpYsI4g9mE+2Bw/3aeSs2rQ==}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-linux-arm64-musl@4.9.6:
-    resolution: {integrity: sha512-gpiG0qQJNdYEVad+1iAsGAbgAnZ8j07FapmnIAQgODKcOTjLEWM9sRb+MbQyVsYCnA0Im6M6QIq6ax7liws6eQ==}
+  /@rollup/rollup-linux-arm64-musl@4.14.2:
+    resolution: {integrity: sha512-cAOTjGNm84gc6tS02D1EXtG7tDRsVSDTBVXOLbj31DkwfZwgTPYZ6aafSU7rD/4R2a34JOwlF9fQayuTSkoclA==}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-linux-riscv64-gnu@4.9.6:
-    resolution: {integrity: sha512-+uCOcvVmFUYvVDr27aiyun9WgZk0tXe7ThuzoUTAukZJOwS5MrGbmSlNOhx1j80GdpqbOty05XqSl5w4dQvcOA==}
+  /@rollup/rollup-linux-powerpc64le-gnu@4.14.2:
+    resolution: {integrity: sha512-4RyT6v1kXb7C0fn6zV33rvaX05P0zHoNzaXI/5oFHklfKm602j+N4mn2YvoezQViRLPnxP8M1NaY4s/5kXO5cw==}
+    cpu: [ppc64]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-riscv64-gnu@4.14.2:
+    resolution: {integrity: sha512-KNUH6jC/vRGAKSorySTyc/yRYlCwN/5pnMjXylfBniwtJx5O7X17KG/0efj8XM3TZU7raYRXJFFReOzNmL1n1w==}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-linux-x64-gnu@4.9.6:
-    resolution: {integrity: sha512-HUNqM32dGzfBKuaDUBqFB7tP6VMN74eLZ33Q9Y1TBqRDn+qDonkAUyKWwF9BR9unV7QUzffLnz9GrnKvMqC/fw==}
+  /@rollup/rollup-linux-s390x-gnu@4.14.2:
+    resolution: {integrity: sha512-xPV4y73IBEXToNPa3h5lbgXOi/v0NcvKxU0xejiFw6DtIYQqOTMhZ2DN18/HrrP0PmiL3rGtRG9gz1QE8vFKXQ==}
+    cpu: [s390x]
+    os: [linux]
+    requiresBuild: true
+    dev: true
+    optional: true
+
+  /@rollup/rollup-linux-x64-gnu@4.14.2:
+    resolution: {integrity: sha512-QBhtr07iFGmF9egrPOWyO5wciwgtzKkYPNLVCFZTmr4TWmY0oY2Dm/bmhHjKRwZoGiaKdNcKhFtUMBKvlchH+Q==}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-linux-x64-musl@4.9.6:
-    resolution: {integrity: sha512-ch7M+9Tr5R4FK40FHQk8VnML0Szi2KRujUgHXd/HjuH9ifH72GUmw6lStZBo3c3GB82vHa0ZoUfjfcM7JiiMrQ==}
+  /@rollup/rollup-linux-x64-musl@4.14.2:
+    resolution: {integrity: sha512-8zfsQRQGH23O6qazZSFY5jP5gt4cFvRuKTpuBsC1ZnSWxV8ZKQpPqOZIUtdfMOugCcBvFGRa1pDC/tkf19EgBw==}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-win32-arm64-msvc@4.9.6:
-    resolution: {integrity: sha512-VD6qnR99dhmTQ1mJhIzXsRcTBvTjbfbGGwKAHcu+52cVl15AC/kplkhxzW/uT0Xl62Y/meBKDZvoJSJN+vTeGA==}
+  /@rollup/rollup-win32-arm64-msvc@4.14.2:
+    resolution: {integrity: sha512-H4s8UjgkPnlChl6JF5empNvFHp77Jx+Wfy2EtmYPe9G22XV+PMuCinZVHurNe8ggtwoaohxARJZbaH/3xjB/FA==}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-win32-ia32-msvc@4.9.6:
-    resolution: {integrity: sha512-J9AFDq/xiRI58eR2NIDfyVmTYGyIZmRcvcAoJ48oDld/NTR8wyiPUu2X/v1navJ+N/FGg68LEbX3Ejd6l8B7MQ==}
+  /@rollup/rollup-win32-ia32-msvc@4.14.2:
+    resolution: {integrity: sha512-djqpAjm/i8erWYF0K6UY4kRO3X5+T4TypIqw60Q8MTqSBaQNpNXDhxdjpZ3ikgb+wn99svA7jxcXpiyg9MUsdw==}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@rollup/rollup-win32-x64-msvc@4.9.6:
-    resolution: {integrity: sha512-jqzNLhNDvIZOrt69Ce4UjGRpXJBzhUBzawMwnaDAwyHriki3XollsewxWzOzz+4yOFDkuJHtTsZFwMxhYJWmLQ==}
+  /@rollup/rollup-win32-x64-msvc@4.14.2:
+    resolution: {integrity: sha512-teAqzLT0yTYZa8ZP7zhFKEx4cotS8Tkk5XiqNMJhD4CpaWB1BHARE4Qy+RzwnXvSAYv+Q3jAqCVBS+PS+Yee8Q==}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
   /@sinclair/typebox@0.27.8:
@@ -912,48 +928,44 @@
     dependencies:
       undici-types: 5.26.5
     dev: true
 
   /@types/prop-types@15.7.11:
     resolution: {integrity: sha512-ga8y9v9uyeiLdpKddhxYQkxNDrfvuPrlFb0N1qnZZByvcElJaXthF1UhvCh9TLWJBEHeNtdnbysW7Y6Uq8CVng==}
 
-  /@types/react-dom@18.2.19:
-    resolution: {integrity: sha512-aZvQL6uUbIJpjZk4U8JZGbau9KDeAwMfmhyWorxgBkqDIEf6ROjRozcmPIicqsUwPUjbkDfHKgGee1Lq65APcA==}
+  /@types/react-dom@18.2.25:
+    resolution: {integrity: sha512-o/V48vf4MQh7juIKZU2QGDfli6p1+OOi5oXx36Hffpc9adsHeXjVp8rHuPkjd8VT8sOJ2Zp05HR7CdpGTIUFUA==}
     dependencies:
-      '@types/react': 18.2.56
+      '@types/react': 18.2.79
     dev: true
 
   /@types/react-syntax-highlighter@15.5.11:
     resolution: {integrity: sha512-ZqIJl+Pg8kD+47kxUjvrlElrraSUrYa4h0dauY/U/FTUuprSCqvUj+9PNQNQzVc6AJgIWUUxn87/gqsMHNbRjw==}
     dependencies:
-      '@types/react': 18.2.56
+      '@types/react': 18.2.79
     dev: true
 
   /@types/react-test-renderer@18.0.7:
     resolution: {integrity: sha512-1+ANPOWc6rB3IkSnElhjv6VLlKg2dSv/OWClUyZimbLsQyBn8Js9Vtdsi3UICJ2rIQ3k2la06dkB+C92QfhKmg==}
     dependencies:
-      '@types/react': 18.2.56
+      '@types/react': 18.2.79
     dev: true
 
   /@types/react-transition-group@4.4.10:
     resolution: {integrity: sha512-hT/+s0VQs2ojCX823m60m5f0sL5idt9SO6Tj6Dg+rdphGPIeJbJ6CxvBYkgkGKrYeDjvIpKTR38UzmtHJOGW3Q==}
     dependencies:
-      '@types/react': 18.2.56
+      '@types/react': 18.2.79
     dev: false
 
-  /@types/react@18.2.56:
-    resolution: {integrity: sha512-NpwHDMkS/EFZF2dONFQHgkPRwhvgq/OAvIaGQzxGSBmaeR++kTg6njr15Vatz0/2VcCEwJQFi6Jf4Q0qBu0rLA==}
+  /@types/react@18.2.79:
+    resolution: {integrity: sha512-RwGAGXPl9kSXwdNTafkOEuFrTBD5SA2B3iEB96xi8+xu5ddUa/cpvyVCSNn+asgLCTHkb5ZxN8gbuibYJi4s1w==}
     dependencies:
       '@types/prop-types': 15.7.11
-      '@types/scheduler': 0.16.8
       csstype: 3.1.3
 
-  /@types/scheduler@0.16.8:
-    resolution: {integrity: sha512-WZLiwShhwLRmeV6zH+GkbOFT6Z6VklCItrDioxUnv+u4Ll+8vKeFySoFyK/0ctcRpOmwAicELfmys1sDc/Rw+A==}
-
   /@types/semver@7.5.6:
     resolution: {integrity: sha512-dn1l8LaMea/IjDoHNd9J52uBbInB796CDffS6VdIxvqYCPSG0V0DzHp76GpaWnlhg88uYyPbXCDIowa86ybd5A==}
     dev: true
 
   /@types/unist@2.0.10:
     resolution: {integrity: sha512-IfYcSBWE3hLpBg8+X2SEa8LVkJdJEkT2Ese2aaLs3ptGdVtABxndrMaxuFlQ1qdFf9Q5rDvDpxI3WwgvKFAsQA==}
     dev: false
@@ -962,60 +974,60 @@
     resolution: {integrity: sha512-XOfUup9r3Y06nFAZh3WvO0rBU4OtlfPB/vgxpjg+NRdGU6CN6djdc6OEiH+PcqHCY6eFLo9Ista73uarf4gnBg==}
     dev: true
 
   /@types/warning@3.0.3:
     resolution: {integrity: sha512-D1XC7WK8K+zZEveUPY+cf4+kgauk8N4eHr/XIHXGlGYkHLud6hK9lYfZk1ry1TNh798cZUCgb6MqGEG8DkJt6Q==}
     dev: false
 
-  /@typescript-eslint/eslint-plugin@7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.56.0)(typescript@5.3.3):
+  /@typescript-eslint/eslint-plugin@7.0.0(@typescript-eslint/parser@6.21.0)(eslint@8.57.0)(typescript@5.4.4):
     resolution: {integrity: sha512-M72SJ0DkcQVmmsbqlzc6EJgb/3Oz2Wdm6AyESB4YkGgCxP8u5jt5jn4/OBMPK3HLOxcttZq5xbBBU7e2By4SZQ==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       '@typescript-eslint/parser': ^6.0.0 || ^6.0.0-alpha
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
       '@eslint-community/regexpp': 4.10.0
-      '@typescript-eslint/parser': 6.21.0(eslint@8.56.0)(typescript@5.3.3)
+      '@typescript-eslint/parser': 6.21.0(eslint@8.57.0)(typescript@5.4.4)
       '@typescript-eslint/scope-manager': 7.0.0
-      '@typescript-eslint/type-utils': 7.0.0(eslint@8.56.0)(typescript@5.3.3)
-      '@typescript-eslint/utils': 7.0.0(eslint@8.56.0)(typescript@5.3.3)
+      '@typescript-eslint/type-utils': 7.0.0(eslint@8.57.0)(typescript@5.4.4)
+      '@typescript-eslint/utils': 7.0.0(eslint@8.57.0)(typescript@5.4.4)
       '@typescript-eslint/visitor-keys': 7.0.0
       debug: 4.3.4
-      eslint: 8.56.0
+      eslint: 8.57.0
       graphemer: 1.4.0
       ignore: 5.3.0
       natural-compare: 1.4.0
       semver: 7.5.4
-      ts-api-utils: 1.0.3(typescript@5.3.3)
-      typescript: 5.3.3
+      ts-api-utils: 1.0.3(typescript@5.4.4)
+      typescript: 5.4.4
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/parser@6.21.0(eslint@8.56.0)(typescript@5.3.3):
+  /@typescript-eslint/parser@6.21.0(eslint@8.57.0)(typescript@5.4.4):
     resolution: {integrity: sha512-tbsV1jPne5CkFQCgPBcDOt30ItF7aJoZL997JSF7MhGQqOeT3svWRYxiqlfA5RUdlHN6Fi+EI9bxqbdyAUZjYQ==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       eslint: ^7.0.0 || ^8.0.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
       '@typescript-eslint/scope-manager': 6.21.0
       '@typescript-eslint/types': 6.21.0
-      '@typescript-eslint/typescript-estree': 6.21.0(typescript@5.3.3)
+      '@typescript-eslint/typescript-estree': 6.21.0(typescript@5.4.4)
       '@typescript-eslint/visitor-keys': 6.21.0
       debug: 4.3.4
-      eslint: 8.56.0
-      typescript: 5.3.3
+      eslint: 8.57.0
+      typescript: 5.4.4
     transitivePeerDependencies:
       - supports-color
     dev: true
 
   /@typescript-eslint/scope-manager@6.21.0:
     resolution: {integrity: sha512-OwLUIWZJry80O99zvqXVEioyniJMa+d2GrqpUTqi5/v5D5rOrppJVBPa0yKCblcigC0/aYAzxxqQ1B+DS2RYsg==}
     engines: {node: ^16.0.0 || >=18.0.0}
@@ -1028,45 +1040,45 @@
     resolution: {integrity: sha512-IxTStwhNDPO07CCrYuAqjuJ3Xf5MrMaNgbAZPxFXAUpAtwqFxiuItxUaVtP/SJQeCdJjwDGh9/lMOluAndkKeg==}
     engines: {node: ^16.0.0 || >=18.0.0}
     dependencies:
       '@typescript-eslint/types': 7.0.0
       '@typescript-eslint/visitor-keys': 7.0.0
     dev: true
 
-  /@typescript-eslint/type-utils@7.0.0(eslint@8.56.0)(typescript@5.3.3):
+  /@typescript-eslint/type-utils@7.0.0(eslint@8.57.0)(typescript@5.4.4):
     resolution: {integrity: sha512-FIM8HPxj1P2G7qfrpiXvbHeHypgo2mFpFGoh5I73ZlqmJOsloSa1x0ZyXCer43++P1doxCgNqIOLqmZR6SOT8g==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/typescript-estree': 7.0.0(typescript@5.3.3)
-      '@typescript-eslint/utils': 7.0.0(eslint@8.56.0)(typescript@5.3.3)
+      '@typescript-eslint/typescript-estree': 7.0.0(typescript@5.4.4)
+      '@typescript-eslint/utils': 7.0.0(eslint@8.57.0)(typescript@5.4.4)
       debug: 4.3.4
-      eslint: 8.56.0
-      ts-api-utils: 1.0.3(typescript@5.3.3)
-      typescript: 5.3.3
+      eslint: 8.57.0
+      ts-api-utils: 1.0.3(typescript@5.4.4)
+      typescript: 5.4.4
     transitivePeerDependencies:
       - supports-color
     dev: true
 
   /@typescript-eslint/types@6.21.0:
     resolution: {integrity: sha512-1kFmZ1rOm5epu9NZEZm1kckCDGj5UJEf7P1kliH4LKu/RkwpsfqqGmY2OOcUs18lSlQBKLDYBOGxRVtrMN5lpg==}
     engines: {node: ^16.0.0 || >=18.0.0}
     dev: true
 
   /@typescript-eslint/types@7.0.0:
     resolution: {integrity: sha512-9ZIJDqagK1TTs4W9IyeB2sH/s1fFhN9958ycW8NRTg1vXGzzH5PQNzq6KbsbVGMT+oyyfa17DfchHDidcmf5cg==}
     engines: {node: ^16.0.0 || >=18.0.0}
     dev: true
 
-  /@typescript-eslint/typescript-estree@6.21.0(typescript@5.3.3):
+  /@typescript-eslint/typescript-estree@6.21.0(typescript@5.4.4):
     resolution: {integrity: sha512-6npJTkZcO+y2/kr+z0hc4HwNfrrP4kNYh57ek7yCNlrBjWQ1Y0OS7jiZTkgumrvkX5HkEKXFZkkdFNkaW2wmUQ==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
@@ -1074,21 +1086,21 @@
       '@typescript-eslint/types': 6.21.0
       '@typescript-eslint/visitor-keys': 6.21.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.3
       semver: 7.5.4
-      ts-api-utils: 1.0.3(typescript@5.3.3)
-      typescript: 5.3.3
+      ts-api-utils: 1.0.3(typescript@5.4.4)
+      typescript: 5.4.4
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/typescript-estree@7.0.0(typescript@5.3.3):
+  /@typescript-eslint/typescript-estree@7.0.0(typescript@5.4.4):
     resolution: {integrity: sha512-JzsOzhJJm74aQ3c9um/aDryHgSHfaX8SHFIu9x4Gpik/+qxLvxUylhTsO9abcNu39JIdhY2LgYrFxTii3IajLA==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
@@ -1096,33 +1108,33 @@
       '@typescript-eslint/types': 7.0.0
       '@typescript-eslint/visitor-keys': 7.0.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.3
       semver: 7.5.4
-      ts-api-utils: 1.0.3(typescript@5.3.3)
-      typescript: 5.3.3
+      ts-api-utils: 1.0.3(typescript@5.4.4)
+      typescript: 5.4.4
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/utils@7.0.0(eslint@8.56.0)(typescript@5.3.3):
+  /@typescript-eslint/utils@7.0.0(eslint@8.57.0)(typescript@5.4.4):
     resolution: {integrity: sha512-kuPZcPAdGcDBAyqDn/JVeJVhySvpkxzfXjJq1X1BFSTYo1TTuo4iyb937u457q4K0In84p6u2VHQGaFnv7VYqg==}
     engines: {node: ^16.0.0 || >=18.0.0}
     peerDependencies:
       eslint: ^8.56.0
     dependencies:
-      '@eslint-community/eslint-utils': 4.4.0(eslint@8.56.0)
+      '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
       '@types/json-schema': 7.0.15
       '@types/semver': 7.5.6
       '@typescript-eslint/scope-manager': 7.0.0
       '@typescript-eslint/types': 7.0.0
-      '@typescript-eslint/typescript-estree': 7.0.0(typescript@5.3.3)
-      eslint: 8.56.0
+      '@typescript-eslint/typescript-estree': 7.0.0(typescript@5.4.4)
+      eslint: 8.57.0
       semver: 7.5.4
     transitivePeerDependencies:
       - supports-color
       - typescript
     dev: true
 
   /@typescript-eslint/visitor-keys@6.21.0:
@@ -1141,62 +1153,62 @@
       eslint-visitor-keys: 3.4.3
     dev: true
 
   /@ungap/structured-clone@1.2.0:
     resolution: {integrity: sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==}
     dev: true
 
-  /@vitejs/plugin-react@4.2.1(vite@5.1.7):
+  /@vitejs/plugin-react@4.2.1(vite@5.2.10):
     resolution: {integrity: sha512-oojO9IDc4nCUUi8qIR11KoQm0XFFLIwsRBwHRR4d/88IWghn1y6ckz/bJ8GHDCsYEJee8mDzqtJxh15/cisJNQ==}
     engines: {node: ^14.18.0 || >=16.0.0}
     peerDependencies:
       vite: ^4.2.0 || ^5.0.0
     dependencies:
       '@babel/core': 7.23.7
       '@babel/plugin-transform-react-jsx-self': 7.23.3(@babel/core@7.23.7)
       '@babel/plugin-transform-react-jsx-source': 7.23.3(@babel/core@7.23.7)
       '@types/babel__core': 7.20.5
       react-refresh: 0.14.0
-      vite: 5.1.7(@types/node@20.11.5)
+      vite: 5.2.10(@types/node@20.11.5)
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@vitest/expect@1.3.1:
-    resolution: {integrity: sha512-xofQFwIzfdmLLlHa6ag0dPV8YsnKOCP1KdAeVVh34vSjN2dcUiXYCD9htu/9eM7t8Xln4v03U9HLxLpPlsXdZw==}
+  /@vitest/expect@1.5.0:
+    resolution: {integrity: sha512-0pzuCI6KYi2SIC3LQezmxujU9RK/vwC1U9R0rLuGlNGcOuDWxqWKu6nUdFsX9tH1WU0SXtAxToOsEjeUn1s3hA==}
     dependencies:
-      '@vitest/spy': 1.3.1
-      '@vitest/utils': 1.3.1
+      '@vitest/spy': 1.5.0
+      '@vitest/utils': 1.5.0
       chai: 4.4.1
     dev: true
 
-  /@vitest/runner@1.3.1:
-    resolution: {integrity: sha512-5FzF9c3jG/z5bgCnjr8j9LNq/9OxV2uEBAITOXfoe3rdZJTdO7jzThth7FXv/6b+kdY65tpRQB7WaKhNZwX+Kg==}
+  /@vitest/runner@1.5.0:
+    resolution: {integrity: sha512-7HWwdxXP5yDoe7DTpbif9l6ZmDwCzcSIK38kTSIt6CFEpMjX4EpCgT6wUmS0xTXqMI6E/ONmfgRKmaujpabjZQ==}
     dependencies:
-      '@vitest/utils': 1.3.1
+      '@vitest/utils': 1.5.0
       p-limit: 5.0.0
       pathe: 1.1.2
     dev: true
 
-  /@vitest/snapshot@1.3.1:
-    resolution: {integrity: sha512-EF++BZbt6RZmOlE3SuTPu/NfwBF6q4ABS37HHXzs2LUVPBLx2QoY/K0fKpRChSo8eLiuxcbCVfqKgx/dplCDuQ==}
+  /@vitest/snapshot@1.5.0:
+    resolution: {integrity: sha512-qpv3fSEuNrhAO3FpH6YYRdaECnnRjg9VxbhdtPwPRnzSfHVXnNzzrpX4cJxqiwgRMo7uRMWDFBlsBq4Cr+rO3A==}
     dependencies:
       magic-string: 0.30.7
       pathe: 1.1.2
       pretty-format: 29.7.0
     dev: true
 
-  /@vitest/spy@1.3.1:
-    resolution: {integrity: sha512-xAcW+S099ylC9VLU7eZfdT9myV67Nor9w9zhf0mGCYJSO+zM2839tOeROTdikOi/8Qeusffvxb/MyBSOja1Uig==}
+  /@vitest/spy@1.5.0:
+    resolution: {integrity: sha512-vu6vi6ew5N5MMHJjD5PoakMRKYdmIrNJmyfkhRpQt5d9Ewhw9nZ5Aqynbi3N61bvk9UvZ5UysMT6ayIrZ8GA9w==}
     dependencies:
       tinyspy: 2.2.1
     dev: true
 
-  /@vitest/utils@1.3.1:
-    resolution: {integrity: sha512-d3Waie/299qqRyHTm2DjADeTaNdNSVsnwHPWrs20JMpjh6eiVq7ggggweO8rc4arhf6rRkWuHKwvxGvejUXZZQ==}
+  /@vitest/utils@1.5.0:
+    resolution: {integrity: sha512-BDU0GNL8MWkRkSRdNFvCUCAVOeHaUlVJ9Tx0TYBZyXaaOTmGtUFObzchCivIBrIwKzvZA7A9sCejVhXM2aY98A==}
     dependencies:
       diff-sequences: 29.6.3
       estree-walker: 3.0.3
       loupe: 2.3.7
       pretty-format: 29.7.0
     dev: true
 
@@ -1402,14 +1414,22 @@
   /array-buffer-byte-length@1.0.0:
     resolution: {integrity: sha512-LPuwb2P+NrQw3XhxGc36+XSvuBPopovXYTR9Ew++Du9Yb/bx5AzBfrIsBoj0EZUifjQU+sHL21sseZ3jerWO/A==}
     dependencies:
       call-bind: 1.0.5
       is-array-buffer: 3.0.2
     dev: true
 
+  /array-buffer-byte-length@1.0.1:
+    resolution: {integrity: sha512-ahC5W1xgou+KTXix4sAO8Ki12Q+jf4i0+tmk3sC+zgcynshkHxzpXdImBehiUYKKKDwvfFiJl1tZt6ewscS1Mg==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      is-array-buffer: 3.0.4
+    dev: true
+
   /array-includes@3.1.7:
     resolution: {integrity: sha512-dlcsNBIiWhPkHdOEEKnehA+RNUWDc4UqFtnIXU4uuYDPtA4LDkr7qip2p0VvFAEXNDr0yWZ9PJyIRiGjRLQzwQ==}
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.5
       define-properties: 1.2.1
       es-abstract: 1.22.3
@@ -1418,14 +1438,26 @@
     dev: true
 
   /array-union@2.1.0:
     resolution: {integrity: sha512-HGyxoOTYUyCM6stUe6EJgnd4EoewAI7zMdfqO+kGjnlZmBDz/cR5pf8r/cR4Wq60sL/p0IkcjUEEPwS3GFrIyw==}
     engines: {node: '>=8'}
     dev: true
 
+  /array.prototype.findlast@1.2.5:
+    resolution: {integrity: sha512-CVvd6FHg1Z3POpBLxO6E6zr+rSKEQ9L6rZHAaY7lLfhKsWYUBBOuMs0e9o24oopj6H+geRCX0YJ+TJLBK2eHyQ==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      define-properties: 1.2.1
+      es-abstract: 1.23.3
+      es-errors: 1.3.0
+      es-object-atoms: 1.0.0
+      es-shim-unscopables: 1.0.2
+    dev: true
+
   /array.prototype.flat@1.3.2:
     resolution: {integrity: sha512-djYB+Zx2vLewY8RWlNCUdHjDXs2XOgm602S9E7P/UpHgfeHL00cRiIF+IN/G/aUJ7kGPb6yO/ErDI5V2s8iycA==}
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.5
       define-properties: 1.2.1
       es-abstract: 1.22.3
@@ -1438,22 +1470,31 @@
     dependencies:
       call-bind: 1.0.5
       define-properties: 1.2.1
       es-abstract: 1.22.3
       es-shim-unscopables: 1.0.2
     dev: true
 
-  /array.prototype.tosorted@1.1.2:
-    resolution: {integrity: sha512-HuQCHOlk1Weat5jzStICBCd83NxiIMwqDg/dHEsoefabn/hJRj5pVdWcPUSpRrwhwxZOsQassMpgN/xRYFBMIg==}
+  /array.prototype.toreversed@1.1.2:
+    resolution: {integrity: sha512-wwDCoT4Ck4Cz7sLtgUmzR5UV3YF5mFHUlbChCzZBQZ+0m2cl/DH3tKgvphv1nKgFsJ48oCSg6p91q2Vm0I/ZMA==}
     dependencies:
       call-bind: 1.0.5
       define-properties: 1.2.1
       es-abstract: 1.22.3
       es-shim-unscopables: 1.0.2
-      get-intrinsic: 1.2.2
+    dev: true
+
+  /array.prototype.tosorted@1.1.3:
+    resolution: {integrity: sha512-/DdH4TiTmOKzyQbp/eadcCVexiCb36xJg7HshYOYJnNZFDj33GEv0P7GxsynpShhq4OLYJzbGcBDkLsDt7MnNg==}
+    dependencies:
+      call-bind: 1.0.5
+      define-properties: 1.2.1
+      es-abstract: 1.22.3
+      es-errors: 1.3.0
+      es-shim-unscopables: 1.0.2
     dev: true
 
   /arraybuffer.prototype.slice@1.0.2:
     resolution: {integrity: sha512-yMBKppFur/fbHu9/6USUe03bZ4knMYiwFBcyiaXB8Go0qNehwX6inYPzK9U0NeQvGxKthcmHcaR8P5MStSRBAw==}
     engines: {node: '>= 0.4'}
     dependencies:
       array-buffer-byte-length: 1.0.0
@@ -1461,39 +1502,54 @@
       define-properties: 1.2.1
       es-abstract: 1.22.3
       get-intrinsic: 1.2.2
       is-array-buffer: 3.0.2
       is-shared-array-buffer: 1.0.2
     dev: true
 
-  /assertion-error@1.1.0:
-    resolution: {integrity: sha512-jgsaNduz+ndvGyFt3uSuWqvy4lCnIJiovtouQN5JZHOKCS2QuhEdbcQHFhVksz2N2U9hXJo8odG7ETyWlEeuDw==}
+  /arraybuffer.prototype.slice@1.0.3:
+    resolution: {integrity: sha512-bMxMKAjg13EBSVscxTaYA4mRc5t1UAXa2kXiGTNfZ079HIWXEkKmkgFrh/nJqamaLSrXO5H4WFFkPEaLJWbs3A==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      array-buffer-byte-length: 1.0.1
+      call-bind: 1.0.7
+      define-properties: 1.2.1
+      es-abstract: 1.23.3
+      es-errors: 1.3.0
+      get-intrinsic: 1.2.4
+      is-array-buffer: 3.0.4
+      is-shared-array-buffer: 1.0.3
     dev: true
 
-  /asynciterator.prototype@1.0.0:
-    resolution: {integrity: sha512-wwHYEIS0Q80f5mosx3L/dfG5t5rjEa9Ft51GTaNt862EnpyGHpgz2RkZvLPp1oF5TnAiTohkEKVEu8pQPJI7Vg==}
-    dependencies:
-      has-symbols: 1.0.3
+  /assertion-error@1.1.0:
+    resolution: {integrity: sha512-jgsaNduz+ndvGyFt3uSuWqvy4lCnIJiovtouQN5JZHOKCS2QuhEdbcQHFhVksz2N2U9hXJo8odG7ETyWlEeuDw==}
     dev: true
 
   /asynckit@0.4.0:
     resolution: {integrity: sha512-Oei9OH4tRh0YqU3GxhX79dM/mwVgvbZJaSNaRk+bshkj0S5cfHcgYakreBjrHwatXKbz+IoIdYLxrKim2MjW0Q==}
     dev: true
 
   /available-typed-arrays@1.0.5:
     resolution: {integrity: sha512-DMD0KiN46eipeziST1LPP/STfDU0sufISXmjSgvVsoU2tqxctQeASejWcfNtxYKqETM1UxQ8sp2OrSBWpHY6sw==}
     engines: {node: '>= 0.4'}
     dev: true
 
+  /available-typed-arrays@1.0.7:
+    resolution: {integrity: sha512-wvUjBtSGN7+7SjNpq/9M2Tg350UZD3q62IFZLbRAR1bSMlCo1ZaeW+BJ+D090e4hIIZLBcTDWe4Mh4jvUDajzQ==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      possible-typed-array-names: 1.0.0
+    dev: true
+
   /balanced-match@1.0.2:
     resolution: {integrity: sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==}
     dev: true
 
-  /bootstrap@5.3.2(@popperjs/core@2.11.8):
-    resolution: {integrity: sha512-D32nmNWiQHo94BKHLmOrdjlL05q1c8oxbtBphQFb9Z5to6eGRDCm0QgeaZ4zFBHzfg2++rqa2JkqCcxDy0sH0g==}
+  /bootstrap@5.3.3(@popperjs/core@2.11.8):
+    resolution: {integrity: sha512-8HLCdWgyoMguSO9o+aH+iuZ+aht+mzW0u3HIMzVu7Srrpv7EBBxTnrFlSCskwdY1+EOFQSm7uMJhNQHkdPcmjg==}
     peerDependencies:
       '@popperjs/core': ^2.11.8
     dependencies:
       '@popperjs/core': 2.11.8
     dev: false
 
   /brace-expansion@1.1.11:
@@ -1540,14 +1596,25 @@
     resolution: {integrity: sha512-C3nQxfFZxFRVoJoGKKI8y3MOEo129NQ+FgQ08iye+Mk4zNZZGdjfs06bVTr+DBSlA66Q2VEcMki/cUCP4SercQ==}
     dependencies:
       function-bind: 1.1.2
       get-intrinsic: 1.2.2
       set-function-length: 1.2.0
     dev: true
 
+  /call-bind@1.0.7:
+    resolution: {integrity: sha512-GHTSNSYICQ7scH7sZ+M2rFopRoLh8t2bLSW6BbgrtLsahOIB5iyAVJf9GjWK3cYTDaMj4XdBpM1cA6pIS0Kv2w==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      es-define-property: 1.0.0
+      es-errors: 1.3.0
+      function-bind: 1.1.2
+      get-intrinsic: 1.2.4
+      set-function-length: 1.2.2
+    dev: true
+
   /callsites@3.1.0:
     resolution: {integrity: sha512-P8BjAsXvZS+VIDUI11hHCQEv74YT67YUi5JJFNWIqL235sBmjX4+qx9Muvls5ivyNENctx46xQLQ3aTuE7ssaQ==}
     engines: {node: '>=6'}
     dev: true
 
   /caniuse-lite@1.0.30001579:
     resolution: {integrity: sha512-u5AUVkixruKHJjw/pj9wISlcMpgFWzSrczLZbrqBSxukQixmg0SJ5sZTpvaFvxU0HoQKd4yoyAogyrAz9pzJnA==}
@@ -1690,14 +1757,41 @@
     resolution: {integrity: sha512-ZYP5VBHshaDAiVZxjbRVcFJpc+4xGgT0bK3vzy1HLN8jTO975HEbuYzZJcHoQEY5K1a0z8YayJkyVETa08eNTg==}
     engines: {node: '>=18'}
     dependencies:
       whatwg-mimetype: 4.0.0
       whatwg-url: 14.0.0
     dev: true
 
+  /data-view-buffer@1.0.1:
+    resolution: {integrity: sha512-0lht7OugA5x3iJLOWFhWK/5ehONdprk0ISXqVFn/NFrDu+cuc8iADFrGQz5BnRK7LLU3JmkbXSxaqX+/mXYtUA==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      es-errors: 1.3.0
+      is-data-view: 1.0.1
+    dev: true
+
+  /data-view-byte-length@1.0.1:
+    resolution: {integrity: sha512-4J7wRJD3ABAzr8wP+OcIcqq2dlUKp4DVflx++hs5h5ZKydWMI6/D/fAot+yh6g2tHh8fLFTvNOaVN357NvSrOQ==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      es-errors: 1.3.0
+      is-data-view: 1.0.1
+    dev: true
+
+  /data-view-byte-offset@1.0.0:
+    resolution: {integrity: sha512-t/Ygsytq+R995EJ5PZlD4Cu56sWa8InXySaViRzw9apusqsOO2bQP+SbYzAhR0pFKoB+43lYy8rWban9JSuXnA==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      es-errors: 1.3.0
+      is-data-view: 1.0.1
+    dev: true
+
   /dayjs@1.11.10:
     resolution: {integrity: sha512-vjAczensTgRcqDERK0SR2XMwsF/tSvnvlv6VcF2GIhg6Sx4yOIt/irsr1RDJsKiIyBzJDpCoXiWWq28MqH2cnQ==}
     dev: false
 
   /debug@4.3.4:
     resolution: {integrity: sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==}
     engines: {node: '>=6.0'}
@@ -1730,14 +1824,23 @@
     engines: {node: '>= 0.4'}
     dependencies:
       get-intrinsic: 1.2.2
       gopd: 1.0.1
       has-property-descriptors: 1.0.1
     dev: true
 
+  /define-data-property@1.1.4:
+    resolution: {integrity: sha512-rBMvIzlpA8v6E+SJZoo++HAYqsLrkg7MSfIinMPFhmkorw7X+dOXVJQs+QT69zGkzMyfDnIMN2Wid1+NbL3T+A==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      es-define-property: 1.0.0
+      es-errors: 1.3.0
+      gopd: 1.0.1
+    dev: true
+
   /define-lazy-prop@2.0.0:
     resolution: {integrity: sha512-Ds09qNh8yw3khSjiJjiUInaGX9xlqZDY7JVryGxdxV7NPeuqQfplOpQ66yJFZut3jLa5zOwkXw1g9EI2uKh4Og==}
     engines: {node: '>=8'}
     dev: true
 
   /define-properties@1.2.1:
     resolution: {integrity: sha512-8QmQKqEASLd5nx0U1B1okLElbUuuttJ/AnYmRXbbbGDWh6uS208EjD4Xqq/I9wK7u0v6O08XhTWnt5XtEbR6Dg==}
@@ -1858,46 +1961,127 @@
       typed-array-byte-length: 1.0.0
       typed-array-byte-offset: 1.0.0
       typed-array-length: 1.0.4
       unbox-primitive: 1.0.2
       which-typed-array: 1.1.13
     dev: true
 
-  /es-iterator-helpers@1.0.15:
-    resolution: {integrity: sha512-GhoY8uYqd6iwUl2kgjTm4CZAf6oo5mHK7BPqx3rKgx893YSsy0LGHV6gfqqQvZt/8xM8xeOnfXBCfqclMKkJ5g==}
+  /es-abstract@1.23.3:
+    resolution: {integrity: sha512-e+HfNH61Bj1X9/jLc5v1owaLYuHdeHHSQlkhCBiTK8rBvKaULl/beGMxwrMXjpYrv4pz22BlY570vVePA2ho4A==}
+    engines: {node: '>= 0.4'}
     dependencies:
-      asynciterator.prototype: 1.0.0
-      call-bind: 1.0.5
+      array-buffer-byte-length: 1.0.1
+      arraybuffer.prototype.slice: 1.0.3
+      available-typed-arrays: 1.0.7
+      call-bind: 1.0.7
+      data-view-buffer: 1.0.1
+      data-view-byte-length: 1.0.1
+      data-view-byte-offset: 1.0.0
+      es-define-property: 1.0.0
+      es-errors: 1.3.0
+      es-object-atoms: 1.0.0
+      es-set-tostringtag: 2.0.3
+      es-to-primitive: 1.2.1
+      function.prototype.name: 1.1.6
+      get-intrinsic: 1.2.4
+      get-symbol-description: 1.0.2
+      globalthis: 1.0.3
+      gopd: 1.0.1
+      has-property-descriptors: 1.0.2
+      has-proto: 1.0.3
+      has-symbols: 1.0.3
+      hasown: 2.0.2
+      internal-slot: 1.0.7
+      is-array-buffer: 3.0.4
+      is-callable: 1.2.7
+      is-data-view: 1.0.1
+      is-negative-zero: 2.0.3
+      is-regex: 1.1.4
+      is-shared-array-buffer: 1.0.3
+      is-string: 1.0.7
+      is-typed-array: 1.1.13
+      is-weakref: 1.0.2
+      object-inspect: 1.13.1
+      object-keys: 1.1.1
+      object.assign: 4.1.5
+      regexp.prototype.flags: 1.5.2
+      safe-array-concat: 1.1.2
+      safe-regex-test: 1.0.3
+      string.prototype.trim: 1.2.9
+      string.prototype.trimend: 1.0.8
+      string.prototype.trimstart: 1.0.8
+      typed-array-buffer: 1.0.2
+      typed-array-byte-length: 1.0.1
+      typed-array-byte-offset: 1.0.2
+      typed-array-length: 1.0.6
+      unbox-primitive: 1.0.2
+      which-typed-array: 1.1.15
+    dev: true
+
+  /es-define-property@1.0.0:
+    resolution: {integrity: sha512-jxayLKShrEqqzJ0eumQbVhTYQM27CfT1T35+gCgDFoL82JLsXqTJ76zv6A0YLOgEnLUMvLzsDsGIrl8NFpT2gQ==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      get-intrinsic: 1.2.4
+    dev: true
+
+  /es-errors@1.3.0:
+    resolution: {integrity: sha512-Zf5H2Kxt2xjTvbJvP2ZWLEICxA6j+hAmMzIlypy4xcBg1vKVnx89Wy0GbS+kf5cwCVFFzdCFh2XSCFNULS6csw==}
+    engines: {node: '>= 0.4'}
+    dev: true
+
+  /es-iterator-helpers@1.0.18:
+    resolution: {integrity: sha512-scxAJaewsahbqTYrGKJihhViaM6DDZDDoucfvzNbK0pOren1g/daDQ3IAhzn+1G14rBG7w+i5N+qul60++zlKA==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
       define-properties: 1.2.1
-      es-abstract: 1.22.3
-      es-set-tostringtag: 2.0.2
+      es-abstract: 1.23.3
+      es-errors: 1.3.0
+      es-set-tostringtag: 2.0.3
       function-bind: 1.1.2
-      get-intrinsic: 1.2.2
+      get-intrinsic: 1.2.4
       globalthis: 1.0.3
-      has-property-descriptors: 1.0.1
-      has-proto: 1.0.1
+      has-property-descriptors: 1.0.2
+      has-proto: 1.0.3
       has-symbols: 1.0.3
-      internal-slot: 1.0.6
+      internal-slot: 1.0.7
       iterator.prototype: 1.1.2
-      safe-array-concat: 1.1.0
+      safe-array-concat: 1.1.2
     dev: true
 
   /es-module-lexer@1.4.1:
     resolution: {integrity: sha512-cXLGjP0c4T3flZJKQSuziYoq7MlT+rnvfZjfp7h+I7K9BNX54kP9nyWvdbwjQ4u1iWbOL4u96fgeZLToQlZC7w==}
     dev: true
 
+  /es-object-atoms@1.0.0:
+    resolution: {integrity: sha512-MZ4iQ6JwHOBQjahnjwaC1ZtIBH+2ohjamzAO3oaHcXYup7qxjF2fixyH+Q71voWHeOkI2q/TnJao/KfXYIZWbw==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      es-errors: 1.3.0
+    dev: true
+
   /es-set-tostringtag@2.0.2:
     resolution: {integrity: sha512-BuDyupZt65P9D2D2vA/zqcI3G5xRsklm5N3xCwuiy+/vKy8i0ifdsQP1sLgO4tZDSCaQUSnmC48khknGMV3D2Q==}
     engines: {node: '>= 0.4'}
     dependencies:
       get-intrinsic: 1.2.2
       has-tostringtag: 1.0.0
       hasown: 2.0.0
     dev: true
 
+  /es-set-tostringtag@2.0.3:
+    resolution: {integrity: sha512-3T8uNMC3OQTHkFUsFq8r/BwAXLHvU/9O9mE0fBc/MY5iq/8H7ncvO947LmYA6ldWw9Uh8Yhf25zu6n7nML5QWQ==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      get-intrinsic: 1.2.4
+      has-tostringtag: 1.0.2
+      hasown: 2.0.2
+    dev: true
+
   /es-shim-unscopables@1.0.2:
     resolution: {integrity: sha512-J3yBRXCzDu4ULnQwxyToo/OjdMx6akgVC7K6few0a7F/0wLtmKKN7I73AH5T2836UuXRqN7Qg+IIUw/+YJksRw==}
     dependencies:
       hasown: 2.0.0
     dev: true
 
   /es-to-primitive@1.2.1:
@@ -1905,43 +2089,43 @@
     engines: {node: '>= 0.4'}
     dependencies:
       is-callable: 1.2.7
       is-date-object: 1.0.5
       is-symbol: 1.0.4
     dev: true
 
-  /esbuild@0.19.11:
-    resolution: {integrity: sha512-HJ96Hev2hX/6i5cDVwcqiJBBtuo9+FeIJOtZ9W1kA5M6AMJRHUZlpYZ1/SbEwtO0ioNAW8rUooVpC/WehY2SfA==}
+  /esbuild@0.20.2:
+    resolution: {integrity: sha512-WdOOppmUNU+IbZ0PaDiTst80zjnrOkyJNHoKupIcVyU8Lvla3Ugx94VzkQ32Ijqd7UhHJy75gNWDMUekcrSJ6g==}
     engines: {node: '>=12'}
     hasBin: true
     requiresBuild: true
     optionalDependencies:
-      '@esbuild/aix-ppc64': 0.19.11
-      '@esbuild/android-arm': 0.19.11
-      '@esbuild/android-arm64': 0.19.11
-      '@esbuild/android-x64': 0.19.11
-      '@esbuild/darwin-arm64': 0.19.11
-      '@esbuild/darwin-x64': 0.19.11
-      '@esbuild/freebsd-arm64': 0.19.11
-      '@esbuild/freebsd-x64': 0.19.11
-      '@esbuild/linux-arm': 0.19.11
-      '@esbuild/linux-arm64': 0.19.11
-      '@esbuild/linux-ia32': 0.19.11
-      '@esbuild/linux-loong64': 0.19.11
-      '@esbuild/linux-mips64el': 0.19.11
-      '@esbuild/linux-ppc64': 0.19.11
-      '@esbuild/linux-riscv64': 0.19.11
-      '@esbuild/linux-s390x': 0.19.11
-      '@esbuild/linux-x64': 0.19.11
-      '@esbuild/netbsd-x64': 0.19.11
-      '@esbuild/openbsd-x64': 0.19.11
-      '@esbuild/sunos-x64': 0.19.11
-      '@esbuild/win32-arm64': 0.19.11
-      '@esbuild/win32-ia32': 0.19.11
-      '@esbuild/win32-x64': 0.19.11
+      '@esbuild/aix-ppc64': 0.20.2
+      '@esbuild/android-arm': 0.20.2
+      '@esbuild/android-arm64': 0.20.2
+      '@esbuild/android-x64': 0.20.2
+      '@esbuild/darwin-arm64': 0.20.2
+      '@esbuild/darwin-x64': 0.20.2
+      '@esbuild/freebsd-arm64': 0.20.2
+      '@esbuild/freebsd-x64': 0.20.2
+      '@esbuild/linux-arm': 0.20.2
+      '@esbuild/linux-arm64': 0.20.2
+      '@esbuild/linux-ia32': 0.20.2
+      '@esbuild/linux-loong64': 0.20.2
+      '@esbuild/linux-mips64el': 0.20.2
+      '@esbuild/linux-ppc64': 0.20.2
+      '@esbuild/linux-riscv64': 0.20.2
+      '@esbuild/linux-s390x': 0.20.2
+      '@esbuild/linux-x64': 0.20.2
+      '@esbuild/netbsd-x64': 0.20.2
+      '@esbuild/openbsd-x64': 0.20.2
+      '@esbuild/sunos-x64': 0.20.2
+      '@esbuild/win32-arm64': 0.20.2
+      '@esbuild/win32-ia32': 0.20.2
+      '@esbuild/win32-x64': 0.20.2
     dev: true
 
   /escalade@3.1.1:
     resolution: {integrity: sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==}
     engines: {node: '>=6'}
     dev: true
 
@@ -1951,35 +2135,37 @@
     dev: true
 
   /escape-string-regexp@4.0.0:
     resolution: {integrity: sha512-TtpcNJ3XAzx3Gq8sWRzJaVajRs0uVxA2YAkdb1jm2YkPz4G6egUFAyA3n5vtEIZefPk5Wa4UXbKuS5fKkJWdgA==}
     engines: {node: '>=10'}
     dev: true
 
-  /eslint-plugin-react-hooks@4.6.0(eslint@8.56.0):
+  /eslint-plugin-react-hooks@4.6.0(eslint@8.57.0):
     resolution: {integrity: sha512-oFc7Itz9Qxh2x4gNHStv3BqJq54ExXmfC+a1NjAta66IAN87Wu0R/QArgIS9qKzX3dXKPI9H5crl9QchNMY9+g==}
     engines: {node: '>=10'}
     peerDependencies:
       eslint: ^3.0.0 || ^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0-0
     dependencies:
-      eslint: 8.56.0
+      eslint: 8.57.0
     dev: true
 
-  /eslint-plugin-react@7.33.2(eslint@8.56.0):
-    resolution: {integrity: sha512-73QQMKALArI8/7xGLNI/3LylrEYrlKZSb5C9+q3OtOewTnMQi5cT+aE9E41sLCmli3I9PGGmD1yiZydyo4FEPw==}
+  /eslint-plugin-react@7.34.1(eslint@8.57.0):
+    resolution: {integrity: sha512-N97CxlouPT1AHt8Jn0mhhN2RrADlUAsk1/atcT2KyA/l9Q/E6ll7OIGwNumFmWfZ9skV3XXccYS19h80rHtgkw==}
     engines: {node: '>=4'}
     peerDependencies:
       eslint: ^3 || ^4 || ^5 || ^6 || ^7 || ^8
     dependencies:
       array-includes: 3.1.7
+      array.prototype.findlast: 1.2.5
       array.prototype.flatmap: 1.3.2
-      array.prototype.tosorted: 1.1.2
+      array.prototype.toreversed: 1.1.2
+      array.prototype.tosorted: 1.1.3
       doctrine: 2.1.0
-      es-iterator-helpers: 1.0.15
-      eslint: 8.56.0
+      es-iterator-helpers: 1.0.18
+      eslint: 8.57.0
       estraverse: 5.3.0
       jsx-ast-utils: 3.3.5
       minimatch: 3.1.2
       object.entries: 1.1.7
       object.fromentries: 2.0.7
       object.hasown: 1.1.3
       object.values: 1.1.7
@@ -2006,23 +2192,23 @@
     dev: true
 
   /eslint-visitor-keys@3.4.3:
     resolution: {integrity: sha512-wpc+LXeiyiisxPlEkUzU6svyS1frIO3Mgxj1fdy7Pm8Ygzguax2N3Fa/D/ag1WqbOprdI+uY6wMUl8/a2G+iag==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     dev: true
 
-  /eslint@8.56.0:
-    resolution: {integrity: sha512-Go19xM6T9puCOWntie1/P997aXxFsOi37JIHRWI514Hc6ZnaHGKY9xFhrU65RT6CcBEzZoGG1e6Nq+DT04ZtZQ==}
+  /eslint@8.57.0:
+    resolution: {integrity: sha512-dZ6+mexnaTIbSBZWgou51U6OmzIhYM2VcNdtiTtI7qPNZm35Akpr0f6vtw3w1Kmn5PYo+tZVfh13WrhpS6oLqQ==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     hasBin: true
     dependencies:
-      '@eslint-community/eslint-utils': 4.4.0(eslint@8.56.0)
+      '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
       '@eslint-community/regexpp': 4.10.0
       '@eslint/eslintrc': 2.1.4
-      '@eslint/js': 8.56.0
+      '@eslint/js': 8.57.0
       '@humanwhocodes/config-array': 0.11.14
       '@humanwhocodes/module-importer': 1.0.1
       '@nodelib/fs.walk': 1.2.8
       '@ungap/structured-clone': 1.2.0
       ajv: 6.12.6
       chalk: 4.1.2
       cross-spawn: 7.0.3
@@ -2260,27 +2446,47 @@
     dependencies:
       function-bind: 1.1.2
       has-proto: 1.0.1
       has-symbols: 1.0.3
       hasown: 2.0.0
     dev: true
 
+  /get-intrinsic@1.2.4:
+    resolution: {integrity: sha512-5uYhsJH8VJBTv7oslg4BznJYhDoRI6waYCxMmCdnTrcCrHA/fCFKoTFz2JKKE0HdDFUF7/oQuhzumXJK7paBRQ==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      es-errors: 1.3.0
+      function-bind: 1.1.2
+      has-proto: 1.0.3
+      has-symbols: 1.0.3
+      hasown: 2.0.0
+    dev: true
+
   /get-stream@8.0.1:
     resolution: {integrity: sha512-VaUJspBffn/LMCJVoMvSAdmscJyS1auj5Zulnn5UoYcY531UWmdwhRWkcGKnGU93m5HSXP9LP2usOryrBtQowA==}
     engines: {node: '>=16'}
     dev: true
 
   /get-symbol-description@1.0.0:
     resolution: {integrity: sha512-2EmdH1YvIQiZpltCNgkuiUnyukzxM/R6NDJX31Ke3BG1Nq5b0S2PhX59UKi9vZpPDQVdqn+1IcaAwnzTT5vCjw==}
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.5
       get-intrinsic: 1.2.2
     dev: true
 
+  /get-symbol-description@1.0.2:
+    resolution: {integrity: sha512-g0QYk1dZBxGwk+Ngc+ltRH2IBp2f7zBkBMBJZCDerh6EhlhSR6+9irMCuT/09zD6qkarHUSn529sK/yL4S27mg==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      es-errors: 1.3.0
+      get-intrinsic: 1.2.4
+    dev: true
+
   /glob-parent@5.1.2:
     resolution: {integrity: sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==}
     engines: {node: '>= 6'}
     dependencies:
       is-glob: 4.0.3
     dev: true
 
@@ -2367,38 +2573,63 @@
 
   /has-property-descriptors@1.0.1:
     resolution: {integrity: sha512-VsX8eaIewvas0xnvinAe9bw4WfIeODpGYikiWYLH+dma0Jw6KHYqWiWfhQlgOVK8D6PvjubK5Uc4P0iIhIcNVg==}
     dependencies:
       get-intrinsic: 1.2.2
     dev: true
 
+  /has-property-descriptors@1.0.2:
+    resolution: {integrity: sha512-55JNKuIW+vq4Ke1BjOTjM2YctQIvCT7GFzHwmfZPGo5wnrgkid0YQtnAleFSqumZm4az3n2BS+erby5ipJdgrg==}
+    dependencies:
+      es-define-property: 1.0.0
+    dev: true
+
   /has-proto@1.0.1:
     resolution: {integrity: sha512-7qE+iP+O+bgF9clE5+UoBFzE65mlBiVj3tKCrlNQ0Ogwm0BjpT/gK4SlLYDMybDh5I3TCTKnPPa0oMG7JDYrhg==}
     engines: {node: '>= 0.4'}
     dev: true
 
+  /has-proto@1.0.3:
+    resolution: {integrity: sha512-SJ1amZAJUiZS+PhsVLf5tGydlaVB8EdFpaSO4gmiUKUOxk8qzn5AIy4ZeJUmh22znIdk/uMAUT2pl3FxzVUH+Q==}
+    engines: {node: '>= 0.4'}
+    dev: true
+
   /has-symbols@1.0.3:
     resolution: {integrity: sha512-l3LCuF6MgDNwTDKkdYGEihYjt5pRPbEg46rtlmnSPlUbgmB8LOIrKJbYYFBSbnPaJexMKtiPO8hmeRjRz2Td+A==}
     engines: {node: '>= 0.4'}
     dev: true
 
   /has-tostringtag@1.0.0:
     resolution: {integrity: sha512-kFjcSNhnlGV1kyoGk7OXKSawH5JOb/LzUc5w9B02hOTO0dfFRjbHQKvg1d6cf3HbeUmtU9VbbV3qzZ2Teh97WQ==}
     engines: {node: '>= 0.4'}
     dependencies:
       has-symbols: 1.0.3
     dev: true
 
+  /has-tostringtag@1.0.2:
+    resolution: {integrity: sha512-NqADB8VjPFLM2V0VvHUewwwsw0ZWBaIdgo+ieHtK3hasLz4qeCRjYcqfB6AQrBggRKppKF8L52/VqdVsO47Dlw==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      has-symbols: 1.0.3
+    dev: true
+
   /hasown@2.0.0:
     resolution: {integrity: sha512-vUptKVTpIJhcczKBbgnS+RtcuYMB8+oNzPK2/Hp3hanz8JmpATdmmgLgSaadVREkDm+e2giHwY3ZRkyjSIDDFA==}
     engines: {node: '>= 0.4'}
     dependencies:
       function-bind: 1.1.2
     dev: true
 
+  /hasown@2.0.2:
+    resolution: {integrity: sha512-0hJU9SCPvmMzIBdZFqNPXWa6dqh7WdH0cII9y+CyS8rG3nL48Bclra9HmKhVVUHyPWNH5Y7xDwAB7bfgSjkUMQ==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      function-bind: 1.1.2
+    dev: true
+
   /hast-util-parse-selector@2.2.5:
     resolution: {integrity: sha512-7j6mrk/qqkSehsM92wQjdIgWM2/BW61u/53G6xmC8i1OmEdKLHbk419QKQUjz6LglWsfqoiHmyMRkP1BGjecNQ==}
     dev: false
 
   /hastscript@6.0.0:
     resolution: {integrity: sha512-nDM6bvd7lIqDUiYEiu5Sl/+6ReP0BMk/2f4U/Rooccxkj0P5nm+acM5PrGJ/t5I8qPGiqZSE6hVAwZEdZIvP4w==}
     dependencies:
@@ -2500,14 +2731,23 @@
     engines: {node: '>= 0.4'}
     dependencies:
       get-intrinsic: 1.2.2
       hasown: 2.0.0
       side-channel: 1.0.4
     dev: true
 
+  /internal-slot@1.0.7:
+    resolution: {integrity: sha512-NGnrKwXzSms2qUUih/ILZ5JBqNTSa1+ZmP6flaIp6KmSElgE9qdndzS3cqjrDovwFdmwsGsLdeFgB6suw+1e9g==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      es-errors: 1.3.0
+      hasown: 2.0.0
+      side-channel: 1.0.4
+    dev: true
+
   /invariant@2.2.4:
     resolution: {integrity: sha512-phJfQVBuaJM5raOpJjSfkiD6BpbCE4Ns//LaXl6wGYtUBY83nWS6Rf9tXm2e8VaK60JEjYldbPif/A2B1C2gNA==}
     dependencies:
       loose-envify: 1.4.0
     dev: false
 
   /is-alphabetical@1.0.4:
@@ -2525,14 +2765,22 @@
     resolution: {integrity: sha512-y+FyyR/w8vfIRq4eQcM1EYgSTnmHXPqaF+IgzgraytCFq5Xh8lllDVmAZolPJiZttZLeFSINPYMaEJ7/vWUa1w==}
     dependencies:
       call-bind: 1.0.5
       get-intrinsic: 1.2.2
       is-typed-array: 1.1.12
     dev: true
 
+  /is-array-buffer@3.0.4:
+    resolution: {integrity: sha512-wcjaerHw0ydZwfhiKbXJWLDY8A7yV7KhjQOpb83hGgGfId/aQa4TOvwyzn2PuswW2gPCYEL/nEAiSVpdOj1lXw==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      get-intrinsic: 1.2.4
+    dev: true
+
   /is-async-function@2.0.0:
     resolution: {integrity: sha512-Y1JXKrfykRJGdlDwdKlLpLyMIiWqWvuSd17TvZk68PLAOGOoF4Xyav1z0Xhoi+gCYjZVeC5SI+hYFOfvXmGRCA==}
     engines: {node: '>= 0.4'}
     dependencies:
       has-tostringtag: 1.0.0
     dev: true
 
@@ -2557,14 +2805,21 @@
 
   /is-core-module@2.13.1:
     resolution: {integrity: sha512-hHrIjvZsftOsvKSn2TRYl63zvxsgE0K+0mYMoH6gD4omR5IWB2KynivBQczo3+wF1cCkjzvptnI9Q0sPU66ilw==}
     dependencies:
       hasown: 2.0.0
     dev: true
 
+  /is-data-view@1.0.1:
+    resolution: {integrity: sha512-AHkaJrsUVW6wq6JS8y3JnM/GJF/9cf+k20+iDzlSaJrinEo5+7vRiteOSwBhHRiAyQATN1AmY4hwzxJKPmYf+w==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      is-typed-array: 1.1.13
+    dev: true
+
   /is-date-object@1.0.5:
     resolution: {integrity: sha512-9YQaSxsAiSwcvS33MBk3wTCVnWK+HhF8VZR2jRxehM16QcVOdHqPn4VPHmRK4lSr38n9JriurInLcP90xsYNfQ==}
     engines: {node: '>= 0.4'}
     dependencies:
       has-tostringtag: 1.0.0
     dev: true
 
@@ -2582,15 +2837,15 @@
     resolution: {integrity: sha512-SbKbANkN603Vi4jEZv49LeVJMn4yGwsbzZworEoyEiutsN3nJYdbO36zfhGJ6QEDpOZIFkDtnq5JRxmvl3jsoQ==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /is-finalizationregistry@1.0.2:
     resolution: {integrity: sha512-0by5vtUJs8iFQb5TYUHHPudOR+qXYIMKtiUzvLIZITZUjknFmziyBJuLhVRc+Ds0dREFlskDNJKYIdIzu/9pfw==}
     dependencies:
-      call-bind: 1.0.5
+      call-bind: 1.0.7
     dev: true
 
   /is-fullwidth-code-point@3.0.0:
     resolution: {integrity: sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==}
     engines: {node: '>=8'}
     dev: true
 
@@ -2617,14 +2872,19 @@
     dev: true
 
   /is-negative-zero@2.0.2:
     resolution: {integrity: sha512-dqJvarLawXsFbNDeJW7zAz8ItJ9cd28YufuuFzh0G8pNHjJMnY08Dv7sYX2uF5UpQOwieAeOExEYAWWfu7ZZUA==}
     engines: {node: '>= 0.4'}
     dev: true
 
+  /is-negative-zero@2.0.3:
+    resolution: {integrity: sha512-5KoIu2Ngpyek75jXodFvnafB6DJgr3u8uuK0LEZJjrU19DrMD3EVERaR8sjz8CCGgpZvxPl9SuE1GMVPFHx1mw==}
+    engines: {node: '>= 0.4'}
+    dev: true
+
   /is-number-object@1.0.7:
     resolution: {integrity: sha512-k1U0IRzLMo7ZlYIfzRu23Oh6MiIFasgpb9X76eqfFZAqwH44UI4KTBvBYIZ1dSL9ZzChTB9ShHfLkR4pdW5krQ==}
     engines: {node: '>= 0.4'}
     dependencies:
       has-tostringtag: 1.0.0
     dev: true
 
@@ -2656,14 +2916,21 @@
 
   /is-shared-array-buffer@1.0.2:
     resolution: {integrity: sha512-sqN2UDu1/0y6uvXyStCOzyhAjCSlHceFoMKJW8W9EU9cvic/QdsZ0kEU93HEy3IUEFZIiH/3w+AH/UQbPHNdhA==}
     dependencies:
       call-bind: 1.0.5
     dev: true
 
+  /is-shared-array-buffer@1.0.3:
+    resolution: {integrity: sha512-nA2hv5XIhLR3uVzDDfCIknerhx8XUKnstuOERPNNIinXG7v9u+ohXF67vxm4TPTEPU6lm61ZkwP3c9PCB97rhg==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+    dev: true
+
   /is-stream@3.0.0:
     resolution: {integrity: sha512-LnQR4bZ9IADDRSkvpqMGvt/tEJWclzklNgSw48V5EAaAeDd6qGvN8ei6k5p0tvxSR171VmGyHuTiAOfxAbr8kA==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     dev: true
 
   /is-string@1.0.7:
     resolution: {integrity: sha512-tE2UXzivje6ofPW7l23cjDOMa09gb7xlAqG6jG5ej6uPV32TlWP3NKPigtaGeHNu9fohccRYvIiZMfOOnOYUtg==}
@@ -2682,29 +2949,36 @@
   /is-typed-array@1.1.12:
     resolution: {integrity: sha512-Z14TF2JNG8Lss5/HMqt0//T9JeHXttXy5pH/DBU4vi98ozO2btxzq9MwYDZYnKwU8nRsz/+GVFVRDq3DkVuSPg==}
     engines: {node: '>= 0.4'}
     dependencies:
       which-typed-array: 1.1.13
     dev: true
 
+  /is-typed-array@1.1.13:
+    resolution: {integrity: sha512-uZ25/bUAlUY5fR4OKT4rZQEBrzQWYV9ZJYGGsUmEJ6thodVJ1HX64ePQ6Z0qPWP+m+Uq6e9UugrE38jeYsDSMw==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      which-typed-array: 1.1.15
+    dev: true
+
   /is-weakmap@2.0.1:
     resolution: {integrity: sha512-NSBR4kH5oVj1Uwvv970ruUkCV7O1mzgVFO4/rev2cLRda9Tm9HrL70ZPut4rOHgY0FNrUu9BCbXA2sdQ+x0chA==}
     dev: true
 
   /is-weakref@1.0.2:
     resolution: {integrity: sha512-qctsuLZmIQ0+vSSMfoVvyFe2+GSEvnmZ2ezTup1SBse9+twCCeial6EEi3Nc2KFcf6+qz2FBPnjXsk8xhKSaPQ==}
     dependencies:
       call-bind: 1.0.5
     dev: true
 
   /is-weakset@2.0.2:
     resolution: {integrity: sha512-t2yVvttHkQktwnNNmBQ98AhENLdPUTDTE21uPqAQ0ARwQfGeQKRVS0NNurH7bTf7RrvcVn1OOge45CnBeHCSmg==}
     dependencies:
-      call-bind: 1.0.5
-      get-intrinsic: 1.2.2
+      call-bind: 1.0.7
+      get-intrinsic: 1.2.4
     dev: true
 
   /is-wsl@2.2.0:
     resolution: {integrity: sha512-fKzAra0rGJUUBwGBgNkHZuToZcn+TtXHpeCgmkMJMMYx1sQDYaCSyjJBSCa2nH1DGm7s3n1oBnohoVTBaN7Lww==}
     engines: {node: '>=8'}
     dependencies:
       is-docker: 2.2.1
@@ -2718,15 +2992,15 @@
     resolution: {integrity: sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==}
     dev: true
 
   /iterator.prototype@1.1.2:
     resolution: {integrity: sha512-DR33HMMr8EzwuRL8Y9D3u2BMj8+RqSE850jfGu59kS7tbmPLzGkZmVSfyCFSDxuZiEY6Rzt3T2NA/qU+NwVj1w==}
     dependencies:
       define-properties: 1.2.1
-      get-intrinsic: 1.2.2
+      get-intrinsic: 1.2.4
       has-symbols: 1.0.3
       reflect.getprototypeof: 1.0.4
       set-function-name: 2.0.1
     dev: true
 
   /jest-worker@27.5.1:
     resolution: {integrity: sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==}
@@ -3185,21 +3459,26 @@
     resolution: {integrity: sha512-nN7pYi0AQqJnoLPC9eHFQ8AcyaixBUOwvqc5TDnIKCMEE6I0y8P7OKA7fPexsXGCGxQDl/cmrLAp26LhcwxZ4A==}
     dependencies:
       jsonc-parser: 3.2.1
       mlly: 1.6.1
       pathe: 1.1.2
     dev: true
 
-  /postcss@8.4.35:
-    resolution: {integrity: sha512-u5U8qYpBCpN13BsiEB0CbR1Hhh4Gc0zLFuedrHJKMctHCHAGrMdG0PRM/KErzAL3CU6/eckEtmHNB3x6e3c0vA==}
+  /possible-typed-array-names@1.0.0:
+    resolution: {integrity: sha512-d7Uw+eZoloe0EHDIYoe+bQ5WXnGMOpmiZFTuMWCwpjzzkL2nTjcKiAk4hh8TjnGye2TwWOk3UXucZ+3rbmBa8Q==}
+    engines: {node: '>= 0.4'}
+    dev: true
+
+  /postcss@8.4.38:
+    resolution: {integrity: sha512-Wglpdk03BSfXkHoQa3b/oulrotAkwrlLDRSOb9D0bN86FdRyE9lppSp33aHNPgBa0JKCoB+drFLZkQoRRYae5A==}
     engines: {node: ^10 || ^12 || >=14}
     dependencies:
       nanoid: 3.3.7
       picocolors: 1.0.0
-      source-map-js: 1.0.2
+      source-map-js: 1.2.0
     dev: true
 
   /prelude-ls@1.2.1:
     resolution: {integrity: sha512-vkcDPrRZo1QZLbn5RLGPpg/WmIQ65qoWWhcGKf/b5eplkkarX0m9z8ppCat4mlOqUsWpyNuYgO3VRyrYHSzX5g==}
     engines: {node: '>= 0.8.0'}
     dev: true
 
@@ -3264,37 +3543,37 @@
 
   /randombytes@2.1.0:
     resolution: {integrity: sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==}
     dependencies:
       safe-buffer: 5.2.1
     dev: true
 
-  /react-bootstrap-icons@1.11.3(react@18.2.0):
-    resolution: {integrity: sha512-f/DAy4UXnjdbaZyUcZKR2I3xim56uCznb9t+u3ojwzDG1p2RUrua/d8R4xplAQ8Bj/LVZwHVSrvO+npvp3l3pw==}
+  /react-bootstrap-icons@1.11.4(react@18.2.0):
+    resolution: {integrity: sha512-lnkOpNEZ/Zr7mNxvjA9efuarCPSgtOuGA55XiRj7ASJnBjb1wEAdtJOd2Aiv9t07r7FLI1IgyZPg9P6jqWD/IA==}
     peerDependencies:
       react: '>=16.8.6'
     dependencies:
       prop-types: 15.8.1
       react: 18.2.0
     dev: false
 
-  /react-bootstrap@2.10.1(@types/react@18.2.56)(react-dom@18.2.0)(react@18.2.0):
-    resolution: {integrity: sha512-J3OpRZIvCTQK+Tg/jOkRUvpYLHMdGeU9KqFUBQrV0d/Qr/3nsINpiOJyZMWnM5SJ3ctZdhPA6eCIKpEJR3Ellg==}
+  /react-bootstrap@2.10.2(@types/react@18.2.79)(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-UvB7mRqQjivdZNxJNEA2yOQRB7L9N43nBnKc33K47+cH90/ujmnMwatTCwQLu83gLhrzAl8fsa6Lqig/KLghaA==}
     peerDependencies:
       '@types/react': '>=16.14.8'
       react: '>=16.14.0'
       react-dom: '>=16.14.0'
     peerDependenciesMeta:
       '@types/react':
         optional: true
     dependencies:
       '@babel/runtime': 7.23.8
       '@restart/hooks': 0.4.15(react@18.2.0)
-      '@restart/ui': 1.6.6(react-dom@18.2.0)(react@18.2.0)
-      '@types/react': 18.2.56
+      '@restart/ui': 1.6.8(react-dom@18.2.0)(react@18.2.0)
+      '@types/react': 18.2.79
       '@types/react-transition-group': 4.4.10
       classnames: 2.5.1
       dom-helpers: 5.2.1
       invariant: 2.2.4
       prop-types: 15.8.1
       prop-types-extra: 1.1.1(react@18.2.0)
       react: 18.2.0
@@ -3326,34 +3605,34 @@
     dev: false
 
   /react-refresh@0.14.0:
     resolution: {integrity: sha512-wViHqhAd8OHeLS/IRMJjTSDHF3U9eWi62F/MledQGPdJGDhodXJ9PBLNGr6WWL7qlH12Mt3TyTpbS+hGXMjCzQ==}
     engines: {node: '>=0.10.0'}
     dev: true
 
-  /react-router-dom@6.22.1(react-dom@18.2.0)(react@18.2.0):
-    resolution: {integrity: sha512-iwMyyyrbL7zkKY7MRjOVRy+TMnS/OPusaFVxM2P11x9dzSzGmLsebkCvYirGq0DWB9K9hOspHYYtDz33gE5Duw==}
+  /react-router-dom@6.22.3(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-7ZILI7HjcE+p31oQvwbokjk6OA/bnFxrhJ19n82Ex9Ph8fNAq+Hm/7KchpMGlTgWhUxRHMMCut+vEtNpWpowKw==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       react: '>=16.8'
       react-dom: '>=16.8'
     dependencies:
-      '@remix-run/router': 1.15.1
+      '@remix-run/router': 1.15.3
       react: 18.2.0
       react-dom: 18.2.0(react@18.2.0)
-      react-router: 6.22.1(react@18.2.0)
+      react-router: 6.22.3(react@18.2.0)
     dev: false
 
-  /react-router@6.22.1(react@18.2.0):
-    resolution: {integrity: sha512-0pdoRGwLtemnJqn1K0XHUbnKiX0S4X8CgvVVmHGOWmofESj31msHo/1YiqcJWK7Wxfq2a4uvvtS01KAQyWK/CQ==}
+  /react-router@6.22.3(react@18.2.0):
+    resolution: {integrity: sha512-dr2eb3Mj5zK2YISHK++foM9w4eBnO23eKnZEDs7c880P6oKbrjz/Svg9+nxqtHQK+oMW4OtjZca0RqPglXxguQ==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       react: '>=16.8'
     dependencies:
-      '@remix-run/router': 1.15.1
+      '@remix-run/router': 1.15.3
       react: 18.2.0
     dev: false
 
   /react-shallow-renderer@16.15.0(react@18.2.0):
     resolution: {integrity: sha512-oScf2FqQ9LFVQgA73vr86xl2NaOIX73rh+YFqcOp68CWj56tSfgtGKrEbyhCj0rSijyG9M1CYprTh39fBi5hzA==}
     peerDependencies:
       react: ^16.0.0 || ^17.0.0 || ^18.0.0
@@ -3407,18 +3686,18 @@
     dependencies:
       loose-envify: 1.4.0
 
   /reflect.getprototypeof@1.0.4:
     resolution: {integrity: sha512-ECkTw8TmJwW60lOTR+ZkODISW6RQ8+2CL3COqtiJKLd6MmB45hN51HprHFziKLGkAuTGQhBb91V8cy+KHlaCjw==}
     engines: {node: '>= 0.4'}
     dependencies:
-      call-bind: 1.0.5
+      call-bind: 1.0.7
       define-properties: 1.2.1
-      es-abstract: 1.22.3
-      get-intrinsic: 1.2.2
+      es-abstract: 1.23.3
+      get-intrinsic: 1.2.4
       globalthis: 1.0.3
       which-builtin-type: 1.1.3
     dev: true
 
   /refractor@3.6.0:
     resolution: {integrity: sha512-MY9W41IOWxxk31o+YvFCNyNzdkc9M20NoZK5vq6jkv4I/uh2zkWcfudj0Q1fovjUQJrNewS9NMzeTtqPf+n5EA==}
     dependencies:
@@ -3436,14 +3715,24 @@
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.5
       define-properties: 1.2.1
       set-function-name: 2.0.1
     dev: true
 
+  /regexp.prototype.flags@1.5.2:
+    resolution: {integrity: sha512-NcDiDkTLuPR+++OCKB0nWafEmhg/Da8aUPLPMQbK+bxKKCm1/S5he+AqYa4PlMCVBalb4/yxIRub6qkEx5yJbw==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      define-properties: 1.2.1
+      es-errors: 1.3.0
+      set-function-name: 2.0.1
+    dev: true
+
   /require-directory@2.1.1:
     resolution: {integrity: sha512-fGxEI7+wsG9xrvdjsrlmL22OMTTiHRwAMroiEeMgq8gzoLC/PQr7RsRDSTLUg/bZAZtF+TVIkHc6/4RIKrui+Q==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /requires-port@1.0.0:
     resolution: {integrity: sha512-KigOCHcocU3XODJxsu8i/j8T9tzT4adHiecwORRQ0ZZFcp7ahwXuRU1m+yuO90C5ZUyGeGfocHDI14M3L3yDAQ==}
@@ -3487,34 +3776,36 @@
     dependencies:
       open: 8.4.2
       picomatch: 2.3.1
       source-map: 0.7.4
       yargs: 17.7.2
     dev: true
 
-  /rollup@4.9.6:
-    resolution: {integrity: sha512-05lzkCS2uASX0CiLFybYfVkwNbKZG5NFQ6Go0VWyogFTXXbR039UVsegViTntkk4OglHBdF54ccApXRRuXRbsg==}
+  /rollup@4.14.2:
+    resolution: {integrity: sha512-WkeoTWvuBoFjFAhsEOHKRoZ3r9GfTyhh7Vff1zwebEFLEFjT1lG3784xEgKiTa7E+e70vsC81roVL2MP4tgEEQ==}
     engines: {node: '>=18.0.0', npm: '>=8.0.0'}
     hasBin: true
     dependencies:
       '@types/estree': 1.0.5
     optionalDependencies:
-      '@rollup/rollup-android-arm-eabi': 4.9.6
-      '@rollup/rollup-android-arm64': 4.9.6
-      '@rollup/rollup-darwin-arm64': 4.9.6
-      '@rollup/rollup-darwin-x64': 4.9.6
-      '@rollup/rollup-linux-arm-gnueabihf': 4.9.6
-      '@rollup/rollup-linux-arm64-gnu': 4.9.6
-      '@rollup/rollup-linux-arm64-musl': 4.9.6
-      '@rollup/rollup-linux-riscv64-gnu': 4.9.6
-      '@rollup/rollup-linux-x64-gnu': 4.9.6
-      '@rollup/rollup-linux-x64-musl': 4.9.6
-      '@rollup/rollup-win32-arm64-msvc': 4.9.6
-      '@rollup/rollup-win32-ia32-msvc': 4.9.6
-      '@rollup/rollup-win32-x64-msvc': 4.9.6
+      '@rollup/rollup-android-arm-eabi': 4.14.2
+      '@rollup/rollup-android-arm64': 4.14.2
+      '@rollup/rollup-darwin-arm64': 4.14.2
+      '@rollup/rollup-darwin-x64': 4.14.2
+      '@rollup/rollup-linux-arm-gnueabihf': 4.14.2
+      '@rollup/rollup-linux-arm64-gnu': 4.14.2
+      '@rollup/rollup-linux-arm64-musl': 4.14.2
+      '@rollup/rollup-linux-powerpc64le-gnu': 4.14.2
+      '@rollup/rollup-linux-riscv64-gnu': 4.14.2
+      '@rollup/rollup-linux-s390x-gnu': 4.14.2
+      '@rollup/rollup-linux-x64-gnu': 4.14.2
+      '@rollup/rollup-linux-x64-musl': 4.14.2
+      '@rollup/rollup-win32-arm64-msvc': 4.14.2
+      '@rollup/rollup-win32-ia32-msvc': 4.14.2
+      '@rollup/rollup-win32-x64-msvc': 4.14.2
       fsevents: 2.3.3
     dev: true
 
   /rrweb-cssom@0.6.0:
     resolution: {integrity: sha512-APM0Gt1KoXBz0iIkkdB/kfvGOwC4UuJFeG/c+yV7wSc7q96cG/kJ0HiYCnzivD9SB53cLV1MlHFNfOuPaadYSw==}
     dev: true
 
@@ -3530,27 +3821,46 @@
     dependencies:
       call-bind: 1.0.5
       get-intrinsic: 1.2.2
       has-symbols: 1.0.3
       isarray: 2.0.5
     dev: true
 
+  /safe-array-concat@1.1.2:
+    resolution: {integrity: sha512-vj6RsCsWBCf19jIeHEfkRMw8DPiBb+DMXklQ/1SGDHOMlHdPUkZXFQ2YdplS23zESTijAcurb1aSgJA3AgMu1Q==}
+    engines: {node: '>=0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      get-intrinsic: 1.2.4
+      has-symbols: 1.0.3
+      isarray: 2.0.5
+    dev: true
+
   /safe-buffer@5.2.1:
     resolution: {integrity: sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==}
     dev: true
 
   /safe-regex-test@1.0.2:
     resolution: {integrity: sha512-83S9w6eFq12BBIJYvjMux6/dkirb8+4zJRA9cxNBVb7Wq5fJBW+Xze48WqR8pxua7bDuAaaAxtVVd4Idjp1dBQ==}
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.5
       get-intrinsic: 1.2.2
       is-regex: 1.1.4
     dev: true
 
+  /safe-regex-test@1.0.3:
+    resolution: {integrity: sha512-CdASjNJPvRa7roO6Ra/gLYBTzYzzPyyBXxIMdGW3USQLyjWEls2RgW5UBTXaQVp+OrpeCK3bLem8smtmheoRuw==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      es-errors: 1.3.0
+      is-regex: 1.1.4
+    dev: true
+
   /safer-buffer@2.1.2:
     resolution: {integrity: sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==}
     dev: true
 
   /saxes@6.0.0:
     resolution: {integrity: sha512-xAg7SOnEhrm5zI3puOOKyy1OMcMlIJZYNJY7xLBwSze0UjhPLnWfj2GF2EpT0jmzaJKIWKHLsaSSajf35bcYnA==}
     engines: {node: '>=v12.22.7'}
@@ -3598,14 +3908,26 @@
       define-data-property: 1.1.1
       function-bind: 1.1.2
       get-intrinsic: 1.2.2
       gopd: 1.0.1
       has-property-descriptors: 1.0.1
     dev: true
 
+  /set-function-length@1.2.2:
+    resolution: {integrity: sha512-pgRc4hJ4/sNjWCSS9AmnS40x3bNMDTknHgL5UaMBTMyJnU90EgWh1Rz+MC9eFu4BuN/UwZjKQuY/1v3rM7HMfg==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      define-data-property: 1.1.4
+      es-errors: 1.3.0
+      function-bind: 1.1.2
+      get-intrinsic: 1.2.4
+      gopd: 1.0.1
+      has-property-descriptors: 1.0.2
+    dev: true
+
   /set-function-name@2.0.1:
     resolution: {integrity: sha512-tMNCiqYVkXIZgc2Hnoy2IvC/f8ezc5koaRFkCjrpWzGpCd3qbZXPzVy9MAZzK1ch/X0jvSkojys3oqJN0qCmdA==}
     engines: {node: '>= 0.4'}
     dependencies:
       define-data-property: 1.1.1
       functions-have-names: 1.2.3
       has-property-descriptors: 1.0.1
@@ -3641,16 +3963,16 @@
     dev: true
 
   /slash@3.0.0:
     resolution: {integrity: sha512-g9Q1haeby36OSStwb4ntCGGGaKsaVSjQ68fBxoQcutl5fS1vuY18H3wSt3jFyFtrkx+Kz0V1G85A4MyAdDMi2Q==}
     engines: {node: '>=8'}
     dev: true
 
-  /source-map-js@1.0.2:
-    resolution: {integrity: sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==}
+  /source-map-js@1.2.0:
+    resolution: {integrity: sha512-itJW8lvSA0TXEphiRoawsCksnlf8SyvmFzIhltqAHluXd88pkCd+cXJVHTDwdCr0IzwptSm035IHQktUu1QUMg==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /source-map-support@0.5.21:
     resolution: {integrity: sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==}
     dependencies:
       buffer-from: 1.1.2
@@ -3707,30 +4029,57 @@
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.5
       define-properties: 1.2.1
       es-abstract: 1.22.3
     dev: true
 
+  /string.prototype.trim@1.2.9:
+    resolution: {integrity: sha512-klHuCNxiMZ8MlsOihJhJEBJAiMVqU3Z2nEXWfWnIqjN0gEFS9J9+IxKozWWtQGcgoa1WUZzLjKPTr4ZHNFTFxw==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      define-properties: 1.2.1
+      es-abstract: 1.23.3
+      es-object-atoms: 1.0.0
+    dev: true
+
   /string.prototype.trimend@1.0.7:
     resolution: {integrity: sha512-Ni79DqeB72ZFq1uH/L6zJ+DKZTkOtPIHovb3YZHQViE+HDouuU4mBrLOLDn5Dde3RF8qw5qVETEjhu9locMLvA==}
     dependencies:
       call-bind: 1.0.5
       define-properties: 1.2.1
       es-abstract: 1.22.3
     dev: true
 
+  /string.prototype.trimend@1.0.8:
+    resolution: {integrity: sha512-p73uL5VCHCO2BZZ6krwwQE3kCzM7NKmis8S//xEC6fQonchbum4eP6kR4DLEjQFO3Wnj3Fuo8NM0kOSjVdHjZQ==}
+    dependencies:
+      call-bind: 1.0.7
+      define-properties: 1.2.1
+      es-object-atoms: 1.0.0
+    dev: true
+
   /string.prototype.trimstart@1.0.7:
     resolution: {integrity: sha512-NGhtDFu3jCEm7B4Fy0DpLewdJQOZcQ0rGbwQ/+stjnrp2i+rlKeCvos9hOIeCmqwratM47OBxY7uFZzjxHXmrg==}
     dependencies:
       call-bind: 1.0.5
       define-properties: 1.2.1
       es-abstract: 1.22.3
     dev: true
 
+  /string.prototype.trimstart@1.0.8:
+    resolution: {integrity: sha512-UXSH262CSZY1tfu3G3Secr6uGLCFVPMhIqHjlgCUtCCcgihYc/xKs9djMTMUOb2j1mVSeU8EU6NWc/iQKU6Gfg==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      define-properties: 1.2.1
+      es-object-atoms: 1.0.0
+    dev: true
+
   /strip-ansi@6.0.1:
     resolution: {integrity: sha512-Y38VPSHcqkFrCpFnQ9vuSXmquuv5oXOKpGeT6aGrr3o3Gc9AlVa6JBfUSOCnbxGGZF+/0ooI7KrPuUSztUdU5A==}
     engines: {node: '>=8'}
     dependencies:
       ansi-regex: 5.0.1
     dev: true
 
@@ -3824,16 +4173,16 @@
     resolution: {integrity: sha512-N+8UisAXDGk8PFXP4HAzVR9nbfmVJ3zYLAWiTIoqC5v5isinhr+r5uaO8+7r3BMfuNIufIsA7RdpVgacC2cSpw==}
     dev: true
 
   /tinybench@2.6.0:
     resolution: {integrity: sha512-N8hW3PG/3aOoZAN5V/NSAEDz0ZixDSSt5b/a05iqtpgfLWMSVuCo7w0k2vVvEjdrIoeGqZzweX2WlyioNIHchA==}
     dev: true
 
-  /tinypool@0.8.2:
-    resolution: {integrity: sha512-SUszKYe5wgsxnNOVlBYO6IC+8VGWdVGZWAqUxp3UErNBtptZvWbwyUOyzNL59zigz2rCA92QiL3wvG+JDSdJdQ==}
+  /tinypool@0.8.3:
+    resolution: {integrity: sha512-Ud7uepAklqRH1bvwy22ynrliC7Dljz7Tm8M/0RBUW+YRa4YHhZ6e4PpgE+fu1zr/WqB1kbeuVrdfeuyIBpy4tw==}
     engines: {node: '>=14.0.0'}
     dev: true
 
   /tinyspy@2.2.1:
     resolution: {integrity: sha512-KYad6Vy5VDWV4GH3fjpseMQ/XU2BhIYP7Vzd0LG44qRWm/Yt2WCOTicFdvmgo6gWaqooMQCawTtILVQJupKu7A==}
     engines: {node: '>=14.0.0'}
     dev: true
@@ -3868,40 +4217,40 @@
   /tr46@5.0.0:
     resolution: {integrity: sha512-tk2G5R2KRwBd+ZN0zaEXpmzdKyOYksXwywulIX95MBODjSzMIuQnQ3m8JxgbhnL1LeVo7lqQKsYa1O3Htl7K5g==}
     engines: {node: '>=18'}
     dependencies:
       punycode: 2.3.1
     dev: true
 
-  /ts-api-utils@1.0.3(typescript@5.3.3):
+  /ts-api-utils@1.0.3(typescript@5.4.4):
     resolution: {integrity: sha512-wNMeqtMz5NtwpT/UZGY5alT+VoKdSsOOP/kqHFcUW1P/VRhH2wJ48+DN2WwUliNbQ976ETwDL0Ifd2VVvgonvg==}
     engines: {node: '>=16.13.0'}
     peerDependencies:
       typescript: '>=4.2.0'
     dependencies:
-      typescript: 5.3.3
+      typescript: 5.4.4
     dev: true
 
-  /ts-loader@9.5.1(typescript@5.3.3)(webpack@5.89.0):
+  /ts-loader@9.5.1(typescript@5.4.4)(webpack@5.89.0):
     resolution: {integrity: sha512-rNH3sK9kGZcH9dYzC7CewQm4NtxJTjSEVRJ2DyBZR7f8/wcta+iV44UPCXc5+nzDzivKtlzV6c9P4e+oFhDLYg==}
     engines: {node: '>=12.0.0'}
     peerDependencies:
       typescript: '*'
       webpack: ^5.0.0
     dependencies:
       chalk: 4.1.2
       enhanced-resolve: 5.15.0
       micromatch: 4.0.5
       semver: 7.5.4
       source-map: 0.7.4
-      typescript: 5.3.3
+      typescript: 5.4.4
       webpack: 5.89.0
     dev: true
 
-  /ts-node@10.9.2(@types/node@20.11.5)(typescript@5.3.3):
+  /ts-node@10.9.2(@types/node@20.11.5)(typescript@5.4.4):
     resolution: {integrity: sha512-f0FFpIdcHgn8zcPSbf1dRevwt047YMnaiJM3u2w2RewrB+fob/zePZcrOyQoLMMO7aBIddLcQIEK5dYjkLnGrQ==}
     hasBin: true
     peerDependencies:
       '@swc/core': '>=1.2.50'
       '@swc/wasm': '>=1.2.50'
       '@types/node': '*'
       typescript: '>=2.7'
@@ -3919,15 +4268,15 @@
       '@types/node': 20.11.5
       acorn: 8.11.3
       acorn-walk: 8.3.2
       arg: 4.1.3
       create-require: 1.1.1
       diff: 4.0.2
       make-error: 1.3.6
-      typescript: 5.3.3
+      typescript: 5.4.4
       v8-compile-cache-lib: 3.0.1
       yn: 3.1.1
     dev: true
 
   /tslib@2.6.2:
     resolution: {integrity: sha512-AEYxH93jGFPn/a2iVAwW87VuUIkR1FVUKB77NwMF7nBTDkDrrT/Hpt/IrCJ0QXhW27jTBDcf5ZY7w6RiqTMw2Q==}
     dev: false
@@ -3954,45 +4303,89 @@
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.5
       get-intrinsic: 1.2.2
       is-typed-array: 1.1.12
     dev: true
 
+  /typed-array-buffer@1.0.2:
+    resolution: {integrity: sha512-gEymJYKZtKXzzBzM4jqa9w6Q1Jjm7x2d+sh19AdsD4wqnMPDYyvwpsIc2Q/835kHuo3BEQ7CjelGhfTsoBb2MQ==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      es-errors: 1.3.0
+      is-typed-array: 1.1.13
+    dev: true
+
   /typed-array-byte-length@1.0.0:
     resolution: {integrity: sha512-Or/+kvLxNpeQ9DtSydonMxCx+9ZXOswtwJn17SNLvhptaXYDJvkFFP5zbfU/uLmvnBJlI4yrnXRxpdWH/M5tNA==}
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.5
       for-each: 0.3.3
       has-proto: 1.0.1
       is-typed-array: 1.1.12
     dev: true
 
+  /typed-array-byte-length@1.0.1:
+    resolution: {integrity: sha512-3iMJ9q0ao7WE9tWcaYKIptkNBuOIcZCCT0d4MRvuuH88fEoEH62IuQe0OtraD3ebQEoTRk8XCBoknUNc1Y67pw==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      for-each: 0.3.3
+      gopd: 1.0.1
+      has-proto: 1.0.3
+      is-typed-array: 1.1.13
+    dev: true
+
   /typed-array-byte-offset@1.0.0:
     resolution: {integrity: sha512-RD97prjEt9EL8YgAgpOkf3O4IF9lhJFr9g0htQkm0rchFp/Vx7LW5Q8fSXXub7BXAODyUQohRMyOc3faCPd0hg==}
     engines: {node: '>= 0.4'}
     dependencies:
       available-typed-arrays: 1.0.5
       call-bind: 1.0.5
       for-each: 0.3.3
       has-proto: 1.0.1
       is-typed-array: 1.1.12
     dev: true
 
+  /typed-array-byte-offset@1.0.2:
+    resolution: {integrity: sha512-Ous0vodHa56FviZucS2E63zkgtgrACj7omjwd/8lTEMEPFFyjfixMZ1ZXenpgCFBBt4EC1J2XsyVS2gkG0eTFA==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      available-typed-arrays: 1.0.7
+      call-bind: 1.0.7
+      for-each: 0.3.3
+      gopd: 1.0.1
+      has-proto: 1.0.3
+      is-typed-array: 1.1.13
+    dev: true
+
   /typed-array-length@1.0.4:
     resolution: {integrity: sha512-KjZypGq+I/H7HI5HlOoGHkWUUGq+Q0TPhQurLbyrVrvnKTBgzLhIJ7j6J/XTQOi0d1RjyZ0wdas8bKs2p0x3Ng==}
     dependencies:
       call-bind: 1.0.5
       for-each: 0.3.3
       is-typed-array: 1.1.12
     dev: true
 
-  /typescript@5.3.3:
-    resolution: {integrity: sha512-pXWcraxM0uxAS+tN0AG/BF2TyqmHO014Z070UsJ+pFvYuRSq8KH8DmWpnbXe0pEPDHXZV3FcAbJkijJ5oNEnWw==}
+  /typed-array-length@1.0.6:
+    resolution: {integrity: sha512-/OxDN6OtAk5KBpGb28T+HZc2M+ADtvRxXrKKbUwtsLgdoxgX13hyy7ek6bFRl5+aBs2yZzB0c4CnQfAtVypW/g==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      call-bind: 1.0.7
+      for-each: 0.3.3
+      gopd: 1.0.1
+      has-proto: 1.0.3
+      is-typed-array: 1.1.13
+      possible-typed-array-names: 1.0.0
+    dev: true
+
+  /typescript@5.4.4:
+    resolution: {integrity: sha512-dGE2Vv8cpVvw28v8HCPqyb08EzbBURxDpuhJvTrusShUfGnhHBafDsLdS1EhhxyL6BJQE+2cT3dDPAv+MQ6oLw==}
     engines: {node: '>=14.17'}
     hasBin: true
     dev: true
 
   /ufo@1.4.0:
     resolution: {integrity: sha512-Hhy+BhRBleFjpJ2vchUNN40qgkh0366FWJGqVLYBHev0vpHTrXSA0ryT+74UiW6KWsldNurQMKGqCm1M2zBciQ==}
     dev: true
@@ -4008,15 +4401,15 @@
 
   /uncontrollable@7.2.1(react@18.2.0):
     resolution: {integrity: sha512-svtcfoTADIB0nT9nltgjujTi7BzVmwjZClOmskKu/E8FW9BXzg9os8OLr4f8Dlnk0rYWJIWr4wv9eKUXiQvQwQ==}
     peerDependencies:
       react: '>=15.0.0'
     dependencies:
       '@babel/runtime': 7.23.8
-      '@types/react': 18.2.56
+      '@types/react': 18.2.79
       invariant: 2.2.4
       react: 18.2.0
       react-lifecycles-compat: 3.0.4
     dev: false
 
   /uncontrollable@8.0.4(react@18.2.0):
     resolution: {integrity: sha512-ulRWYWHvscPFc0QQXvyJjY6LIXU56f0h8pQFvhxiKk5V1fcI8gp9Ht9leVAhrVjzqMw0BgjspBINx9r6oyJUvQ==}
@@ -4077,37 +4470,37 @@
       rollup-plugin-visualizer: 5.12.0
       tmp: 0.2.3
     transitivePeerDependencies:
       - rollup
       - supports-color
     dev: true
 
-  /vite-node@1.3.1(@types/node@20.11.5):
-    resolution: {integrity: sha512-azbRrqRxlWTJEVbzInZCTchx0X69M/XPTCz4H+TLvlTcR/xH/3hkRqhOakT41fMJCMzXTu4UvegkZiEoJAWvng==}
+  /vite-node@1.5.0(@types/node@20.11.5):
+    resolution: {integrity: sha512-tV8h6gMj6vPzVCa7l+VGq9lwoJjW8Y79vst8QZZGiuRAfijU+EEWuc0kFpmndQrWhMMhet1jdSF+40KSZUqIIw==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     dependencies:
       cac: 6.7.14
       debug: 4.3.4
       pathe: 1.1.2
       picocolors: 1.0.0
-      vite: 5.1.7(@types/node@20.11.5)
+      vite: 5.2.10(@types/node@20.11.5)
     transitivePeerDependencies:
       - '@types/node'
       - less
       - lightningcss
       - sass
       - stylus
       - sugarss
       - supports-color
       - terser
     dev: true
 
-  /vite@5.1.7(@types/node@20.11.5):
-    resolution: {integrity: sha512-sgnEEFTZYMui/sTlH1/XEnVNHMujOahPLGMxn1+5sIT45Xjng1Ec1K78jRP15dSmVgg5WBin9yO81j3o9OxofA==}
+  /vite@5.2.10(@types/node@20.11.5):
+    resolution: {integrity: sha512-PAzgUZbP7msvQvqdSD+ErD5qGnSFiGOoWmV5yAKUEI0kdhjbH6nMWVyZQC/hSc4aXwc0oJ9aEdIiF9Oje0JFCw==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
       '@types/node': ^18.0.0 || >=20.0.0
       less: '*'
       lightningcss: ^1.21.0
       sass: '*'
@@ -4127,30 +4520,30 @@
         optional: true
       sugarss:
         optional: true
       terser:
         optional: true
     dependencies:
       '@types/node': 20.11.5
-      esbuild: 0.19.11
-      postcss: 8.4.35
-      rollup: 4.9.6
+      esbuild: 0.20.2
+      postcss: 8.4.38
+      rollup: 4.14.2
     optionalDependencies:
       fsevents: 2.3.3
     dev: true
 
-  /vitest@1.3.1(@types/node@20.11.5)(jsdom@24.0.0):
-    resolution: {integrity: sha512-/1QJqXs8YbCrfv/GPQ05wAZf2eakUPLPa18vkJAKE7RXOKfVHqMZZ1WlTjiwl6Gcn65M5vpNUB6EFLnEdRdEXQ==}
+  /vitest@1.5.0(@types/node@20.11.5)(jsdom@24.0.0):
+    resolution: {integrity: sha512-d8UKgR0m2kjdxDWX6911uwxout6GHS0XaGH1cksSIVVG8kRlE7G7aBw7myKQCvDI5dT4j7ZMa+l706BIORMDLw==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
       '@edge-runtime/vm': '*'
       '@types/node': ^18.0.0 || >=20.0.0
-      '@vitest/browser': 1.3.1
-      '@vitest/ui': 1.3.1
+      '@vitest/browser': 1.5.0
+      '@vitest/ui': 1.5.0
       happy-dom: '*'
       jsdom: '*'
     peerDependenciesMeta:
       '@edge-runtime/vm':
         optional: true
       '@types/node':
         optional: true
@@ -4160,34 +4553,34 @@
         optional: true
       happy-dom:
         optional: true
       jsdom:
         optional: true
     dependencies:
       '@types/node': 20.11.5
-      '@vitest/expect': 1.3.1
-      '@vitest/runner': 1.3.1
-      '@vitest/snapshot': 1.3.1
-      '@vitest/spy': 1.3.1
-      '@vitest/utils': 1.3.1
+      '@vitest/expect': 1.5.0
+      '@vitest/runner': 1.5.0
+      '@vitest/snapshot': 1.5.0
+      '@vitest/spy': 1.5.0
+      '@vitest/utils': 1.5.0
       acorn-walk: 8.3.2
       chai: 4.4.1
       debug: 4.3.4
       execa: 8.0.1
       jsdom: 24.0.0
       local-pkg: 0.5.0
       magic-string: 0.30.7
       pathe: 1.1.2
       picocolors: 1.0.0
       std-env: 3.7.0
       strip-literal: 2.0.0
       tinybench: 2.6.0
-      tinypool: 0.8.2
-      vite: 5.1.7(@types/node@20.11.5)
-      vite-node: 1.3.1(@types/node@20.11.5)
+      tinypool: 0.8.3
+      vite: 5.2.10(@types/node@20.11.5)
+      vite-node: 1.5.0(@types/node@20.11.5)
       why-is-node-running: 2.2.2
     transitivePeerDependencies:
       - less
       - lightningcss
       - sass
       - stylus
       - sugarss
@@ -4330,14 +4723,25 @@
       available-typed-arrays: 1.0.5
       call-bind: 1.0.5
       for-each: 0.3.3
       gopd: 1.0.1
       has-tostringtag: 1.0.0
     dev: true
 
+  /which-typed-array@1.1.15:
+    resolution: {integrity: sha512-oV0jmFtUky6CXfkqehVvBP/LSWJ2sy4vWMioiENyJLePrBO/yKyV9OyJySfAKosh+RYkIl5zJCNZ8/4JncrpdA==}
+    engines: {node: '>= 0.4'}
+    dependencies:
+      available-typed-arrays: 1.0.7
+      call-bind: 1.0.7
+      for-each: 0.3.3
+      gopd: 1.0.1
+      has-tostringtag: 1.0.2
+    dev: true
+
   /which@2.0.2:
     resolution: {integrity: sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==}
     engines: {node: '>= 8'}
     hasBin: true
     dependencies:
       isexe: 2.0.0
     dev: true
```

### Comparing `bowtie_json_schema-2024.4.3/frontend/tsconfig.json` & `bowtie_json_schema-2024.4.4/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/public/favicon.svg` & `bowtie_json_schema-2024.4.4/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/index.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.4.4/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/NavBar.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             aria-controls="collapse-navbar-nav"
             aria-expanded="false"
             aria-label="Toggle navigation"
             onClick={() => setIsNavbarOpen(!isNavbarOpen)}
           />
         </div>
         <Collapse in={isNavbarOpen}>
-          <div className="collapse navbar-collapse" id="navbarSupportedContent">
+          <div className="navbar-collapse" id="navbarSupportedContent">
             <ul className="navbar-nav me-auto mb-2 mb-lg-0 align-items-baseline">
               {isDialectPage && (
                 <>
                   <li className="nav-item">
                     <Link className="nav-link" to={{ hash: "run-info" }}>
                       Run Info
                     </Link>
```

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.4.4/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.4.4/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.4.4/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.4.4/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.4.4/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.4.4/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.4.4/frontend/src/data/parseReportData.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.4.4/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.4.4/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.4.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.4.4/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.4.4/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.4.4/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.4.4/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.4.4/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.4.4/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.4.4/implementations/java-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.4.4/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 io-interfaces = { module = "io.openapiprocessor:io-interfaces" }
 io-jackson = { module = "io.openapiprocessor:io-jackson" }
 
 jackson-bom = "com.fasterxml.jackson:jackson-bom:2.17.0"
 jackson-databind = { module = "com.fasterxml.jackson.core:jackson-databind" }
 jackson-kotlin = { module = "com.fasterxml.jackson.module:jackson-module-kotlin" }
 
-logback = "ch.qos.logback:logback-classic:1.5.3"
+logback = "ch.qos.logback:logback-classic:1.5.6"
 
 [plugins]
 kotlin = { id = "org.jetbrains.kotlin.jvm", version.ref = "kotlin" }
```

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.4.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.4.4/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.4.4/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.4.4/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.4.4/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.4.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.4.4/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.4.4/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.4.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.4.4/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.4.4/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.4.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.4.4/implementations/rust-boon/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -300,17 +300,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
```

### Comparing `bowtie_json_schema-2024.4.3/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.4.4/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.4.4/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -937,37 +937,37 @@
 checksum = "836fa6a3e1e547f9a2c4040802ec865b5d85f4014efe00555d7090a3dcaa1090"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
```

### Comparing `bowtie_json_schema-2024.4.3/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.4.4/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.4.4/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.4.4/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.4.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/test_github.py` & `bowtie_json_schema-2024.4.4/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/test_hypothesis.py` & `bowtie_json_schema-2024.4.4/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/test_integration.py` & `bowtie_json_schema-2024.4.4/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from io import BytesIO
 from pathlib import Path
 from pprint import pformat
 from textwrap import dedent, indent
 import asyncio
 import json as _json
 import os
-import re
 import sys
 import tarfile
 
 from aiodocker.exceptions import DockerError
 from markdown_it import MarkdownIt
 from markdown_it.tree import SyntaxTreeNode
 import pexpect
@@ -25,14 +24,17 @@
     False  # frigging py.test
 )
 
 
 HERE = Path(__file__).parent
 FAUXMPLEMENTATIONS = HERE / "fauxmplementations"
 
+# Make believe we're wide for tests to avoid line breaks in rich-click.
+WIDE_TERMINAL_ENV = dict(os.environ, TERMINAL_WIDTH="512")
+
 
 def tag(name: str):
     return f"bowtie-integration-tests/{name}"
 
 
 async def bowtie(*argv, stdin: str = "", exit_code=0, json=False):
     """
@@ -44,14 +46,15 @@
         sys.executable,
         "-m",
         "bowtie",
         *argv,
         stdin=asyncio.subprocess.PIPE,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
+        env=WIDE_TERMINAL_ENV,
     )
     raw_stdout, raw_stderr = await process.communicate(stdin.encode())
     decoded = stdout, stderr = raw_stdout.decode(), raw_stderr.decode()
 
     if exit_code == -1:
         assert process.returncode != 0, decoded
     else:
@@ -479,15 +482,15 @@
         "--dialect",
         dialect,
         exit_code=-1,
     ) as send:
         results, stderr = await send("")
 
     assert results == []
-    assert "not a known dialect" in stderr.lower(), stderr
+    assert "not a known dialect" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_nonurl_dialect(envsonschema):
     dialect = ";;;;;"
     async with run(
         "-i",
@@ -495,30 +498,30 @@
         "--dialect",
         dialect,
         exit_code=-1,
     ) as send:
         results, stderr = await send("")
 
     assert results == []
-    assert "not a known dialect" in stderr.lower(), stderr
+    assert "not a known dialect" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_unsupported_known_dialect(only_draft3):
     async with run(
         "-i",
         only_draft3,
         "--dialect",
         str(Dialect.by_alias()["draft2020-12"].uri),
         exit_code=-1,
     ) as send:
         results, stderr = await send("")
 
     assert results == []
-    assert "does not support" in stderr.lower(), stderr
+    assert "does not support" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_restarts_crashed_implementations(envsonschema):
     async with run("-i", envsonschema) as send:
         results, stderr = await send(
             """
@@ -556,15 +559,15 @@
             """,  # noqa: E501
         )
 
     assert results == [
         {tag("envsonschema"): TestResult.INVALID},
         {tag("envsonschema"): TestResult.INVALID},
     ], stderr
-    assert "failed to start" in stderr.lower(), stderr
+    assert "failed to start" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_it_exits_when_no_implementations_succeed(succeed_immediately):
     """
     Don't uselessly "run" tests on no implementations.
     """
@@ -574,15 +577,15 @@
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             {"description": "2", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             {"description": "3", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             """,  # noqa: E501
         )
 
     assert results == []
-    assert "failed to start" in stderr.lower(), stderr
+    assert "failed to start" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_it_handles_immediately_broken_implementations(
     fail_immediately,
     envsonschema,
 ):
@@ -596,15 +599,15 @@
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             {"description": "2", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             """,  # noqa: E501
         )
 
-    assert "failed to start" in stderr.lower(), stderr
+    assert "failed to start" in stderr, stderr
     assert "BOOM!" in stderr, stderr
     assert results == [
         {tag("envsonschema"): TestResult.INVALID},
         {tag("envsonschema"): TestResult.INVALID},
     ], stderr
 
 
@@ -623,15 +626,15 @@
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             {"description": "2", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             """,  # noqa: E501
         )
 
-    assert "failed to start" in stderr.lower(), stderr
+    assert "failed to start" in stderr, stderr
     assert "BOOM!" in stderr, stderr
     assert results == [
         {tag("envsonschema"): TestResult.INVALID},
         {tag("envsonschema"): TestResult.INVALID},
     ], stderr
 
 
@@ -747,15 +750,15 @@
     async with run("-i", missing_homepage, "-V", exit_code=-1) as send:
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             """,  # noqa: E501
         )
 
-    assert "failed to start" in stderr.lower(), stderr
+    assert "failed to start" in stderr, stderr
     assert "'homepage' is a required" in stderr, stderr
     assert results == [], stderr
 
 
 @pytest.mark.asyncio
 async def test_it_preserves_all_metadata(with_versions):
     async with run("-i", with_versions, "-V") as send:
@@ -911,27 +914,27 @@
         envsonschema,
         "--max-fail",
         "2",
         "--fail-fast",
         exit_code=-1,
     )
     assert stdout == ""
-    assert "--fail-fast and --max-fail / --max-error" in stderr.lower(), stderr
+    assert "don't provide both" in stderr, stderr
 
     stdout, stderr = await bowtie(
         "run",
         "-i",
         envsonschema,
         "--fail-fast",
         "--max-fail",
         "2",
         exit_code=-1,
     )
     assert stdout == ""
-    assert "--fail-fast and --max-fail / --max-error" in stderr.lower(), stderr
+    assert "don't provide both" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_filter(envsonschema):
     async with run("-i", envsonschema, "-k", "baz") as send:
         results, stderr = await send(
             """
@@ -1375,15 +1378,15 @@
         "info",
         "-i",
         succeed_immediately,
         exit_code=-1,
     )
 
     assert stdout.strip() in {"", "{}"}  # empty, but ignore if JSON or not
-    assert "failed to start" in stderr.lower(), stderr
+    assert "failed to start" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_filter_implementations_no_arguments():
     stdout, stderr = [], ""
 
     try:
@@ -2010,15 +2013,15 @@
     _, stderr = await bowtie(
         "suite",
         "-i",
         envsonschema,
         tmp_path,
         exit_code=-1,
     )
-    assert re.search(r"does not contain .* cases", stderr), stderr
+    assert "does not contain" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_validate_mismatched_dialect(envsonschema, tmp_path):
     tmp_path.joinpath("schema.json").write_text(
         '{"$schema": "https://json-schema.org/draft/2020-12/schema"}',
     )
```

### Comparing `bowtie_json_schema-2024.4.3/tests/test_report.py` & `bowtie_json_schema-2024.4.4/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/test_schemas.py` & `bowtie_json_schema-2024.4.4/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.4.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/.gitignore` & `bowtie_json_schema-2024.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/LICENSE` & `bowtie_json_schema-2024.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/README.rst` & `bowtie_json_schema-2024.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/hatch_build.py` & `bowtie_json_schema-2024.4.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.4.3/pyproject.toml` & `bowtie_json_schema-2024.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -46,22 +46,22 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: File Formats :: JSON :: JSON Schema",
 ]
 dynamic = ["version"]
 dependencies = [
   "aiodocker",
   "attrs>=22.2.0",
-  "click",
   "diagnostic",
   "github3.py",
   "jsonschema>=4.19.0",
   "jsonschema_lexer",
   "referencing>=0.31.0",
   "referencing-loaders>=0.4.2",
   "rich",
+  "rich-click>=1.8.0dev6",
   "rpds.py>=0.18.0",
   "structlog",
   "typing-extensions; python_version<'3.11'",
   "url.py",
 ]
 
 [project.optional-dependencies]
```

### Comparing `bowtie_json_schema-2024.4.3/PKG-INFO` & `bowtie_json_schema-2024.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
@@ -22,22 +22,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: File Formats :: JSON :: JSON Schema
 Requires-Python: >=3.10
 Requires-Dist: aiodocker
 Requires-Dist: attrs>=22.2.0
-Requires-Dist: click
 Requires-Dist: diagnostic
 Requires-Dist: github3-py
 Requires-Dist: jsonschema-lexer
 Requires-Dist: jsonschema>=4.19.0
 Requires-Dist: referencing-loaders>=0.4.2
 Requires-Dist: referencing>=0.31.0
 Requires-Dist: rich
+Requires-Dist: rich-click>=1.8.0dev6
 Requires-Dist: rpds-py>=0.18.0
 Requires-Dist: structlog
 Requires-Dist: typing-extensions; python_version < '3.11'
 Requires-Dist: url-py
 Provides-Extra: strategies
 Requires-Dist: hypothesis>=6.92.1; extra == 'strategies'
 Description-Content-Type: text/x-rst
```

