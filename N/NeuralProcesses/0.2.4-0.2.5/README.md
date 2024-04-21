# Comparing `tmp/neuralprocesses-0.2.4.tar.gz` & `tmp/neuralprocesses-0.2.5.tar.gz`

## Comparing `neuralprocesses-0.2.4.tar` & `neuralprocesses-0.2.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/_version.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/aggregate.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/augment.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/chain.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coding.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/datadims.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/disc.py
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/likelihood.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/mask.py
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/materialise.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/numdata.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/parallel.py
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/util.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/architectures/__init__.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/architectures/agnp.py
--rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/architectures/climate.py
--rw-r--r--   0        0        0    15137 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/architectures/convgnp.py
--rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/architectures/fullconvgnp.py
--rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/architectures/gnp.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/architectures/util.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/__init__.py
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/aggregate.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/attention.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/augment.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/copy.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/deepset.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/densecov.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/functional.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/fuse.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/inputs.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/mapdiag.py
--rw-r--r--   0        0        0    25832 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/nn.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/shaping.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/setconv/__init__.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/setconv/density.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/setconv/identity.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/coders/setconv/setconv.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/__init__.py
--rw-r--r--   0        0        0    11031 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/antarctica.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/batch.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/bimodal.py
--rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/data.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/eeg.py
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/gp.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/mixgp.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/mixture.py
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/predefined.py
--rw-r--r--   0        0        0    12613 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/predprey.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/sawtooth.py
--rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/temperature.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/data/util.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/__init__.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/beta.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/dirac.py
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/dist.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/geom.py
--rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/normal.py
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/spikeslab.py
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/transformed.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/dist/uniform.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/model/__init__.py
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/model/ar.py
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/model/elbo.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/model/loglik.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/model/model.py
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/model/predict.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/model/util.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/tensorflow/__init__.py
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/tensorflow/nn.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/torch/__init__.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/neuralprocesses/torch/nn.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/LICENCE.txt
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/README.md
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 neuralprocesses-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/_version.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/aggregate.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/augment.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/chain.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coding.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/datadims.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/disc.py
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/likelihood.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/mask.py
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/materialise.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/numdata.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/parallel.py
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/util.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/architectures/__init__.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/architectures/agnp.py
+-rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/architectures/climate.py
+-rw-r--r--   0        0        0    15137 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/architectures/convgnp.py
+-rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/architectures/fullconvgnp.py
+-rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/architectures/gnp.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/architectures/util.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/__init__.py
+-rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/aggregate.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/attention.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/augment.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/copy.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/deepset.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/densecov.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/functional.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/fuse.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/inputs.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/mapdiag.py
+-rw-r--r--   0        0        0    25832 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/nn.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/shaping.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/setconv/__init__.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/setconv/density.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/setconv/identity.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/coders/setconv/setconv.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/__init__.py
+-rw-r--r--   0        0        0    11031 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/antarctica.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/batch.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/bimodal.py
+-rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/data.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/eeg.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/gp.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/mixgp.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/mixture.py
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/predefined.py
+-rw-r--r--   0        0        0    12613 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/predprey.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/sawtooth.py
+-rw-r--r--   0        0        0    27362 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/temperature.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/data/util.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/__init__.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/beta.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/dirac.py
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/dist.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/geom.py
+-rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/normal.py
+-rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/spikeslab.py
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/transformed.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/dist/uniform.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/model/__init__.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/model/ar.py
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/model/elbo.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/model/loglik.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/model/model.py
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/model/predict.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/model/util.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/tensorflow/__init__.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/tensorflow/nn.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/torch/__init__.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/neuralprocesses/torch/nn.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/LICENCE.txt
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/README.md
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 neuralprocesses-0.2.5/PKG-INFO
```

### Comparing `neuralprocesses-0.2.4/neuralprocesses/__init__.py` & `neuralprocesses-0.2.5/neuralprocesses/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/aggregate.py` & `neuralprocesses-0.2.5/neuralprocesses/aggregate.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/augment.py` & `neuralprocesses-0.2.5/neuralprocesses/augment.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/chain.py` & `neuralprocesses-0.2.5/neuralprocesses/chain.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coding.py` & `neuralprocesses-0.2.5/neuralprocesses/coding.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/datadims.py` & `neuralprocesses-0.2.5/neuralprocesses/datadims.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/disc.py` & `neuralprocesses-0.2.5/neuralprocesses/disc.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/likelihood.py` & `neuralprocesses-0.2.5/neuralprocesses/likelihood.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/mask.py` & `neuralprocesses-0.2.5/neuralprocesses/mask.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/materialise.py` & `neuralprocesses-0.2.5/neuralprocesses/materialise.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/numdata.py` & `neuralprocesses-0.2.5/neuralprocesses/numdata.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/parallel.py` & `neuralprocesses-0.2.5/neuralprocesses/parallel.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/util.py` & `neuralprocesses-0.2.5/neuralprocesses/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/architectures/agnp.py` & `neuralprocesses-0.2.5/neuralprocesses/architectures/agnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/architectures/climate.py` & `neuralprocesses-0.2.5/neuralprocesses/architectures/climate.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/architectures/convgnp.py` & `neuralprocesses-0.2.5/neuralprocesses/architectures/convgnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/architectures/fullconvgnp.py` & `neuralprocesses-0.2.5/neuralprocesses/architectures/fullconvgnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/architectures/gnp.py` & `neuralprocesses-0.2.5/neuralprocesses/architectures/gnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/architectures/util.py` & `neuralprocesses-0.2.5/neuralprocesses/architectures/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/aggregate.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/aggregate.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/attention.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/attention.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/augment.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/augment.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/deepset.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/deepset.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/densecov.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/densecov.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/functional.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/functional.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/fuse.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/fuse.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/mapdiag.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/mapdiag.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/nn.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/nn.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/shaping.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/shaping.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/setconv/density.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/setconv/density.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/setconv/identity.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/setconv/identity.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/coders/setconv/setconv.py` & `neuralprocesses-0.2.5/neuralprocesses/coders/setconv/setconv.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/antarctica.py` & `neuralprocesses-0.2.5/neuralprocesses/data/antarctica.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/batch.py` & `neuralprocesses-0.2.5/neuralprocesses/data/batch.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/bimodal.py` & `neuralprocesses-0.2.5/neuralprocesses/data/bimodal.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/data.py` & `neuralprocesses-0.2.5/neuralprocesses/data/data.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/eeg.py` & `neuralprocesses-0.2.5/neuralprocesses/data/eeg.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/gp.py` & `neuralprocesses-0.2.5/neuralprocesses/data/gp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/mixgp.py` & `neuralprocesses-0.2.5/neuralprocesses/data/mixgp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/mixture.py` & `neuralprocesses-0.2.5/neuralprocesses/data/mixture.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/predefined.py` & `neuralprocesses-0.2.5/neuralprocesses/data/predefined.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/predprey.py` & `neuralprocesses-0.2.5/neuralprocesses/data/predprey.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/sawtooth.py` & `neuralprocesses-0.2.5/neuralprocesses/data/sawtooth.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/temperature.py` & `neuralprocesses-0.2.5/neuralprocesses/data/temperature.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/data/util.py` & `neuralprocesses-0.2.5/neuralprocesses/data/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/dist/beta.py` & `neuralprocesses-0.2.5/neuralprocesses/dist/beta.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/dist/dirac.py` & `neuralprocesses-0.2.5/neuralprocesses/dist/dirac.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/dist/dist.py` & `neuralprocesses-0.2.5/neuralprocesses/dist/dist.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/dist/geom.py` & `neuralprocesses-0.2.5/neuralprocesses/dist/geom.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/dist/normal.py` & `neuralprocesses-0.2.5/neuralprocesses/dist/normal.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/dist/spikeslab.py` & `neuralprocesses-0.2.5/neuralprocesses/dist/spikeslab.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/dist/transformed.py` & `neuralprocesses-0.2.5/neuralprocesses/dist/transformed.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/dist/uniform.py` & `neuralprocesses-0.2.5/neuralprocesses/dist/uniform.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/model/ar.py` & `neuralprocesses-0.2.5/neuralprocesses/model/ar.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/model/elbo.py` & `neuralprocesses-0.2.5/neuralprocesses/model/elbo.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/model/loglik.py` & `neuralprocesses-0.2.5/neuralprocesses/model/loglik.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/model/model.py` & `neuralprocesses-0.2.5/neuralprocesses/model/model.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/model/predict.py` & `neuralprocesses-0.2.5/neuralprocesses/model/predict.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,35 +14,42 @@
     state: B.RandomState,
     model: Model,
     contexts: list,
     xt,
     *,
     num_samples=50,
     batch_size=16,
