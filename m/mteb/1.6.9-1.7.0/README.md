# Comparing `tmp/mteb-1.6.9.tar.gz` & `tmp/mteb-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.6.9.tar", last modified: Mon Apr 15 20:34:30 2024, max compression
+gzip compressed data, was "mteb-1.7.0.tar", last modified: Sat Apr 20 19:42:00 2024, max compression
```

## Comparing `mteb-1.6.9.tar` & `mteb-1.7.0.tar`

### file list

```diff
@@ -1,482 +1,734 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.878722 mteb-1.6.9/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-15 20:34:26.000000 mteb-1.6.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23576 2024-04-15 20:34:30.878722 mteb-1.6.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2024-04-15 20:34:26.000000 mteb-1.6.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.806722 mteb-1.6.9/mteb/
--rw-r--r--   0 root         (0) root         (0)     2135 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.810722 mteb-1.6.9/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     2347 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    11806 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     9841 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7082 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/iso_15924_to_script.json
--rw-r--r--   0 root         (0) root         (0)   193114 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/iso_639_3_to_language.json
--rw-r--r--   0 root         (0) root         (0)      542 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/languages.py
--rw-r--r--   0 root         (0) root         (0)     5225 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.810722 mteb-1.6.9/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    12990 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5849 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    12487 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/BitextMining/dan/
--rw-r--r--   0 root         (0) root         (0)     1443 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2281 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5969 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1423 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5709 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/BitextMining/vie/
--rw-r--r--   0 root         (0) root         (0)     2889 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     1520 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.818722 mteb-1.6.9/mteb/tasks/Classification/dan/
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2511 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.818722 mteb-1.6.9/mteb/tasks/Classification/eng/
--rw-r--r--   0 root         (0) root         (0)     1041 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      990 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/NewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1281 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.818722 mteb-1.6.9/mteb/tasks/Classification/hin/
--rw-r--r--   0 root         (0) root         (0)     2195 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/hin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.818722 mteb-1.6.9/mteb/tasks/Classification/jpn/
--rw-r--r--   0 root         (0) root         (0)     3550 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/jpn/WRIMEClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1575 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1611 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     6099 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/nob/
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/nob/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1173 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/nob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/pol/
--rw-r--r--   0 root         (0) root         (0)     4922 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/pol/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/swe/
--rw-r--r--   0 root         (0) root         (0)     1043 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/swe/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/swe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/vie/
--rw-r--r--   0 root         (0) root         (0)     3368 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/zho/
--rw-r--r--   0 root         (0) root         (0)     6571 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/zho/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)     1729 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Clustering/deu/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1100 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.826722 mteb-1.6.9/mteb/tasks/Clustering/eng/
--rw-r--r--   0 root         (0) root         (0)     1101 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1061 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1135 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.826722 mteb-1.6.9/mteb/tasks/Clustering/fra/
--rw-r--r--   0 root         (0) root         (0)     1911 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1625 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1942 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2723 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2737 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3442 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/nob/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/nob/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/pol/
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/pol/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/spa/
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3926 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/swe/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/zho/
--rw-r--r--   0 root         (0) root         (0)     3639 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/zho/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/PairClassification/deu/
--rw-r--r--   0 root         (0) root         (0)     2862 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/PairClassification/eng/
--rw-r--r--   0 root         (0) root         (0)     1152 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2798 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/PairClassification/pol/
--rw-r--r--   0 root         (0) root         (0)     3577 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/pol/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/PairClassification/zho/
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3054 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/fra/
--rw-r--r--   0 root         (0) root         (0)     1195 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/fra/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/fra/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/zho/
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/zho/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     3005 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.838722 mteb-1.6.9/mteb/tasks/Retrieval/code/
--rw-r--r--   0 root         (0) root         (0)     3377 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/code/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.838722 mteb-1.6.9/mteb/tasks/Retrieval/dan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/dan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3794 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/dan/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2583 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3148 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/dan/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.838722 mteb-1.6.9/mteb/tasks/Retrieval/deu/
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1228 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2876 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1175 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3705 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/fra/
--rw-r--r--   0 root         (0) root         (0)     2145 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2475 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/jpn/
--rw-r--r--   0 root         (0) root         (0)     2853 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/kor/
--rw-r--r--   0 root         (0) root         (0)      906 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/kor/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3277 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3432 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2979 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3145 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3952 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/nob/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2708 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/nob/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/pol/
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/spa/
--rw-r--r--   0 root         (0) root         (0)     2125 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3219 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2619 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/vie/
--rw-r--r--   0 root         (0) root         (0)     3798 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/zho/
--rw-r--r--   0 root         (0) root         (0)    10384 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      575 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/deu/
--rw-r--r--   0 root         (0) root         (0)     1370 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/eng/
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/fra/
--rw-r--r--   0 root         (0) root         (0)     1472 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/fra/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1600 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2712 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/pol/
--rw-r--r--   0 root         (0) root         (0)     2268 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/pol/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/spa/
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/spa/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/zho/
--rw-r--r--   0 root         (0) root         (0)     7122 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/zho/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.858722 mteb-1.6.9/mteb/tasks/Summarization/eng/
--rw-r--r--   0 root         (0) root         (0)     1243 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.858722 mteb-1.6.9/mteb/tasks/Summarization/fra/
--rw-r--r--   0 root         (0) root         (0)     1304 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/fra/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.878722 mteb-1.6.9/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23576 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19373 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2169 2024-04-15 20:34:27.000000 mteb-1.6.9/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.798722 mteb-1.6.9/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.862722 mteb-1.6.9/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)     5524 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      298 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1015 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      304 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1028 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.862722 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
--rw-r--r--   0 root         (0) root         (0)      340 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1014 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      302 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/model.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)     1001 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     5535 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)    16669 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)    18247 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1022 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)      294 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)      176 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5929 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/medicalqaretrieval/
--rw-r--r--   0 root         (0) root         (0)     1889 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/medicalqaretrieval/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5217 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/mteb_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.802722 mteb-1.6.9/scripts/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1334 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)      988 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_law.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 20:34:30.878722 mteb-1.6.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.878722 mteb-1.6.9/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     3715 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     2269 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_all_abstasks.py
--rw-r--r--   0 root         (0) root         (0)     1420 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_mteb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.541706 mteb-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-20 19:41:56.000000 mteb-1.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23583 2024-04-20 19:42:00.541706 mteb-1.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9185 2024-04-20 19:41:56.000000 mteb-1.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.393707 mteb-1.7.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.413707 mteb-1.7.0/docs/mmteb/
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-20 19:41:56.000000 mteb-1.7.0/docs/mmteb/create_points_table.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-20 19:41:56.000000 mteb-1.7.0/docs/mmteb/validate_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.413707 mteb-1.7.0/mteb/
+-rw-r--r--   0 root         (0) root         (0)     2273 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.421707 mteb-1.7.0/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5876 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)    24826 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskInstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     9793 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7082 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/iso_15924_to_script.json
+-rw-r--r--   0 root         (0) root         (0)   193114 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/iso_639_3_to_language.json
+-rw-r--r--   0 root         (0) root         (0)      541 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/abstasks/languages.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.421707 mteb-1.7.0/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13004 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.421707 mteb-1.7.0/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8927 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)      789 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    13983 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      820 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.421707 mteb-1.7.0/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.425707 mteb-1.7.0/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      470 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.425707 mteb-1.7.0/mteb/tasks/BitextMining/dan/
+-rw-r--r--   0 root         (0) root         (0)     1443 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.425707 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5709 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.425707 mteb-1.7.0/mteb/tasks/BitextMining/vie/
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/BitextMining/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.425707 mteb-1.7.0/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.425707 mteb-1.7.0/mteb/tasks/Classification/ara/
+-rw-r--r--   0 root         (0) root         (0)     1725 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ara/TweetEmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ara/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.425707 mteb-1.7.0/mteb/tasks/Classification/bam/
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/bam/BambaraSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/bam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.429707 mteb-1.7.0/mteb/tasks/Classification/ben/
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ben/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.429707 mteb-1.7.0/mteb/tasks/Classification/bul/
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/bul/BulgarianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/bul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.429707 mteb-1.7.0/mteb/tasks/Classification/ces/
+-rw-r--r--   0 root         (0) root         (0)     1704 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.429707 mteb-1.7.0/mteb/tasks/Classification/dan/
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/dan/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/dan/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/dan/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/dan/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.429707 mteb-1.7.0/mteb/tasks/Classification/ell/
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ell/GreekSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/eng/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/eng/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/eng/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/eng/NewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/est/
+-rw-r--r--   0 root         (0) root         (0)     2407 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/est/estonian_valence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/fas/
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/fas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/fra/
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/hin/
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/hin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/hrv/
+-rw-r--r--   0 root         (0) root         (0)     2028 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/hrv/CroatianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/hrv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/ind/
+-rw-r--r--   0 root         (0) root         (0)     2881 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ind/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/ita/
+-rw-r--r--   0 root         (0) root         (0)     4105 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ita/ItaHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ita/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3550 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/jpn/WRIMEClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.433707 mteb-1.7.0/mteb/tasks/Classification/kur/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/kur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.437707 mteb-1.7.0/mteb/tasks/Classification/mkd/
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/mkd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.437707 mteb-1.7.0/mteb/tasks/Classification/mlt/
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/mlt/MalteseSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/mlt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.437707 mteb-1.7.0/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.437707 mteb-1.7.0/mteb/tasks/Classification/nld/
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/nld/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.437707 mteb-1.7.0/mteb/tasks/Classification/nob/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/nob/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/nob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/pol/
+-rw-r--r--   0 root         (0) root         (0)     4922 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/pol/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/ron/
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/ron/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/slk/
+-rw-r--r--   0 root         (0) root         (0)     2078 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/slk/SlovakSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/slk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/swe/
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/swe/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/swe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/tur/
+-rw-r--r--   0 root         (0) root         (0)     1518 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/tur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/uig/
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/uig/UyghurSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/uig/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/vie/
+-rw-r--r--   0 root         (0) root         (0)     3368 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/zho/
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/zho/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Classification/zul/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Classification/zul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.441707 mteb-1.7.0/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1319 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.445707 mteb-1.7.0/mteb/tasks/Clustering/deu/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.445707 mteb-1.7.0/mteb/tasks/Clustering/eng/
+-rw-r--r--   0 root         (0) root         (0)     1101 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.449707 mteb-1.7.0/mteb/tasks/Clustering/fra/
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/fra/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.449707 mteb-1.7.0/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.449707 mteb-1.7.0/mteb/tasks/Clustering/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/nob/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/nob/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.449707 mteb-1.7.0/mteb/tasks/Clustering/pol/
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/pol/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.449707 mteb-1.7.0/mteb/tasks/Clustering/rom/
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.449707 mteb-1.7.0/mteb/tasks/Clustering/spa/
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.449707 mteb-1.7.0/mteb/tasks/Clustering/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3917 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/swe/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.453707 mteb-1.7.0/mteb/tasks/Clustering/zho/
+-rw-r--r--   0 root         (0) root         (0)     3639 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/zho/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Clustering/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.453707 mteb-1.7.0/mteb/tasks/InstructionRetrieval/
+-rw-r--r--   0 root         (0) root         (0)      176 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/InstructionRetrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.453707 mteb-1.7.0/mteb/tasks/InstructionRetrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/InstructionRetrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.453707 mteb-1.7.0/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      344 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.453707 mteb-1.7.0/mteb/tasks/PairClassification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.453707 mteb-1.7.0/mteb/tasks/PairClassification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.453707 mteb-1.7.0/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2780 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.453707 mteb-1.7.0/mteb/tasks/PairClassification/pol/
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/pol/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.457707 mteb-1.7.0/mteb/tasks/PairClassification/zho/
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/PairClassification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.457707 mteb-1.7.0/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.457707 mteb-1.7.0/mteb/tasks/Reranking/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/eng/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/eng/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.457707 mteb-1.7.0/mteb/tasks/Reranking/fra/
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/fra/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/fra/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.457707 mteb-1.7.0/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.457707 mteb-1.7.0/mteb/tasks/Reranking/zho/
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/zho/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Reranking/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.457707 mteb-1.7.0/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     3401 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.457707 mteb-1.7.0/mteb/tasks/Retrieval/code/
+-rw-r--r--   0 root         (0) root         (0)     3377 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/code/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.461707 mteb-1.7.0/mteb/tasks/Retrieval/dan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/dan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/dan/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/dan/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.461707 mteb-1.7.0/mteb/tasks/Retrieval/deu/
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.469707 mteb-1.7.0/mteb/tasks/Retrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.469707 mteb-1.7.0/mteb/tasks/Retrieval/est/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/est/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/est/estqa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.473707 mteb-1.7.0/mteb/tasks/Retrieval/fra/
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.473707 mteb-1.7.0/mteb/tasks/Retrieval/hun/
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/hun/HunSum2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.473707 mteb-1.7.0/mteb/tasks/Retrieval/jpn/
+-rw-r--r--   0 root         (0) root         (0)     2853 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.473707 mteb-1.7.0/mteb/tasks/Retrieval/kor/
+-rw-r--r--   0 root         (0) root         (0)      906 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/kor/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/kor/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.473707 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.473707 mteb-1.7.0/mteb/tasks/Retrieval/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/nob/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/nob/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.477707 mteb-1.7.0/mteb/tasks/Retrieval/pol/
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.477707 mteb-1.7.0/mteb/tasks/Retrieval/spa/
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.477707 mteb-1.7.0/mteb/tasks/Retrieval/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/swe/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.477707 mteb-1.7.0/mteb/tasks/Retrieval/vie/
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.481706 mteb-1.7.0/mteb/tasks/Retrieval/zho/
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Retrieval/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.481706 mteb-1.7.0/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      678 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.481706 mteb-1.7.0/mteb/tasks/STS/deu/
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.481706 mteb-1.7.0/mteb/tasks/STS/eng/
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.481706 mteb-1.7.0/mteb/tasks/STS/fra/
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/fra/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.481706 mteb-1.7.0/mteb/tasks/STS/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/jpn/JSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/STS/kor/
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/kor/KlueSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/kor/KorSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/STS/pol/
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/pol/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/STS/ron/
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/ron/RonSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/STS/spa/
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/spa/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/STS/zho/
+-rw-r--r--   0 root         (0) root         (0)     7122 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/zho/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/STS/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/Summarization/eng/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Summarization/eng/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Summarization/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.485707 mteb-1.7.0/mteb/tasks/Summarization/fra/
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/Summarization/fra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      288 2024-04-20 19:41:56.000000 mteb-1.7.0/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.537706 mteb-1.7.0/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23583 2024-04-20 19:42:00.000000 mteb-1.7.0/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34031 2024-04-20 19:42:00.000000 mteb-1.7.0/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 19:42:00.000000 mteb-1.7.0/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-20 19:42:00.000000 mteb-1.7.0/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-20 19:42:00.000000 mteb-1.7.0/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-20 19:42:00.000000 mteb-1.7.0/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-04-20 19:41:57.000000 mteb-1.7.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.409707 mteb-1.7.0/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.489707 mteb-1.7.0/results/GritLM__GritLM-7B/
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-20 19:41:56.000000 mteb-1.7.0/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-04-20 19:41:56.000000 mteb-1.7.0/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-04-20 19:41:56.000000 mteb-1.7.0/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.409707 mteb-1.7.0/results/dangvantuan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.493707 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      250 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/BSARDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      675 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
+-rw-r--r--   0 root         (0) root         (0)      676 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
+-rw-r--r--   0 root         (0) root         (0)      332 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      335 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)     2801 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      820 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/SICKFr.json
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/STS22.json
+-rw-r--r--   0 root         (0) root         (0)      921 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
+-rw-r--r--   0 root         (0) root         (0)      221 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-04-20 19:41:56.000000 mteb-1.7.0/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.409707 mteb-1.7.0/results/intfloat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.493707 mteb-1.7.0/results/intfloat/multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      384 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat/multilingual-e5-small/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat/multilingual-e5-small/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat/multilingual-e5-small/SlovakSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.493707 mteb-1.7.0/results/intfloat__e5-small/
+-rw-r--r--   0 root         (0) root         (0)      439 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__e5-small/TurkishProductSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.493707 mteb-1.7.0/results/intfloat__e5-small-v2/
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.497707 mteb-1.7.0/results/intfloat__multilingual-e5-base/
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      733 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-base/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.509706 mteb-1.7.0/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/BambaraSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/BulgarianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      463 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/GermanDPR.json
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/GreekSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/ItaHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7814 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7703 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3392 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      403 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)      298 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      304 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      372 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-20 19:41:56.000000 mteb-1.7.0/results/intfloat__multilingual-e5-small/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.409707 mteb-1.7.0/results/sentence-transformers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.513706 mteb-1.7.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SlovakSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.513706 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      302 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      194 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/model.json
+-rw-r--r--   0 root         (0) root         (0)      194 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.529706 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      344 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      762 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      759 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)      291 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7839 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7915 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      736 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3382 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3376 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)    16669 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)    18247 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      741 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      471 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)      294 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)      176 2024-04-20 19:41:56.000000 mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5924 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/medicalqaretrieval/
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/medicalqaretrieval/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.533706 mteb-1.7.0/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.537706 mteb-1.7.0/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.537706 mteb-1.7.0/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.537706 mteb-1.7.0/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/mteb_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.413707 mteb-1.7.0/scripts/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.537706 mteb-1.7.0/scripts/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.537706 mteb-1.7.0/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/run_mteb_law.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-20 19:41:56.000000 mteb-1.7.0/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 19:42:00.541706 mteb-1.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:42:00.537706 mteb-1.7.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_all_abstasks.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_mteb.py
+-rw-r--r--   0 root         (0) root         (0)      278 2024-04-20 19:41:56.000000 mteb-1.7.0/tests/test_retrieval_abstask.py
```

### Comparing `mteb-1.6.9/LICENSE` & `mteb-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/PKG-INFO` & `mteb-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.6.9
+Version: 1.7.0
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -226,15 +226,15 @@
 Requires-Dist: scikit_learn>=1.0.2
 Requires-Dist: scipy
 Requires-Dist: sentence_transformers>=2.2.0
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: rich
 Requires-Dist: pytrec-eval-terrier>=0.5.6
