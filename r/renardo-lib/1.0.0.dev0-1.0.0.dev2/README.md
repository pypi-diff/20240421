# Comparing `tmp/renardo_lib-1.0.0.dev0.tar.gz` & `tmp/renardo_lib-1.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renardo_lib-1.0.0.dev0.tar", last modified: Sun Apr 21 19:51:20 2024, max compression
+gzip compressed data, was "renardo_lib-1.0.0.dev2.tar", last modified: Sun Apr 21 19:58:25 2024, max compression
```

## Comparing `renardo_lib-1.0.0.dev0.tar` & `renardo_lib-1.0.0.dev2.tar`

### file list

```diff
@@ -1,388 +1,388 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.166358 renardo_lib-1.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    15008 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-21 19:51:20.166358 renardo_lib-1.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.110357 renardo_lib-1.0.0.dev0/renardo_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Bang.py
--rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Chords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.110357 renardo_lib-1.0.0.dev0/renardo_lib/Code/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Code/foxdot_func_cmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Code/foxdot_live_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Code/foxdot_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Code/foxdot_when_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Code/main_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.110357 renardo_lib-1.0.0.dev0/renardo_lib/Custom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Custom/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.114358 renardo_lib-1.0.0.dev0/renardo_lib/Effects/
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Effects/NewEffects.py
--rw-r--r--   0 runner    (1001) docker     (127)    27917 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Effects/Util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Effects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.114358 renardo_lib-1.0.0.dev0/renardo_lib/EspGrid/
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/EspGrid/EspGridHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/EspGrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.114358 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/PArp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.114358 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/SonicPi/
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/SonicPi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/SonicPi/generate_sonic_pi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.114358 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/Composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/MidiFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/Sinsy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/VRender.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/VoiceSpecificator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    14855 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Midi.py
--rw-r--r--   0 runner    (1001) docker     (127)   106660 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/OSC3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.114358 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Generators.py
--rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/PGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/PlayString.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Rest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/PlayerMethods.py
--rw-r--r--   0 runner    (1001) docker     (127)    49956 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Players.py
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Repeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.118358 renardo_lib-1.0.0.dev0/renardo_lib/SCLang/
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/SCLang/Env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/SCLang/SCLang.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/SCLang/SynthDef.py
--rw-r--r--   0 runner    (1001) docker     (127)    21463 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/SCLang/_SynthDefs.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/SCLang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Scale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.118358 renardo_lib-1.0.0.dev0/renardo_lib/ServerManager/
--rw-r--r--   0 runner    (1001) docker     (127)    31930 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/ServerManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.118358 renardo_lib-1.0.0.dev0/renardo_lib/Settings/
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Settings/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    26215 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/TimeVar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.118358 renardo_lib-1.0.0.dev0/renardo_lib/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.118358 renardo_lib-1.0.0.dev0/renardo_lib/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/00_intro.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/01_playing_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/02_algorithmic_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/03_playing_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/04_using_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/05_player_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/06_rests.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/07_basic_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/08_scales.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/09_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/10_using_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/11_playing_custom_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/12_synthdefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/13_advanced_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/14_player_attributes_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/demo/15_pattern_generator_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.122358 renardo_lib-1.0.0.dev0/renardo_lib/osc/
--rw-r--r--   0 runner    (1001) docker     (127)    31169 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/Buffers.scd
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/Info.scd
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/OscFunc.scd
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/Record.scd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.130358 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/DFM1.scd
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/Equalizer.scd
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/FrequencyModulationPulse.scd
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/FrequencyModulationSaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/FrequencyModulationSine.scd
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/H_Equalizer.scd
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/L_Equalizer.scd
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/M_Equalizer.scd
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/MoogFF.scd
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/Ringmod.scd
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/SLPF.scd
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/bandPassFilter.scd
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/bitcrush.scd
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/chop.scd
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/chorus.scd
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/coarse.scd
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/combDelay.scd
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/comp.scd
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/dirt_krush.scd
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/disto_mod.scd
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/distortion.scd
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/dubdelay.scd
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/fdist.scd
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/fdistc.scd
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/feeddelay.scd
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/filterSwell.scd
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/flanger.scd
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/formantFilter.scd
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/frequencyModulate.scd
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/fxout.scd
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/glissando.scd
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/highPassFilter.scd
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/krush.scd
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/leg.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/lofi.scd
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/lowPassFilter.scd
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/makeSound.scd
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/octafuz.scd
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/octer.scd
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/output.scd
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/overdriveDistortion.scd
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/phaser.scd
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/pitchBend.scd
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/pitchShift.scd
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/pitchshifter.scd
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/position.scd
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/resonz.scd
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/reverb.scd
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/reverb_stereo.scd
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/ring_modulation.scd
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/sample_atk.scd
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/sidechain.scd
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/slideFrom.scd
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/slideTo.scd
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/spinPan.scd
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/squiz.scd
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/startSound.scd
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/striate.scd
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/stutterfx.scd
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/tanhDisto.scd
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/tek.scd
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/tremolo.scd
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/trimLength.scd
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/trimPos.scd
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/triode.scd
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/vibrato.scd
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/volume.scd
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/wavefold.scd
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/waveloss.scd
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/wavesShapeDistortion.scd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.130358 renardo_lib-1.0.0.dev0/renardo_lib/osc/scenvelopes/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scenvelopes/BasicEnvelope.scd
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scenvelopes/MaskEnvelope.scd
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scenvelopes/PercussiveEnvelope.scd
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scenvelopes/RampEnvelope.scd
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scenvelopes/SwellEnvelope.scd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.162358 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/abass.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/acidbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/alva.scd
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ambi.scd
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/angel.scd
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/angst.scd
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/arpy.scd
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/audioin.scd
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bass.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bassguitar.scd
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bchaos.scd
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bell.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bellmod.scd
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/benoit.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/birdy.scd
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/blip.scd
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/blips.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bnoise.scd
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/borgan.scd
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bounce.scd
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bphase.scd
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/brass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/brown.scd
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bug.scd
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/charm.scd
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/chimebell.scd
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/chipsy.scd
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/click.scd
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/clip.scd
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/cluster.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/combs.scd
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/creep.scd
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/crunch.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/cs80lead.scd
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dab.scd
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dafbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dblbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dirt.scd
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/donk.scd
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/donk1.scd
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/donk2.scd
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/donkysub.scd
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/donorgan.scd
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dopple.scd
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/drone.scd
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dub.scd
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dust.scd
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dustv.scd
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ebass.scd
--rwxr-xr-x   0 runner    (1001) docker     (127)      939 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ecello.scd
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/eeri.scd
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/eoboe.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/epiano.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/faim.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/faim2.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/feel.scd
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/filthysaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/flute.scd
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fm.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fmbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fmrhodes.scd
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/four.scd
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fuzz.scd
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/garfield.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/gaze.scd
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/glass.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/glitchbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/glitcher.scd
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/gong.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/grat.scd
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/gray.scd
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/growl.scd
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/gsynth.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/harp.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/hnoise.scd
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/hoover.scd
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/hydra.scd
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/jbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/kalimba.scd
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/karp.scd
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/keys.scd
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/klank.scd
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ladder.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/lapin.scd
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/laserbeam.scd
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/latoo.scd
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/lazer.scd
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/lfnoise.scd
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/linesaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/longsaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/loop.scd
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/marimba.scd
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/mhpad.scd
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/mhping.scd
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/moogbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/moogpluck.scd
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/moogpluck2.scd
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/mpluck.scd
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/mySynth.scd
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/noise.scd
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/noisynth.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/noquarter.scd
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/nylon.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/organ.scd
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/organ2.scd
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/orient.scd
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pads.scd
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pasha.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/phazer.scd
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/piano.scd
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pianovel.scd
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pink.scd
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/play1.scd
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/play2.scd
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pluck.scd
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pmcrotal.scd
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ppad.scd
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/prayerbell.scd
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/prof.scd
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/prophet.scd
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pulse.scd
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/quin.scd
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/radio.scd
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rave.scd
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/razz.scd
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rhodes.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rhpiano.scd
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ripple.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/risseto.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rissetobell.scd
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rlead.scd
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rsaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rsin.scd
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/saw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sawbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/scatter.scd
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/scrap.scd
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/scratch.scd
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/shore.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sillyvoice.scd
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sine.scd
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sinepad.scd
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/siren.scd
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sitar.scd
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/snick.scd
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/soft.scd
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/soprano.scd
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sos.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sosbell.scd
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/space.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/spacesaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/spark.scd
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/spick.scd
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sputter.scd
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/square.scd
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/squish.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ssaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/star.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/stargazer.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/steeldrum.scd
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/stretch.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/strings.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/subbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/subbass2.scd
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/supersaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/swell.scd
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tb303.scd
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/total.scd
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tremsynth.scd
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tribell.scd
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tritri.scd
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/triwave.scd
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tubularbell.scd
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/twang.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tworgan.scd
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tworgan2.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tworgan3.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tworgan4.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/varcell.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/varicelle.scd
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/varsaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/vibass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/video.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/vinsine.scd
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/viola.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/virus.scd
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/vrender.scd
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/waves.scd
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/windmaker.scd
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/wobble.scd
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/wobblebass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/wsaw.scd
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/wsawbass.scd
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/xylophone.scd
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/zap.scd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.162358 renardo_lib-1.0.0.dev0/renardo_lib/preset/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/renardo_lib/preset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.166358 renardo_lib-1.0.0.dev0/renardo_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-21 19:51:20.000000 renardo_lib-1.0.0.dev0/renardo_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-04-21 19:51:20.000000 renardo_lib-1.0.0.dev0/renardo_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:51:20.000000 renardo_lib-1.0.0.dev0/renardo_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 19:51:20.000000 renardo_lib-1.0.0.dev0/renardo_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 19:51:20.000000 renardo_lib-1.0.0.dev0/renardo_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:51:20.166358 renardo_lib-1.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:51:20.162358 renardo_lib-1.0.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/tests/test_generator_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-21 19:51:16.000000 renardo_lib-1.0.0.dev0/tests/test_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.813135 renardo_lib-1.0.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    15008 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-04-21 19:58:25.813135 renardo_lib-1.0.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.761135 renardo_lib-1.0.0.dev2/renardo_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Bang.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Chords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.761135 renardo_lib-1.0.0.dev2/renardo_lib/Code/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Code/foxdot_func_cmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Code/foxdot_live_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Code/foxdot_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Code/foxdot_when_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Code/main_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.761135 renardo_lib-1.0.0.dev2/renardo_lib/Custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Custom/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.761135 renardo_lib-1.0.0.dev2/renardo_lib/Effects/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Effects/NewEffects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27917 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Effects/Util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Effects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.761135 renardo_lib-1.0.0.dev2/renardo_lib/EspGrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/EspGrid/EspGridHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/EspGrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.761135 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/PArp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.761135 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/SonicPi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/SonicPi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/SonicPi/generate_sonic_pi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.765135 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/Composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/MidiFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/Sinsy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/VRender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/VoiceSpecificator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14855 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Midi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106660 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/OSC3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.765135 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/PGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/PlayString.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/PlayerMethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49956 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Players.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Repeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.765135 renardo_lib-1.0.0.dev2/renardo_lib/SCLang/
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/SCLang/Env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/SCLang/SCLang.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/SCLang/SynthDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21463 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/SCLang/_SynthDefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/SCLang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Scale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.765135 renardo_lib-1.0.0.dev2/renardo_lib/ServerManager/
+-rw-r--r--   0 runner    (1001) docker     (127)    31930 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/ServerManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.765135 renardo_lib-1.0.0.dev2/renardo_lib/Settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Settings/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26215 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/TimeVar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.765135 renardo_lib-1.0.0.dev2/renardo_lib/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.769135 renardo_lib-1.0.0.dev2/renardo_lib/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/00_intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/01_playing_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/02_algorithmic_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/03_playing_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/04_using_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/05_player_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/06_rests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/07_basic_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/08_scales.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/09_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/10_using_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/11_playing_custom_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/12_synthdefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/13_advanced_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/14_player_attributes_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/demo/15_pattern_generator_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.769135 renardo_lib-1.0.0.dev2/renardo_lib/osc/
+-rw-r--r--   0 runner    (1001) docker     (127)    31169 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/Buffers.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/Info.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/OscFunc.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/Record.scd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.781135 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/DFM1.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/Equalizer.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/FrequencyModulationPulse.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/FrequencyModulationSaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/FrequencyModulationSine.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/H_Equalizer.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/L_Equalizer.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/M_Equalizer.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/MoogFF.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/Ringmod.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/SLPF.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/bandPassFilter.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/bitcrush.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/chop.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/chorus.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/coarse.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/combDelay.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/comp.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/dirt_krush.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/disto_mod.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/distortion.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/dubdelay.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/fdist.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/fdistc.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/feeddelay.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/filterSwell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/flanger.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/formantFilter.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/frequencyModulate.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/fxout.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/glissando.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/highPassFilter.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/krush.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/leg.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/lofi.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/lowPassFilter.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/makeSound.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/octafuz.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/octer.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/output.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/overdriveDistortion.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/phaser.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/pitchBend.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/pitchShift.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/pitchshifter.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/position.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/resonz.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/reverb.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/reverb_stereo.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/ring_modulation.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/sample_atk.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/sidechain.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/slideFrom.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/slideTo.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/spinPan.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/squiz.scd
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/startSound.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/striate.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/stutterfx.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/tanhDisto.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/tek.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/tremolo.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/trimLength.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/trimPos.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/triode.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/vibrato.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/volume.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/wavefold.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/waveloss.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/wavesShapeDistortion.scd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.781135 renardo_lib-1.0.0.dev2/renardo_lib/osc/scenvelopes/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scenvelopes/BasicEnvelope.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scenvelopes/MaskEnvelope.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scenvelopes/PercussiveEnvelope.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scenvelopes/RampEnvelope.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scenvelopes/SwellEnvelope.scd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.813135 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/abass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/acidbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/alva.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ambi.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/angel.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/angst.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/arpy.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/audioin.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bassguitar.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bchaos.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bellmod.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/benoit.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/birdy.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/blip.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/blips.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bnoise.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/borgan.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bounce.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bphase.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/brass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/brown.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bug.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/charm.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/chimebell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/chipsy.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/click.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/clip.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/cluster.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/combs.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/creep.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/crunch.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/cs80lead.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dab.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dafbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dblbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dirt.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/donk.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/donk1.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/donk2.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/donkysub.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/donorgan.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dopple.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/drone.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dub.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dust.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dustv.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ebass.scd
+-rwxr-xr-x   0 runner    (1001) docker     (127)      939 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ecello.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/eeri.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/eoboe.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/epiano.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/faim.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/faim2.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/feel.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/filthysaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/flute.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fm.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fmbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fmrhodes.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/four.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fuzz.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/garfield.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/gaze.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/glass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/glitchbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/glitcher.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/gong.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/grat.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/gray.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/growl.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/gsynth.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/harp.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/hnoise.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/hoover.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/hydra.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/jbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/kalimba.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/karp.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/keys.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/klank.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ladder.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/lapin.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/laserbeam.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/latoo.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/lazer.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/lfnoise.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/linesaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/longsaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/loop.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/marimba.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/mhpad.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/mhping.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/moogbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/moogpluck.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/moogpluck2.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/mpluck.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/mySynth.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/noise.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/noisynth.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/noquarter.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/nylon.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/organ.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/organ2.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/orient.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pads.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pasha.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/phazer.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/piano.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pianovel.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pink.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/play1.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/play2.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pluck.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pmcrotal.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ppad.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/prayerbell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/prof.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/prophet.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pulse.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/quin.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/radio.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rave.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/razz.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rhodes.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rhpiano.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ripple.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/risseto.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rissetobell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rlead.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rsaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rsin.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/saw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sawbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/scatter.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/scrap.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/scratch.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/shore.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sillyvoice.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sine.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sinepad.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/siren.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sitar.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/snick.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/soft.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/soprano.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sos.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sosbell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/space.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/spacesaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/spark.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/spick.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sputter.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/square.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/squish.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ssaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/star.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/stargazer.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/steeldrum.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/stretch.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/strings.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/subbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/subbass2.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/supersaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/swell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tb303.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/total.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tremsynth.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tribell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tritri.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/triwave.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tubularbell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/twang.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tworgan.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tworgan2.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tworgan3.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tworgan4.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/varcell.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/varicelle.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/varsaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/vibass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/video.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/vinsine.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/viola.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/virus.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/vrender.scd
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/waves.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/windmaker.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/wobble.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/wobblebass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/wsaw.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/wsawbass.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/xylophone.scd
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/zap.scd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.813135 renardo_lib-1.0.0.dev2/renardo_lib/preset/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/renardo_lib/preset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.813135 renardo_lib-1.0.0.dev2/renardo_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-04-21 19:58:25.000000 renardo_lib-1.0.0.dev2/renardo_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-04-21 19:58:25.000000 renardo_lib-1.0.0.dev2/renardo_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:58:25.000000 renardo_lib-1.0.0.dev2/renardo_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 19:58:25.000000 renardo_lib-1.0.0.dev2/renardo_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 19:58:25.000000 renardo_lib-1.0.0.dev2/renardo_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:58:25.813135 renardo_lib-1.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:58:25.813135 renardo_lib-1.0.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/tests/test_generator_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-21 19:58:21.000000 renardo_lib-1.0.0.dev2/tests/test_patterns.py
```

### Comparing `renardo_lib-1.0.0.dev0/LICENSE` & `renardo_lib-1.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/PKG-INFO` & `renardo_lib-1.0.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: renardo_lib
-Version: 1.0.0.dev0
+Version: 1.0.0.dev2
 Summary: Python livecoding environment - New fork of FoxDot
 Home-page: http://renardo.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: renardo_gatherer==0.1.3