+    dtype_lik=None,
 ):
     """Use a model to predict.
 
     Args:
         state (random state, optional): Random state.
         model (:class:`.Model`): Model.
         xc (input): Inputs of the context set.
         yc (tensor): Output of the context set.
         xt (input): Inputs of the target set.
         num_samples (int, optional): Number of samples to produce. Defaults to 50.
         batch_size (int, optional): Batch size. Defaults to 16.
+        dtype_lik (dtype, optional): Data type to use for the likelihood computation.
+            Defaults to the 64-bit variant of the data type of `xt`.
 
     Returns:
         random state, optional: Random state.
         tensor: Marginal mean.
         tensor: Marginal variance.
         tensor: `num_samples` noiseless samples.
         tensor: `num_samples` noisy samples.
     """
     float = B.dtype_float(xt)
-    float64 = B.promote_dtypes(float, np.float64)
+
+    # For the likelihood computation, default to using a 64-bit version of the data
+    # type of `xt`.
+    if not dtype_lik:
+        dtype_lik = B.promote_dtypes(float, np.float64)
 
     # Collect noiseless samples, noisy samples, first moments, and second moments.
     ft, yt = [], []
     m1s, m2s = [], []
 
     done_num_samples = 0
     while done_num_samples < num_samples:
@@ -50,16 +57,15 @@
         this_num_samples = min(num_samples - done_num_samples, batch_size)
 
         state, pred = model(
             state,
             contexts,
             xt,
             dtype_enc_sample=float,
-            # Run likelihood with `float64`s to ease the numerics as much as possible.
-            dtype_lik=float64,
+            dtype_lik=dtype_lik,
             num_samples=this_num_samples,
         )
 
         # If the number of samples is equal to one but `num_samples > 1`, then the
         # encoding was a `Dirac`, so we can stop batching. In this case, we can
         # efficiently compute everything that we need and exit.
         if this_num_samples > 1 and shape_batch(pred, 0) == 1:
```

### Comparing `neuralprocesses-0.2.4/neuralprocesses/model/util.py` & `neuralprocesses-0.2.5/neuralprocesses/model/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/tensorflow/__init__.py` & `neuralprocesses-0.2.5/neuralprocesses/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/tensorflow/nn.py` & `neuralprocesses-0.2.5/neuralprocesses/tensorflow/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from functools import partial
 from typing import Optional, Union
 
 import lab.tensorflow as B
 import numpy as np
 from plum import convert
 
@@ -115,22 +116,31 @@
 
     # Get the right layer kind.
     if transposed:
         suffix = "Transpose"
     else:
         suffix = ""
 
+    if groups > 1:
+        if transposed:
+            warnings.warn(
+                "Keras does not depthwise separable transposed convolutions! "
+                "Using non-separable convolutions for the transposed convolutions. "
+                "This could be a LOT more expensive."
+            )
+        else:
+            additional_args["groups"] = groups
+
     conv_layer = getattr(tf.keras.layers, f"Conv{dim}D{suffix}")(
         input_shape=(in_channels,) + (None,) * dim,
         filters=out_channels,
         kernel_size=kernel,
         strides=stride,
         padding="same",
         dilation_rate=dilation,
-        groups=groups,
         use_bias=bias,
         data_format=data_format,
         dtype=dtype,
         **additional_args,
     )
     if data_format == "channels_first":
         return conv_layer
```

### Comparing `neuralprocesses-0.2.4/neuralprocesses/torch/__init__.py` & `neuralprocesses-0.2.5/neuralprocesses/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/neuralprocesses/torch/nn.py` & `neuralprocesses-0.2.5/neuralprocesses/torch/nn.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/LICENCE.txt` & `neuralprocesses-0.2.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/README.md` & `neuralprocesses-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.4/pyproject.toml` & `neuralprocesses-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license = {text="MIT"}
 readme = "README.md"
 dynamic = ["version"]
 
 requires-python = ">=3.8"
 dependencies = [
     "numpy>=1.16",
-    "backends>=1.4.31",
+    "backends>=1.6.2",
     "backends-matrix>=1.2.10",
     "plum-dispatch>=2.3.0",
     "stheno>=1.3.10",
     "wbml>=0.3.18",
 ]
 
 [project.optional-dependencies]
@@ -36,15 +36,15 @@
     "build",
     "tox",
     "jupyter-book",
     "mypy",
     "pyright",
     "torch",
     "tensorflow",
-    "tensorflow-probability",
+    "tensorflow-probability[tf]",
 ]
 
 [project.urls]
 repository = "https://github.com/wesselb/neuralprocesses"
 
 [tool.hatch.build]
 include = ["neuralprocesses*"]
```

### Comparing `neuralprocesses-0.2.4/PKG-INFO` & `neuralprocesses-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: NeuralProcesses
-Version: 0.2.4
+Version: 0.2.5
 Summary: A framework for composing Neural Processes in Python
 Project-URL: repository, https://github.com/wesselb/neuralprocesses
 Author-email: Wessel Bruinsma <wessel.p.bruinsma@gmail.com>
 License: MIT
 License-File: LICENCE.txt
 Requires-Python: >=3.8
 Requires-Dist: backends-matrix>=1.2.10
-Requires-Dist: backends>=1.4.31
+Requires-Dist: backends>=1.6.2
 Requires-Dist: numpy>=1.16
 Requires-Dist: plum-dispatch>=2.3.0
 Requires-Dist: stheno>=1.3.10
 Requires-Dist: wbml>=0.3.18
 Provides-Extra: dev
 Requires-Dist: black==23.7.0; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
@@ -23,15 +23,15 @@
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: numpy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: tensorflow; extra == 'dev'
-Requires-Dist: tensorflow-probability; extra == 'dev'
+Requires-Dist: tensorflow-probability[tf]; extra == 'dev'
 Requires-Dist: torch; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # [Neural Processes](http://github.com/wesselb/neuralprocesses)
```