-Requires-Dist: pydantic
+Requires-Dist: pydantic>=2.0.0
 Requires-Dist: typing_extensions
 Requires-Dist: eval_type_backport
 Provides-Extra: dev
 Requires-Dist: ruff>=0.0.254; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
@@ -448,15 +448,15 @@
 | 📈 [Leaderboard] | The interactive leaderboard of the benchmark |
 | 🤖 [Adding a model] | Information related to how to submit a model to the leaderboard |
 | 👩‍💻 [Adding a dataset] | How to add a new task/dataset to MTEB | 
 | 🤝  [Contributing] | How to contribute to MTEB and set it up for development |
 <!-- | 🌐 [MMTEB] | An open-source effort to extend MTEB to cover a broad set of languages |   -->
 
 [Tasks]: docs/tasks.md
-[Contributing]: contributing.md
+[Contributing]: CONTRIBUTING.md
 [Adding a model]: docs/adding_a_model.md
 [Adding a dataset]: docs/adding_a_dataset.md
 [Leaderboard]: https://huggingface.co/spaces/mteb/leaderboard
 [MMTEB]: docs/mmteb/readme.md
 
 ## Citing
```

### Comparing `mteb-1.6.9/README.md` & `mteb-1.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 | 📈 [Leaderboard] | The interactive leaderboard of the benchmark |
 | 🤖 [Adding a model] | Information related to how to submit a model to the leaderboard |
 | 👩‍💻 [Adding a dataset] | How to add a new task/dataset to MTEB | 
 | 🤝  [Contributing] | How to contribute to MTEB and set it up for development |
 <!-- | 🌐 [MMTEB] | An open-source effort to extend MTEB to cover a broad set of languages |   -->
 
 [Tasks]: docs/tasks.md
-[Contributing]: contributing.md
+[Contributing]: CONTRIBUTING.md
 [Adding a model]: docs/adding_a_model.md
 [Adding a dataset]: docs/adding_a_dataset.md
 [Leaderboard]: https://huggingface.co/spaces/mteb/leaderboard
 [MMTEB]: docs/mmteb/readme.md
 
 ## Citing
```

### Comparing `mteb-1.6.9/mteb/__init__.py` & `mteb-1.7.0/mteb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,20 @@
     "ToxicConversationsClassification",
     "TweetSentimentExtractionClassification",
     "TwentyNewsgroupsClustering",
     "TwitterSemEval2015",
     "TwitterURLCorpus",
 ]
 
+MTEB_RETRIEVAL_WITH_INSTRUCTIONS = [
+    "RobustInstructionRetrieval",
+    "NewsInstructionRetrieval",
+    "CoreInstructionRetrieval",
+]
+
 MTEB_RETRIEVAL_LAW = [
     "LegalSummarization",
     "LegalBenchConsumerContractsQA",
     "LegalBenchCorporateLobbying",
     "AILACasedocs",
     "AILAStatutes",
     "LeCaRDv2",
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTask.py` & `mteb-1.7.0/mteb/abstasks/AbsTask.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,56 +23,49 @@
         self.seed = seed
         random.seed(self.seed)
         np.random.seed(self.seed)
         torch.manual_seed(self.seed)
         torch.cuda.manual_seed_all(self.seed)
 
     def dataset_transform(self):
-        """
-        Transform operations applied to the dataset after loading.
+        """Transform operations applied to the dataset after loading.
         Override this method if your dataset requires any transformation.
         """
         pass
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
+        """Load dataset from HuggingFace hub"""
         if self.data_loaded:
             return
         self.dataset = datasets.load_dataset(**self.metadata_dict["dataset"])
         self.dataset_transform()
         self.data_loaded = True
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = dict(self.metadata)
         return metadata_dict
 
     @abstractmethod
     def evaluate(self, model, split="test"):
-        """
-        Evaluates a Sentence Embedding Model on the task.
+        """Evaluates a Sentence Embedding Model on the task.
         Returns a dict (that can be serialized to json).
         :param model: Sentence embedding method. Implements a encode(sentences) method, that encodes sentences
         and returns a numpy matrix with the sentence embeddings
         :param split: Which datasplit to be used.
         """
         raise NotImplementedError
 
     @property
     def languages(self) -> set[str]:
-        """
-        Returns the languages of the task
-        """
+        """Returns the languages of the task"""
         return self.metadata.languages
 
     def __repr__(self) -> str:
-        """
-        Format the representation of the task such that it appears as:
+        """Format the representation of the task such that it appears as:
 
         TaskObjectName(name='{name}', languages={lang1, lang2, ...})
         """
         langs = self.languages
         if len(langs) > 3:
             langs = list(langs)[:3]
             langs.append("...")
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.7.0/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from ..evaluation.evaluators import BitextMiningEvaluator
 from .AbsTask import AbsTask
 
 logger = logging.getLogger(__name__)
 
 
 class AbsTaskBitextMining(AbsTask):
-    """
-    Abstract class for BitextMining tasks
+    """Abstract class for BitextMining tasks
     The similarity is computed between pairs and the results are ranked.
 
     self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns:
         id: str
         sentence1: str
         sentence2: str
     """
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.7.0/mteb/abstasks/AbsTaskClassification.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 )
 from .AbsTask import AbsTask
 
 logger = logging.getLogger(__name__)
 
 
 class AbsTaskClassification(AbsTask):
-    """
-    Abstract class for kNN classification tasks
+    """Abstract class for kNN classification tasks
     The similarity is computed between pairs and the results are ranked.
 
     self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns:
         text: str
         label: int
     """
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.7.0/mteb/abstasks/AbsTaskClustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from ..evaluation.evaluators import ClusteringEvaluator
 from .AbsTask import AbsTask
 
 logger = logging.getLogger(__name__)
 
 
 class AbsTaskClustering(AbsTask):
-    """
-    Abstract class for Clustering tasks
+    """Abstract class for Clustering tasks
     The similarity is computed between pairs and the results are ranked.
 
     self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns:
         sentences: list of str
         labels: list of str
     """
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.7.0/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from ..evaluation.evaluators import PairClassificationEvaluator
 from .AbsTask import AbsTask
 
 logger = logging.getLogger(__name__)
 
 
 class AbsTaskPairClassification(AbsTask):
-    """
-    Abstract class for PairClassificationTasks
+    """Abstract class for PairClassificationTasks
     The similarity is computed between pairs and the results are ranked. Average precision
     is computed to measure how well the methods can be used for pairwise pair classification.
 
     self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns:
         sent1: list[str]
         sent2: list[str]
         labels: list[int]
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.7.0/mteb/abstasks/AbsTaskReranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 from ..evaluation.evaluators import RerankingEvaluator
 from .AbsTask import AbsTask
 
 
 class AbsTaskReranking(AbsTask):