-Requires-Dist: fastnumbersmidiutil
+Requires-Dist: fastnumbers
+Requires-Dist: midiutil
 
 Renardo v0.9 - FoxDot fork
 ===========================
 
 Renardo/FoxDot is a Python programming environment that provides a fast and user-friendly abstraction to SuperCollider. It also comes with its own IDE, which means it can be used straight out of the box; all you need is Python and SuperCollider and you're ready to go!
 
 ## Important
```

### Comparing `renardo_lib-1.0.0.dev0/README.md` & `renardo_lib-1.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Bang.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Bang.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Buffers.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Buffers.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Code/foxdot_func_cmp.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Code/foxdot_func_cmp.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Code/foxdot_live_function.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Code/foxdot_live_function.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Code/foxdot_tokenize.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Code/foxdot_tokenize.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Code/foxdot_when_statement.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Code/foxdot_when_statement.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Code/main_lib.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Code/main_lib.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Constants.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Constants.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Effects/NewEffects.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Effects/NewEffects.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Effects/Util.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Effects/Util.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/EspGrid/EspGridHelper.py` & `renardo_lib-1.0.0.dev2/renardo_lib/EspGrid/EspGridHelper.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Extensions/PArp.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Extensions/PArp.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Extensions/SonicPi/__init__.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Extensions/SonicPi/__init__.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/Composer.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/Composer.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/MidiFactory.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/MidiFactory.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/VRender.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/VRender.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/VoiceSpecificator.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/VoiceSpecificator.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Extensions/VRender/__init__.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Extensions/VRender/__init__.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Groups.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Groups.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Key.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Key.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Logging.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Logging.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Midi.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Midi.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/OSC3.py` & `renardo_lib-1.0.0.dev2/renardo_lib/OSC3.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Generators.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Generators.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Main.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Main.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Operations.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Operations.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/PGroups.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/PGroups.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Parse.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Parse.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/PlayString.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/PlayString.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Rest.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Rest.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Sequences.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Sequences.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/Utils.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/Utils.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Patterns/__init__.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/PlayerMethods.py` & `renardo_lib-1.0.0.dev2/renardo_lib/PlayerMethods.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Players.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Players.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Repeat.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Repeat.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Root.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Root.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/SCLang/Env.py` & `renardo_lib-1.0.0.dev2/renardo_lib/SCLang/Env.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/SCLang/SCLang.py` & `renardo_lib-1.0.0.dev2/renardo_lib/SCLang/SCLang.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/SCLang/SynthDef.py` & `renardo_lib-1.0.0.dev2/renardo_lib/SCLang/SynthDef.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/SCLang/_SynthDefs.py` & `renardo_lib-1.0.0.dev2/renardo_lib/SCLang/_SynthDefs.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Scale.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Scale.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/ServerManager/__init__.py` & `renardo_lib-1.0.0.dev2/renardo_lib/ServerManager/__init__.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Settings/__init__.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Settings/__init__.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Settings/conf.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Settings/conf.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/TimeVar.py` & `renardo_lib-1.0.0.dev2/renardo_lib/TimeVar.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/Utils/__init__.py` & `renardo_lib-1.0.0.dev2/renardo_lib/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/__init__.py` & `renardo_lib-1.0.0.dev2/renardo_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     except KeyboardInterrupt:
         return
 
 # Util class
 
 class _util:
     def __repr__(self):