-    """
-    Abstract class for re-ranking experiments.
+    """Abstract class for re-ranking experiments.
 
     self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns:
         query: str
         positive: list[str]
         negative: list[str]
     """
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.7.0/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -189,16 +189,15 @@
             }
         )
         qrels_ds = qrels_ds.cast(features)
         self.qrels = qrels_ds
 
 
 class AbsTaskRetrieval(AbsTask):
-    """
-    Abstract class for re-ranking experiments.
+    """Abstract class for re-ranking experiments.
 
     Child-classes must implement the following properties:
 
     self.corpus: dict[str, dict[str, str]]
         Semantically, it should contain dict[split_name, dict[sample_id, dict[str, str]]]
         E.g. {"test": {"document_one": {"_id": "d1", "title": "title", "text": "text"}}}
 
@@ -319,7 +318,47 @@
             **{f"ndcg_at_{k.split('@')[1]}": v for (k, v) in ndcg.items()},
             **{f"map_at_{k.split('@')[1]}": v for (k, v) in _map.items()},
             **{f"recall_at_{k.split('@')[1]}": v for (k, v) in recall.items()},
             **{f"precision_at_{k.split('@')[1]}": v for (k, v) in precision.items()},
             **{f"mrr_at_{k.split('@')[1]}": v for (k, v) in mrr.items()},
         }
         return scores
+
+    def calculate_metadata_metrics(self) -> None:
+        self.load_data()
+
+        for split in self.metadata_dict["eval_splits"]:
+            if self.is_multilingual:
+                for lang in self.relevant_docs.keys():
+                    process_language(
+                        self.relevant_docs[lang][split],
+                        self.queries[lang][split],
+                        self.corpus[lang][split],
+                        lang,
+                    )
+            else:
+                process_language(
+                    self.relevant_docs[split], self.queries[split], self.corpus[split]
+                )
+
+
+def process_language(relevant_docs, queries, corpus, lang=None):
+    total_length, num_pairs = calculate_length_and_count(relevant_docs, queries, corpus)
+    average_length = total_length / num_pairs if num_pairs else 0
+    num_documents = len(queries) + len(corpus)
+
+    language_description = f" for language {lang}" if lang else ""
+    print(f"Average character length{language_description} is {average_length}")
+    print(f"Number of queries and documents{language_description} is {num_documents}")
+
+
+def calculate_length_and_count(relevant_docs, queries, corpus):
+    total_length = 0
+    num_pairs = 0
+    for query_id, docs in relevant_docs.items():
+        query = queries[query_id]
+        for doc_id in docs:
+            doc = corpus[doc_id]
+            doc_text = doc["title"] + doc["text"]
+            total_length += len(query) + len(doc_text)
+            num_pairs += 1
+    return total_length, num_pairs
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.7.0/mteb/abstasks/AbsTaskSTS.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from ..evaluation.evaluators import STSEvaluator
 from .AbsTask import AbsTask
 
 logger = logging.getLogger(__name__)
 
 
 class AbsTaskSTS(AbsTask):
-    """
-    Abstract class for STS experiments.
+    """Abstract class for STS experiments.
 
     self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns::
         sentence1: str
         sentence2: str
         score: float
     """
```

### Comparing `mteb-1.6.9/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.7.0/mteb/abstasks/AbsTaskSummarization.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from ..evaluation.evaluators import SummarizationEvaluator
 from .AbsTask import AbsTask
 
 logger = logging.getLogger(__name__)
 
 
 class AbsTaskSummarization(AbsTask):
-    """
-    Abstract class for summarization experiments.
+    """Abstract class for summarization experiments.
 
     self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns:
         text: str
         human_summaries: list[str]
         machine_summaries: list[str]
         relevance: list[float] (the score of the machine generated summaries)
     """
```

### Comparing `mteb-1.6.9/mteb/abstasks/CrosslingualTask.py` & `mteb-1.7.0/mteb/abstasks/CrosslingualTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,15 @@
         if langs is not None and len(langs) > 0:
             self.langs = langs
         else:
             self.langs = self.metadata_dict["eval_langs"]
         self.is_crosslingual = True
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
+        """Load dataset from HuggingFace hub"""
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
                 name=lang, **self.metadata_dict["dataset"]
             )
```

### Comparing `mteb-1.6.9/mteb/abstasks/LangMapping.py` & `mteb-1.7.0/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/abstasks/MultilingualTask.py` & `mteb-1.7.0/mteb/abstasks/MultilingualTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,15 @@
                 langs  # TODO: case where user provides langs not in the dataset
             )
         else:
             self.langs = self.metadata_dict["eval_langs"]
         self.is_multilingual = True
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
+        """Load dataset from HuggingFace hub"""
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
                 name=lang,
                 **self.metadata_dict.get("dataset", None),
```

### Comparing `mteb-1.6.9/mteb/abstasks/TaskMetadata.py` & `mteb-1.7.0/mteb/abstasks/TaskMetadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "Code retrieval",
     "False Friends",
 ]
 
 TASK_DOMAIN = Literal[
     "Academic",
     "Blog",
+    "Constructed",
     "Encyclopaedic",
     "Fiction",
     "Government",
     "Legal",
     "Medical",
     "News",
     "Non-fiction",
@@ -78,14 +79,15 @@
     "Classification",
     "Clustering",
     "PairClassification",
     "Reranking",
     "Retrieval",
     "STS",
     "Summarization",
+    "InstructionRetrieval",
 ]
 
 TASK_CATEGORY = Literal[
     "s2s",  # Sentence-to-sentence
     "s2p",  # Sentence-to-paragraph
     "p2p",  # Paragraph-to-paragraph
 ]
@@ -109,16 +111,15 @@
 
 PROGRAMMING_LANGS = ["python", "javascript", "go", "ruby", "java", "php"]
 
 logger = logging.getLogger(__name__)
 
 
 class TaskMetadata(BaseModel):
-    """
-    Metadata for a task.
+    """Metadata for a task.
 
     Args:
         dataset: All arguments to pass to datasets.load_dataset to load the dataset for the task. Refer to https://huggingface.co/docs/datasets/v2.18.0/en/package_reference/loading_methods#datasets.load_dataset
         name: The name of the task.
         description: A description of the task.
         type: The type of the task. These includes "Classification", "Summarization", "STS", "Retrieval", "Reranking", "Clustering",
             "PairClassification", "BitextMining". The type should match the abstask type.
@@ -175,17 +176,15 @@
     bibtex_citation: str | None
 
     n_samples: dict[SPLIT_NAME, int] | None
     avg_character_length: dict[SPLIT_NAME, float] | None
 
     @field_validator("dataset")
     def _check_dataset_path_is_specified(cls, dataset):
-        """
-        This method checks that the dataset path is specified.
-        """
+        """This method checks that the dataset path is specified."""
         if "path" not in dataset or dataset["path"] is None:
             raise ValueError(
                 "You must specify the path to the dataset in the dataset dictionary. "
                 "See https://huggingface.co/docs/datasets/main/en/package_reference/loading_methods#datasets.load_dataset"
             )
         return dataset
 
@@ -200,31 +199,27 @@
                 "Revision missing for the dataset %s. It is encourage to specify a dataset revision for reproducability.",
                 dataset["path"],
             )
         return dataset
 
     @field_validator("eval_langs")
     def _check_eval_langs(cls, eval_langs):
-        """
-        This method checks that the eval_langs are specified as a list of languages.
-        """
+        """This method checks that the eval_langs are specified as a list of languages."""
         if isinstance(eval_langs, dict):
             for langs in eval_langs.values():
                 for code in langs:
                     cls._check_language_code(code)
         else:
             for code in eval_langs:
                 cls._check_language_code(code)
         return eval_langs
 
     @staticmethod
     def _check_language_code(code):
-        """
-        This method checks that the language code (e.g. "eng-Latn") is valid.
-        """
+        """This method checks that the language code (e.g. "eng-Latn") is valid."""
         lang, script = code.split("-")
         if script == "Code":
             if lang in PROGRAMMING_LANGS:
                 return  # override for code
             else:
                 raise ValueError(
                     f"Programming language {lang} is not a valid programming language."
@@ -236,32 +231,28 @@
         if script not in ISO_TO_SCRIPT:
             raise ValueError(
                 f"Invalid script code: {script}, you can find valid ISO 15924 codes in {path_to_lang_scripts}"
             )
 
     @property
     def languages(self) -> set[str]:
-        """
-        Return the languages of the dataset as iso639-3 codes.
-        """
+        """Return the languages of the dataset as iso639-3 codes."""
 
         def get_lang(lang: str) -> str:
             return lang.split("-")[0]
 
         if isinstance(self.eval_langs, dict):
             return set(
                 get_lang(lang) for langs in self.eval_langs.values() for lang in langs
             )
         return set(get_lang(lang) for lang in self.eval_langs)
 
     @property
     def scripts(self) -> set[str]:
-        """
-        Return the scripts of the dataset as iso15924 codes.
-        """
+        """Return the scripts of the dataset as iso15924 codes."""
 
         def get_script(lang: str) -> str:
             return lang.split("-")[1]
 
         if isinstance(self.eval_langs, dict):
             return set(
                 get_script(lang) for langs in self.eval_langs.values() for lang in langs
```

### Comparing `mteb-1.6.9/mteb/abstasks/iso_15924_to_script.json` & `mteb-1.7.0/mteb/abstasks/iso_15924_to_script.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/abstasks/iso_639_3_to_language.json` & `mteb-1.7.0/mteb/abstasks/iso_639_3_to_language.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/abstasks/languages.py` & `mteb-1.7.0/mteb/abstasks/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Language codes (ISO 639-3) obtained from: https://iso639-3.sil.org/sites/iso639-3/files/downloads/iso-639-3.tab
+"""Language codes (ISO 639-3) obtained from: https://iso639-3.sil.org/sites/iso639-3/files/downloads/iso-639-3.tab
 Script codes (ISO 15924) obtained from: https://unicode.org/iso15924/iso15924.txt
 """
 
 import json
 from pathlib import Path
 
 path_to_lang_codes = Path(__file__).parent / "iso_639_3_to_language.json"
```

### Comparing `mteb-1.6.9/mteb/cmd.py` & `mteb-1.7.0/mteb/cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""
-entry point for the library
+"""entry point for the library
+
 example call:
   pip install git+https://github.com/embeddings-benchmark/mteb-draft.git
   mteb -m average_word_embeddings_komninos \
        -t Banking77Classification EmotionClassification \
        --output_folder mteb_output \
        --verbosity 3
 """
```

### Comparing `mteb-1.6.9/mteb/evaluation/MTEB.py` & `mteb-1.7.0/mteb/evaluation/MTEB.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,35 +26,34 @@
         task_categories: List[str] | None = None,
         task_langs: List[str] | None = None,
         tasks: List[Union[str, AbsTask]] | None = None,
         version=None,
         err_logs_path="error_logs.txt",
         **kwargs,
     ):
-        """
-        Create an Evaluation pipeline. The tasks selected
+        """Create an Evaluation pipeline. The tasks selected
         depends on the parameters. One can specify the tasks types
         they want to evaluate (e.g. Clustering, Retrieval, etc.)
         the categories of tasks they want (e.g. Sentence2Sentence,
         Sentence2Paragraph, etc.) and the version of the benchmark.
         The selected tasks will be the tasks satisfying conditions
         from the 3 arguments. Alternatively, one can specify a list
         of tasks to be evaluated with the `tasks` argument. If
         `tasks` is specified, we filter tasks based on `task_langs`
 
         Args:
             task_types: List of task types (Clustering, Retrieval..) to be evaluated. If None, all tasks will be evaluated
             task_categories: List of task categories (s2s, p2p..) to be evaluated. If None, all tasks will be evaluated
-        task_langs: List of languages to be evaluated. if None, all languages will be evaluated. ["eng-Latn", "deu_Latn"] will evaluate on all tasks
-            with these languages.
-        tasks: List of tasks to be evaluated. If specified, we filter tasks based on `task_langs` only
-        version: Version of the benchmark to use. If None, latest is used
-        err_logs_path: Path to save error logs
+            task_langs: List of languages to be evaluated. if None, all languages will be evaluated. ["eng-Latn", "deu_Latn"] will evaluate on all tasks
+                with these languages.
+            tasks: List of tasks to be evaluated. If specified, we filter tasks based on `task_langs` only
+            version: Version of the benchmark to use. If None, latest is used
+            err_logs_path: Path to save error logs
+            kwargs: Additional arguments to be passed to the tasks
         """
-
         if tasks is not None:
             self._tasks = tasks
             assert (
                 task_types is None and task_categories is None
             ), "Cannot specify both `tasks` and `task_types`/`task_categories`"
         else:
             self._task_types = task_types
@@ -138,28 +137,24 @@
                     console.print(
                         f"{prefix}{name}{category}{multilingual}{crosslingual}"
                     )
                 console.print("\n")
 
     @classmethod
     def mteb_tasks(cls):
-        """
-        Get all tasks available in the MTEB.
-        """
+        """Get all tasks available in the MTEB."""
         instance = cls()
         instance._display_tasks(instance.tasks_cls, name="MTEB tasks")
 
     def print_selected_tasks(self):
         """Print the selected tasks."""
         self._display_tasks(self.tasks, name="Selected tasks")
 
     def select_tasks(self, **kwargs):
-        """
-        Select the tasks to be evaluated.
-        """
+        """Select the tasks to be evaluated."""
         # Get all existing tasks
         tasks_categories_cls = [cls for cls in AbsTask.__subclasses__()]
         self.tasks_cls = [
             cls(langs=self._task_langs, **kwargs)
             for cat_cls in tasks_categories_cls
             for cls in cat_cls.__subclasses__()
             if cat_cls.__name__.startswith("AbsTask")
@@ -212,17 +207,15 @@
             filtered_tasks,
         )
 
         # Get final list of tasks
         self.tasks = list(filtered_tasks)
 
     def load_tasks_data(self):
-        """
-        Load datasets for the selected tasks.
-        """
+        """Load datasets for the selected tasks."""
         logger.info(f"\n\n## Loading datasets for {len(self.tasks)} tasks")
         for task in self.tasks:
             logger.info(f"\n# Loading dataset for {task.metadata_dict['name']}")
             task.load_data()
 
     def run(
         self,
@@ -230,16 +223,15 @@
         verbosity=1,
         output_folder="results/result",
         eval_splits=None,
         overwrite_results=False,
         raise_error: bool = True,
         **kwargs,
     ):
-        """
-        Run the evaluation pipeline on the selected tasks.
+        """Run the evaluation pipeline on the selected tasks.
 
         Parameters
         ----------
         model:
             Model to be used for evaluation
         verbosity: int
             Verbosity level. Default is 1.
```

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,15 @@
         query_embeddings,
         corpus_embeddings,
         query_chunk_size=100,
         corpus_chunk_size=500000,
         top_k=10,
         score_function=cos_sim,
     ):
-        """
-        This function performs a cosine similarity search between a list of query embeddings  and a list of corpus embeddings.
+        """This function performs a cosine similarity search between a list of query embeddings  and a list of corpus embeddings.
         It can be used for Information Retrieval / Semantic Search for corpora up to about 1 Million entries.
         :param query_embeddings: A 2 dimensional tensor with the query embeddings.
         :param corpus_embeddings: A 2 dimensional tensor with the corpus embeddings.
         :param query_chunk_size: Process 100 queries simultaneously. Increasing that value increases the speed, but requires more memory.
         :param corpus_chunk_size: Scans the corpus 100k entries at a time. Increasing that value increases the speed, but requires more memory.
         :param top_k: Retrieve top k matching entries.
         :param score_function: Function for computing scores. By default, cosine similarity.
```

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,17 +150,18 @@
         scores["f1"] = max_f1
         if len(np.unique(self.y_train)) == 2:
             scores["ap"] = max_ap
         return scores, test_cache
 
     @staticmethod
     def _cos_sim(a: Tensor, b: Tensor):
-        """
-        Computes the cosine similarity cos_sim(a[i], b[j]) for all i and j.
-        :return: Matrix with res[i][j]  = cos_sim(a[i], b[j])
+        """Computes the cosine similarity cos_sim(a[i], b[j]) for all i and j.
+
+        Return:
+            Matrix with res[i][j]  = cos_sim(a[i], b[j])
         """
         if not isinstance(a, torch.Tensor):
             a = torch.tensor(a)
 
         if not isinstance(b, torch.Tensor):
             b = torch.tensor(b)
 
@@ -172,16 +173,15 @@
 
         a_norm = torch.nn.functional.normalize(a, p=2, dim=1)
         b_norm = torch.nn.functional.normalize(b, p=2, dim=1)
         return torch.mm(a_norm, b_norm.transpose(0, 1))
 
     @staticmethod
     def _euclidean_dist(a: Tensor, b: Tensor):
-        """
-        Computes the euclidean distance euclidean_dist(a[i], b[j]) for all i and j.
+        """Computes the euclidean distance euclidean_dist(a[i], b[j]) for all i and j.
         :return: Matrix with res[i][j]  = euclidean_dist(a[i], b[j])
         """
         if not isinstance(a, torch.Tensor):
             a = torch.tensor(a)
 
         if not isinstance(b, torch.Tensor):
             b = torch.tensor(b)
@@ -192,16 +192,15 @@
         if len(b.shape) == 1:
             b = b.unsqueeze(0)
 
         return torch.cdist(a, b, p=2)
 
     @staticmethod
     def _dot_score(a: Tensor, b: Tensor):
-        """
-        Computes the dot-product dot_prod(a[i], b[j]) for all i and j.
+        """Computes the dot-product dot_prod(a[i], b[j]) for all i and j.
         :return: Matrix with res[i][j]  = dot_prod(a[i], b[j])
         """
         if not isinstance(a, torch.Tensor):
             a = torch.tensor(a)
 
         if not isinstance(b, torch.Tensor):
             b = torch.tensor(b)
```

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/Evaluator.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,28 @@
 from abc import ABC, abstractmethod
 
 import numpy as np
 import torch
 
 
 class Evaluator(ABC):
-    """
-    Base class for all evaluators
+    """Base class for all evaluators
     Extend this class and implement __call__ for custom evaluators.
     """
 
     def __init__(self, seed=42, **kwargs):
         self.seed = seed
         random.seed(self.seed)
         np.random.seed(self.seed)
         torch.manual_seed(self.seed)
         torch.cuda.manual_seed_all(self.seed)
 
     @abstractmethod
     def __call__(self, model):
-        """
-        This is called during training to evaluate the model.
+        """This is called during training to evaluate the model.
         It returns scores.
 
         Parameters
         ----------
         model:
             the model to evaluate
         """
```

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 from .Evaluator import Evaluator
 
 logger = logging.getLogger(__name__)
 
 
 class PairClassificationEvaluator(Evaluator):
-    """
-    Evaluate a model based on the similarity of the embeddings by calculating the accuracy of identifying similar and
+    """Evaluate a model based on the similarity of the embeddings by calculating the accuracy of identifying similar and
     dissimilar sentences.
     The metrics are the cosine similarity as well as euclidean and Manhattan distance
     The returned score is the accuracy with a specified metric.
     The results are written in a CSV. If a CSV already exists, then values are appended.
     The labels need to be 0 for dissimilar pairs and 1 for similar pairs.
     :param sentences1: The first column of sentences
     :param sentences2: The second column of sentences
@@ -88,16 +87,15 @@
         ]:
             output_scores[short_name] = self._compute_metrics(scores, labels, reverse)
 
         return output_scores
 
     @staticmethod
     def _compute_metrics(scores, labels, high_score_more_similar):
-        """
-        Compute the metrics for the given scores and labels.
+        """Compute the metrics for the given scores and labels.
 
         Args:
             scores (`np.ndarray` of shape (n_pairs, )): The similarity/dissimilarity scores for the pairs.
             labels (`np.ndarray` of shape (n_pairs, )): The labels for the pairs.
             high_score_more_similar (`bool`): If true, then the higher the score, the more similar the pairs are.
 
         Returns:
```

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from .Evaluator import Evaluator
 from .utils import cos_sim
 
 logger = logging.getLogger(__name__)
 
 
 class RerankingEvaluator(Evaluator):
-    """
-    This class evaluates a SentenceTransformer model for the task of re-ranking.
+    """This class evaluates a SentenceTransformer model for the task of re-ranking.
     Given a query and a list of documents, it computes the score [query, doc_i] for all possible
     documents and sorts them in decreasing order. Then, MRR@10 and MAP is compute to measure the quality of the ranking.
     :param samples: Must be a list and each element is of the form:
         - {'query': '', 'positive': [], 'negative': []}. Query is the search query, positive is a list of positive
         (relevant) documents, negative is a list of negative (irrelevant) documents.
         - {'query': [], 'positive': [], 'negative': []}. Where query is a list of strings, which embeddings we average
         to get the query embedding.
@@ -64,16 +63,15 @@
         return (
             self.compute_metrics_batched(model)
             if self.use_batched_encoding
             else self.compute_metrics_individual(model)
         )
 
     def compute_metrics_batched(self, model):
-        """
-        Computes the metrices in a batched way, by batching all queries and
+        """Computes the metrices in a batched way, by batching all queries and
         all documents together
         """
         all_mrr_scores = []
         all_ap_scores = []
 
         # using encode_queries and encode_corpus functions if they exists,
         # which can be defined by users to add different instructions for query and passage conveniently
@@ -141,16 +139,15 @@
 
         mean_ap = np.mean(all_ap_scores)
         mean_mrr = np.mean(all_mrr_scores)
 
         return {"map": mean_ap, "mrr": mean_mrr}
 
     def compute_metrics_individual(self, model):
-        """
-        Embeds every (query, positive, negative) tuple individually.
+        """Embeds every (query, positive, negative) tuple individually.
         Is slower than the batched version, but saves memory as only the
         embeddings for one tuple are needed. Useful when you have
         a really large test set
         """
         all_mrr_scores = []
         all_ap_scores = []
 
@@ -188,64 +185,63 @@
 
         mean_ap = np.mean(all_ap_scores)
         mean_mrr = np.mean(all_mrr_scores)
 
         return {"map": mean_ap, "mrr": mean_mrr}
 
     def _compute_metrics_instance(self, query_emb, docs_emb, is_relevant):
-        """
-        Computes metrics for a single instance = (query, positives, negatives)
+        """Computes metrics for a single instance = (query, positives, negatives)
 
         Args:
             query_emb (`torch.Tensor` of shape `(num_queries, hidden_size)`): Query embedding
                 if `num_queries` > 0: we take the closest document to any of the queries
             docs_emb (`torch.Tensor` of shape `(num_pos+num_neg, hidden_size)`): Candidates documents embeddings
             is_relevant (`List[bool]` of length `num_pos+num_neg`): True if the document is relevant
 
         Returns:
             scores (`Dict[str, float]`):
                 - `mrr`: Mean Reciprocal Rank @ `self.mrr_at_k`
                 - `ap`: Average Precision
         """
-
         pred_scores = self.similarity_fct(query_emb, docs_emb)
         if len(pred_scores.shape) > 1:
             pred_scores = torch.amax(pred_scores, dim=0)
 
         pred_scores_argsort = torch.argsort(-pred_scores)  # Sort in decreasing order
 
         mrr = self.mrr_at_k_score(is_relevant, pred_scores_argsort, self.mrr_at_k)
         ap = self.ap_score(is_relevant, pred_scores.cpu().tolist())
         return {"mrr": mrr, "ap": ap}
 
     @staticmethod
-    def mrr_at_k_score(is_relevant, pred_ranking, k):
-        """
-        Computes MRR@k score
+    def mrr_at_k_score(
+        is_relevant: list[bool], pred_ranking: list[int], k: int
+    ) -> float:
+        """Computes MRR@k score
 
         Args:
-            is_relevant (`List[bool]` of length `num_pos+num_neg`): True if the document is relevant
-            pred_ranking (`List[int]` of length `num_pos+num_neg`): Indices of the documents sorted in decreasing order
+            is_relevant: True if the document is relevant
+            pred_ranking: Indices of the documents sorted in decreasing order
                 of the similarity score
+            k: Top-k documents to consider
 
         Returns:
-            mrr_score (`float`): MRR@k score
+            The MRR@k score
         """
         mrr_score = 0
         for rank, index in enumerate(pred_ranking[:k]):
             if is_relevant[index]:
                 mrr_score = 1 / (rank + 1)
                 break
 
         return mrr_score
 
     @staticmethod
     def ap_score(is_relevant, pred_scores):
-        """
-        Computes AP score
+        """Computes AP score
 
         Args:
             is_relevant (`List[bool]` of length `num_pos+num_neg`): True if the document is relevant
             pred_scores (`List[float]` of length `num_pos+num_neg`): Predicted similarity scores
 
         Returns:
             ap_score (`float`): AP score
```

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import heapq
 import logging
+from collections import defaultdict
 from typing import Dict, List, Tuple
 
 import pytrec_eval
 import torch
 from sentence_transformers import SentenceTransformer
 from sentence_transformers.models import Transformer, WordEmbeddings
 
@@ -27,14 +28,16 @@
         self.score_function_desc = {
             "cos_sim": "Cosine Similarity",
             "dot": "Dot Product",
         }
         self.corpus_chunk_size = corpus_chunk_size
         self.show_progress_bar = kwargs.get("show_progress_bar", True)
         self.convert_to_tensor = kwargs.get("convert_to_tensor", True)
+        self.save_corpus_embeddings = kwargs.get("save_corpus_embeddings", False)
+        self.corpus_embeddings = defaultdict(list)
         self.results = {}
 
     def search(
         self,
         corpus: dict[str, dict[str, str]],
         queries: dict[str, str],
         top_k: int,
@@ -57,14 +60,15 @@
         self.results = {qid: {} for qid in query_ids}
         queries = [queries[qid] for qid in queries]
         query_embeddings = self.model.encode_queries(
             queries,
             batch_size=self.batch_size,
             show_progress_bar=self.show_progress_bar,
             convert_to_tensor=self.convert_to_tensor,
+            **kwargs,
         )
 
         logger.info("Sorting Corpus by document length (Longest first)...")
 
         corpus_ids = sorted(
             corpus,
             key=lambda k: len(corpus[k].get("title", "") + corpus[k].get("text", "")),
@@ -85,31 +89,46 @@
             qid: [] for qid in query_ids
         }  # Keep only the top-k docs for each query
         for batch_num, corpus_start_idx in enumerate(itr):
             logger.info("Encoding Batch {}/{}...".format(batch_num + 1, len(itr)))
             corpus_end_idx = min(corpus_start_idx + self.corpus_chunk_size, len(corpus))
 
             # Encode chunk of corpus
-            sub_corpus_embeddings = self.model.encode_corpus(
-                corpus[corpus_start_idx:corpus_end_idx],
-                batch_size=self.batch_size,
-                show_progress_bar=self.show_progress_bar,
-                convert_to_tensor=self.convert_to_tensor,
-            )
+            if (
+                self.save_corpus_embeddings
+                and "qid" in kwargs
+                and len(self.corpus_embeddings[kwargs["qid"]])
+            ):
+                sub_corpus_embeddings = torch.tensor(
+                    self.corpus_embeddings[kwargs["qid"]][batch_num]
+                )
+            else:
+                # Encode chunk of corpus
+                sub_corpus_embeddings = self.model.encode_corpus(
+                    corpus[corpus_start_idx:corpus_end_idx],
+                    batch_size=self.batch_size,
+                    show_progress_bar=self.show_progress_bar,
+                    convert_to_tensor=self.convert_to_tensor,
+                )
+                if self.save_corpus_embeddings and "qid" in kwargs:
+                    self.corpus_embeddings[kwargs["qid"]].append(sub_corpus_embeddings)
 
             # Compute similarites using either cosine-similarity or dot product
             cos_scores = self.score_functions[score_function](
                 query_embeddings, sub_corpus_embeddings
             )
             cos_scores[torch.isnan(cos_scores)] = -1
 
             # Get top-k values
             cos_scores_top_k_values, cos_scores_top_k_idx = torch.topk(
                 cos_scores,
-                min(top_k + 1, len(cos_scores[1])),
+                min(
+                    top_k + 1,
+                    len(cos_scores[1]) if len(cos_scores) > 1 else len(cos_scores[-1]),
+                ),
                 dim=1,
                 largest=True,
                 sorted=return_sorted,
             )
             cos_scores_top_k_values = cos_scores_top_k_values.cpu().tolist()
             cos_scores_top_k_idx = cos_scores_top_k_idx.cpu().tolist()
 
@@ -133,52 +152,68 @@
             for score, corpus_id in result_heaps[qid]:
                 self.results[qid][corpus_id] = score
 
         return self.results
 
 
 class DRESModel:
-    """
-    Dense Retrieval Exact Search (DRES) requires an encode_queries & encode_corpus method.
+    """Dense Retrieval Exact Search (DRES) requires an encode_queries & encode_corpus method.
     This class converts a model with just an .encode method into DRES format.
     """
 
     def __init__(self, model, sep=" ", **kwargs):
         self.model = model
         self.sep = sep
         self.use_sbert_model = isinstance(model, SentenceTransformer)
+        self.save_corpus_embeddings = kwargs.get("save_corpus_embeddings", False)
+        self.corpus_embeddings = {}
 
     def encode_queries(self, queries: List[str], batch_size: int, **kwargs):
         if self.use_sbert_model:
             if isinstance(self.model._first_module(), Transformer):
                 logger.info(
                     f"Queries will be truncated to {self.model.get_max_seq_length()} tokens."
                 )
             elif isinstance(self.model._first_module(), WordEmbeddings):
                 logger.warning(
                     "Queries will not be truncated. This could lead to memory issues. In that case please lower the batch_size."
                 )
         return self.model.encode(queries, batch_size=batch_size, **kwargs)
 
     def encode_corpus(self, corpus: List[Dict[str, str]], batch_size: int, **kwargs):
+        if (
+            "qid" in kwargs
+            and self.save_corpus_embeddings
+            and len(self.corpus_embeddings) > 0
+        ):
+            return self.corpus_embeddings[kwargs["qid"]]
+
         if isinstance(corpus, dict):
             sentences = [
                 (corpus["title"][i] + self.sep + corpus["text"][i]).strip()
                 if "title" in corpus
                 else corpus["text"][i].strip()
                 for i in range(len(corpus["text"]))
             ]
         else:
             sentences = [
                 (doc["title"] + self.sep + doc["text"]).strip()
                 if "title" in doc
                 else doc["text"].strip()
                 for doc in corpus
             ]
-        return self.model.encode(sentences, batch_size=batch_size, **kwargs)
+
+        corpus_embeddings = self.model.encode(
+            sentences, batch_size=batch_size, **kwargs
+        )
+        if self.save_corpus_embeddings and "qid" in kwargs:
+            if type(corpus_embeddings) == torch.tensor:
+                corpus_embeddings = corpus_embeddings.cpu().detach()
+            self.corpus_embeddings[kwargs["qid"]] = corpus_embeddings
+        return corpus_embeddings
 
 
 def is_dres_compatible(model):
     for method in ["encode_queries", "encode_corpus"]:
         op = getattr(model, method, None)
         if not (callable(op)):
             return False