-        return "Renardo ver. 1.0.0.dev0"
+        return "Renardo ver. 1.0.0.dev2"
     def reload(self):
         Server.reset()
         SynthDefs.reload()
         FxList.reload()
         Samples.reset()
         return
     def reassign_clock(self):
```

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/00_intro.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/00_intro.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/01_playing_notes.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/01_playing_notes.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/02_algorithmic_manipulation.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/02_algorithmic_manipulation.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/03_playing_samples.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/03_playing_samples.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/04_using_patterns.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/04_using_patterns.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/05_player_attributes.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/05_player_attributes.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/07_basic_clock.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/07_basic_clock.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/08_scales.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/08_scales.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/09_groups.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/09_groups.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/10_using_vars.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/10_using_vars.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/11_playing_custom_samples.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/11_playing_custom_samples.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/12_synthdefs.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/12_synthdefs.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/13_advanced_clock.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/13_advanced_clock.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/14_player_attributes_reference.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/14_player_attributes_reference.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/demo/15_pattern_generator_reference.py` & `renardo_lib-1.0.0.dev2/renardo_lib/demo/15_pattern_generator_reference.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/Buffers.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/Buffers.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/Info.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/Info.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/chorus.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/chorus.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/dubdelay.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/dubdelay.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/fdistc.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/fdistc.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/lofi.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/lofi.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/stutterfx.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/stutterfx.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/sceffects/tek.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/sceffects/tek.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/abass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/abass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/acidbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/acidbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/alva.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/alva.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ambi.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ambi.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/angel.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/angel.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/angst.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/angst.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/arpy.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/arpy.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bassguitar.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bassguitar.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bchaos.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bchaos.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bellmod.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bellmod.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/benoit.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/benoit.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/birdy.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/birdy.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/blip.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/blip.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/blips.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/blips.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bnoise.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bnoise.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/borgan.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/borgan.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bounce.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bounce.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bphase.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bphase.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/brass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/brass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/bug.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/bug.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/charm.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/charm.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/chimebell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/chimebell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/chipsy.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/chipsy.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/click.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/click.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/cluster.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/cluster.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/combs.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/combs.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/cs80lead.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/cs80lead.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dab.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dab.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dafbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dafbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dblbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dblbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dirt.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dirt.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/donkysub.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/donkysub.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/donorgan.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/donorgan.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dopple.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dopple.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/drone.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/drone.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/dustv.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/dustv.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ebass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ebass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ecello.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ecello.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/eeri.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/eeri.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/eoboe.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/eoboe.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/epiano.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/epiano.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/faim.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/faim.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/faim2.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/faim2.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/feel.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/feel.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/filthysaw.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/filthysaw.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/flute.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/flute.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fm.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fm.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fmbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fmbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fmrhodes.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fmrhodes.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/four.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/four.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/fuzz.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/fuzz.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/garfield.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/garfield.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/gaze.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/gaze.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/glass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/glass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/glitchbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/glitchbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/glitcher.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/glitcher.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/gong.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/gong.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/grat.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/grat.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/growl.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/growl.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/gsynth.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/gsynth.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/harp.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/harp.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/hnoise.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/hnoise.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/hoover.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/hoover.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/hydra.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/hydra.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/jbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/jbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/kalimba.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/kalimba.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/karp.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/karp.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/keys.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/keys.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/klank.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/klank.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ladder.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ladder.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/lapin.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/lapin.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/laserbeam.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/laserbeam.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/latoo.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/latoo.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/lazer.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/lazer.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/lfnoise.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/lfnoise.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/linesaw.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/linesaw.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/longsaw.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/longsaw.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/loop.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/loop.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/marimba.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/marimba.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/mhpad.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/mhpad.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/mhping.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/mhping.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/moogbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/moogbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/moogpluck.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/moogpluck.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/moogpluck2.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/moogpluck2.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/mpluck.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/mpluck.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/noisynth.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/noisynth.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/noquarter.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/noquarter.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/nylon.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/nylon.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/organ.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/organ.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/organ2.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/organ2.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/orient.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/orient.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pads.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pads.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pasha.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pasha.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/phazer.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/phazer.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/piano.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/piano.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pianovel.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pianovel.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pink.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pink.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pluck.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pluck.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/pmcrotal.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/pmcrotal.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ppad.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ppad.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/prayerbell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/prayerbell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/prof.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/prof.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/prophet.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/prophet.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/quin.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/quin.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/radio.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/radio.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/razz.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/razz.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rhodes.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rhodes.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rhpiano.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rhpiano.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ripple.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ripple.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/risseto.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/risseto.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rissetobell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rissetobell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rlead.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rlead.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rsaw.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rsaw.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/rsin.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/rsin.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sawbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sawbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/scatter.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/scatter.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/scrap.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/scrap.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/scratch.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/scratch.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/shore.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/shore.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sillyvoice.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sillyvoice.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sine.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sine.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sinepad.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sinepad.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/siren.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/siren.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sitar.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sitar.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/soft.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/soft.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/soprano.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/soprano.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sos.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sos.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sosbell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sosbell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/space.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/space.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/spacesaw.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/spacesaw.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/spark.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/spark.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/spick.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/spick.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/sputter.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/sputter.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/square.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/square.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/ssaw.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/ssaw.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/star.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/star.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/stargazer.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/stargazer.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/steeldrum.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/steeldrum.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/strings.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/strings.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/subbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/subbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/subbass2.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/subbass2.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/supersaw.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/supersaw.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/swell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/swell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tb303.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tb303.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/total.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/total.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tremsynth.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tremsynth.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tribell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tribell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tritri.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tritri.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/triwave.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/triwave.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tubularbell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tubularbell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/twang.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/twang.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tworgan.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tworgan.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tworgan2.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tworgan2.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tworgan3.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tworgan3.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/tworgan4.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/tworgan4.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/varcell.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/varcell.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/varicelle.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/varicelle.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/vibass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/vibass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/vinsine.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/vinsine.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/viola.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/viola.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/virus.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/virus.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/waves.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/waves.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/windmaker.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/windmaker.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/wobble.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/wobble.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/wobblebass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/wobblebass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/wsaw.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/wsaw.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/wsawbass.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/wsawbass.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/xylophone.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/xylophone.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib/osc/scsyndef/zap.scd` & `renardo_lib-1.0.0.dev2/renardo_lib/osc/scsyndef/zap.scd`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib.egg-info/PKG-INFO` & `renardo_lib-1.0.0.dev2/renardo_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: renardo_lib
-Version: 1.0.0.dev0
+Version: 1.0.0.dev2
 Summary: Python livecoding environment - New fork of FoxDot
 Home-page: http://renardo.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: renardo_gatherer==0.1.3