@@ -186,15 +221,15 @@
 
 
 # Adapted from https://github.com/beir-cellar/beir/blob/f062f038c4bfd19a8ca942a9910b1e0d218759d4/beir/retrieval/evaluation.py#L9
 class RetrievalEvaluator(Evaluator):
     def __init__(
         self,
         retriever=None,
-        k_values: List[int] = [1, 3, 5, 10, 100, 1000],
+        k_values: List[int] = [1, 3, 5, 10, 20, 100, 1000],
         score_function: str = "cos_sim",
         **kwargs,
     ):
         super().__init__(**kwargs)
         if is_dres_compatible(retriever):
             logger.info(
                 "The custom encode_queries and encode_corpus functions of the model will be used"
```

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.7.0/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/evaluation/evaluators/utils.py` & `mteb-1.7.0/mteb/evaluation/evaluators/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import logging
 from typing import Dict, List, Tuple
 
+import pandas as pd
 import torch
 
 
 def cos_sim(a, b):
-    """
-    Computes the cosine similarity cos_sim(a[i], b[j]) for all i and j.
-    :return: Matrix with res[i][j]  = cos_sim(a[i], b[j])
-    """
+    """Computes the cosine similarity cos_sim(a[i], b[j]) for all i and j.
+
+    Return:
+        Matrix with res[i][j]  = cos_sim(a[i], b[j])
+    """  # noqa: D402
     if not isinstance(a, torch.Tensor):
         a = torch.tensor(a)
 
     if not isinstance(b, torch.Tensor):
         b = torch.tensor(b)
 
     if len(a.shape) == 1:
@@ -25,16 +27,15 @@
 
     a_norm = torch.nn.functional.normalize(a, p=2, dim=1)
     b_norm = torch.nn.functional.normalize(b, p=2, dim=1)
     return torch.mm(a_norm, b_norm.transpose(0, 1))
 
 
 def dot_score(a: torch.Tensor, b: torch.Tensor):
-    """
-    Computes the dot-product dot_prod(a[i], b[j]) for all i and j.
+    """Computes the dot-product dot_prod(a[i], b[j]) for all i and j.
     :return: Matrix with res[i][j]  = dot_prod(a[i], b[j])
     """
     if not isinstance(a, torch.Tensor):
         a = torch.tensor(a)
 
     if not isinstance(b, torch.Tensor):
         b = torch.tensor(b)
@@ -185,7 +186,63 @@
                     break
 
     for k in k_values:
         top_k_acc[f"Accuracy@{k}"] = round(top_k_acc[f"Accuracy@{k}"] / len(qrels), 5)
         logging.info("Accuracy@{}: {:.4f}".format(k, top_k_acc[f"Accuracy@{k}"]))
 
     return top_k_acc
+
+
+def get_rank_from_dict(
+    dict_of_results: dict[str, float], doc_id: str
+) -> Tuple[int, float]:
+    tuple_of_id_score = dict_of_results.items()
+    sorted_by_score = sorted(tuple_of_id_score, key=lambda x: x[1], reverse=True)
+    for i, (id, score) in enumerate(sorted_by_score):
+        if id == doc_id:
+            return i + 1, score
+
+    return len(sorted_by_score) + 1, 0
+
+
+def evaluate_change(
+    original_run: dict[str, dict[str, float]],
+    new_run: dict[str, dict[str, float]],
+    changed_qrels: dict[str, List[str]],
+) -> dict[str, float]:
+    changes = []
+    for qid in changed_qrels.keys():
+        original_qid_run = original_run[qid]
+        new_qid_run = new_run[qid]
+        for idx, changed_doc in enumerate(changed_qrels[qid]):
+            original_rank, original_score = get_rank_from_dict(
+                original_qid_run, changed_doc
+            )
+            new_rank, new_score = get_rank_from_dict(new_qid_run, changed_doc)
+            change = int(original_rank - new_rank)
+            changes.append(
+                {
+                    "qid": qid,
+                    "doc_id": changed_doc,
+                    "change": change,
+                    "relevance": 0,
+                    "og_rank": original_rank,
+                    "new_rank": new_rank,
+                    "og_score": original_score,
+                    "new_score": new_score,
+                }
+            )
+
+    # we now have a DF of [qid, doc_id, change] to run our calculations with
+    changes_df = pd.DataFrame(changes)
+    changes_df["p-MRR"] = changes_df.apply(lambda x: rank_score(x), axis=1)
+    qid_wise = changes_df.groupby("qid").agg({"p-MRR": "mean"})
+    return {
+        "p-MRR": qid_wise["p-MRR"].mean(),
+    }
+
+
+def rank_score(x: dict[str, float]) -> float:
+    if x["og_rank"] >= x["new_rank"]:
+        return ((1 / x["og_rank"]) / (1 / x["new_rank"])) - 1
+    else:
+        return 1 - ((1 / x["new_rank"]) / (1 / x["og_rank"]))
```

### Comparing `mteb-1.6.9/mteb/logging.py` & `mteb-1.7.0/mteb/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,20 @@
 
 
 def _get_library_name() -> str:
     return __name__.split(".")[0]
 
 
 def _get_library_root_logger() -> logging.Logger:
-    """
-    Return the root logger of the library.
-    """
+    """Return the root logger of the library."""
     return logging.getLogger(_get_library_name())
 
 
 def enable_explicit_format() -> None:
-    """
-    Enable explicit formatting for every MTEB's logger. The explicit formatter is as follows:
+    """Enable explicit formatting for every MTEB's logger. The explicit formatter is as follows:
     ```
         [LEVELNAME|FILENAME|LINE NUMBER] TIME >> MESSAGE
     ```
     All handlers currently bound to the root logger are affected by this method.
     """
     handlers = _get_library_root_logger().handlers
```

### Comparing `mteb-1.6.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py` & `mteb-1.7.0/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.7.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.7.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,15 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
+        """Load dataset from HuggingFace hub and convert it to the standard format."""
         if self.data_loaded:
             return
 
         self.dataset = {}
 
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(**self.metadata_dict["dataset"])
```

### Comparing `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.7.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,17 +261,15 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples={"dev": 997, "devtest": 1012},
         avg_character_length={},
     )
 
     def load_data(self, **kwargs: Any) -> None:
-        """
-        Load dataset from HuggingFace hub
-        """
+        """Load dataset from HuggingFace hub"""
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
                 name=lang,
                 **self.metadata_dict["dataset"],
```

### Comparing `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.7.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.7.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py` & `mteb-1.7.0/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py` & `mteb-1.7.0/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/__init__.py` & `mteb-1.7.0/mteb/tasks/Classification/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,61 @@
 from __future__ import annotations
 
+from .ara.HotelReviewSentimentClassification import *
+from .ara.RestaurantReviewSentimentClassification import *
+from .ara.TweetEmotionClassification import *
+from .ara.TweetSarcasmClassification import *
+from .bam.BambaraSentimentClassification import *
+from .ben.BengaliHateSpeechClassification import *
+from .bul.BulgarianSentimentClassification import *
+from .bul.BulgarianStoreReviewSentimentClassfication import *
+from .ces.CzechSubjectivityClassification import *
 from .dan.AngryTweetsClassification import *
 from .dan.DalajClassification import *
 from .dan.DanishPoliticalCommentsClassification import *
 from .dan.DKHateClassification import *
 from .dan.LccSentimentClassification import *
+from .ell.GreekSentimentClassification import *
 from .eng.AmazonPolarityClassification import *
 from .eng.Banking77Classification import *
 from .eng.EmotionClassification import *
 from .eng.ImdbClassification import *
 from .eng.NewsClassification import *
 from .eng.ToxicConversationsClassification import *
 from .eng.TweetSentimentExtractionClassification import *
+from .est.estonian_valence import *
+from .fas.PersianFoodSentimentClassification import *
+from .fra.MovieReviewSentimentClassification import *
 from .hin.HindiDiscourseClassification import *
+from .hrv.CroatianSentimentClassification import *
+from .ind.IndonesianIdClickbaitClassification import *
+from .ita.ItaHateClassification import *
+from .ita.ItalianLinguistAcceptabilityClassification import *
 from .jpn.WRIMEClassification import *
+from .kur.KurdishSentimentClassification import *
+from .mkd.MacedonianTweetSentimentClassification import *
+from .mlt.MalteseSentimentClassification import *
 from .multilingual.AmazonCounterfactualClassification import *
 from .multilingual.AmazonReviewsClassification import *
 from .multilingual.MasakhaNEWSClassification import *
 from .multilingual.MassiveIntentClassification import *
 from .multilingual.MassiveScenarioClassification import *
 from .multilingual.MTOPDomainClassification import *
 from .multilingual.MTOPIntentClassification import *
 from .multilingual.NordicLangClassification import *
 from .multilingual.ScalaClassification import *
+from .nld.DutchBookReviewSentimentClassification import *
 from .nob.NoRecClassification import *
 from .nob.NorwegianParliamentClassification import *
 from .pol.PolishClassification import *
+from .ron.RomanianSentimentClassification import *
+from .slk.SlovakSentimentClassification import *
 from .swe.SweRecClassification import *
+from .tur.TurkishMovieSentimentClassification import *
+from .tur.TurkishProductSentimentClassification import *
+from .uig.UyghurSentimentClassification import *
 from .vie.VieStudentFeedbackClassification import *
 from .zho.CMTEBClassification import *
-from .zho.YueOpenriceReviewClassification import YueOpenriceReviewClassification  # noqa: F401
+from .zho.YueOpenriceReviewClassification import (
+    YueOpenriceReviewClassification,  # noqa: F401
+)
+from .zul.IsiZuluNewsClassification import *
```

### Comparing `mteb-1.6.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/dan/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/dan/DKHateClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/dan/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/dan/DalajClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/dan/DalajClassification.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
         return metadata_dict
 
     def dataset_transform(self):
-        """
-        This dataset consist of two columns of relevance, "original_sentence" and "corrected_sentence".
+        """This dataset consist of two columns of relevance, "original_sentence" and "corrected_sentence".
         We will use the original sentence as we "wrong" sentence and the corrected sentence as the "correct" sentence
         """
 
         def __convert_sample_to_classification(sample):
             text = sample["original_sentence"] + sample["corrected_sentence"]
             label = [1] * len(sample["original_sentence"]) + [0] * len(
                 sample["corrected_sentence"]
```

### Comparing `mteb-1.6.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/dan/LccSentimentClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/dan/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/eng/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/eng/Banking77Classification.py` & `mteb-1.7.0/mteb/tasks/Classification/eng/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/eng/EmotionClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/eng/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/eng/ImdbClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/eng/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/eng/NewsClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/eng/NewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/eng/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/hin/HindiDiscourseClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/jpn/WRIMEClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/jpn/WRIMEClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/nob/NoRecClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/nob/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/pol/PolishClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/pol/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/swe/SweRecClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/swe/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/zho/CMTEBClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/zho/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py` & `mteb-1.7.0/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/__init__.py` & `mteb-1.7.0/mteb/tasks/Clustering/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 from .fra.MLSUMClusteringP2P import *
 from .fra.MLSUMClusteringS2S import *
 from .multilingual.MasakhaNEWSClusteringP2P import *
 from .multilingual.MasakhaNEWSClusteringS2S import *
 from .nob.snl_clustering import *
 from .nob.vg_clustering import *
 from .pol.PolishClustering import *
+from .rom.RomaniBibleClustering import *
 from .spa.FloresClusteringS2S import *
 from .spa.SpanishNewsClusteringP2P import *
 from .swe.swedn_clustering import *
 from .zho.CMTEBClustering import *
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/BigPatentClustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/RedditClustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/eng/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,15 @@
     )
 
     def create_description(self, example):
         example["text"] = example["title"] + " " + example["text"]
         return example
 
     def dataset_transform(self):
-        """
-        Convert to standard format
-        """
+        """Convert to standard format"""
         self.dataset = self.dataset.remove_columns("uuid")
         self.dataset = self.dataset.map(self.create_description)
         texts = self.dataset["documents"]["text"]
         topics = self.dataset["documents"]["topic"]
         new_format = {
             "sentences": [split.tolist() for split in np.array_split(texts, 10)],
             "labels": [split.tolist() for split in np.array_split(topics, 10)],
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,15 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def dataset_transform(self):
-        """
-        Convert to standard format
-        """
+        """Convert to standard format"""
         self.dataset = self.dataset.remove_columns("uuid")
         self.dataset = self.dataset.remove_columns("text")
         titles = self.dataset["documents"]["title"]
         topics = self.dataset["documents"]["topic"]
         new_format = {
             "sentences": [split.tolist() for split in np.array_split(titles, 10)],
             "labels": [split.tolist() for split in np.array_split(topics, 10)],
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/fra/HALClusteringS2S.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,15 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def dataset_transform(self):
-        """
-        Convert to standard format
-        """
+        """Convert to standard format"""
         self.dataset = self.dataset.remove_columns("hal_id")
         titles = self.dataset["test"]["title"]
         domains = self.dataset["test"]["domain"]
         new_format = {
             "sentences": [split.tolist() for split in np.array_split(titles, 10)],
             "labels": [split.tolist() for split in np.array_split(domains, 10)],
         }
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,22 +34,33 @@
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
+    def load_data(self, **kwargs):
+        """Load dataset from HuggingFace hub and convert it to the standard format."""
+        if self.data_loaded:
+            return
+        self.dataset = datasets.load_dataset(
+            self.metadata.dataset["path"],
+            self.metadata.dataset["name"],
+            split=self.metadata.eval_splits[0],
+            revision=self.metadata.dataset["revision"],
+        )
+        self.dataset_transform()
+        self.data_loaded = True
+
     def create_description(self, example):
         example["text"] = example["title"] + " " + example["text"]
         return example
 
     def dataset_transform(self):
-        """
-        Convert to standard format
-        """
+        """Convert to standard format"""
         self.dataset = self.dataset.map(self.create_description)
         self.dataset = self.dataset.remove_columns(["summary", "url", "date", "title"])
         texts = self.dataset["text"]
         topics = self.dataset["topic"]
         new_format = {
             "sentences": [split.tolist() for split in np.array_split(texts, 10)],
             "labels": [split.tolist() for split in np.array_split(topics, 10)],
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,18 +34,29 @@
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
+    def load_data(self, **kwargs):
+        """Load dataset from HuggingFace hub and convert it to the standard format."""
+        if self.data_loaded:
+            return
+        self.dataset = datasets.load_dataset(
+            self.metadata.dataset["path"],
+            self.metadata.dataset["name"],
+            split=self.metadata.eval_splits[0],
+            revision=self.metadata.dataset["revision"],
+        )
+        self.dataset_transform()
+        self.data_loaded = True
+
     def dataset_transform(self):
-        """
-        Convert to standard format
-        """
+        """Convert to standard format"""
         self.dataset = self.dataset.remove_columns(["summary", "text", "url", "date"])
         new_format = {
             "sentences": [
                 split.tolist() for split in np.array_split(self.dataset["title"], 10)
             ],
             "labels": [
                 split.tolist() for split in np.array_split(self.dataset["topic"], 10)
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,32 +52,28 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
+        """Load dataset from HuggingFace hub and convert it to the standard format."""
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
                 name=lang,
                 **self.metadata_dict["dataset"],
             )
             self.dataset_transform(lang)
         self.data_loaded = True
 
     def dataset_transform(self, lang):
-        """
-        Convert to standard format
-        """
+        """Convert to standard format"""
         self.dataset[lang].pop("train")
         self.dataset[lang].pop("validation")
 
         self.dataset[lang] = self.dataset[lang].remove_columns(
             ["url", "text", "headline"]
         )
         texts = self.dataset[lang]["test"]["headline_text"]
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,32 +54,28 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
+        """Load dataset from HuggingFace hub and convert it to the standard format."""
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
                 name=lang,
                 **self.metadata_dict["dataset"],
             )
             self.dataset_transform(lang)
         self.data_loaded = True
 
     def dataset_transform(self, lang):
-        """
-        Convert to standard format
-        """
+        """Convert to standard format"""
         self.dataset[lang].pop("train")
         self.dataset[lang].pop("validation")
 
         self.dataset[lang] = self.dataset[lang].remove_columns(
             ["url", "text", "headline_text"]
         )
         texts = self.dataset[lang]["test"]["headline"]
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/nob/snl_clustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/nob/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/nob/vg_clustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/nob/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/pol/PolishClustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/pol/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py` & `mteb-1.7.0/mteb/tasks/Clustering/spa/FloresClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py` & `mteb-1.7.0/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/swe/swedn_clustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/swe/swedn_clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,15 @@
   year={2021}
 }""",
         n_samples={"all": 2048},
         avg_character_length={"all": 1619.71},
     )
 
     def dataset_transform(self):
-        """
-        The article_category clusters differ between the splits (with the test set only having 1 cluster). Therefore we combine it all into one
+        """The article_category clusters differ between the splits (with the test set only having 1 cluster). Therefore we combine it all into one
         cluster.
         """
         splits = ["train", "validation"]
         # performance of sample models with test set: 8.74, 2.43 -removing test-> 11.26, 4.27
         # this is due to the test set only having 1 cluster which is "other"
 
         headlines = []
```

### Comparing `mteb-1.6.9/mteb/tasks/Clustering/zho/CMTEBClustering.py` & `mteb-1.7.0/mteb/tasks/Clustering/zho/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py` & `mteb-1.7.0/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py` & `mteb-1.7.0/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py` & `mteb-1.7.0/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py` & `mteb-1.7.0/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.7.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
+        """Load dataset from HuggingFace hub"""
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
                 lang=lang,
                 quality=100,
```

### Comparing `mteb-1.6.9/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.7.0/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/PairClassification/pol/PolishPC.py` & `mteb-1.7.0/mteb/tasks/PairClassification/pol/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py` & `mteb-1.7.0/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py` & `mteb-1.7.0/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Reranking/eng/MindSmallReranking.py` & `mteb-1.7.0/mteb/tasks/Reranking/eng/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Reranking/eng/SciDocsReranking.py` & `mteb-1.7.0/mteb/tasks/Reranking/eng/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py` & `mteb-1.7.0/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Reranking/fra/AlloprofReranking.py` & `mteb-1.7.0/mteb/tasks/Reranking/fra/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Reranking/fra/SyntecReranking.py` & `mteb-1.7.0/mteb/tasks/Reranking/fra/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.7.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Reranking/zho/CMTEBReranking.py` & `mteb-1.7.0/mteb/tasks/Reranking/zho/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/__init__.py` & `mteb-1.7.0/mteb/tasks/Retrieval/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,34 +29,44 @@
 from .eng.FEVERRetrieval import *
 from .eng.FiQA2018Retrieval import *
 from .eng.HagridRetrieval import *
 from .eng.HotpotQARetrieval import *
 from .eng.LegalBenchConsumerContractsQARetrieval import *
 from .eng.LegalBenchCorporateLobbyingRetrieval import *
 from .eng.LegalSummarizationRetrieval import *
+from .eng.LEMBNarrativeQARetrieval import *
+from .eng.LEMBNeedleRetrieval import *
+from .eng.LEMBPasskeyRetrieval import *
+from .eng.LEMBQMSumRetrieval import *
+from .eng.LEMBSummScreenFDRetrieval import *
+from .eng.LEMBWikimQARetrieval import *
 from .eng.MedicalQARetrieval import *
 from .eng.MSMARCORetrieval import *
 from .eng.MSMARCOv2Retrieval import *
 from .eng.NarrativeQARetrieval import *
 from .eng.NFCorpusRetrieval import *
 from .eng.NQRetrieval import *
 from .eng.QuoraRetrieval import *
 from .eng.SCIDOCSRetrieval import *
 from .eng.SciFactRetrieval import *
 from .eng.Touche2020Retrieval import *
 from .eng.TRECCOVIDRetrieval import *
+from .est.estqa import *
 from .fra.AlloprofRetrieval import *
 from .fra.BSARDRetrieval import *
 from .fra.SyntecRetrieval import *
+from .hun.HunSum2 import *
 from .jpn.JaQuADRetrieval import *
 from .kor.KoMiracl import *
 from .kor.KoStrategyQA import *
 from .multilingual.MintakaRetrieval import *
 from .multilingual.MIRACLRetrieval import *
 from .multilingual.MultiLongDocRetrieval import *
+from .multilingual.NeuCLIR2022Retrieval import *
+from .multilingual.NeuCLIR2023Retrieval import *
 from .multilingual.XMarketRetrieval import *
 from .multilingual.XPQARetrieval import *
 from .nob.norquad import *
 from .nob.snl_retrieval import *
 from .pol.ArguAnaPLRetrieval import *
 from .pol.DBPediaPLRetrieval import *
 from .pol.FiQAPLRetrieval import *
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/dan/dan_fever.py` & `mteb-1.7.0/mteb/tasks/Retrieval/dan/dan_fever.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,15 @@
 """,
         n_samples={"train": 8897},
         avg_character_length={"train": 124.84},
         task_subtypes=["Claim verification"],
     )
 
     def dataset_transform(self) -> None:
-        """
-        and transform to a retrieval datset, which have the following attributes
+        """And transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document data like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
         """
         self.corpus = {}
         self.relevant_docs = {}
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/dan/t2nord_retrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,15 @@
         bibtex_citation=None,
         n_samples={"test": 4096},
         avg_character_length={"test": 784.11},
         task_subtypes=["Article retrieval"],
     )
 
     def dataset_transform(self) -> None:
-        """
-        and transform to a retrieval datset, which have the following attributes
+        """And transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
         """
         self.corpus = {}
         self.relevant_docs = {}
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/dan/twitterhjerne.py` & `mteb-1.7.0/mteb/tasks/Retrieval/dan/twitterhjerne.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 """,
         n_samples={"train": 340},
         avg_character_length={"train": 138.23},
         task_subtypes=["Question answering"],
     )
 
     def dataset_transform(self) -> None:
-        """
-        and transform to a retrieval datset, which have the following attributes
+        """And transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
         """
         self.corpus = {}
         self.relevant_docs = {}
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 class GermanDPR(AbsTaskRetrieval):
     _EVAL_SPLIT = "test"
 
     metadata = TaskMetadata(
         name="GermanDPR",
         description="GermanDPR is a German Question Answering dataset for open-domain QA. It associates questions with a textual context containing the answer",
-        reference="https://www.deepset.ai/germanquad",
+        reference="https://huggingface.co/datasets/deepset/germandpr",
         dataset={
-            "path": "deepset/germanquad",
-            "revision": "fff05ceaf2ffbe5b65c7e0c57e678f7b7e1a0581",
+            "path": "deepset/germandpr",
+            "revision": "5129d02422a66be600ac89cd3e8531b4f97d347d",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=["deu-Latn"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/HagridRetrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,15 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """
-        Loads the different split of the dataset (queries/corpus/relevants)
-        """
+        """Loads the different split of the dataset (queries/corpus/relevants)"""
         if self.data_loaded:
             return
 
         data = datasets.load_dataset(
             "miracl/hagrid",
             split=self.metadata.eval_splits[0],
             revision=self.metadata_dict["dataset"].get("revision", None),
@@ -71,22 +69,20 @@
                 d["query_id"]: {d["answer_id"]: 1} for d in proc_data
             }
         }
 
         self.data_loaded = True
 
     def preprocess_data(self, dataset: Dict) -> List[Dict]:
-        """
-        Preprocessed the data in a format easirer
+        """Preprocessed the data in a format easirer
         to handle for the loading of queries and corpus
         ------
         PARAMS
         dataset : the hagrid dataset (json)
         """
-
         preprocessed_data = []
         for d in dataset:
             # get the best answer among positively rated answers
             best_answer = self.get_best_answer(d)
             # if no good answer found, skip
             if best_answer is not None:
                 preprocessed_data.append(
@@ -97,16 +93,15 @@
                         "answer_text": best_answer,
                     }
                 )
 
         return preprocessed_data
 
     def get_best_answer(self, data: Dict) -> str:
-        """
-        Get the best answer among available answers
+        """Get the best answer among available answers
         of a query.
         WARNING : May return None if no good answer available
         --------
         PARAMS:
         data: a dict representing one element of the dataset
         """
         good_answers = [
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/NQRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class AlloprofRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="AlloprofRetrieval",
         description="This dataset was provided by AlloProf, an organisation in Quebec, Canada offering resources and a help forum curated by a large number of teachers to students on all subjects taught from in primary and secondary school",
         reference="https://huggingface.co/datasets/antoinelb7/alloprof",
         dataset={
             "path": "lyon-nlp/alloprof",
-            "revision": "2df7bee4080bedf2e97de3da6bd5c7bc9fc9c4d2",
+            "revision": "fcf295ea64c750f41fadbaa37b9b861558e1bfbd",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["fra-Latn"],
         main_score="ndcg_at_10",
         date=None,
@@ -49,15 +49,15 @@
         )
         eval_split = self.metadata_dict["eval_splits"][0]
         self.queries = {
             eval_split: {str(q["id"]): q["text"] for q in queries_raw[eval_split]}
         }
         self.corpus = {
             eval_split: {
-                str(d["uuid"]): {"text": d["text"]} for d in corpus_raw["documents"]
+                str(d["uuid"]): {"text": d["text"]} for d in corpus_raw[eval_split]
             }
         }
 
         self.relevant_docs = {eval_split: {}}
         for q in queries_raw[eval_split]:
             for r in q["relevant"]:
                 self.relevant_docs[eval_split][str(q["id"])] = {r: 1}
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/fra/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/fra/SyntecRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 
     metadata = TaskMetadata(
         name="SyntecRetrieval",
         description="This dataset has been built from the Syntec Collective bargaining agreement.",
         reference="https://huggingface.co/datasets/lyon-nlp/mteb-fr-retrieval-syntec-s2p",
         dataset={
             "path": "lyon-nlp/mteb-fr-retrieval-syntec-s2p",
-            "revision": "aa460cd4d177e6a3c04fcd2affd95e8243289033",
+            "revision": "19661ccdca4dfc2d15122d776b61685f48c68ca9",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=_EVAL_SPLITS,
         eval_langs=["fra-Latn"],
         main_score="map",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
-        dialect=None,
+        dialect=[],
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 90},
+        avg_character_length={"test": 62},
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
         # fetch both subsets of the dataset
         corpus_raw = datasets.load_dataset(
@@ -46,27 +46,26 @@
             **self.metadata_dict["dataset"],
         )
         queries_raw = datasets.load_dataset(
             name="queries",
             **self.metadata_dict["dataset"],
         )
 
+        eval_split = self.metadata_dict["eval_splits"][0]
         self.queries = {
-            self._EVAL_SPLITS[0]: {
-                str(i): q["Question"] for i, q in enumerate(queries_raw["queries"])
+            eval_split: {
+                str(i): q["Question"] for i, q in enumerate(queries_raw[eval_split])
             }
         }
 
-        corpus_raw = corpus_raw["documents"]
+        corpus_raw = corpus_raw[eval_split]
         corpus_raw = corpus_raw.rename_column("content", "text")
-        self.corpus = {
-            self._EVAL_SPLITS[0]: {str(row["id"]): row for row in corpus_raw}
-        }
+        self.corpus = {eval_split: {str(row["id"]): row for row in corpus_raw}}
 
         self.relevant_docs = {
-            self._EVAL_SPLITS[0]: {
+            eval_split: {
                 str(i): {str(q["Article"]): 1}
-                for i, q in enumerate(queries_raw["queries"])
+                for i, q in enumerate(queries_raw[eval_split])
             }
         }
 
         self.data_loaded = True
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/kor/KoMiracl.py` & `mteb-1.7.0/mteb/tasks/Retrieval/kor/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py` & `mteb-1.7.0/mteb/tasks/Retrieval/kor/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/nob/norquad.py` & `mteb-1.7.0/mteb/tasks/Retrieval/nob/norquad.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     abstract = "In this paper we present NorQuAD: the first Norwegian question answering dataset for machine reading comprehension. The dataset consists of 4,752 manually created question-answer pairs. We here detail the data collection procedure and present statistics of the dataset. We also benchmark several multilingual and Norwegian monolingual language models on the dataset and compare them against human performance. The dataset will be made freely available.",
 }""",
         n_samples={"test": 2602},
         avg_character_length={"test": 502.19},
     )
 
     def dataset_transform(self) -> None:
-        """
-        and transform to a retrieval datset, which have the following attributes
+        """And transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
         """
         self.corpus = {}
         self.relevant_docs = {}
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/nob/snl_retrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/nob/snl_retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 }""",
         n_samples={"test": 2048},
         avg_character_length={"test": 1101.30},
         task_subtypes=["Article retrieval"],
     )
 
     def dataset_transform(self) -> None:
-        """
-        and transform to a retrieval datset, which have the following attributes
+        """And transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
         """
         self.corpus = {}
         self.relevant_docs = {}
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/NQPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py` & `mteb-1.7.0/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py` & `mteb-1.7.0/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/swe/swedn_retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     year={2021}
 }""",
         n_samples={"test": 2048},
         avg_character_length={"test": 1946.35},
     )
 
     def dataset_transform(self) -> None:
-        """
-        and transform to a retrieval datset, which have the following attributes
+        """And transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
         """
         self.corpus = {}
         self.relevant_docs = {}
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/swe/swefaq_retrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,15 @@
         text_creation="found",
         bibtex_citation=None,
         n_samples={"test": 1024},
         avg_character_length={"test": 195.44},
     )
 
     def dataset_transform(self) -> None:
-        """
-        and transform to a retrieval datset, which have the following attributes
+        """And transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
         """
         self.corpus = {}
         self.relevant_docs = {}
```

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py` & `mteb-1.7.0/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py` & `mteb-1.7.0/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/eng/BiossesSTS.py` & `mteb-1.7.0/mteb/tasks/STS/eng/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/eng/STS12STS.py` & `mteb-1.7.0/mteb/tasks/STS/eng/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/eng/STS13STS.py` & `mteb-1.7.0/mteb/tasks/STS/eng/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/eng/STS14STS.py` & `mteb-1.7.0/mteb/tasks/STS/eng/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/eng/STS15STS.py` & `mteb-1.7.0/mteb/tasks/STS/eng/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/eng/STS16STS.py` & `mteb-1.7.0/mteb/tasks/STS/eng/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py` & `mteb-1.7.0/mteb/tasks/STS/eng/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/eng/SickrSTS.py` & `mteb-1.7.0/mteb/tasks/STS/eng/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/fra/SickFrSTS.py` & `mteb-1.7.0/mteb/tasks/STS/fra/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.7.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.7.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.7.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/pol/PolishSTS.py` & `mteb-1.7.0/mteb/tasks/STS/pol/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/spa/STSES.py` & `mteb-1.7.0/mteb/tasks/STS/spa/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/STS/zho/CMTEBSTS.py` & `mteb-1.7.0/mteb/tasks/STS/zho/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py` & `mteb-1.7.0/mteb/tasks/Summarization/eng/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py` & `mteb-1.7.0/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/mteb.egg-info/PKG-INFO` & `mteb-1.7.0/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.6.9
+Version: 1.7.0
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -226,15 +226,15 @@
 Requires-Dist: scikit_learn>=1.0.2
 Requires-Dist: scipy
 Requires-Dist: sentence_transformers>=2.2.0
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: rich
 Requires-Dist: pytrec-eval-terrier>=0.5.6
-Requires-Dist: pydantic
+Requires-Dist: pydantic>=2.0.0
 Requires-Dist: typing_extensions
 Requires-Dist: eval_type_backport
 Provides-Extra: dev
 Requires-Dist: ruff>=0.0.254; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
@@ -448,15 +448,15 @@
 | 📈 [Leaderboard] | The interactive leaderboard of the benchmark |
 | 🤖 [Adding a model] | Information related to how to submit a model to the leaderboard |
 | 👩‍💻 [Adding a dataset] | How to add a new task/dataset to MTEB | 
 | 🤝  [Contributing] | How to contribute to MTEB and set it up for development |
 <!-- | 🌐 [MMTEB] | An open-source effort to extend MTEB to cover a broad set of languages |   -->
 
 [Tasks]: docs/tasks.md
-[Contributing]: contributing.md
+[Contributing]: CONTRIBUTING.md
 [Adding a model]: docs/adding_a_model.md
 [Adding a dataset]: docs/adding_a_dataset.md
 [Leaderboard]: https://huggingface.co/spaces/mteb/leaderboard
 [MMTEB]: docs/mmteb/readme.md
 
 ## Citing
```

### Comparing `mteb-1.6.9/pyproject.toml` & `mteb-1.7.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.6.9"
+version = "1.7.0"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
@@ -32,15 +32,15 @@
     "scikit_learn>=1.0.2",
     "scipy",
     "sentence_transformers>=2.2.0",
     "torch",
     "tqdm",
     "rich",
     "pytrec-eval-terrier>=0.5.6",