-Requires-Dist: fastnumbersmidiutil
+Requires-Dist: fastnumbers
+Requires-Dist: midiutil
 
 Renardo v0.9 - FoxDot fork
 ===========================
 
 Renardo/FoxDot is a Python programming environment that provides a fast and user-friendly abstraction to SuperCollider. It also comes with its own IDE, which means it can be used straight out of the box; all you need is Python and SuperCollider and you're ready to go!
 
 ## Important
```

### Comparing `renardo_lib-1.0.0.dev0/renardo_lib.egg-info/SOURCES.txt` & `renardo_lib-1.0.0.dev2/renardo_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/setup.py` & `renardo_lib-1.0.0.dev2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description=f.read()
 
 setup(
     name='renardo_lib',
-    version="1.0.0.dev0",
+    version="1.0.0.dev2",
     description='Python livecoding environment - New fork of FoxDot',
     author='Elie Gavoty',
     author_email='eliegavoty@free.fr',
     license='cc-by-sa-4.0',
     url='http://renardo.org/',
     packages=[
         'renardo_lib',
@@ -32,11 +32,11 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     # entry_points={'gui_scripts' : ['FoxDotEditor = FoxDotEditor.__init__:main']},
     # data_files=[('', 'LICENSE')],
     package_data = {'renardo_lib': ['README.md','demo/**', 'osc/**'],},
     install_requires=[
         'renardo_gatherer==0.1.3',
-        'fastnumbers'
+        'fastnumbers',
         'midiutil',
     ],
 )
```

### Comparing `renardo_lib-1.0.0.dev0/tests/test_buffers.py` & `renardo_lib-1.0.0.dev2/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `renardo_lib-1.0.0.dev0/tests/test_generator_pattern.py` & `renardo_lib-1.0.0.dev2/tests/test_generator_pattern.py`

 * *Files identical despite different names*