-    "pydantic",
+    "pydantic>=2.0.0",
     "typing_extensions",
     "eval_type_backport",
 ]
 
 
 [project.urls]
 homepage = "https://github.com/embeddings-benchmark/mteb"
@@ -60,16 +60,27 @@
 [tool.setuptools.package-data]
 "*" = ["*.json"]
 
 [tool.ruff]
 target-version = "py38"
 
 [tool.ruff.lint]
-select = ["E4", "E7", "E9", "F", "I"]
-ignore = ["E203", "E501", "E741", "F403"]
+select = ["F", "I", "E", "D"]
+ignore = ["E501",   # line too long 
+        "E741",     # ambiguous variable name
+        "F403",     # undefined import
+        "D100",     # Missing docstring in public module
+        "D101",     # Missing docstring in public class
+        "D102",     # Missing docstring in public method
+        "D103",     # Missing docstring in public function
+        "D104",     # Missing docstring in public package
+        "D107",     # Missing docstring in __init__
+        "D205",     # 1 blank line required between summary line and description
+        "D415",     # First line should end with a period
+]
 ignore-init-module-imports = true
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.flake8-annotations]
 mypy-init-return = true
```

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/DanFEVER.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json` & `mteb-1.7.0/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json` & `mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json` & `mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json` & `mteb-1.7.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/amazon_polarity/create_data.py` & `mteb-1.7.0/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.7.0/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/arxiv/script_clustering.py` & `mteb-1.7.0/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/arxiv/script_raw.py` & `mteb-1.7.0/scripts/data/arxiv/script_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Take data from https://www.kaggle.com/datasets/Cornell-University/arxiv?resource=download and
+"""Take data from https://www.kaggle.com/datasets/Cornell-University/arxiv?resource=download and
 only keep useful information
 """
 
 from __future__ import annotations
 
 import gzip
 import json
```

### Comparing `mteb-1.6.9/scripts/data/biorxiv/script_clustering.py` & `mteb-1.7.0/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/biorxiv/script_raw.py` & `mteb-1.7.0/scripts/data/biorxiv/script_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Fetch data from https://api.biorxiv.org/ and keep useful information
-"""
+"""Fetch data from https://api.biorxiv.org/ and keep useful information"""
 
 from __future__ import annotations
 
 import gzip
 
 import jsonlines
 import requests
```

### Comparing `mteb-1.6.9/scripts/data/bucc/create_data.py` & `mteb-1.7.0/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/create_task_table.py` & `mteb-1.7.0/scripts/data/create_task_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 }
 
 
 DATAPATH = "/gpfsscratch/rech/six/commun/commun/experiments/muennighoff/mteb"
 
 
 def load_data(hf_hub_name, subset=None):
-    """
-    Load dataset from Hub via cloning for easy offline usage with HF_DATASETS_OFFLINE=1
+    """Load dataset from Hub via cloning for easy offline usage with HF_DATASETS_OFFLINE=1
     Can be replaced with just `load_dataset(hf_hub_name, subset)` if preferred
     """
     from datasets import load_dataset
 
     path = os.path.join(DATAPATH, hf_hub_name)
     if os.path.exists(path):
         dataset = load_dataset(path, subset)
```

### Comparing `mteb-1.6.9/scripts/data/germanquad/process_data.py` & `mteb-1.7.0/scripts/data/germanquad/process_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """See clarin-knext/arguana-pl, clarin-knext/arguana-pl-qrels and
-beir.datasets.data_loader_hf.HFDataLoader for BEIR format."""
+beir.datasets.data_loader_hf.HFDataLoader for BEIR format.
+"""
 
 from __future__ import annotations
 
 from datasets import Dataset, DatasetDict, Features, Value, load_dataset
 
 dataset = load_dataset("deepset/germanquad")
 dataset.pop("train")
```

### Comparing `mteb-1.6.9/scripts/data/hal/create_data.py` & `mteb-1.7.0/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/imdb/create_data.py` & `mteb-1.7.0/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/medicalqaretrieval/create_data.py` & `mteb-1.7.0/scripts/data/medicalqaretrieval/create_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from typing import Dict
 
 from datasets import load_dataset
 from huggingface_hub import create_repo, upload_file
 
 
 def preprocess_data(example: Dict) -> Dict:
-    """
-    Preprocessed the data in a format easier
+    """Preprocessed the data in a format easier
     to handle for the loading of queries and corpus
     ------
     PARAMS
     example : element in med-qa dataset
     """
     return {
         "query-id": str(uuid.uuid4()),
```

### Comparing `mteb-1.6.9/scripts/data/medrxiv/script_clustering.py` & `mteb-1.7.0/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/medrxiv/script_raw.py` & `mteb-1.7.0/scripts/data/medrxiv/script_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Fetch data from https://api.biorxiv.org/ and keep useful information
-"""
+"""Fetch data from https://api.biorxiv.org/ and keep useful information"""
 
 from __future__ import annotations
 
 import gzip
 
 import jsonlines
 import requests
```

### Comparing `mteb-1.6.9/scripts/data/mind/prepare_data.py` & `mteb-1.7.0/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/redditp2p/script_clustering.py` & `mteb-1.7.0/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.7.0/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.7.0/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Preparation (Scraping the data):
+"""Preparation (Scraping the data):
 pip install semeval_8_2022_ia_downloader
 python3 -m semeval_8_2022_ia_downloader.cli --links_file=semeval-2022_task8_train-data_batch.csv --dump_dir=train
 
 wget https://competitions.codalab.org/my/datasets/download/6798bbee-77fa-452d-bde2-96b8631acb5d
 mv 6798bbee-77fa-452d-bde2-96b8631acb5d final_evaluation_data.csv
 python3 -m semeval_8_2022_ia_downloader.cli --links_file=final_evaluation_data.csv --dump_dir=test
 """
```

### Comparing `mteb-1.6.9/scripts/data/summeval_fr/create_data.py` & `mteb-1.7.0/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.7.0/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/merge_cqadupstack.py` & `mteb-1.7.0/scripts/merge_cqadupstack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Merges CQADupstack subset results
+"""Merges CQADupstack subset results
 Usage: python merge_cqadupstack.py path_to_results_folder
 """
 
 from __future__ import annotations
 
 import glob
 import json
```

### Comparing `mteb-1.6.9/scripts/mteb_meta.py` & `mteb-1.7.0/scripts/mteb_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Usage: python mteb_meta.py path_to_results_folder
+"""Usage: python mteb_meta.py path_to_results_folder
 
 Creates evaluation results metadata for the model card.
 E.g.
 ---
 tags:
 - mteb
 model-index:
```

### Comparing `mteb-1.6.9/scripts/run_mteb_chinese.py` & `mteb-1.7.0/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/run_mteb_english.py` & `mteb-1.7.0/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/run_mteb_french.py` & `mteb-1.7.0/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/run_mteb_german.py` & `mteb-1.7.0/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/run_mteb_korean.py` & `mteb-1.7.0/scripts/run_mteb_korean.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 TASK_LIST_PAIR_CLASSIFICATION = []
 
 TASK_LIST_RERANKING = []
 
 TASK_LIST_RETRIEVAL = ["Ko-StrategyQA", "Ko-miracl"]
 
-TASK_LIST_STS = []
+TASK_LIST_STS = ["KLUE-STS", "KorSTS"]
 
 TASK_LIST = (
     TASK_LIST_CLASSIFICATION
     + TASK_LIST_CLUSTERING
     + TASK_LIST_PAIR_CLASSIFICATION
     + TASK_LIST_RERANKING
     + TASK_LIST_RETRIEVAL
```

### Comparing `mteb-1.6.9/scripts/run_mteb_law.py` & `mteb-1.7.0/scripts/run_mteb_law.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/scripts/run_mteb_polish.py` & `mteb-1.7.0/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/tests/test_ClusteringEvaluator.py` & `mteb-1.7.0/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/tests/test_PairClassificationEvaluator.py` & `mteb-1.7.0/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/tests/test_RerankingEvaluator.py` & `mteb-1.7.0/tests/test_RerankingEvaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from mteb.evaluation.evaluators import RerankingEvaluator
 
 TOL = 0.0001
 
 
 class TestRerankingEvaluator:
     def setup_method(self):
-        """setup any state tied to the execution of the given method in a
-        class.  setup_method is invoked for every test method of a class.
-        """
+        """Setup any state tied to the execution of the given method in a class.
 
+        setup_method is invoked for every test method of a class.
+        """
         self.evaluator = RerankingEvaluator([])
 
     def test_mrr_at_k(self):
         is_relevant = [1, 1, 1, 0, 0, 0, 0, 0, 0]
         pred_ranking = [5, 2, 6, 1, 3, 4, 7, 8, 9]
 
         assert self.evaluator.mrr_at_k_score(
```

### Comparing `mteb-1.6.9/tests/test_RetrievalEvaluator.py` & `mteb-1.7.0/tests/test_RetrievalEvaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from mteb.evaluation.evaluators import RetrievalEvaluator
 
 TOL = 0.0001
 
 
 class TestRetrievalEvaluator:
     def setup_method(self):
-        """setup any state tied to the execution of the given method in a
-        class.  setup_method is invoked for every test method of a class.
-        """
+        """Setup any state tied to the execution of the given method in a class.
 
+        setup_method is invoked for every test method of a class.
+        """
         self.evaluator = RetrievalEvaluator()
 
     def test_metrics_at_k(self):
         # Qid: {Docid: Relevance}
         relevant_docs = {
             "0": {"0": 1, "1": 1},
             "1": {"1": 1},
```

### Comparing `mteb-1.6.9/tests/test_TaskMetadata.py` & `mteb-1.7.0/tests/test_TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.9/tests/test_all_abstasks.py` & `mteb-1.7.0/tests/test_all_abstasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 from unittest.mock import Mock, patch
 
 import aiohttp
 import pytest
 
 from mteb import MTEB
 from mteb.abstasks import AbsTask
+from mteb.abstasks.AbsTaskInstructionRetrieval import AbsTaskInstructionRetrieval
 from mteb.abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 logging.basicConfig(level=logging.INFO)
 
 
 @pytest.mark.parametrize("task", MTEB().tasks_cls)
 @patch("datasets.load_dataset")
 def test_load_data(mock_load_dataset: Mock, task: AbsTask):
     # TODO: We skip because this load_data is completely different.
-    if isinstance(task, AbsTaskRetrieval):
+    if isinstance(task, AbsTaskRetrieval) or isinstance(
+        task, AbsTaskInstructionRetrieval
+    ):
         pytest.skip()
     with patch.object(task, "dataset_transform") as mock_dataset_transform:
         task.load_data()
         mock_load_dataset.assert_called()
 
         # They don't yet but should they so they can be expanded more easily?
         if not task.is_crosslingual and not task.is_multilingual:
@@ -60,12 +63,10 @@
         pretty_print = "\n".join(
             [f"{ds[0]} - revision {ds[1]}" for ds in does_not_exist]
         )
         assert False, f"Datasets not available on Hugging Face:\n{pretty_print}"
 
 
 def test_dataset_availability():
-    """
-    Checks if the datasets are available on Hugging Face using both their name and revision.
-    """
+    """Checks if the datasets are available on Hugging Face using both their name and revision."""
     tasks = MTEB().tasks_cls
     asyncio.run(check_datasets_are_available_on_hf(tasks))
```

### Comparing `mteb-1.6.9/tests/test_mteb.py` & `mteb-1.7.0/tests/test_mteb.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 from mteb.abstasks import AbsTask
 from mteb.tasks.BitextMining.dan.BornholmskBitextMining import BornholmBitextMining
 
 logging.basicConfig(level=logging.INFO)
 
 
 def test_two_mteb_tasks():
-    """
-    Test that two tasks can be fetched and run
-    """
+    """Test that two tasks can be fetched and run"""
     model = SentenceTransformer("average_word_embeddings_komninos")
     eval = MTEB(
         tasks=[
             "STS12",
             "SummEval",
         ]
     )
@@ -43,20 +41,16 @@
 @pytest.mark.parametrize(
     "model_name",
     [
         "average_word_embeddings_levy_dependency",
     ],
 )
 def test_mteb_task(task: Union[str, AbsTask], model_name: str):
-    """
-    Test that a task can be fetched and run
-    """
+    """Test that a task can be fetched and run"""
     model = SentenceTransformer(model_name)
     eval = MTEB(tasks=[task])
     eval.run(model, output_folder="tests/results", overwrite_results=True)
 
 
 def test_all_tasks_fetch():
-    """
-    Test that all tasks can be fetched
-    """
+    """Test that all tasks can be fetched"""
     MTEB.mteb_tasks()
```

