# Comparing `tmp/terminaltexteffects-0.9.0.tar.gz` & `tmp/terminaltexteffects-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminaltexteffects-0.9.0.tar", max compression
+gzip compressed data, was "terminaltexteffects-0.9.1.tar", max compression
```

## Comparing `terminaltexteffects-0.9.0.tar` & `terminaltexteffects-0.9.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rwxr-xr-x   0        0        0     1072 2023-08-13 20:34:07.346818 terminaltexteffects-0.9.0/LICENSE
--rwxr-xr-x   0        0        0    11802 2024-05-05 17:40:35.415508 terminaltexteffects-0.9.0/README.md
--rwxr-xr-x   0        0        0      474 2024-05-05 17:42:21.861321 terminaltexteffects-0.9.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-08-12 13:15:55.921216 terminaltexteffects-0.9.0/terminaltexteffects/__init__.py
--rwxr-xr-x   0        0        0     2000 2024-05-05 17:33:51.712767 terminaltexteffects-0.9.0/terminaltexteffects/__main__.py
--rwxr-xr-x   0        0        0        0 2023-07-22 17:59:37.688921 terminaltexteffects-0.9.0/terminaltexteffects/effects/__init__.py
--rwxr-xr-x   0        0        0    18085 2024-05-05 17:33:51.713740 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_beams.py
--rwxr-xr-x   0        0        0    16120 2024-05-05 17:33:51.714107 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_binarypath.py
--rwxr-xr-x   0        0        0    19300 2024-05-05 17:33:51.714496 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_blackhole.py
--rwxr-xr-x   0        0        0    11021 2024-05-05 17:33:51.714822 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_bouncyballs.py
--rwxr-xr-x   0        0        0    17875 2024-05-05 17:33:51.715218 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_bubbles.py
--rwxr-xr-x   0        0        0     8339 2024-05-05 17:33:51.715538 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_burn.py
--rwxr-xr-x   0        0        0    11659 2024-05-05 17:33:51.715867 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_crumble.py
--rwxr-xr-x   0        0        0    11586 2024-05-05 17:33:51.716195 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_decrypt.py
--rwxr-xr-x   0        0        0    13939 2024-05-05 17:33:51.716552 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_errorcorrect.py
--rwxr-xr-x   0        0        0     7902 2024-05-05 17:33:51.716878 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_expand.py
--rwxr-xr-x   0        0        0    14326 2024-05-05 17:33:51.717255 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_fireworks.py
--rwxr-xr-x   0        0        0    10710 2024-05-05 17:33:51.717659 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_middleout.py
--rwxr-xr-x   0        0        0    17434 2024-05-05 17:33:51.718058 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_orbittingvolley.py
--rwxr-xr-x   0        0        0    11316 2024-05-05 17:33:51.718406 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_overflow.py
--rwxr-xr-x   0        0        0    12513 2024-05-05 17:33:51.718766 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_pour.py
--rwxr-xr-x   0        0        0    12234 2024-05-05 17:33:51.719204 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_print.py
--rwxr-xr-x   0        0        0    10173 2024-05-05 17:33:51.719565 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_rain.py
--rwxr-xr-x   0        0        0     7981 2024-05-05 17:33:51.719877 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_random_sequence.py
--rwxr-xr-x   0        0        0    19899 2024-05-05 17:33:51.720292 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_rings.py
--rwxr-xr-x   0        0        0     8394 2024-05-05 17:33:51.720652 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_scattered.py
--rwxr-xr-x   0        0        0    13977 2024-05-05 17:33:51.721014 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_slide.py
--rwxr-xr-x   0        0        0    14420 2024-05-05 17:33:51.721447 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_spotlights.py
--rwxr-xr-x   0        0        0    11432 2024-05-05 17:33:51.721806 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_spray.py
--rwxr-xr-x   0        0        0    15385 2024-05-05 17:33:51.722171 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_swarm.py
--rwxr-xr-x   0        0        0    20593 2024-05-05 17:33:51.722595 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_synthgrid.py
--rwxr-xr-x   0        0        0    13959 2024-05-05 17:33:51.722984 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_unstable.py
--rwxr-xr-x   0        0        0     8650 2024-05-05 17:33:51.723333 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_verticalslice.py
--rwxr-xr-x   0        0        0    22923 2024-05-05 17:33:51.723759 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_vhstape.py
--rwxr-xr-x   0        0        0    10624 2024-05-05 17:33:51.724110 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_waves.py
--rwxr-xr-x   0        0        0     9791 2024-05-05 17:33:51.724444 terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_wipe.py
--rwxr-xr-x   0        0        0        0 2024-05-05 17:33:51.724578 terminaltexteffects-0.9.0/terminaltexteffects/engine/__init__.py
--rwxr-xr-x   0        0        0    22748 2024-05-05 17:33:51.741057 terminaltexteffects-0.9.0/terminaltexteffects/engine/animation.py
--rwxr-xr-x   0        0        0    11162 2024-05-05 17:33:51.752448 terminaltexteffects-0.9.0/terminaltexteffects/engine/base_character.py
--rwxr-xr-x   0        0        0     3656 2024-05-05 17:33:51.798186 terminaltexteffects-0.9.0/terminaltexteffects/engine/base_effect.py
--rwxr-xr-x   0        0        0    22354 2024-05-05 17:33:51.800192 terminaltexteffects-0.9.0/terminaltexteffects/engine/motion.py
--rwxr-xr-x   0        0        0    30059 2024-05-05 17:33:51.801858 terminaltexteffects-0.9.0/terminaltexteffects/engine/terminal.py
--rwxr-xr-x   0        0        0        0 2024-04-12 11:52:35.092907 terminaltexteffects-0.9.0/terminaltexteffects/py.typed
--rwxr-xr-x   0        0        0     4931 2024-05-05 17:33:51.816796 terminaltexteffects-0.9.0/terminaltexteffects/template/effect_template.py
--rwxr-xr-x   0        0        0        0 2023-07-22 17:59:26.632934 terminaltexteffects-0.9.0/terminaltexteffects/utils/__init__.py
--rwxr-xr-x   0        0        0     2432 2024-05-05 17:33:51.818449 terminaltexteffects-0.9.0/terminaltexteffects/utils/ansitools.py
--rwxr-xr-x   0        0        0    12883 2024-05-05 17:33:51.829129 terminaltexteffects-0.9.0/terminaltexteffects/utils/argsdataclass.py
--rwxr-xr-x   0        0        0    15541 2024-05-05 17:33:51.830302 terminaltexteffects-0.9.0/terminaltexteffects/utils/argvalidators.py
--rwxr-xr-x   0        0        0     2399 2024-05-05 17:33:51.832912 terminaltexteffects-0.9.0/terminaltexteffects/utils/colorterm.py
--rwxr-xr-x   0        0        0    13639 2024-05-05 17:33:51.833389 terminaltexteffects-0.9.0/terminaltexteffects/utils/easing.py
--rwxr-xr-x   0        0        0        0 2024-04-26 11:00:38.378584 terminaltexteffects-0.9.0/terminaltexteffects/utils/exceptions.py
--rwxr-xr-x   0        0        0     9843 2024-05-05 17:33:51.833880 terminaltexteffects-0.9.0/terminaltexteffects/utils/geometry.py
--rwxr-xr-x   0        0        0    10033 2024-05-05 17:33:51.834296 terminaltexteffects-0.9.0/terminaltexteffects/utils/graphics.py
--rwxr-xr-x   0        0        0     7140 2024-05-05 17:33:51.847877 terminaltexteffects-0.9.0/terminaltexteffects/utils/hexterm.py
--rw-r--r--   0        0        0    12332 1970-01-01 00:00:00.000000 terminaltexteffects-0.9.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-08-13 20:34:07.346818 terminaltexteffects-0.9.1/LICENSE
+-rwxr-xr-x   0        0        0    12812 2024-05-11 11:39:58.361920 terminaltexteffects-0.9.1/README.md
+-rwxr-xr-x   0        0        0      474 2024-05-11 11:44:03.957471 terminaltexteffects-0.9.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-08-12 13:15:55.921216 terminaltexteffects-0.9.1/terminaltexteffects/__init__.py
+-rwxr-xr-x   0        0        0     2054 2024-05-11 11:36:03.464604 terminaltexteffects-0.9.1/terminaltexteffects/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-07-22 17:59:37.688921 terminaltexteffects-0.9.1/terminaltexteffects/effects/__init__.py
+-rwxr-xr-x   0        0        0    17753 2024-05-11 02:30:33.705429 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_beams.py
+-rwxr-xr-x   0        0        0    15747 2024-05-11 02:30:33.705887 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_binarypath.py
+-rwxr-xr-x   0        0        0    18978 2024-05-11 02:30:33.706344 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_blackhole.py
+-rwxr-xr-x   0        0        0    10743 2024-05-11 02:30:33.706729 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_bouncyballs.py
+-rwxr-xr-x   0        0        0    17536 2024-05-11 02:30:33.707172 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_bubbles.py
+-rwxr-xr-x   0        0        0     7978 2024-05-11 02:30:33.707521 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_burn.py
+-rwxr-xr-x   0        0        0    11370 2024-05-11 02:30:33.707917 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_crumble.py
+-rwxr-xr-x   0        0        0    11098 2024-05-11 02:30:33.708254 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_decrypt.py
+-rwxr-xr-x   0        0        0    13625 2024-05-11 02:30:33.708606 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_errorcorrect.py
+-rwxr-xr-x   0        0        0     7643 2024-05-11 02:30:33.709011 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_expand.py
+-rwxr-xr-x   0        0        0    14006 2024-05-11 02:30:33.709598 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_fireworks.py
+-rwxr-xr-x   0        0        0    10352 2024-05-11 02:30:33.709967 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_middleout.py
+-rwxr-xr-x   0        0        0    17071 2024-05-11 02:30:33.710369 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_orbittingvolley.py
+-rwxr-xr-x   0        0        0    10990 2024-05-11 02:30:33.722626 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_overflow.py
+-rwxr-xr-x   0        0        0    12173 2024-05-11 02:30:33.722985 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_pour.py
+-rwxr-xr-x   0        0        0    11913 2024-05-11 02:30:33.723338 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_print.py
+-rwxr-xr-x   0        0        0     9893 2024-05-11 02:30:33.723681 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_rain.py
+-rwxr-xr-x   0        0        0     7648 2024-05-11 02:30:33.724000 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_random_sequence.py
+-rwxr-xr-x   0        0        0    19574 2024-05-11 02:30:33.724409 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_rings.py
+-rwxr-xr-x   0        0        0     8099 2024-05-11 02:30:33.736965 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_scattered.py
+-rwxr-xr-x   0        0        0    13682 2024-05-11 02:30:33.739745 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_slide.py
+-rwxr-xr-x   0        0        0    14154 2024-05-11 02:30:33.741774 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_spotlights.py
+-rwxr-xr-x   0        0        0    11045 2024-05-11 02:30:33.744093 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_spray.py
+-rwxr-xr-x   0        0        0    15062 2024-05-11 02:30:33.746289 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_swarm.py
+-rwxr-xr-x   0        0        0    20266 2024-05-11 02:30:33.748715 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_synthgrid.py
+-rwxr-xr-x   0        0        0    13906 2024-05-11 02:30:33.750929 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_unstable.py
+-rwxr-xr-x   0        0        0     8383 2024-05-11 02:30:33.752675 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_verticalslice.py
+-rwxr-xr-x   0        0        0    22571 2024-05-11 02:30:33.754914 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_vhstape.py
+-rwxr-xr-x   0        0        0    10335 2024-05-11 02:30:33.756690 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_waves.py
+-rwxr-xr-x   0        0        0     9519 2024-05-11 02:30:33.758437 terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_wipe.py
+-rwxr-xr-x   0        0        0        0 2024-05-05 17:33:51.724578 terminaltexteffects-0.9.1/terminaltexteffects/engine/__init__.py
+-rwxr-xr-x   0        0        0    22748 2024-05-05 17:33:51.741057 terminaltexteffects-0.9.1/terminaltexteffects/engine/animation.py
+-rwxr-xr-x   0        0        0    11162 2024-05-05 17:33:51.752448 terminaltexteffects-0.9.1/terminaltexteffects/engine/base_character.py
+-rwxr-xr-x   0        0        0     4837 2024-05-11 02:30:33.760461 terminaltexteffects-0.9.1/terminaltexteffects/engine/base_effect.py
+-rwxr-xr-x   0        0        0    22354 2024-05-05 17:33:51.800192 terminaltexteffects-0.9.1/terminaltexteffects/engine/motion.py
+-rwxr-xr-x   0        0        0    30452 2024-05-11 11:04:22.775041 terminaltexteffects-0.9.1/terminaltexteffects/engine/terminal.py
+-rwxr-xr-x   0        0        0        0 2024-04-12 11:52:35.092907 terminaltexteffects-0.9.1/terminaltexteffects/py.typed
+-rwxr-xr-x   0        0        0     4780 2024-05-11 02:30:33.763094 terminaltexteffects-0.9.1/terminaltexteffects/template/effect_template.py
+-rwxr-xr-x   0        0        0        0 2023-07-22 17:59:26.632934 terminaltexteffects-0.9.1/terminaltexteffects/utils/__init__.py
+-rwxr-xr-x   0        0        0     2432 2024-05-05 17:33:51.818449 terminaltexteffects-0.9.1/terminaltexteffects/utils/ansitools.py
+-rwxr-xr-x   0        0        0    12883 2024-05-05 17:33:51.829129 terminaltexteffects-0.9.1/terminaltexteffects/utils/argsdataclass.py
+-rwxr-xr-x   0        0        0    15541 2024-05-09 10:47:29.473915 terminaltexteffects-0.9.1/terminaltexteffects/utils/argvalidators.py
+-rwxr-xr-x   0        0        0     2399 2024-05-05 17:33:51.832912 terminaltexteffects-0.9.1/terminaltexteffects/utils/colorterm.py
+-rwxr-xr-x   0        0        0    13639 2024-05-05 17:33:51.833389 terminaltexteffects-0.9.1/terminaltexteffects/utils/easing.py
+-rwxr-xr-x   0        0        0        0 2024-04-26 11:00:38.378584 terminaltexteffects-0.9.1/terminaltexteffects/utils/exceptions.py
+-rwxr-xr-x   0        0        0     9843 2024-05-05 17:33:51.833880 terminaltexteffects-0.9.1/terminaltexteffects/utils/geometry.py
+-rwxr-xr-x   0        0        0    10349 2024-05-11 02:41:27.527818 terminaltexteffects-0.9.1/terminaltexteffects/utils/graphics.py
+-rwxr-xr-x   0        0        0     7140 2024-05-05 17:33:51.847877 terminaltexteffects-0.9.1/terminaltexteffects/utils/hexterm.py
+-rw-r--r--   0        0        0    13342 1970-01-01 00:00:00.000000 terminaltexteffects-0.9.1/PKG-INFO
```

### Comparing `terminaltexteffects-0.9.0/LICENSE` & `terminaltexteffects-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/README.md` & `terminaltexteffects-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,31 +67,33 @@
 
 <details>
 
 <summary>TTE Command Line Options</summary>
 
 ```markdown
 options:
--h, --help            show this help message and exit
+  -h, --help            show this help message and exit
   --tab-width (int > 0)
                         Number of spaces to use for a tab character. (default: 4)
   --xterm-colors        Convert any colors specified in RBG hex to the closest XTerm-256 color. (default: False)
   --no-color            Disable all colors in the effect. (default: False)
   --wrap-text           Wrap text wider than the output area width. (default: False)
   --frame-rate FRAME_RATE
                         Target frame rate for the animation. (default: 100)
-  --terminal-dimensions TERMINAL_DIMENSIONS TERMINAL_DIMENSIONS
-                        Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal
-                        width. (default: (0, 0))
+  --terminal-width TERMINAL_WIDTH
+                        Terminal width, if set to 0 the terminal width is detected automatically. (default: 0)
+  --terminal-height TERMINAL_HEIGHT
+                        Terminal height, if set to 0 the terminal height is detected automatically. (default: 0)
   --ignore-terminal-dimensions
                         Ignore the terminal dimensions and use the input data dimensions for the output area. (default: False)
+
 Effect:
   Name of the effect to apply. Use <effect> -h for effect specific help.
 
-  {beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,dev,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,test,unstable,verticalslice,vhstape,waves,wipe}
+  {beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,unstable,verticalslice,vhstape,waves,wipe}
                         Available Effects
     beams               Create beams which travel over the output area illuminating the characters behind them.
     binarypath          Binary representations of each character move through the terminal towards the home coordinate of the character.
     blackhole           Characters are consumed by a black hole and explode outwards.
     bouncyballs         Characters are bouncy balls falling from the top of the output area.
     bubbles             Characters are formed into bubbles that float down and pop.
     burn                Burns vertically in the output area.
@@ -104,27 +106,27 @@
     orbittingvolley     Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.
     overflow            Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered.
     pour                Pours the characters into position from the given direction.
     print               Lines are printed one at a time following a print head. Print head performs line feed, carriage return.
     rain                Rain characters from the top of the output area.
     randomsequence      Prints the input data in a random sequence.
     rings               Characters are dispersed and form into spinning rings.
-    scattered           Move the characters into place from random starting locations.
+    scattered           Text is scattered across the output area and moves into position.
     slide               Slide characters into view from outside the terminal.
     spotlights          Spotlights search the text area, illuminating characters, before converging in the center and expanding.
     spray               Draws the characters spawning at varying rates from a single point.
     swarm               Characters are grouped into swarms and move around the terminal before settling into position.
     synthgrid           Create a grid which fills with characters dissolving into the final text.
     unstable            Spawn characters jumbled, explode them to the edge of the output area, then reassemble them in the correct layout.
     verticalslice       Slices the input in half vertically and slides it into place from opposite directions.
     vhstape             Lines of characters glitch left and right and lose detail like an old VHS tape.
     waves               Waves travel across the terminal leaving behind the characters.
     wipe                Wipes the text across the terminal to reveal characters.
 
-Ex: ls -a | tte crumble --final-gradient-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction diagonal
+Ex: ls -a | python -m terminaltexteffects decrypt --typing-speed 2 --ciphertext-colors 008000 00cb00 00ff00 --final-gradient-stops eda000 --final-gradient-steps 12 --final-gradient-direction vertical
 ```
 
 </details>
 
 ```cat your_text | tte <effect> [options]```
 
 OR
@@ -239,30 +241,53 @@
 
 ## In-Development Preview
 
 Any effects shown below are in development and will be available in the next release.
 
 ## Latest Release Notes
 
-## 0.9.0
+## 0.9.1
 
 ---
 
-### New Features (0.9.0)
+### New Features (0.9.1)
+
+---
+
+#### New Engine Features (0.9.1)
+
+* Terminal dimension auto-detection supports automatically detecting a single dimensions.
+
+### Changes (0.9.1)
 
 ---
 
-#### New Engine Features (0.9.0)
+#### Effects Changes (0.9.1)
+
+* All effects have been updated to use the new `update()` method and `frame` property of
+  `base_effect.BaseEffectIterator`. See Engine Changes for more info.
+
+#### Engine Changes (0.9.1)
+
+* `base_effect.BaseEffectIterator` now has an `update()` method which calls the `tick()` method of all active characters
+  and manages the `active_characters` list.
+* `base_effect.BaseEffectIterator` has a `frame` property which calls `Terminal.get_formatted_output_string()` and
+  returns the string.
+* `TerminalConfig.terminal_dimensions` has been split into `TerminalConfig.terminal_width` and
+  `TerminalConfig.terminal_height` to simply the command line argument for dimensions and make it more obvious which
+  dimensions is being specified when interacting with `effect.terminal_config`.
+
+#### Other Changes (0.9.1)
 
-* Linear easing function added.
+* Updated help output for `--terminal-dimensions` argument.
 
-### Changes (0.9.0)
+### Bug Fixes (0.9.1)
 
 ---
 
-#### Other Changes (0.9.0)
+#### Engine Fixes (0.9.1)
 
-* Major re-organization of the codebase and significant documentation changes and additions.
+* Fixed division by zero error when the terminal height was set to 1.
 
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/main/LICENSE.md) for more information.
```

#### html2text {}

```diff
@@ -39,22 +39,22 @@
 full installation and usage guide. ### Application Quickstart #### Options TTE
 Command Line Options ```markdown options: -h, --help show this help message and
 exit --tab-width (int > 0) Number of spaces to use for a tab character.
 (default: 4) --xterm-colors Convert any colors specified in RBG hex to the
 closest XTerm-256 color. (default: False) --no-color Disable all colors in the
 effect. (default: False) --wrap-text Wrap text wider than the output area
 width. (default: False) --frame-rate FRAME_RATE Target frame rate for the
-animation. (default: 100) --terminal-dimensions TERMINAL_DIMENSIONS
-TERMINAL_DIMENSIONS Use the terminal dimensions to limit the size of the output
-area and support wrapping. If False, the output area is determined by the input
-data dimensions and may overflow the terminal width. (default: (0, 0)) --
-ignore-terminal-dimensions Ignore the terminal dimensions and use the input
-data dimensions for the output area. (default: False) Effect: Name of the
-effect to apply. Use -h for effect specific help.
-{beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,dev,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,test,unstable,verticalslice,vhstape,waves,wipe}
+animation. (default: 100) --terminal-width TERMINAL_WIDTH Terminal width, if
+set to 0 the terminal width is detected automatically. (default: 0) --terminal-
+height TERMINAL_HEIGHT Terminal height, if set to 0 the terminal height is
+detected automatically. (default: 0) --ignore-terminal-dimensions Ignore the
+terminal dimensions and use the input data dimensions for the output area.
+(default: False) Effect: Name of the effect to apply. Use -h for effect
+specific help.
+{beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,unstable,verticalslice,vhstape,waves,wipe}
 Available Effects beams Create beams which travel over the output area
 illuminating the characters behind them. binarypath Binary representations of
 each character move through the terminal towards the home coordinate of the
 character. blackhole Characters are consumed by a black hole and explode
 outwards. bouncyballs Characters are bouncy balls falling from the top of the
 output area. bubbles Characters are formed into bubbles that float down and
 pop. burn Burns vertically in the output area. crumble Characters lose color
@@ -67,29 +67,30 @@
 volleys of characters inward to build the input text from the center out.
 overflow Input text overflows ands scrolls the terminal in a random order until
 eventually appearing ordered. pour Pours the characters into position from the
 given direction. print Lines are printed one at a time following a print head.
 Print head performs line feed, carriage return. rain Rain characters from the
 top of the output area. randomsequence Prints the input data in a random
 sequence. rings Characters are dispersed and form into spinning rings.
-scattered Move the characters into place from random starting locations. slide
-Slide characters into view from outside the terminal. spotlights Spotlights
-search the text area, illuminating characters, before converging in the center
-and expanding. spray Draws the characters spawning at varying rates from a
-single point. swarm Characters are grouped into swarms and move around the
-terminal before settling into position. synthgrid Create a grid which fills
+scattered Text is scattered across the output area and moves into position.
+slide Slide characters into view from outside the terminal. spotlights
+Spotlights search the text area, illuminating characters, before converging in
+the center and expanding. spray Draws the characters spawning at varying rates
+from a single point. swarm Characters are grouped into swarms and move around
+the terminal before settling into position. synthgrid Create a grid which fills
 with characters dissolving into the final text. unstable Spawn characters
 jumbled, explode them to the edge of the output area, then reassemble them in
 the correct layout. verticalslice Slices the input in half vertically and
 slides it into place from opposite directions. vhstape Lines of characters
 glitch left and right and lose detail like an old VHS tape. waves Waves travel
 across the terminal leaving behind the characters. wipe Wipes the text across
-the terminal to reveal characters. Ex: ls -a | tte crumble --final-gradient-
-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction
-diagonal ``` ```cat your_text | tte [options]``` OR ```cat your_text | python -
+the terminal to reveal characters. Ex: ls -a | python -m terminaltexteffects
+decrypt --typing-speed 2 --ciphertext-colors 008000 00cb00 00ff00 --final-
+gradient-stops eda000 --final-gradient-steps 12 --final-gradient-direction
+vertical ``` ```cat your_text | tte [options]``` OR ```cat your_text | python -
 m terminaltexteffects [options]``` * Use ``` -h``` to view options for a
 specific effect, such as color or movement direction. * Ex: ```tte decrypt -
 h``` For more information, view the [Application Usage Guide](https://
 chrisbuilds.github.io/terminaltexteffects/appguide/). ### Library Quickstart
 All effects are iterators which return a string representing the current frame.
 Basic usage is as simple as importing the effect, instantiating it with the
 input text, and iterating over the effect. ```python from
@@ -132,13 +133,25 @@
 057338f4e007) #### Swarm ![swarm_demo](https://github.com/ChrisBuilds/
 terminaltexteffects/assets/57874186/305e8390-a0fb-4edb-a541-7b52cef77c09) ####
 VHSTape ![vhstape_demo](https://github.com/ChrisBuilds/terminaltexteffects/
 assets/57874186/720abbf4-f97d-4ce9-96ee-15ef973488d2) #### Waves ![waves_demo]
 (https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/ea9b04ca-
 e526-4c7e-b98d-a98a42f7137f) ## In-Development Preview Any effects shown below
 are in development and will be available in the next release. ## Latest Release
-Notes ## 0.9.0 --- ### New Features (0.9.0) --- #### New Engine Features
-(0.9.0) * Linear easing function added. ### Changes (0.9.0) --- #### Other
-Changes (0.9.0) * Major re-organization of the codebase and significant
-documentation changes and additions. ## License Distributed under the MIT
-License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/
-main/LICENSE.md) for more information.
+Notes ## 0.9.1 --- ### New Features (0.9.1) --- #### New Engine Features
+(0.9.1) * Terminal dimension auto-detection supports automatically detecting a
+single dimensions. ### Changes (0.9.1) --- #### Effects Changes (0.9.1) * All
+effects have been updated to use the new `update()` method and `frame` property
+of `base_effect.BaseEffectIterator`. See Engine Changes for more info. ####
+Engine Changes (0.9.1) * `base_effect.BaseEffectIterator` now has an `update()`
+method which calls the `tick()` method of all active characters and manages the
+`active_characters` list. * `base_effect.BaseEffectIterator` has a `frame`
+property which calls `Terminal.get_formatted_output_string()` and returns the
+string. * `TerminalConfig.terminal_dimensions` has been split into
+`TerminalConfig.terminal_width` and `TerminalConfig.terminal_height` to simply
+the command line argument for dimensions and make it more obvious which
+dimensions is being specified when interacting with `effect.terminal_config`.
+#### Other Changes (0.9.1) * Updated help output for `--terminal-dimensions`
+argument. ### Bug Fixes (0.9.1) --- #### Engine Fixes (0.9.1) * Fixed division
+by zero error when the terminal height was set to 1. ## License Distributed
+under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/
+terminaltexteffects/blob/main/LICENSE.md) for more information.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/__main__.py` & `terminaltexteffects-0.9.1/terminaltexteffects/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from terminaltexteffects.utils.argsdataclass import ArgsDataClass
 
 
 def main():
     parser = (argparse.ArgumentParser)(
         prog="terminaltexteffects",
         description="Apply visual effects to terminal text piped in from stdin.",
-        epilog="Ex: ls -a | python -m terminaltexteffects --xterm-colors decrypt -a 0.002 --ciphertext-color 00ff00 --plaintext-color ff0000 --final-color 0000ff",
+        epilog="Ex: ls -a | python -m terminaltexteffects decrypt --typing-speed 2 --ciphertext-colors 008000 00cb00 00ff00 --final-gradient-stops eda000 --final-gradient-steps 12 --final-gradient-direction vertical",
     )
 
     TerminalConfig._add_args_to_parser(parser)
 
     subparsers = parser.add_subparsers(
         title="Effect",
         description="Name of the effect to apply. Use <effect> -h for effect specific help.",
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_beams.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_beams.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
     @classmethod
     def get_effect_class(cls):
         return Beams
 
 
 class BeamsIterator(BaseEffectIterator[BeamsConfig]):
-    class _Group:
+    class Group:
         def __init__(self, characters: list[EffectCharacter], direction: str, terminal: Terminal, args: BeamsConfig):
             self.characters = characters
             self.direction: str = direction
             self.terminal = terminal
             direction_speed_range = {
                 "row": (args.beam_row_speed_range[0], args.beam_row_speed_range[1]),
                 "column": (args.beam_column_speed_range[0], args.beam_column_speed_range[1]),
@@ -225,104 +225,100 @@
             return return_value
 
         def complete(self) -> bool:
             return not self.characters
 
     def __init__(self, effect: "Beams") -> None:
         super().__init__(effect)
-        self._pending_groups: list[BeamsIterator._Group] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._active_groups: list[BeamsIterator._Group] = []
-        self._delay = 0
-        self._phase = "beams"
-        self._final_wipe_groups = self._terminal.get_characters_grouped(
+        self.pending_groups: list[BeamsIterator.Group] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.active_groups: list[BeamsIterator.Group] = []
+        self.delay = 0
+        self.phase = "beams"
+        self.final_wipe_groups = self.terminal.get_characters_grouped(
             Terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT
         )
-        self._build()
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters(fill_chars=True):
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters(fill_chars=True):
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
 
-        beam_gradient = graphics.Gradient(*self._config.beam_gradient_stops, steps=self._config.beam_gradient_steps)
-        groups: list[BeamsIterator._Group] = []
-        for row in self._terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True):
-            groups.append(BeamsIterator._Group(row, "row", self._terminal, self._config))
-        for column in self._terminal.get_characters_grouped(
+        beam_gradient = graphics.Gradient(*self.config.beam_gradient_stops, steps=self.config.beam_gradient_steps)
+        groups: list[BeamsIterator.Group] = []
+        for row in self.terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True):
+            groups.append(BeamsIterator.Group(row, "row", self.terminal, self.config))
+        for column in self.terminal.get_characters_grouped(
             Terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT, fill_chars=True
         ):
-            groups.append(BeamsIterator._Group(column, "column", self._terminal, self._config))
+            groups.append(BeamsIterator.Group(column, "column", self.terminal, self.config))
         for group in groups:
             for character in group.characters:
                 beam_row_scn = character.animation.new_scene(id="beam_row")
                 beam_column_scn = character.animation.new_scene(id="beam_column")
                 beam_row_scn.apply_gradient_to_symbols(
-                    beam_gradient, self._config.beam_row_symbols, self._config.beam_gradient_frames
+                    beam_gradient, self.config.beam_row_symbols, self.config.beam_gradient_frames
                 )
                 beam_column_scn.apply_gradient_to_symbols(
-                    beam_gradient, self._config.beam_column_symbols, self._config.beam_gradient_frames
+                    beam_gradient, self.config.beam_column_symbols, self.config.beam_gradient_frames
                 )
                 faded_color = character.animation.adjust_color_brightness(
-                    self._character_final_color_map[character], 0.3
+                    self.character_final_color_map[character], 0.3
                 )
-                fade_gradient = graphics.Gradient(self._character_final_color_map[character], faded_color, steps=10)
+                fade_gradient = graphics.Gradient(self.character_final_color_map[character], faded_color, steps=10)
                 beam_row_scn.apply_gradient_to_symbols(fade_gradient, character.input_symbol, 5)
                 beam_column_scn.apply_gradient_to_symbols(fade_gradient, character.input_symbol, 5)
-                brighten_gradient = graphics.Gradient(faded_color, self._character_final_color_map[character], steps=10)
+                brighten_gradient = graphics.Gradient(faded_color, self.character_final_color_map[character], steps=10)
                 brigthen_scn = character.animation.new_scene(id="brighten")
                 brigthen_scn.apply_gradient_to_symbols(
-                    brighten_gradient, character.input_symbol, self._config.final_gradient_frames
+                    brighten_gradient, character.input_symbol, self.config.final_gradient_frames
                 )
-        self._pending_groups = groups
-        random.shuffle(self._pending_groups)
+        self.pending_groups = groups
+        random.shuffle(self.pending_groups)
 
     def __next__(self) -> str:
-        if self._phase != "complete" or self._active_chars:
-            if self._phase == "beams":
-                if not self._delay:
-                    if self._pending_groups:
+        if self.phase != "complete" or self.active_characters:
+            if self.phase == "beams":
+                if not self.delay:
+                    if self.pending_groups:
                         for _ in range(random.randint(1, 5)):
-                            if self._pending_groups:
-                                self._active_groups.append(self._pending_groups.pop(0))
-                    self._delay = self._config.beam_delay
+                            if self.pending_groups:
+                                self.active_groups.append(self.pending_groups.pop(0))
+                    self.delay = self.config.beam_delay
                 else:
-                    self._delay -= 1
-                for group in self._active_groups:
+                    self.delay -= 1
+                for group in self.active_groups:
                     group.increment_next_character_counter()
                     if int(group.next_character_counter) > 1:
                         for _ in range(int(group.next_character_counter)):
                             if not group.complete():
                                 next_char = group.get_next_character()
                                 if next_char:
-                                    self._active_chars.append(next_char)
-                self._active_groups = [group for group in self._active_groups if not group.complete()]
-                if not self._pending_groups and not self._active_groups and not self._active_chars:
-                    self._phase = "final_wipe"
-            elif self._phase == "final_wipe":
-                if self._final_wipe_groups:
-                    for _ in range(self._config.final_wipe_speed):
-                        if not self._final_wipe_groups:
+                                    self.active_characters.append(next_char)
+                self.active_groups = [group for group in self.active_groups if not group.complete()]
+                if not self.pending_groups and not self.active_groups and not self.active_characters:
+                    self.phase = "final_wipe"
+            elif self.phase == "final_wipe":
+                if self.final_wipe_groups:
+                    for _ in range(self.config.final_wipe_speed):
+                        if not self.final_wipe_groups:
                             break
-                        next_group = self._final_wipe_groups.pop(0)
+                        next_group = self.final_wipe_groups.pop(0)
                         for character in next_group:
                             character.animation.activate_scene(character.animation.query_scene("brighten"))
-                            self._terminal.set_character_visibility(character, True)
-                            self._active_chars.append(character)
+                            self.terminal.set_character_visibility(character, True)
+                            self.active_characters.append(character)
                 else:
-                    self._phase = "complete"
-            next_frame = self._terminal.get_formatted_output_string()
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+                    self.phase = "complete"
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Beams(BaseEffect[BeamsConfig]):
     """Creates beams which travel over the output area illuminating the characters.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_binarypath.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_binarypath.py`

 * *Files 9% similar despite different names*

```diff
@@ -132,46 +132,45 @@
 
         def _activate_source_character(self) -> None:
             self.terminal.set_character_visibility(self.character, True)
             self.character.animation.activate_scene(self.character.animation.query_scene("collapse_scn"))
 
     def __init__(self, effect: "BinaryPath") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._pending_binary_representations: list[BinaryPathIterator._BinaryRepresentation] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._last_frame_provided = False
-        self._active_binary_reps: list[BinaryPathIterator._BinaryRepresentation] = []
-        self._complete = False
-        self._phase = "travel"
-        self._final_wipe_chars = self._terminal.get_characters_grouped(
-            grouping=self._terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT
+        self.pending_chars: list[EffectCharacter] = []
+        self.pending_binary_representations: list[BinaryPathIterator._BinaryRepresentation] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.last_frame_provided = False
+        self.active_binary_reps: list[BinaryPathIterator._BinaryRepresentation] = []
+        self.complete = False
+        self.phase = "travel"
+        self.final_wipe_chars = self.terminal.get_characters_grouped(
+            grouping=self.terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT
         )
-        self._max_active_binary_groups: int = 0
-        self._build()
+        self.max_active_binary_groups: int = 0
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
 
-        for character in self._terminal.get_characters():
-            bin_rep = BinaryPathIterator._BinaryRepresentation(character, self._terminal)
+        for character in self.terminal.get_characters():
+            bin_rep = BinaryPathIterator._BinaryRepresentation(character, self.terminal)
             for binary_char in bin_rep.binary_string:
-                bin_rep.binary_characters.append(self._terminal.add_character(binary_char, Coord(0, 0)))
+                bin_rep.binary_characters.append(self.terminal.add_character(binary_char, Coord(0, 0)))
                 bin_rep.pending_binary_characters.append(bin_rep.binary_characters[-1])
-            self._pending_binary_representations.append(bin_rep)
+            self.pending_binary_representations.append(bin_rep)
 
-        for bin_rep in self._pending_binary_representations:
+        for bin_rep in self.pending_binary_representations:
             path_coords: list[Coord] = []
-            starting_coord = self._terminal.output_area.random_coord(outside_scope=True)
+            starting_coord = self.terminal.output_area.random_coord(outside_scope=True)
             path_coords.append(starting_coord)
             last_orientation = random.choice(("col", "row"))
             while path_coords[-1] != bin_rep.character.input_coord:
                 last_coord = path_coords[-1]
                 if last_coord.column > bin_rep.character.input_coord.column:
                     column_direction = -1
                 elif last_coord.column == bin_rep.character.input_coord.column:
@@ -187,15 +186,15 @@
                 max_column_distance = abs(last_coord.column - bin_rep.character.input_coord.column)
                 max_row_distance = abs(last_coord.row - bin_rep.character.input_coord.row)
                 if last_orientation == "col" and max_row_distance > 0:
                     next_coord = Coord(
                         last_coord.column,
                         last_coord.row
                         + (
-                            random.randint(1, min(max_row_distance, max(10, int(self._terminal._input_width * 0.2))))
+                            random.randint(1, min(max_row_distance, max(10, int(self.terminal._input_width * 0.2))))
                             * row_direction
                         ),
                     )
                     last_orientation = "row"
                 elif last_orientation == "row" and max_column_distance > 0:
                     next_coord = Coord(
                         last_coord.column + (random.randint(1, min(max_column_distance, 4)) * column_direction),
@@ -208,85 +207,83 @@
                 path_coords.append(next_coord)
 
             path_coords.append(next_coord)
             final_coord = bin_rep.character.input_coord
             path_coords.append(final_coord)
             for bin_effectchar in bin_rep.binary_characters:
                 bin_effectchar.motion.set_coordinate(path_coords[0])
-                digital_path = bin_effectchar.motion.new_path(speed=self._config.movement_speed)
+                digital_path = bin_effectchar.motion.new_path(speed=self.config.movement_speed)
                 for coord in path_coords:
                     digital_path.new_waypoint(coord)
                 bin_effectchar.motion.activate_path(digital_path)
                 bin_effectchar.layer = 1
                 color_scn = bin_effectchar.animation.new_scene()
-                color_scn.add_frame(bin_effectchar.symbol, 1, color=random.choice(self._config.binary_colors))
+                color_scn.add_frame(bin_effectchar.symbol, 1, color=random.choice(self.config.binary_colors))
                 bin_effectchar.animation.activate_scene(color_scn)
 
-        for character in self._terminal.get_characters():
+        for character in self.terminal.get_characters():
             collapse_scn = character.animation.new_scene(ease=easing.in_quad, id="collapse_scn")
-            dim_color = character.animation.adjust_color_brightness(self._character_final_color_map[character], 0.5)
+            dim_color = character.animation.adjust_color_brightness(self.character_final_color_map[character], 0.5)
             dim_gradient = graphics.Gradient("ffffff", dim_color, steps=10)
             collapse_scn.apply_gradient_to_symbols(dim_gradient, character.input_symbol, 7)
 
             brighten_scn = character.animation.new_scene(id="brighten_scn")
-            brighten_gradient = graphics.Gradient(dim_color, self._character_final_color_map[character], steps=10)
+            brighten_gradient = graphics.Gradient(dim_color, self.character_final_color_map[character], steps=10)
             brighten_scn.apply_gradient_to_symbols(brighten_gradient, character.input_symbol, 2)
-        self._max_active_binary_groups = max(
-            1, int(self._config.active_binary_groups * len(self._pending_binary_representations))
+        self.max_active_binary_groups = max(
+            1, int(self.config.active_binary_groups * len(self.pending_binary_representations))
         )
 
     def __next__(self) -> str:
-        if not self._complete or self._active_chars:
-            if self._phase == "travel":
+        if not self.complete or self.active_characters:
+            if self.phase == "travel":
                 while (
-                    len(self._active_binary_reps) < self._max_active_binary_groups
-                    and self._pending_binary_representations
+                    len(self.active_binary_reps) < self.max_active_binary_groups and self.pending_binary_representations
                 ):
-                    next_binary_rep = self._pending_binary_representations.pop(
-                        random.randrange(len(self._pending_binary_representations))
+                    next_binary_rep = self.pending_binary_representations.pop(
+                        random.randrange(len(self.pending_binary_representations))
                     )
                     next_binary_rep.is_active = True
-                    self._active_binary_reps.append(next_binary_rep)
+                    self.active_binary_reps.append(next_binary_rep)
 
-                if self._active_binary_reps:
-                    for active_rep in self._active_binary_reps:
+                if self.active_binary_reps:
+                    for active_rep in self.active_binary_reps:
                         if active_rep.pending_binary_characters:
                             next_char = active_rep.pending_binary_characters.pop(0)
-                            self._active_chars.append(next_char)
-                            self._terminal.set_character_visibility(next_char, True)
+                            self.active_characters.append(next_char)
+                            self.terminal.set_character_visibility(next_char, True)
                         elif active_rep._travel_complete():
                             active_rep._deactivate()
                             active_rep._activate_source_character()
-                            self._active_chars.append(active_rep.character)
+                            self.active_characters.append(active_rep.character)
 
-                    self._active_binary_reps = [
-                        binary_rep for binary_rep in self._active_binary_reps if binary_rep.is_active
+                    self.active_binary_reps = [
+                        binary_rep for binary_rep in self.active_binary_reps if binary_rep.is_active
                     ]
 
-                if not self._active_chars:
-                    self._phase = "wipe"
+                if not self.active_characters:
+                    self.phase = "wipe"
 
-            if self._phase == "wipe":
-                if self._final_wipe_chars:
-                    next_group = self._final_wipe_chars.pop(0)
+            if self.phase == "wipe":
+                if self.final_wipe_chars:
+                    next_group = self.final_wipe_chars.pop(0)
                     for character in next_group:
                         character.animation.activate_scene(character.animation.query_scene("brighten_scn"))
-                        self._terminal.set_character_visibility(character, True)
-                        self._active_chars.append(character)
+                        self.terminal.set_character_visibility(character, True)
+                        self.active_characters.append(character)
                 else:
-                    self._complete = True
-            next_frame = self._terminal.get_formatted_output_string()
-            for character in self._active_chars:
-                character.tick()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
-        elif not self._last_frame_provided:
-            self._last_frame_provided = True
-            return self._terminal.get_formatted_output_string()
+                    self.complete = True
+
+            self.update()
+            return self.frame
+
+        elif not self.last_frame_provided:
+            self.last_frame_provided = True
+            return self.frame
+
         else:
             raise StopIteration
 
 
 class BinaryPath(BaseEffect):
     """Decodes characters into their binary form. Characters travel from outside the output area towards their input coordinate, moving at right angles.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_blackhole.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_blackhole.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,29 +99,28 @@
     def get_effect_class(cls):
         return Blackhole
 
 
 class BlackholeIterator(BaseEffectIterator[BlackholeConfig]):
     def __init__(self, effect: "Blackhole") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._blackhole_chars: list[EffectCharacter] = []
-        self._awaiting_consumption_chars: list[EffectCharacter] = []
-        self._blackhole_radius = max(
+        self.pending_chars: list[EffectCharacter] = []
+        self.blackhole_chars: list[EffectCharacter] = []
+        self.awaiting_consumption_chars: list[EffectCharacter] = []
+        self.blackhole_radius = max(
             min(
-                round(self._terminal.output_area.right * 0.3),
-                round(self._terminal.output_area.top * 0.3),
+                round(self.terminal.output_area.right * 0.3),
+                round(self.terminal.output_area.top * 0.3),
             ),
             3,
         )
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _prepare_blackhole(self) -> None:
+    def prepare_blackhole(self) -> None:
         star_symbols = [
             "*",
             "✸",
             "✺",
             "✹",
             "✷",
             "✵",
@@ -138,71 +137,71 @@
             "⬦",
             "⬥",
         ]
         starfield_colors = graphics.Gradient("4a4a4d", "ffffff", steps=6).spectrum
         gradient_map = {}
         for color in starfield_colors:
             gradient_map[color] = graphics.Gradient(color, "000000", steps=10)
-        available_chars = list(self._terminal._input_characters)
-        while len(self._blackhole_chars) < self._blackhole_radius * 3 and available_chars:
-            self._blackhole_chars.append(available_chars.pop(random.randrange(0, len(available_chars))))
+        available_chars = list(self.terminal._input_characters)
+        while len(self.blackhole_chars) < self.blackhole_radius * 3 and available_chars:
+            self.blackhole_chars.append(available_chars.pop(random.randrange(0, len(available_chars))))
         black_hole_ring_positions = geometry.find_coords_on_circle(
-            self._terminal.output_area.center,
-            self._blackhole_radius,
-            len(self._blackhole_chars),
+            self.terminal.output_area.center,
+            self.blackhole_radius,
+            len(self.blackhole_chars),
         )
-        for position_index, character in enumerate(self._blackhole_chars):
+        for position_index, character in enumerate(self.blackhole_chars):
             starting_pos = black_hole_ring_positions[position_index]
             blackhole_path = character.motion.new_path(id="blackhole", speed=0.5, ease=easing.in_out_sine)
             blackhole_path.new_waypoint(starting_pos)
             blackhole_scn = character.animation.new_scene(id="blackhole")
-            blackhole_scn.add_frame("✸", 1, color=self._config.blackhole_color)
+            blackhole_scn.add_frame("✸", 1, color=self.config.blackhole_color)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_ACTIVATED,
                 blackhole_path,
                 EventHandler.Action.SET_LAYER,
                 1,
             )
             # make rotation waypoints
             blackhole_rotation_path = character.motion.new_path(id="blackhole_rotation", speed=0.2, loop=True)
             for coord in black_hole_ring_positions[position_index:] + black_hole_ring_positions[:position_index]:
                 blackhole_rotation_path.new_waypoint(coord, id=str(len(blackhole_rotation_path.waypoints)))
-        for character in self._terminal.get_characters():
-            self._terminal.set_character_visibility(character, True)
+        for character in self.terminal.get_characters():
+            self.terminal.set_character_visibility(character, True)
             starting_scn = character.animation.new_scene()
             star_symbol = random.choice(star_symbols)
             star_color = random.choice(starfield_colors)
             starting_scn.add_frame(star_symbol, 1, color=star_color)
             character.animation.activate_scene(starting_scn)
-            if character not in self._blackhole_chars:
-                starfield_coord = self._terminal.output_area.random_coord()
+            if character not in self.blackhole_chars:
+                starfield_coord = self.terminal.output_area.random_coord()
                 character.motion.set_coordinate(starfield_coord)
-                if starfield_coord.row > self._terminal.output_area.center_row:
+                if starfield_coord.row > self.terminal.output_area.center_row:
                     if starfield_coord.column in range(
-                        round(self._terminal.output_area.right * 0.4),
-                        round(self._terminal.output_area.right * 0.7),
+                        round(self.terminal.output_area.right * 0.4),
+                        round(self.terminal.output_area.right * 0.7),
                     ):
                         # if within the top center 40% of the screen
-                        control_point = Coord(self._terminal.output_area.center.column, starfield_coord.row)
+                        control_point = Coord(self.terminal.output_area.center.column, starfield_coord.row)
                     else:
-                        control_point = Coord(starfield_coord.column, self._terminal.output_area.center_row)
+                        control_point = Coord(starfield_coord.column, self.terminal.output_area.center_row)
 
-                elif starfield_coord.row < self._terminal.output_area.center_row:
+                elif starfield_coord.row < self.terminal.output_area.center_row:
                     if starfield_coord.column in range(
-                        round(self._terminal.output_area.right * 0.4),
-                        round(self._terminal.output_area.right * 0.7),
+                        round(self.terminal.output_area.right * 0.4),
+                        round(self.terminal.output_area.right * 0.7),
                     ):
                         # if within the bottom center 40% of the screen
-                        control_point = Coord(self._terminal.output_area.center.column, starfield_coord.row)
+                        control_point = Coord(self.terminal.output_area.center.column, starfield_coord.row)
                     else:
-                        control_point = Coord(starfield_coord.column, self._terminal.output_area.center_row)
+                        control_point = Coord(starfield_coord.column, self.terminal.output_area.center_row)
                 else:
-                    control_point = self._terminal.output_area.center
+                    control_point = self.terminal.output_area.center
                 singularity_path = character.motion.new_path(id="singularity", speed=0.3, ease=easing.in_expo)
-                singularity_path.new_waypoint(self._terminal.output_area.center, bezier_control=control_point)
+                singularity_path.new_waypoint(self.terminal.output_area.center, bezier_control=control_point)
                 consumed_scn = character.animation.new_scene()
                 for color in gradient_map[star_color]:
                     consumed_scn.add_frame(star_symbol, 1, color=color)
                 consumed_scn.add_frame(" ", 1)
                 consumed_scn.sync = animation.SyncMetric.DISTANCE
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_ACTIVATED,
@@ -212,47 +211,47 @@
                 )
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_ACTIVATED,
                     singularity_path,
                     EventHandler.Action.ACTIVATE_SCENE,
                     consumed_scn,
                 )
-                self._awaiting_consumption_chars.append(character)
-        random.shuffle(self._awaiting_consumption_chars)
+                self.awaiting_consumption_chars.append(character)
+        random.shuffle(self.awaiting_consumption_chars)
 
-    def _rotate_blackhole(self) -> None:
-        for character in self._blackhole_chars:
+    def rotate_blackhole(self) -> None:
+        for character in self.blackhole_chars:
             character.motion.activate_path(character.motion.query_path("blackhole_rotation"))
-            self._active_chars.append(character)
+            self.active_characters.append(character)
 
-    def _collapse_blackhole(self) -> None:
+    def collapse_blackhole(self) -> None:
         black_hole_ring_positions = geometry.find_coords_on_circle(
-            self._terminal.output_area.center,
-            self._blackhole_radius + 3,
-            len(self._blackhole_chars),
+            self.terminal.output_area.center,
+            self.blackhole_radius + 3,
+            len(self.blackhole_chars),
         )
         unstable_symbols = ["◦", "◎", "◉", "●", "◉", "◎", "◦"]
         point_char_made = False
-        for character in self._blackhole_chars:
+        for character in self.blackhole_chars:
             next_pos = black_hole_ring_positions.pop(0)
             expand_path = character.motion.new_path(speed=0.1, ease=easing.in_expo)
             expand_path.new_waypoint(next_pos)
             collapse_path = character.motion.new_path(speed=0.3, ease=easing.in_expo)
-            collapse_path.new_waypoint(self._terminal.output_area.center)
+            collapse_path.new_waypoint(self.terminal.output_area.center)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE,
                 expand_path,
                 EventHandler.Action.ACTIVATE_PATH,
                 collapse_path,
             )
             if not point_char_made:
                 point_scn = character.animation.new_scene()
                 for _ in range(3):
                     for symbol in unstable_symbols:
-                        point_scn.add_frame(symbol, 6, color=random.choice(self._config.star_colors))
+                        point_scn.add_frame(symbol, 6, color=random.choice(self.config.star_colors))
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE,
                     collapse_path,
                     EventHandler.Action.ACTIVATE_SCENE,
                     point_scn,
                 )
                 character.event_handler.register_event(
@@ -260,30 +259,30 @@
                     collapse_path,
                     EventHandler.Action.SET_LAYER,
                     3,
                 )
                 point_char_made = True
 
             character.motion.activate_path(expand_path)
-            self._active_chars.append(character)
+            self.active_characters.append(character)
 
-    def _explode_singularity(self) -> None:
+    def explode_singularity(self) -> None:
         star_colors = ["ffcc0d", "ff7326", "ff194d", "bf2669", "702a8c" "049dbf"]
-        for character in self._terminal.get_characters():
+        for character in self.terminal.get_characters():
             nearby_coord = geometry.find_coords_on_circle(character.input_coord, 3, 5)[random.randrange(0, 5)]
             nearby_path = character.motion.new_path(speed=random.randint(2, 3) / 10, ease=easing.out_expo)
             nearby_path.new_waypoint(nearby_coord)
             input_path = character.motion.new_path(speed=random.randint(3, 5) / 100, ease=easing.in_cubic)
             input_path.new_waypoint(character.input_coord)
             explode_scn = character.animation.new_scene()
             explode_star_color = random.choice(star_colors)
             explode_scn.add_frame(character.input_symbol, 1, color=explode_star_color)
             cooling_scn = character.animation.new_scene()
             cooling_gradient = graphics.Gradient(
-                explode_star_color, self._character_final_color_map[character], steps=10
+                explode_star_color, self.character_final_color_map[character], steps=10
             )
             cooling_scn.apply_gradient_to_symbols(cooling_gradient, character.input_symbol, 20)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE,
                 nearby_path,
                 EventHandler.Action.ACTIVATE_PATH,
                 input_path,
@@ -292,85 +291,81 @@
                 EventHandler.Event.PATH_COMPLETE,
                 nearby_path,
                 EventHandler.Action.ACTIVATE_SCENE,
                 cooling_scn,
             )
             character.animation.activate_scene(explode_scn)
             character.motion.activate_path(nearby_path)
-            self._active_chars.append(character)
+            self.active_characters.append(character)
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        self._prepare_blackhole()
-        self.formation_delay = max(100 // len(self._blackhole_chars), 10)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        self.prepare_blackhole()
+        self.formation_delay = max(100 // len(self.blackhole_chars), 10)
         self.f_delay = self.formation_delay
         self.next_char_consuming_delay = 0
-        self.max_consume = max(min(int(0.1 * len(self._terminal._input_characters)), 15), 2)
+        self.max_consume = max(min(int(0.1 * len(self.terminal._input_characters)), 15), 2)
         self.phase = "forming"
-        self.awaiting_blackhole_chars = list(self._blackhole_chars)
+        self.awaiting_blackhole_chars = list(self.blackhole_chars)
 
     def __next__(self) -> str:
-        if self._active_chars or self.phase != "complete":
+        if self.active_characters or self.phase != "complete":
             if self.phase == "forming":
                 if self.awaiting_blackhole_chars:
                     if not self.f_delay:
                         next_char = self.awaiting_blackhole_chars.pop(0)
                         next_char.motion.activate_path(next_char.motion.query_path("blackhole"))
                         next_char.animation.activate_scene(next_char.animation.query_scene("blackhole"))
-                        self._active_chars.append(next_char)
+                        self.active_characters.append(next_char)
                         self.f_delay = self.formation_delay
                     else:
                         self.f_delay -= 1
                 else:
-                    if not self._active_chars:
-                        self._rotate_blackhole()
+                    if not self.active_characters:
+                        self.rotate_blackhole()
                         self.phase = "consuming"
             elif self.phase == "consuming":
-                if self._awaiting_consumption_chars:
+                if self.awaiting_consumption_chars:
                     if not self.next_char_consuming_delay:
                         for _ in range(random.randrange(1, self.max_consume)):
-                            if self._awaiting_consumption_chars:
-                                next_char = self._awaiting_consumption_chars.pop(0)
+                            if self.awaiting_consumption_chars:
+                                next_char = self.awaiting_consumption_chars.pop(0)
                                 next_char.motion.activate_path(next_char.motion.query_path("singularity"))
-                                self._active_chars.append(next_char)
+                                self.active_characters.append(next_char)
                             else:
                                 break
                         self.max_consume += 1
                         self.next_char_consuming_delay = random.randrange(0, 10)
                     else:
                         self.next_char_consuming_delay -= 1
 
                 else:
-                    if all(character in self._blackhole_chars for character in self._active_chars):
+                    if all(character in self.blackhole_chars for character in self.active_characters):
                         self.phase = "collapsing"
 
             elif self.phase == "collapsing":
-                self._collapse_blackhole()
+                self.collapse_blackhole()
                 self.phase = "exploding"
             elif self.phase == "exploding":
                 if all(
                     [
                         character.motion.active_path is None and character.animation.active_scene is None
-                        for character in self._blackhole_chars
+                        for character in self.blackhole_chars
                     ]
                 ):
-                    self._explode_singularity()
+                    self.explode_singularity()
                     self.phase = "complete"
 
-            for character in self._active_chars:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+            self.update()
+            return self.frame
 
         else:
             raise StopIteration
 
 
 class Blackhole(BaseEffect[BlackholeConfig]):
     """Creates a blackhole in a starfield, consumes the stars, explodes the input data back into position.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_bouncyballs.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_bouncyballs.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,78 +122,75 @@
     def get_effect_class(cls):
         return BouncyBalls
 
 
 class BouncyBallsIterator(BaseEffectIterator[BouncyBallsConfig]):
     def __init__(self, effect: "BouncyBalls"):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._group_by_row: dict[int, list[EffectCharacter | None]] = {}
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.group_by_row: dict[int, list[EffectCharacter | None]] = {}
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            color = random.choice(self._config.ball_colors)
-            symbol = random.choice(self._config.ball_symbols)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            color = random.choice(self.config.ball_colors)
+            symbol = random.choice(self.config.ball_symbols)
             ball_scene = character.animation.new_scene()
             ball_scene.add_frame(symbol, 1, color=color)
             final_scene = character.animation.new_scene()
-            char_final_gradient = graphics.Gradient(color, self._character_final_color_map[character], steps=10)
+            char_final_gradient = graphics.Gradient(color, self.character_final_color_map[character], steps=10)
             final_scene.apply_gradient_to_symbols(char_final_gradient, character.input_symbol, 10)
             character.motion.set_coordinate(
-                Coord(character.input_coord.column, int(self._terminal.output_area.top * random.uniform(1.0, 1.5)))
+                Coord(character.input_coord.column, int(self.terminal.output_area.top * random.uniform(1.0, 1.5)))
             )
             input_coord_path = character.motion.new_path(
-                speed=self._config.movement_speed, ease=self._config.movement_easing
+                speed=self.config.movement_speed, ease=self.config.movement_easing
             )
             input_coord_path.new_waypoint(character.input_coord)
             character.motion.activate_path(input_coord_path)
             character.animation.activate_scene(ball_scene)
             character.event_handler.register_event(
                 character.event_handler.Event.PATH_COMPLETE,
                 input_coord_path,
                 character.event_handler.Action.ACTIVATE_SCENE,
                 final_scene,
             )
-            self._pending_chars.append(character)
-        for character in sorted(self._pending_chars, key=lambda c: c.input_coord.row):
-            if character.input_coord.row not in self._group_by_row:
-                self._group_by_row[character.input_coord.row] = []
-            self._group_by_row[character.input_coord.row].append(character)
-        self._pending_chars.clear()
+            self.pending_chars.append(character)
+        for character in sorted(self.pending_chars, key=lambda c: c.input_coord.row):
+            if character.input_coord.row not in self.group_by_row:
+                self.group_by_row[character.input_coord.row] = []
+            self.group_by_row[character.input_coord.row].append(character)
+        self.pending_chars.clear()
         self.ball_delay = 0
 
     def __next__(self) -> str:
-        if self._group_by_row or self._active_chars or self._pending_chars:
-            if not self._pending_chars and self._group_by_row:
-                self._pending_chars.extend(self._group_by_row.pop(min(self._group_by_row.keys())))  # type: ignore
-            if self._pending_chars:
+        if self.group_by_row or self.active_characters or self.pending_chars:
+            if not self.pending_chars and self.group_by_row:
+                self.pending_chars.extend(self.group_by_row.pop(min(self.group_by_row.keys())))  # type: ignore
+            if self.pending_chars:
                 if self.ball_delay == 0:
                     for _ in range(random.randint(2, 6)):
-                        if self._pending_chars:
-                            next_character = self._pending_chars.pop(random.randint(0, len(self._pending_chars) - 1))
-                            self._terminal.set_character_visibility(next_character, True)
-                            self._active_chars.append(next_character)
+                        if self.pending_chars:
+                            next_character = self.pending_chars.pop(random.randint(0, len(self.pending_chars) - 1))
+                            self.terminal.set_character_visibility(next_character, True)
+                            self.active_characters.append(next_character)
                         else:
                             break
-                    self.ball_delay = self._config.ball_delay
+                    self.ball_delay = self.config.ball_delay
                 else:
                     self.ball_delay -= 1
 
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class BouncyBalls(BaseEffect[BouncyBallsConfig]):
     """Characters fall from the top of the output area as bouncy balls before settling into place.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_bubbles.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_bubbles.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,75 +141,75 @@
 
     @classmethod
     def get_effect_class(cls):
         return Bubbles
 
 
 class BubblesIterator(BaseEffectIterator[BubblesConfig]):
-    class _Bubble:
+    class Bubble:
         def __init__(
             self,
             effect: "BubblesIterator",
             origin: Coord,
             characters: list[EffectCharacter],
             terminal: Terminal,
         ):
             self.effect = effect
             self.characters = characters
             self.terminal = terminal
             self.radius = max(len(self.characters) // 5, 1)
             self.origin = origin
             self.anchor_char = self.terminal.add_character(" ", self.origin)
-            if self.effect._config.pop_condition == "row":
+            if self.effect.config.pop_condition == "row":
                 self.lowest_row = min([char.input_coord.row for char in self.characters])
             else:
-                self.lowest_row = self.effect._terminal.output_area.bottom
+                self.lowest_row = self.effect.terminal.output_area.bottom
             self.set_character_coordinates()
             self.landed = False
             self.make_waypoints()
             self.make_gradients()
 
         def set_character_coordinates(self) -> None:
             for i, char in enumerate(self.characters):
                 point = geometry.find_coords_on_circle(
                     self.anchor_char.motion.current_coord, self.radius, len(self.characters), unique=False
                 )[i]
                 char.motion.set_coordinate(point)
                 if point.row == self.lowest_row:
                     self.landed = True
 
-            if self.effect._config.pop_condition == "anywhere":
+            if self.effect.config.pop_condition == "anywhere":
                 if random.random() < 0.002:
                     self.landed = True
 
         def make_waypoints(self):
             waypoint_column = random.randint(
-                self.effect._terminal.output_area.left, self.effect._terminal.output_area.right
+                self.effect.terminal.output_area.left, self.effect.terminal.output_area.right
             )
-            floor_path = self.anchor_char.motion.new_path(speed=self.effect._config.bubble_speed)
+            floor_path = self.anchor_char.motion.new_path(speed=self.effect.config.bubble_speed)
             floor_path.new_waypoint(Coord(waypoint_column, self.lowest_row))
             self.anchor_char.motion.activate_path(floor_path)
 
         def make_gradients(self) -> None:
-            if self.effect._config.rainbow:
+            if self.effect.config.rainbow:
                 rainbow_gradient = list(self.effect.rainbow_gradient.spectrum)
                 gradient_offset = 0
                 for character in self.characters:
                     sheen_scene = character.animation.new_scene()
                     for step in rainbow_gradient:
                         sheen_scene.add_frame(character.input_symbol, 5, color=step)
                     gradient_offset += 2
                     gradient_offset %= len(rainbow_gradient)
                     rainbow_gradient = rainbow_gradient[gradient_offset:] + rainbow_gradient[:gradient_offset]
                     character.animation.activate_scene(sheen_scene)
                     if character.animation.active_scene:
                         character.animation.active_scene.is_looping = True
 
             else:
-                bubble_color = random.choice(self.effect._config.bubble_colors)
+                bubble_color = random.choice(self.effect.config.bubble_colors)
                 for character in self.characters:
                     sheen_scene = character.animation.new_scene()
                     sheen_scene.add_frame(character.input_symbol, 1, color=bubble_color)
                     character.animation.activate_scene(sheen_scene)
 
         def pop(self) -> None:
             char: EffectCharacter
@@ -242,43 +242,42 @@
             self.anchor_char.motion.move()
             self.set_character_coordinates()
             for character in self.characters:
                 character.animation.step_animation()
 
     def __init__(self, effect: "Bubbles"):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._bubbles: list[BubblesIterator._Bubble] = []
+        self.pending_chars: list[EffectCharacter] = []
+        self.bubbles: list[BubblesIterator.Bubble] = []
         red = "e81416"
         orange = "ffa500"
         yellow = "faeb36"
         green = "79c314"
         blue = "487de7"
         indigo = "4b369d"
         violet = "70369d"
         self.rainbow_gradient = graphics.Gradient(red, orange, yellow, green, blue, indigo, violet, steps=5)
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
             character.layer = 1
             pop_1_scene = character.animation.new_scene(id="pop_1")
             pop_2_scene = character.animation.new_scene()
-            pop_1_scene.add_frame("*", 20, color=self._config.pop_color)
-            pop_2_scene.add_frame("'", 20, color=self._config.pop_color)
+            pop_1_scene.add_frame("*", 20, color=self.config.pop_color)
+            pop_2_scene.add_frame("'", 20, color=self.config.pop_color)
             final_scene = character.animation.new_scene()
             char_final_gradient = graphics.Gradient(
-                self._config.pop_color, self._character_final_color_map[character], steps=10
+                self.config.pop_color, self.character_final_color_map[character], steps=10
             )
             final_scene.apply_gradient_to_symbols(char_final_gradient, character.input_symbol, 10)
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE, pop_1_scene, EventHandler.Action.ACTIVATE_SCENE, pop_2_scene
             )
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
@@ -293,59 +292,54 @@
             )
             final_path.new_waypoint(character.input_coord)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE, final_path, EventHandler.Action.SET_LAYER, 0
             )
 
         unbubbled_chars = []
-        for char_list in self._terminal.get_characters_grouped(
-            grouping=self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP
-        ):
+        for char_list in self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.ROW_BOTTOM_TO_TOP):
             unbubbled_chars.extend(char_list)
-        self._bubbles = []
+        self.bubbles = []
         while unbubbled_chars:
             bubble_group = []
             if len(unbubbled_chars) < 5:
                 bubble_group.extend(unbubbled_chars)
                 unbubbled_chars.clear()
             else:
                 for _ in range(random.randint(5, min(len(unbubbled_chars), 20))):
                     bubble_group.append(unbubbled_chars.pop(0))
             bubble_origin = Coord(
-                random.randint(self._terminal.output_area.left, self._terminal.output_area.right),
-                self._terminal.output_area.top,
+                random.randint(self.terminal.output_area.left, self.terminal.output_area.right),
+                self.terminal.output_area.top,
             )
-            new_bubble = BubblesIterator._Bubble(self, bubble_origin, bubble_group, self._terminal)
-            self._bubbles.append(new_bubble)
-        self.animating_bubbles: list[BubblesIterator._Bubble] = []
+            new_bubble = BubblesIterator.Bubble(self, bubble_origin, bubble_group, self.terminal)
+            self.bubbles.append(new_bubble)
+        self.animating_bubbles: list[BubblesIterator.Bubble] = []
         self.steps_since_last_bubble = 0
 
     def __next__(self) -> str:
-        if self.animating_bubbles or self._active_chars or self._bubbles:
-            if self._bubbles and self.steps_since_last_bubble >= self._config.bubble_delay:
-                next_bubble = self._bubbles.pop(0)
+        if self.animating_bubbles or self.active_characters or self.bubbles:
+            if self.bubbles and self.steps_since_last_bubble >= self.config.bubble_delay:
+                next_bubble = self.bubbles.pop(0)
                 next_bubble.activate()
                 self.animating_bubbles.append(next_bubble)
                 self.steps_since_last_bubble = 0
             self.steps_since_last_bubble += 1
 
             for bubble in self.animating_bubbles:
                 if bubble.landed:
                     bubble.pop()
-                    self._active_chars.extend(bubble.characters)
+                    self.active_characters.extend(bubble.characters)
 
             self.animating_bubbles = [bubble for bubble in self.animating_bubbles if not bubble.landed]
             for bubble in self.animating_bubbles:
                 bubble.move()
-            for character in self._active_chars:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
 
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Bubbles(BaseEffect[BubblesConfig]):
     """Forms bubbles with the characters. Bubbles float down and pop.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_burn.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_burn.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,80 +91,75 @@
     def get_effect_class(cls):
         return Burn
 
 
 class BurnIterator(BaseEffectIterator[BurnConfig]):
     def __init__(self, effect: "Burn"):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
+    def build(self) -> None:
         vertical_build_order = [
             "'",
             ".",
             "▖",
             "▙",
             "█",
             "▜",
             "▀",
             "▝",
             ".",
         ]
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        fire_gradient = graphics.Gradient(*self._config.burn_colors, steps=10)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        fire_gradient = graphics.Gradient(*self.config.burn_colors, steps=10)
         groups = {
             column_index: column
             for column_index, column in enumerate(
-                self._terminal.get_characters_grouped(grouping=self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT)
+                self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT)
             )
         }
 
         def groups_remaining(rows) -> bool:
             return any(row for row in rows.values())
 
         while groups_remaining(groups):
             keys = [key for key in groups.keys() if groups[key]]
             next_char = groups[random.choice(keys)].pop(0)
-            self._terminal.set_character_visibility(next_char, True)
-            next_char.animation.set_appearance(next_char.input_symbol, color=self._config.starting_color)
+            self.terminal.set_character_visibility(next_char, True)
+            next_char.animation.set_appearance(next_char.input_symbol, color=self.config.starting_color)
             burn_scn = next_char.animation.new_scene(id="burn")
             burn_scn.apply_gradient_to_symbols(fire_gradient, vertical_build_order, 12)
             final_color_scn = next_char.animation.new_scene()
             for color in graphics.Gradient(
-                fire_gradient.spectrum[-1], self._character_final_color_map[next_char], steps=8
+                fire_gradient.spectrum[-1], self.character_final_color_map[next_char], steps=8
             ):
                 final_color_scn.add_frame(next_char.input_symbol, 4, color=color)
             next_char.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE, burn_scn, EventHandler.Action.ACTIVATE_SCENE, final_color_scn
             )
 
-            self._pending_chars.append(next_char)
+            self.pending_chars.append(next_char)
 
     def __next__(self) -> str:
-        if self._pending_chars or self._active_chars:
+        if self.pending_chars or self.active_characters:
             for _ in range(random.randint(2, 4)):
-                if self._pending_chars:
-                    next_char = self._pending_chars.pop(0)
+                if self.pending_chars:
+                    next_char = self.pending_chars.pop(0)
                     next_char.animation.activate_scene(next_char.animation.query_scene("burn"))
-                    # self.terminal.set_character_visibility(next_char, True)
-                    self._active_chars.append(next_char)
+                    self.active_characters.append(next_char)
 
-            for character in self._active_chars:
-                character.animation.step_animation()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Burn(BaseEffect[BurnConfig]):
     """Characters are ignited and burn up the screen.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_crumble.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_crumble.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,48 +73,47 @@
         return Crumble
 
 
 class CrumbleIterator(BaseEffectIterator[CrumbleConfig]):
     def __init__(self, effect: "Crumble"):
         super().__init__(effect)
 
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            strengthen_flash_gradient = graphics.Gradient(self._character_final_color_map[character], "ffffff", steps=6)
-            strengthen_gradient = graphics.Gradient("ffffff", self._character_final_color_map[character], steps=9)
-            weak_color = character.animation.adjust_color_brightness(self._character_final_color_map[character], 0.65)
-            dust_color = character.animation.adjust_color_brightness(self._character_final_color_map[character], 0.55)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            strengthen_flash_gradient = graphics.Gradient(self.character_final_color_map[character], "ffffff", steps=6)
+            strengthen_gradient = graphics.Gradient("ffffff", self.character_final_color_map[character], steps=9)
+            weak_color = character.animation.adjust_color_brightness(self.character_final_color_map[character], 0.65)
+            dust_color = character.animation.adjust_color_brightness(self.character_final_color_map[character], 0.55)
             weaken_gradient = graphics.Gradient(weak_color, dust_color, steps=9)
-            self._terminal.set_character_visibility(character, True)
+            self.terminal.set_character_visibility(character, True)
             # set up initial and falling stage
             initial_scn = character.animation.new_scene()
             initial_scn.add_frame(character.input_symbol, 1, color=weak_color)
             character.animation.activate_scene(initial_scn)
             fall_path = character.motion.new_path(
                 speed=0.2,
                 ease=easing.out_bounce,
             )
-            fall_path.new_waypoint(Coord(character.input_coord.column, self._terminal.output_area.bottom))
+            fall_path.new_waypoint(Coord(character.input_coord.column, self.terminal.output_area.bottom))
             weaken_scn = character.animation.new_scene(id="weaken")
             weaken_scn.apply_gradient_to_symbols(weaken_gradient, character.input_symbol, 6)
 
             top_path = character.motion.new_path(id="top", speed=0.5, ease=easing.out_quint)
             top_path.new_waypoint(
-                Coord(character.input_coord.column, self._terminal.output_area.top),
-                bezier_control=Coord(self._terminal.output_area.center_column, self._terminal.output_area.center_row),
+                Coord(character.input_coord.column, self.terminal.output_area.top),
+                bezier_control=Coord(self.terminal.output_area.center_column, self.terminal.output_area.center_row),
             )
             # set up reset stage
             input_path = character.motion.new_path(id="input", speed=0.3)
             input_path.new_waypoint(character.input_coord)
             strengthen_flash_scn = character.animation.new_scene()
             strengthen_flash_scn.apply_gradient_to_symbols(strengthen_flash_gradient, character.input_symbol, 4)
             strengthen_scn = character.animation.new_scene()
@@ -141,72 +140,69 @@
             )
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
                 strengthen_flash_scn,
                 EventHandler.Action.ACTIVATE_SCENE,
                 strengthen_scn,
             )
-            self._pending_chars.append(character)
-        random.shuffle(self._pending_chars)
+            self.pending_chars.append(character)
+        random.shuffle(self.pending_chars)
         self.fall_delay = 20
         self.max_fall_delay = 20
         self.min_fall_delay = 15
         self.reset = False
         self.fall_group_maxsize = 1
         self.stage = "falling"
-        self.unvacuumed_chars = list(self._terminal._input_characters)
+        self.unvacuumed_chars = list(self.terminal._input_characters)
         random.shuffle(self.unvacuumed_chars)
 
     def __next__(self) -> str:
         if self.stage != "complete":
             if self.stage == "falling":
-                if self._pending_chars:
+                if self.pending_chars:
                     if self.fall_delay == 0:
                         # Determine the size of the next group of falling characters
                         fall_group_size = random.randint(1, self.fall_group_maxsize)
                         # Add the next group of falling characters to the animating characters list
                         for _ in range(fall_group_size):
-                            if self._pending_chars:
-                                next_char = self._pending_chars.pop(0)
+                            if self.pending_chars:
+                                next_char = self.pending_chars.pop(0)
                                 next_char.animation.activate_scene(next_char.animation.query_scene("weaken"))
-                                self._active_chars.append(next_char)
+                                self.active_characters.append(next_char)
                         # Reset the fall delay and adjust the fall group size and delay range
                         self.fall_delay = random.randint(self.min_fall_delay, self.max_fall_delay)
                         if random.randint(1, 10) > 4:  # 60% chance to modify the fall delay and group size
                             self.fall_group_maxsize += 1
                             self.min_fall_delay = max(0, self.min_fall_delay - 1)
                             self.max_fall_delay = max(0, self.max_fall_delay - 1)
                     else:
                         self.fall_delay -= 1
-                if not self._pending_chars and not self._active_chars:
+                if not self.pending_chars and not self.active_characters:
                     self.stage = "vacuuming"
             elif self.stage == "vacuuming":
                 if self.unvacuumed_chars:
                     for _ in range(random.randint(3, 10)):
                         if self.unvacuumed_chars:
                             next_char = self.unvacuumed_chars.pop(0)
                             next_char.motion.activate_path(next_char.motion.query_path("top"))
-                            self._active_chars.append(next_char)
-                if not self._active_chars:
+                            self.active_characters.append(next_char)
+                if not self.active_characters:
                     self.stage = "resetting"
 
             elif self.stage == "resetting":
                 if not self.reset:
-                    for character in self._terminal.get_characters():
+                    for character in self.terminal.get_characters():
                         character.motion.activate_path(character.motion.query_path("input"))
-                        self._active_chars.append(character)
+                        self.active_characters.append(character)
                     self.reset = True
-                if not self._active_chars:
+                if not self.active_characters:
                     self.stage = "complete"
 
-            next_frame = self._terminal.get_formatted_output_string()
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Crumble(BaseEffect[CrumbleConfig]):
     """Characters crumble into dust before being vacuumed up and reformed.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_decrypt.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_decrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,120 +97,115 @@
         keyboard = list(range(33, 127))
         blocks = list(range(9608, 9632))
         box_drawing = list(range(9472, 9599))
         misc = list(range(174, 452))
 
     def __init__(self, effect: "Decrypt") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._typing_pending_chars: list[EffectCharacter] = []
-        self._decrypting_pending_chars: list[EffectCharacter] = []
-        self._phase = "typing"
-        self._active_chars: list[EffectCharacter] = []
-        self._encrypted_symbols: list[str] = []
-        self._scenes: dict[str, animation.Scene] = {}
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._make_encrypted_symbols()
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.typing_pending_chars: list[EffectCharacter] = []
+        self.decrypting_pending_chars: list[EffectCharacter] = []
+        self.phase = "typing"
+        self.encrypted_symbols: list[str] = []
+        self.scenes: dict[str, animation.Scene] = {}
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.make_encrypted_symbols()
+        self.build()
 
-    def _make_encrypted_symbols(self) -> None:
+    def make_encrypted_symbols(self) -> None:
         for n in DecryptIterator._DecryptChars.keyboard:
-            self._encrypted_symbols.append(chr(n))
+            self.encrypted_symbols.append(chr(n))
         for n in DecryptIterator._DecryptChars.blocks:
-            self._encrypted_symbols.append(chr(n))
+            self.encrypted_symbols.append(chr(n))
         for n in DecryptIterator._DecryptChars.box_drawing:
-            self._encrypted_symbols.append(chr(n))
+            self.encrypted_symbols.append(chr(n))
         for n in DecryptIterator._DecryptChars.misc:
-            self._encrypted_symbols.append(chr(n))
+            self.encrypted_symbols.append(chr(n))
 
-    def _make_decrypting_animation_scenes(self, character: EffectCharacter) -> None:
+    def make_decrypting_animation_scenes(self, character: EffectCharacter) -> None:
         fast_decrypt_scene = character.animation.new_scene(id="fast_decrypt")
-        color = random.choice(self._config.ciphertext_colors)
+        color = random.choice(self.config.ciphertext_colors)
         for _ in range(80):
-            symbol = random.choice(self._encrypted_symbols)
+            symbol = random.choice(self.encrypted_symbols)
             fast_decrypt_scene.add_frame(symbol, 3, color=color)
             duration = 3
         slow_decrypt_scene = character.animation.new_scene(id="slow_decrypt")
         for _ in range(random.randint(1, 15)):  # 1-15 longer duration units
-            symbol = random.choice(self._encrypted_symbols)
+            symbol = random.choice(self.encrypted_symbols)
             if random.randint(0, 100) <= 30:  # 30% chance of extra long duration
                 duration = random.randrange(50, 125)  # wide long duration range reduces 'waves' in the animation
             else:
                 duration = random.randrange(5, 10)  # shorter duration creates flipping effect
             slow_decrypt_scene.add_frame(symbol, duration, color=color)
         discovered_scene = character.animation.new_scene(id="discovered")
-        discovered_gradient = graphics.Gradient("ffffff", self._character_final_color_map[character], steps=10)
+        discovered_gradient = graphics.Gradient("ffffff", self.character_final_color_map[character], steps=10)
         discovered_scene.apply_gradient_to_symbols(discovered_gradient, character.input_symbol, 8)
 
-    def _prepare_data_for_type_effect(self) -> None:
-        for character in self._terminal.get_characters():
+    def prepare_data_for_type_effect(self) -> None:
+        for character in self.terminal.get_characters():
             typing_scene = character.animation.new_scene(id="typing")
             for block_char in ["▉", "▓", "▒", "░"]:
-                typing_scene.add_frame(block_char, 2, color=random.choice(self._config.ciphertext_colors))
+                typing_scene.add_frame(block_char, 2, color=random.choice(self.config.ciphertext_colors))
 
             typing_scene.add_frame(
-                random.choice(self._encrypted_symbols), 2, color=random.choice(self._config.ciphertext_colors)
+                random.choice(self.encrypted_symbols), 2, color=random.choice(self.config.ciphertext_colors)
             )
-            self._typing_pending_chars.append(character)
+            self.typing_pending_chars.append(character)
 
-    def _prepare_data_for_decrypt_effect(self) -> None:
-        for character in self._terminal.get_characters():
-            self._make_decrypting_animation_scenes(character)
+    def prepare_data_for_decrypt_effect(self) -> None:
+        for character in self.terminal.get_characters():
+            self.make_decrypting_animation_scenes(character)
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
                 character.animation.query_scene("fast_decrypt"),
                 EventHandler.Action.ACTIVATE_SCENE,
                 character.animation.query_scene("slow_decrypt"),
             )
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE,
                 character.animation.query_scene("slow_decrypt"),
                 EventHandler.Action.ACTIVATE_SCENE,
                 character.animation.query_scene("discovered"),
             )
             character.animation.activate_scene(character.animation.query_scene("fast_decrypt"))
-            self._decrypting_pending_chars.append(character)
+            self.decrypting_pending_chars.append(character)
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        self._prepare_data_for_type_effect()
-        self._prepare_data_for_decrypt_effect()
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        self.prepare_data_for_type_effect()
+        self.prepare_data_for_decrypt_effect()
 
     def __next__(self) -> str:
-        if self._phase == "typing":
-            if self._typing_pending_chars or self._active_chars:
-                if self._typing_pending_chars:
+        if self.phase == "typing":
+            if self.typing_pending_chars or self.active_characters:
+                if self.typing_pending_chars:
                     if random.randint(0, 100) <= 75:
-                        for _ in range(self._config.typing_speed):
-                            if self._typing_pending_chars:
-                                next_character = self._typing_pending_chars.pop(0)
-                                self._terminal.set_character_visibility(next_character, True)
+                        for _ in range(self.config.typing_speed):
+                            if self.typing_pending_chars:
+                                next_character = self.typing_pending_chars.pop(0)
+                                self.terminal.set_character_visibility(next_character, True)
                                 next_character.animation.activate_scene(next_character.animation.query_scene("typing"))
-                                self._active_chars.append(next_character)
-                for character in self._active_chars:
-                    character.tick()
-                self._active_chars = [character for character in self._active_chars if character.is_active]
-                return self._terminal.get_formatted_output_string()
+                                self.active_characters.append(next_character)
+                self.update()
+                return self.frame
             else:
-                self._active_chars = self._decrypting_pending_chars
-                for char in self._active_chars:
+                self.active_characters = self.decrypting_pending_chars
+                for char in self.active_characters:
                     char.animation.activate_scene(char.animation.query_scene("fast_decrypt"))
-                self._phase = "decrypting"
+                self.phase = "decrypting"
 
-        if self._phase == "decrypting":
-            if self._active_chars:
-                for character in self._active_chars:
-                    character.tick()
-                self._active_chars = [character for character in self._active_chars if character.is_active]
-                return self._terminal.get_formatted_output_string()
+        if self.phase == "decrypting":
+            if self.active_characters:
+                self.update()
+                return self.frame
             else:
                 raise StopIteration
         else:
             raise StopIteration
 
 
 class Decrypt(BaseEffect[DecryptConfig]):
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_errorcorrect.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_errorcorrect.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,69 +122,68 @@
     def get_effect_class(cls):
         return ErrorCorrect
 
 
 class ErrorCorrectIterator(BaseEffectIterator[ErrorCorrectConfig]):
     def __init__(self, effect: "ErrorCorrect") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._swapped: list[tuple[EffectCharacter, EffectCharacter]] = []
-        self._swap_delay = 0
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.swapped: list[tuple[EffectCharacter, EffectCharacter]] = []
+        self.swap_delay = 0
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        for character in self._terminal.get_characters():
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
             spawn_scene = character.animation.new_scene()
-            spawn_scene.add_frame(character.input_symbol, 1, color=self._character_final_color_map[character])
+            spawn_scene.add_frame(character.input_symbol, 1, color=self.character_final_color_map[character])
             character.animation.activate_scene(spawn_scene)
-            self._terminal.set_character_visibility(character, True)
-        all_characters: list[EffectCharacter] = list(self._terminal._input_characters)
-        correcting_gradient = graphics.Gradient(self._config.error_color, self._config.correct_color, steps=10)
+            self.terminal.set_character_visibility(character, True)
+        all_characters: list[EffectCharacter] = list(self.terminal._input_characters)
+        correcting_gradient = graphics.Gradient(self.config.error_color, self.config.correct_color, steps=10)
         block_symbol = "▓"
         block_wipe_start = ("▁", "▂", "▃", "▄", "▅", "▆", "▇", "█")
         block_wipe_end = ("▇", "▆", "▅", "▄", "▃", "▂", "▁")
-        for _ in range(int(self._config.error_pairs * len(self._terminal.get_characters()))):
+        for _ in range(int(self.config.error_pairs * len(self.terminal.get_characters()))):
             if len(all_characters) < 2:
                 break
             char1 = all_characters.pop(random.randrange(len(all_characters)))
             char2 = all_characters.pop(random.randrange(len(all_characters)))
             char1.motion.set_coordinate(char2.input_coord)
-            char1_input_coord_path = char1.motion.new_path(id="input_coord", speed=self._config.movement_speed)
+            char1_input_coord_path = char1.motion.new_path(id="input_coord", speed=self.config.movement_speed)
             char1_input_coord_path.new_waypoint(char1.input_coord)
             char2.motion.set_coordinate(char1.input_coord)
-            char2_input_coord_path = char2.motion.new_path(id="input_coord", speed=self._config.movement_speed)
+            char2_input_coord_path = char2.motion.new_path(id="input_coord", speed=self.config.movement_speed)
             char2_input_coord_path.new_waypoint(char2.input_coord)
-            self._swapped.append((char1, char2))
+            self.swapped.append((char1, char2))
             for character in (char1, char2):
                 first_block_wipe = character.animation.new_scene()
                 last_block_wipe = character.animation.new_scene()
                 for block in block_wipe_start:
-                    first_block_wipe.add_frame(block, 3, color=self._config.error_color)
+                    first_block_wipe.add_frame(block, 3, color=self.config.error_color)
                 for block in block_wipe_end:
-                    last_block_wipe.add_frame(block, 3, color=self._config.correct_color)
+                    last_block_wipe.add_frame(block, 3, color=self.config.correct_color)
                 initial_scene = character.animation.new_scene()
-                initial_scene.add_frame(character.input_symbol, 1, color=self._config.error_color)
+                initial_scene.add_frame(character.input_symbol, 1, color=self.config.error_color)
                 character.animation.activate_scene(initial_scene)
                 error_scene = character.animation.new_scene(id="error")
                 for _ in range(10):
-                    error_scene.add_frame(block_symbol, 3, color=self._config.error_color)
+                    error_scene.add_frame(block_symbol, 3, color=self.config.error_color)
                     error_scene.add_frame(character.input_symbol, 3, color="ffffff")
                 correcting_scene = character.animation.new_scene(sync=animation.SyncMetric.DISTANCE)
                 correcting_scene.apply_gradient_to_symbols(correcting_gradient, "█", 3)
                 final_scene = character.animation.new_scene()
                 char_final_gradient = graphics.Gradient(
-                    self._config.correct_color, self._character_final_color_map[character], steps=10
+                    self.config.correct_color, self.character_final_color_map[character], steps=10
                 )
                 final_scene.apply_gradient_to_symbols(char_final_gradient, character.input_symbol, 3)
                 input_coord_path = character.motion.query_path("input_coord")
                 character.event_handler.register_event(
                     EventHandler.Event.SCENE_COMPLETE,
                     error_scene,
                     EventHandler.Action.ACTIVATE_SCENE,
@@ -225,28 +224,25 @@
                     EventHandler.Event.SCENE_COMPLETE,
                     last_block_wipe,
                     EventHandler.Action.ACTIVATE_SCENE,
                     final_scene,
                 )
 
     def __next__(self) -> str:
-        if self._swapped and not self._swap_delay:
-            next_pair = self._swapped.pop(0)
+        if self.swapped and not self.swap_delay:
+            next_pair = self.swapped.pop(0)
             for char in next_pair:
                 char.animation.activate_scene(char.animation.query_scene("error"))
-                self._active_chars.append(char)
-            self._swap_delay = self._config.swap_delay
-        elif self._swap_delay:
-            self._swap_delay -= 1
-        if self._active_chars:
-            for character in self._active_chars:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+                self.active_characters.append(char)
+            self.swap_delay = self.config.swap_delay
+        elif self.swap_delay:
+            self.swap_delay -= 1
+        if self.active_characters:
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class ErrorCorrect(BaseEffect[ErrorCorrectConfig]):
     """Swaps characters from an incorrect initial position to the correct position.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_expand.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_expand.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,55 +102,52 @@
 
 class ExpandIterator(BaseEffectIterator[ExpandConfig]):
     def __init__(
         self,
         effect: "Expand",
     ):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        for character in self._terminal.get_characters():
-            character.motion.set_coordinate(self._terminal.output_area.center)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            character.motion.set_coordinate(self.terminal.output_area.center)
             input_coord_path = character.motion.new_path(
-                speed=self._config.movement_speed,
-                ease=self._config.expand_easing,
+                speed=self.config.movement_speed,
+                ease=self.config.expand_easing,
             )
             input_coord_path.new_waypoint(character.input_coord)
-            self._terminal.set_character_visibility(character, True)
-            self._active_chars.append(character)
+            self.terminal.set_character_visibility(character, True)
+            self.active_characters.append(character)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_ACTIVATED, input_coord_path, EventHandler.Action.SET_LAYER, 1
             )
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE, input_coord_path, EventHandler.Action.SET_LAYER, 0
             )
             character.motion.activate_path(input_coord_path)
             gradient_scn = character.animation.new_scene()
             gradient = graphics.Gradient(
-                final_gradient.spectrum[0], self._character_final_color_map[character], steps=10
+                final_gradient.spectrum[0], self.character_final_color_map[character], steps=10
             )
-            gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self._config.final_gradient_frames)
+            gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self.config.final_gradient_frames)
             character.animation.activate_scene(gradient_scn)
 
     def __next__(self) -> str:
-        if self._active_chars:
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+        if self.active_characters:
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Expand(BaseEffect[ExpandConfig]):
     """Characters expand from the center.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_fireworks.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_fireworks.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,45 +129,44 @@
     def get_effect_class(cls):
         return Fireworks
 
 
 class FireworksIterator(BaseEffectIterator[FireworksConfig]):
     def __init__(self, effect: "Fireworks"):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._shells: list[list[EffectCharacter]] = []
-        self._firework_volume = max(1, round(self._config.firework_volume * len(self._terminal._input_characters)))
-        self._explode_distance = max(1, round(self._terminal.output_area.right * self._config.explode_distance))
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._launch_delay: int = 0
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.shells: list[list[EffectCharacter]] = []
+        self.firework_volume = max(1, round(self.config.firework_volume * len(self.terminal._input_characters)))
+        self.explode_distance = max(1, round(self.terminal.output_area.right * self.config.explode_distance))
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.launch_delay: int = 0
+        self.build()
 
     def prepare_waypoints(self) -> None:
         firework_shell: list[EffectCharacter] = []
-        for character in self._terminal.get_characters():
-            if len(firework_shell) == self._firework_volume or not firework_shell:
-                self._shells.append(firework_shell)
+        for character in self.terminal.get_characters():
+            if len(firework_shell) == self.firework_volume or not firework_shell:
+                self.shells.append(firework_shell)
                 firework_shell = []
-                origin_x = random.randrange(0, self._terminal.output_area.right)
-                if not self._config.explode_anywhere:
+                origin_x = random.randrange(0, self.terminal.output_area.right)
+                if not self.config.explode_anywhere:
                     min_row = character.input_coord.row
                 else:
-                    min_row = self._terminal.output_area.bottom
-                origin_y = random.randrange(min_row, self._terminal.output_area.top + 1)
+                    min_row = self.terminal.output_area.bottom
+                origin_y = random.randrange(min_row, self.terminal.output_area.top + 1)
                 origin_coord = Coord(origin_x, origin_y)
-                explode_waypoint_coords = geometry.find_coords_in_circle(origin_coord, self._explode_distance)
-            character.motion.set_coordinate(Coord(origin_x, self._terminal.output_area.bottom))
+                explode_waypoint_coords = geometry.find_coords_in_circle(origin_coord, self.explode_distance)
+            character.motion.set_coordinate(Coord(origin_x, self.terminal.output_area.bottom))
             apex_path = character.motion.new_path(id="apex_pth", speed=0.2, ease=easing.out_expo)
             apex_wpt = apex_path.new_waypoint(origin_coord)
             explode_path = character.motion.new_path(speed=0.15, ease=easing.out_circ)
             explode_wpt = explode_path.new_waypoint(random.choice(explode_waypoint_coords))
 
             bloom_control_point = geometry.find_coord_at_distance(
-                apex_wpt.coord, explode_wpt.coord, self._explode_distance // 2
+                apex_wpt.coord, explode_wpt.coord, self.explode_distance // 2
             )
             bloom_wpt = explode_path.new_waypoint(
                 Coord(bloom_control_point.column, max(1, bloom_control_point.row - 7)),
                 bezier_control=bloom_control_point,
             )
             input_path = character.motion.new_path(id="input_pth", speed=0.3, ease=easing.in_out_quart)
             input_control_point = Coord(bloom_wpt.coord.column, 1)
@@ -188,37 +187,37 @@
                 EventHandler.Event.PATH_COMPLETE, explode_path, EventHandler.Action.ACTIVATE_PATH, input_path
             )
 
             character.motion.activate_path(apex_path)
 
             firework_shell.append(character)
         if firework_shell:
-            self._shells.append(firework_shell)
+            self.shells.append(firework_shell)
 
     def prepare_scenes(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        for firework_shell in self._shells:
-            shell_color = random.choice(self._config.firework_colors)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for firework_shell in self.shells:
+            shell_color = random.choice(self.config.firework_colors)
             for character in firework_shell:
                 # launch scene
                 launch_scn = character.animation.new_scene()
-                launch_scn.add_frame(self._config.firework_symbol, 2, color=shell_color)
-                launch_scn.add_frame(self._config.firework_symbol, 1, color="FFFFFF")
+                launch_scn.add_frame(self.config.firework_symbol, 2, color=shell_color)
+                launch_scn.add_frame(self.config.firework_symbol, 1, color="FFFFFF")
                 launch_scn.is_looping = True
                 # bloom scene
                 bloom_scn = character.animation.new_scene()
                 bloom_scn.add_frame(character.input_symbol, 1, color=shell_color)
                 # fall scene
                 fall_scn = character.animation.new_scene()
-                fall_gradient = graphics.Gradient(shell_color, self._character_final_color_map[character], steps=15)
+                fall_gradient = graphics.Gradient(shell_color, self.character_final_color_map[character], steps=15)
                 fall_scn.apply_gradient_to_symbols(fall_gradient, character.input_symbol, 15)
                 character.animation.activate_scene(launch_scn)
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE,
                     character.motion.query_path("apex_pth"),
                     EventHandler.Action.ACTIVATE_SCENE,
                     bloom_scn,
@@ -226,32 +225,29 @@
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_ACTIVATED,
                     character.motion.query_path("input_pth"),
                     EventHandler.Action.ACTIVATE_SCENE,
                     fall_scn,
                 )
 
-    def _build(self) -> None:
+    def build(self) -> None:
         self.prepare_waypoints()
         self.prepare_scenes()
 
     def __next__(self) -> str:
-        if self._shells or self._active_chars:
-            if self._shells and self._launch_delay == 0:
-                next_group = self._shells.pop()
+        if self.shells or self.active_characters:
+            if self.shells and self.launch_delay == 0:
+                next_group = self.shells.pop()
                 for character in next_group:
-                    self._terminal.set_character_visibility(character, True)
-                    self._active_chars.append(character)
-                self._launch_delay = int(self._config.launch_delay * random.uniform(0.5, 1.5))
-            for character in self._active_chars:
-                character.tick()
-            self._launch_delay -= 1
-            next_frame = self._terminal.get_formatted_output_string()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+                    self.terminal.set_character_visibility(character, True)
+                    self.active_characters.append(character)
+                self.launch_delay = int(self.config.launch_delay * random.uniform(0.5, 1.5))
+            self.launch_delay -= 1
+            self.update()
+            return self.frame
 
         else:
             raise StopIteration
 
 
 class Fireworks(BaseEffect[FireworksConfig]):
     """Launches characters up the screen where they explode like fireworks and fall into place.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_middleout.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_middleout.py`

 * *Files 11% similar despite different names*

```diff
@@ -128,72 +128,66 @@
     def get_effect_class(cls):
         return MiddleOut
 
 
 class MiddleOutIterator(BaseEffectIterator[MiddleOutConfig]):
     def __init__(self, effect: "MiddleOut"):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._phase = "center"
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.phase = "center"
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            character.motion.set_coordinate(self._terminal.output_area.center)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            character.motion.set_coordinate(self.terminal.output_area.center)
             # setup waypoints
-            if self._config.expand_direction == "vertical":
+            if self.config.expand_direction == "vertical":
                 column = character.input_coord.column
-                row = self._terminal.output_area.center_row
+                row = self.terminal.output_area.center_row
             else:
-                column = self._terminal.output_area.center_column
+                column = self.terminal.output_area.center_column
                 row = character.input_coord.row
             center_path = character.motion.new_path(
-                speed=self._config.center_movement_speed, ease=self._config.center_easing
+                speed=self.config.center_movement_speed, ease=self.config.center_easing
             )
             center_path.new_waypoint(Coord(column, row))
             full_path = character.motion.new_path(
-                id="full", speed=self._config.full_movement_speed, ease=self._config.full_easing
+                id="full", speed=self.config.full_movement_speed, ease=self.config.full_easing
             )
             full_path.new_waypoint(character.input_coord, id="full")
 
             # setup scenes
             full_scene = character.animation.new_scene(id="full")
             full_gradient = graphics.Gradient(
-                self._config.starting_color, self._character_final_color_map[character], steps=10
+                self.config.starting_color, self.character_final_color_map[character], steps=10
             )
             full_scene.apply_gradient_to_symbols(full_gradient, character.input_symbol, 10)
 
             # initialize character state
             character.motion.activate_path(center_path)
-            character.animation.set_appearance(character.input_symbol, self._config.starting_color)
-            self._terminal.set_character_visibility(character, True)
-            self._active_chars.append(character)
+            character.animation.set_appearance(character.input_symbol, self.config.starting_color)
+            self.terminal.set_character_visibility(character, True)
+            self.active_characters.append(character)
 
     def __next__(self) -> str:
-        if self._active_chars:
-            if (
-                all([character.motion.active_path is None for character in self._active_chars])
-                and self._phase == "center"
-            ):
-                for character in self._active_chars:
-                    character.motion.activate_path(character.motion.query_path("full"))
-                    character.animation.activate_scene(character.animation.query_scene("full"))
-                self._phase = "full"
-            for character in self._active_chars:
-                character.tick()
-            if self._phase == "full":
-                self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+        if self.phase == "center" and not self.active_characters:
+            self.phase = "full"
+            self.active_characters = self.terminal.get_characters()
+            for character in self.active_characters:
+                character.motion.activate_path(character.motion.query_path("full"))
+                character.animation.activate_scene(character.animation.query_scene("full"))
+        if self.active_characters:
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class MiddleOut(BaseEffect[MiddleOutConfig]):
     """Text expands in a single row or column in the middle of the output area then out.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_orbittingvolley.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_orbittingvolley.py`

 * *Files 20% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
     @classmethod
     def get_effect_class(cls):
         return OrbittingVolley
 
 
 class OrbittingVolleyIterator(BaseEffectIterator[OrbittingVolleyConfig]):
-    class _Launcher:
+    class Launcher:
         def __init__(self, terminal: Terminal, args: OrbittingVolleyConfig, starting_edge_coord: Coord, symbol: str):
             self.terminal = terminal
             self.args = args
             self.character = self.terminal.add_character(symbol, starting_edge_coord)
             self.magazine: list[EffectCharacter] = []
 
         def build_paths(self) -> None:
@@ -194,129 +194,125 @@
                 self.terminal.set_character_visibility(next_char, True)
             else:
                 next_char = None
             return next_char
 
     def __init__(self, effect: "OrbittingVolley"):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
+        self.pending_chars: list[EffectCharacter] = []
         self.final_gradient = graphics.Gradient(
-            *self._config.final_gradient_stops, steps=self._config.final_gradient_steps
+            *self.config.final_gradient_stops, steps=self.config.final_gradient_steps
         )
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self.final_gradient_coordinate_map: dict[Coord, graphics.Color] = (
             self.final_gradient.build_coordinate_color_mapping(
-                self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+                self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
             )
         )
-        self._complete = False
-        self._build()
+        self.complete = False
+        self.build()
 
-    def _build(self) -> None:
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = self.final_gradient_coordinate_map[character.input_coord]
+    def build(self) -> None:
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = self.final_gradient_coordinate_map[character.input_coord]
             input_path = character.motion.new_path(
-                speed=self._config.character_movement_speed,
-                ease=self._config.character_easing,
+                speed=self.config.character_movement_speed,
+                ease=self.config.character_easing,
                 id="input_path",
                 layer=1,
             )
             input_path.new_waypoint(character.input_coord)
-            character.animation.set_appearance(character.input_symbol, self._character_final_color_map[character])
-        self._launchers: list[OrbittingVolleyIterator._Launcher] = []
+            character.animation.set_appearance(character.input_symbol, self.character_final_color_map[character])
+        self._launchers: list[OrbittingVolleyIterator.Launcher] = []
         for coord, symbol in (
             (
-                Coord(self._terminal.output_area.left, self._terminal.output_area.top),
-                self._config.top_launcher_symbol,
+                Coord(self.terminal.output_area.left, self.terminal.output_area.top),
+                self.config.top_launcher_symbol,
             ),
             (
-                Coord(self._terminal.output_area.right, self._terminal.output_area.top),
-                self._config.right_launcher_symbol,
+                Coord(self.terminal.output_area.right, self.terminal.output_area.top),
+                self.config.right_launcher_symbol,
             ),
             (
-                Coord(self._terminal.output_area.right, self._terminal.output_area.bottom),
-                self._config.bottom_launcher_symbol,
+                Coord(self.terminal.output_area.right, self.terminal.output_area.bottom),
+                self.config.bottom_launcher_symbol,
             ),
             (
-                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
-                self._config.left_launcher_symbol,
+                Coord(self.terminal.output_area.left, self.terminal.output_area.bottom),
+                self.config.left_launcher_symbol,
             ),
         ):
-            launcher = OrbittingVolleyIterator._Launcher(self._terminal, self._config, coord, symbol)
+            launcher = OrbittingVolleyIterator.Launcher(self.terminal, self.config, coord, symbol)
             launcher.character.layer = 2
-            self._terminal.set_character_visibility(launcher.character, True)
-            self._active_chars.append(launcher.character)
+            self.terminal.set_character_visibility(launcher.character, True)
+            self.active_characters.append(launcher.character)
             self._launchers.append(launcher)
         self._main_launcher = self._launchers[0]
         self._main_launcher.character.animation.set_appearance(
             self._main_launcher.character.input_symbol, self.final_gradient.spectrum[-1]
         )
         self._main_launcher.build_paths()
         self._main_launcher.character.motion.activate_path(self._main_launcher.character.motion.query_path("perimeter"))
         self._sorted_chars = []
-        for char_list in self._terminal.get_characters_grouped(Terminal.CharacterGroup.CENTER_TO_OUTSIDE_DIAMONDS):
+        for char_list in self.terminal.get_characters_grouped(Terminal.CharacterGroup.CENTER_TO_OUTSIDE_DIAMONDS):
             self._sorted_chars.extend(char_list)
         for launcher, character in zip(cycle(self._launchers), self._sorted_chars):
             launcher.magazine.append(character)
         self._delay = 0
 
-    def _set_launcher_coordinates(self, parent: _Launcher, child: _Launcher) -> None:
-        parent_progress = parent.character.motion.current_coord.column / self._terminal.output_area.right
-        if child.character.input_coord == Coord(self._terminal.output_area.right, self._terminal.output_area.top):
-            child_row = self._terminal.output_area.top - int((self._terminal.output_area.top * parent_progress))
-            child.character.motion.set_coordinate(Coord(self._terminal.output_area.right, max(1, child_row)))
-        elif child.character.input_coord == Coord(self._terminal.output_area.right, self._terminal.output_area.bottom):
-            child_column = self._terminal.output_area.right - int((self._terminal.output_area.right * parent_progress))
-            child.character.motion.set_coordinate(Coord(max(1, child_column), self._terminal.output_area.bottom))
-        elif child.character.input_coord == Coord(self._terminal.output_area.left, self._terminal.output_area.bottom):
-            child_row = self._terminal.output_area.bottom + int((self._terminal.output_area.top * parent_progress))
+    def _set_launcher_coordinates(self, parent: Launcher, child: Launcher) -> None:
+        parent_progress = parent.character.motion.current_coord.column / self.terminal.output_area.right
+        if child.character.input_coord == Coord(self.terminal.output_area.right, self.terminal.output_area.top):
+            child_row = self.terminal.output_area.top - int((self.terminal.output_area.top * parent_progress))
+            child.character.motion.set_coordinate(Coord(self.terminal.output_area.right, max(1, child_row)))
+        elif child.character.input_coord == Coord(self.terminal.output_area.right, self.terminal.output_area.bottom):
+            child_column = self.terminal.output_area.right - int((self.terminal.output_area.right * parent_progress))
+            child.character.motion.set_coordinate(Coord(max(1, child_column), self.terminal.output_area.bottom))
+        elif child.character.input_coord == Coord(self.terminal.output_area.left, self.terminal.output_area.bottom):
+            child_row = self.terminal.output_area.bottom + int((self.terminal.output_area.top * parent_progress))
             child.character.motion.set_coordinate(
-                Coord(self._terminal.output_area.left, min(self._terminal.output_area.top, child_row))
+                Coord(self.terminal.output_area.left, min(self.terminal.output_area.top, child_row))
             )
         color = self.final_gradient_coordinate_map[child.character.motion.current_coord]
         child.character.animation.set_appearance(child.character.input_symbol, color)
 
     def __next__(self) -> str:
-        if any([launcher.magazine for launcher in self._launchers]) or len(self._active_chars) > 1:
+        if any([launcher.magazine for launcher in self._launchers]) or len(self.active_characters) > 1:
             if self._main_launcher.character.motion.active_path is None:
                 perimeter_path = self._main_launcher.character.motion.query_path("perimeter")
                 self._main_launcher.character.motion.set_coordinate(perimeter_path.waypoints[0].coord)
                 self._main_launcher.character.motion.activate_path(perimeter_path)
-                self._active_chars.append(self._main_launcher.character)
+                self.active_characters.append(self._main_launcher.character)
             self._main_launcher.character.animation.set_appearance(
-                self._config.top_launcher_symbol,
+                self.config.top_launcher_symbol,
                 self.final_gradient_coordinate_map[self._main_launcher.character.motion.current_coord],
             )
             for launcher in self._launchers[1:]:
                 self._set_launcher_coordinates(self._main_launcher, launcher)
             if not self._delay:
                 for launcher in self._launchers:
                     characters_to_launch = max(
-                        int((self._config.volley_size * len(self._terminal._input_characters)) / 4), 1
+                        int((self.config.volley_size * len(self.terminal._input_characters)) / 4), 1
                     )
                     for _ in range(characters_to_launch):
                         next_char = launcher.launch()
                         if next_char:
-                            self._active_chars.append(next_char)
-                self._delay = self._config.launch_delay
+                            self.active_characters.append(next_char)
+                self._delay = self.config.launch_delay
             else:
                 self._delay -= 1
 
-            for character in self._active_chars:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+            self.update()
+            return self.frame
         else:
-            if not self._complete:
-                self._complete = True
+            if not self.complete:
+                self.complete = True
                 for launcher in self._launchers:
-                    self._terminal.set_character_visibility(launcher.character, False)
-                return self._terminal.get_formatted_output_string()
+                    self.terminal.set_character_visibility(launcher.character, False)
+                return self.frame
             else:
                 raise StopIteration
 
 
 class OrbittingVolley(BaseEffect[OrbittingVolleyConfig]):
     """Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_overflow.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_overflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     @classmethod
     def get_effect_class(cls):
         return Overflow
 
 
 class OverflowIterator(BaseEffectIterator[OverflowConfig]):
-    class _Row:
+    class Row:
         def __init__(self, characters: list[EffectCharacter], final: bool = False) -> None:
             self.characters = characters
             self.current_index = 0
             self.final = final
 
         def move_up(self) -> None:
             for character in self.characters:
@@ -121,92 +121,87 @@
 
         def set_color(self, color: int | str) -> None:
             for character in self.characters:
                 character.animation.set_appearance(character.input_symbol, color)
 
     def __init__(self, effect: "Overflow"):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._pending_rows: list[OverflowIterator._Row] = []
-        self._active_rows: list[OverflowIterator._Row] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.pending_rows: list[OverflowIterator.Row] = []
+        self.active_rows: list[OverflowIterator.Row] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters(fill_chars=True):
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        lower_range, upper_range = self._config.overflow_cycles_range
-        rows = self._terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM)
+        for character in self.terminal.get_characters(fill_chars=True):
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        lower_range, upper_range = self.config.overflow_cycles_range
+        rows = self.terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM)
         if upper_range > 0:
             for _ in range(random.randint(lower_range, upper_range)):
                 random.shuffle(rows)
                 for row in rows:
                     copied_characters = [
-                        self._terminal.add_character(character.input_symbol, character.input_coord) for character in row
+                        self.terminal.add_character(character.input_symbol, character.input_coord) for character in row
                     ]
-                    self._pending_rows.append(OverflowIterator._Row(copied_characters))
+                    self.pending_rows.append(OverflowIterator.Row(copied_characters))
         # add rows in correct order to the end of self.pending_rows
-        for row in self._terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True):
-            next_row = OverflowIterator._Row(row)
+        for row in self.terminal.get_characters_grouped(Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True):
+            next_row = OverflowIterator.Row(row)
             for character in next_row.characters:
-                character.animation.set_appearance(character.symbol, self._character_final_color_map[character])
+                character.animation.set_appearance(character.symbol, self.character_final_color_map[character])
             next_row.set_color(
-                final_gradient.get_color_at_fraction(row[0].input_coord.row / self._terminal.output_area.top)
+                final_gradient.get_color_at_fraction(row[0].input_coord.row / self.terminal.output_area.top)
             )
-            self._pending_rows.append(OverflowIterator._Row(row, final=True))
+            self.pending_rows.append(OverflowIterator.Row(row, final=True))
         self._delay = 0
         self._overflow_gradient = graphics.Gradient(
-            *self._config.overflow_gradient_stops,
-            steps=max((self._terminal.output_area.top // max(1, len(self._config.overflow_gradient_stops) - 1)), 1),
+            *self.config.overflow_gradient_stops,
+            steps=max((self.terminal.output_area.top // max(1, len(self.config.overflow_gradient_stops) - 1)), 1),
         )
 
     def __next__(self) -> str:
-        if self._pending_rows:
+        if self.pending_rows:
             if not self._delay:
-                for _ in range(random.randint(1, self._config.overflow_speed)):
-                    if self._pending_rows:
-                        for row in self._active_rows:
+                for _ in range(random.randint(1, self.config.overflow_speed)):
+                    if self.pending_rows:
+                        for row in self.active_rows:
                             row.move_up()
                             if not row.final:
                                 row.set_color(
                                     self._overflow_gradient.spectrum[
                                         min(
                                             row.characters[0].motion.current_coord.row,
                                             len(self._overflow_gradient.spectrum) - 1,
                                         )
                                     ]
                                 )
-                        next_row = self._pending_rows.pop(0)
+                        next_row = self.pending_rows.pop(0)
                         next_row.setup()
                         next_row.move_up()
                         if not next_row.final:
                             next_row.set_color(self._overflow_gradient.spectrum[0])
                         for character in next_row.characters:
-                            self._terminal.set_character_visibility(character, True)
-                        self._active_rows.append(next_row)
+                            self.terminal.set_character_visibility(character, True)
+                        self.active_rows.append(next_row)
                 self._delay = random.randint(0, 3)
 
             else:
                 self._delay -= 1
-            self._active_rows = [
+            self.active_rows = [
                 row
-                for row in self._active_rows
-                if row.characters[0].motion.current_coord.row <= self._terminal.output_area.top
+                for row in self.active_rows
+                if row.characters[0].motion.current_coord.row <= self.terminal.output_area.top
             ]
-            for character in self._active_chars:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Overflow(BaseEffect[OverflowConfig]):
     """Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_pour.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_pour.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,96 +145,92 @@
         UP = auto()
         DOWN = auto()
         LEFT = auto()
         RIGHT = auto()
 
     def __init__(self, effect: "Pour") -> None:
         super().__init__(effect)
-        self._pending_groups: list[list[EffectCharacter]] = []
-        self._active_characters: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_groups: list[list[EffectCharacter]] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
+    def build(self) -> None:
         self._pour_direction = {
             "down": PourIterator.PourDirection.DOWN,
             "up": PourIterator.PourDirection.UP,
             "left": PourIterator.PourDirection.LEFT,
             "right": PourIterator.PourDirection.RIGHT,
-        }.get(self._config.pour_direction, PourIterator.PourDirection.DOWN)
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        }.get(self.config.pour_direction, PourIterator.PourDirection.DOWN)
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         sort_map = {
             PourIterator.PourDirection.DOWN: Terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
             PourIterator.PourDirection.UP: Terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
             PourIterator.PourDirection.LEFT: Terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
             PourIterator.PourDirection.RIGHT: Terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
         }
-        groups = self._terminal.get_characters_grouped(grouping=sort_map[self._pour_direction])
+        groups = self.terminal.get_characters_grouped(grouping=sort_map[self._pour_direction])
         for i, group in enumerate(groups):
             for character in group:
-                self._terminal.set_character_visibility(character, False)
+                self.terminal.set_character_visibility(character, False)
                 if self._pour_direction == PourIterator.PourDirection.DOWN:
-                    character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
+                    character.motion.set_coordinate(Coord(character.input_coord.column, self.terminal.output_area.top))
                 elif self._pour_direction == PourIterator.PourDirection.UP:
                     character.motion.set_coordinate(
-                        Coord(character.input_coord.column, self._terminal.output_area.bottom)
+                        Coord(character.input_coord.column, self.terminal.output_area.bottom)
                     )
                 elif self._pour_direction == PourIterator.PourDirection.LEFT:
-                    character.motion.set_coordinate(Coord(self._terminal.output_area.right, character.input_coord.row))
+                    character.motion.set_coordinate(Coord(self.terminal.output_area.right, character.input_coord.row))
                 elif self._pour_direction == PourIterator.PourDirection.RIGHT:
-                    character.motion.set_coordinate(Coord(self._terminal.output_area.left, character.input_coord.row))
+                    character.motion.set_coordinate(Coord(self.terminal.output_area.left, character.input_coord.row))
                 input_coord_path = character.motion.new_path(
-                    speed=self._config.movement_speed,
-                    ease=self._config.movement_easing,
+                    speed=self.config.movement_speed,
+                    ease=self.config.movement_easing,
                 )
                 input_coord_path.new_waypoint(character.input_coord)
                 character.motion.activate_path(input_coord_path)
 
                 pour_gradient = graphics.Gradient(
-                    self._config.starting_color,
-                    self._character_final_color_map[character],
-                    steps=self._config.final_gradient_steps,
+                    self.config.starting_color,
+                    self.character_final_color_map[character],
+                    steps=self.config.final_gradient_steps,
                 )
                 pour_scn = character.animation.new_scene()
                 pour_scn.apply_gradient_to_symbols(
-                    pour_gradient, character.input_symbol, self._config.final_gradient_frames
+                    pour_gradient, character.input_symbol, self.config.final_gradient_frames
                 )
                 character.animation.activate_scene(pour_scn)
             if i % 2 == 0:
-                self._pending_groups.append(group)
+                self.pending_groups.append(group)
             else:
-                self._pending_groups.append(group[::-1])
+                self.pending_groups.append(group[::-1])
         self.gap = 0
-        self.current_group = self._pending_groups.pop(0)
+        self.current_group = self.pending_groups.pop(0)
 
     def __next__(self) -> str:
-        if self._pending_groups or self._active_characters or self.current_group:
+        if self.pending_groups or self.active_characters or self.current_group:
             if not self.current_group:
-                if self._pending_groups:
-                    self.current_group = self._pending_groups.pop(0)
+                if self.pending_groups:
+                    self.current_group = self.pending_groups.pop(0)
             if self.current_group:
                 if not self.gap:
-                    for _ in range(self._config.pour_speed):
+                    for _ in range(self.config.pour_speed):
                         if self.current_group:
                             next_character = self.current_group.pop(0)
-                            self._terminal.set_character_visibility(next_character, True)
-                            self._active_characters.append(next_character)
-                    self.gap = self._config.gap
+                            self.terminal.set_character_visibility(next_character, True)
+                            self.active_characters.append(next_character)
+                    self.gap = self.config.gap
                 else:
                     self.gap -= 1
-            for character in self._active_characters:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
-            self._active_characters = [character for character in self._active_characters if character.is_active]
-            return next_frame
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Pour(BaseEffect[PourConfig]):
     """Pours the characters back and forth from the top, bottom, left, or right.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_print.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_print.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     @classmethod
     def get_effect_class(cls):
         return Print
 
 
 class PrintIterator(BaseEffectIterator[PrintConfig]):
-    class _Row:
+    class Row:
         def __init__(
             self,
             characters: list[EffectCharacter],
             character_final_color_map: dict[EffectCharacter, graphics.Color],
             typing_head_color: str | int,
         ):
             self.untyped_chars: list[EffectCharacter] = []
@@ -137,100 +137,95 @@
                 next_char = self.untyped_chars.pop(0)
                 self.typed_chars.append(next_char)
                 return next_char
             return None
 
     def __init__(self, effect: "Print"):
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._pending_rows: list[PrintIterator._Row] = []
-        self._processed_rows: list[PrintIterator._Row] = []
-        self._typing_head = self._terminal.add_character("█", Coord(1, 1))
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.pending_rows: list[PrintIterator.Row] = []
+        self.processed_rows: list[PrintIterator.Row] = []
+        self.typing_head = self.terminal.add_character("█", Coord(1, 1))
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
+    def build(self) -> None:
         self.final_gradient = graphics.Gradient(
-            *self._config.final_gradient_stops, steps=self._config.final_gradient_steps
+            *self.config.final_gradient_stops, steps=self.config.final_gradient_steps
         )
         final_gradient_mapping = self.final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters(fill_chars=True):
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        input_rows = self._terminal.get_characters_grouped(
-            grouping=self._terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True
+        for character in self.terminal.get_characters(fill_chars=True):
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        input_rows = self.terminal.get_characters_grouped(
+            grouping=self.terminal.CharacterGroup.ROW_TOP_TO_BOTTOM, fill_chars=True
         )
         for input_row in input_rows:
-            self._pending_rows.append(
-                PrintIterator._Row(
+            self.pending_rows.append(
+                PrintIterator.Row(
                     input_row,
-                    self._character_final_color_map,
-                    self._character_final_color_map[input_row[-1]],
+                    self.character_final_color_map,
+                    self.character_final_color_map[input_row[-1]],
                 )
             )
-        self._current_row: PrintIterator._Row = self._pending_rows.pop(0)
+        self._current_row: PrintIterator.Row = self.pending_rows.pop(0)
         self._typing = True
         self._delay = 0
         self._last_column = 0
 
     def __next__(self) -> str:
-        if self._active_chars or self._typing:
-            if self._typing_head.motion.active_path:
+        if self.active_characters or self._typing:
+            if self.typing_head.motion.active_path:
                 pass
             elif self._delay:
                 self._delay -= 1
             else:
                 self._delay = random.randint(0, 0)
                 if self._current_row.untyped_chars:
-                    for _ in range(min(len(self._current_row.untyped_chars), self._config.print_speed)):
+                    for _ in range(min(len(self._current_row.untyped_chars), self.config.print_speed)):
                         next_char = self._current_row.type_char()
                         if next_char:
-                            self._terminal.set_character_visibility(next_char, True)
-                            self._active_chars.append(next_char)
+                            self.terminal.set_character_visibility(next_char, True)
+                            self.active_characters.append(next_char)
                             self._last_column = next_char.input_coord.column
                 else:
-                    self._processed_rows.append(self._current_row)
-                    if self._pending_rows:
-                        for row in self._processed_rows:
+                    self.processed_rows.append(self._current_row)
+                    if self.pending_rows:
+                        for row in self.processed_rows:
                             row.move_up()
-                        self._current_row = self._pending_rows.pop(0)
+                        self._current_row = self.pending_rows.pop(0)
                         current_row_height = self._current_row.untyped_chars[0].input_coord.row
-                        self._typing_head.motion.set_coordinate(Coord(self._last_column, 1))
-                        self._terminal.set_character_visibility(self._typing_head, True)
-                        self._typing_head.motion.paths.clear()
-                        carriage_return_path = self._typing_head.motion.new_path(
-                            speed=self._config.print_head_return_speed,
-                            ease=self._config.print_head_easing,
+                        self.typing_head.motion.set_coordinate(Coord(self._last_column, 1))
+                        self.terminal.set_character_visibility(self.typing_head, True)
+                        self.typing_head.motion.paths.clear()
+                        carriage_return_path = self.typing_head.motion.new_path(
+                            speed=self.config.print_head_return_speed,
+                            ease=self.config.print_head_easing,
                             id="carriage_return_path",
                         )
                         carriage_return_path.new_waypoint(Coord(1, 1))
-                        self._typing_head.motion.activate_path(carriage_return_path)
-                        self._typing_head.animation.set_appearance(
-                            self._typing_head.input_symbol,
+                        self.typing_head.motion.activate_path(carriage_return_path)
+                        self.typing_head.animation.set_appearance(
+                            self.typing_head.input_symbol,
                             self.final_gradient.get_color_at_fraction(
-                                current_row_height / self._terminal.output_area.top
+                                current_row_height / self.terminal.output_area.top
                             ),
                         )
-                        self._typing_head.event_handler.register_event(
+                        self.typing_head.event_handler.register_event(
                             EventHandler.Event.PATH_COMPLETE,
                             carriage_return_path,
                             EventHandler.Action.CALLBACK,
-                            EventHandler.Callback(self._terminal.set_character_visibility, False),
+                            EventHandler.Callback(self.terminal.set_character_visibility, False),
                         )
-                        self._active_chars.append(self._typing_head)
+                        self.active_characters.append(self.typing_head)
                     else:
                         self._typing = False
-            for character in self._active_chars:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Print(BaseEffect[PrintConfig]):
     """Prints the input data one line at at time with a carriage return and line feed.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_rain.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_rain.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,75 +114,71 @@
     def get_effect_class(cls):
         return Rain
 
 
 class RainIterator(BaseEffectIterator[RainConfig]):
     def __init__(self, effect: "Rain") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._group_by_row: dict[int, list[EffectCharacter | None]] = {}
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.group_by_row: dict[int, list[EffectCharacter | None]] = {}
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
 
-        for character in self._terminal.get_characters():
-            raindrop_color = random.choice(self._config.rain_colors)
+        for character in self.terminal.get_characters():
+            raindrop_color = random.choice(self.config.rain_colors)
             rain_scn = character.animation.new_scene()
-            rain_scn.add_frame(random.choice(self._config.rain_symbols), 1, color=raindrop_color)
-            raindrop_gradient = graphics.Gradient(raindrop_color, self._character_final_color_map[character], steps=7)
+            rain_scn.add_frame(random.choice(self.config.rain_symbols), 1, color=raindrop_color)
+            raindrop_gradient = graphics.Gradient(raindrop_color, self.character_final_color_map[character], steps=7)
             fade_scn = character.animation.new_scene()
             fade_scn.apply_gradient_to_symbols(raindrop_gradient, character.input_symbol, 5)
             character.animation.activate_scene(rain_scn)
-            character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
+            character.motion.set_coordinate(Coord(character.input_coord.column, self.terminal.output_area.top))
             input_path = character.motion.new_path(
-                speed=random.uniform(self._config.movement_speed[0], self._config.movement_speed[1]),
-                ease=self._config.movement_easing,
+                speed=random.uniform(self.config.movement_speed[0], self.config.movement_speed[1]),
+                ease=self.config.movement_easing,
             )
             input_path.new_waypoint(character.input_coord)
 
             character.event_handler.register_event(
                 character.event_handler.Event.PATH_COMPLETE,
                 input_path,
                 character.event_handler.Action.ACTIVATE_SCENE,
                 fade_scn,
             )
             character.motion.activate_path(input_path)
-            self._pending_chars.append(character)
-        for character in sorted(self._pending_chars, key=lambda c: c.input_coord.row):
-            if character.input_coord.row not in self._group_by_row:
-                self._group_by_row[character.input_coord.row] = []
-            self._group_by_row[character.input_coord.row].append(character)
-        self._pending_chars.clear()
+            self.pending_chars.append(character)
+        for character in sorted(self.pending_chars, key=lambda c: c.input_coord.row):
+            if character.input_coord.row not in self.group_by_row:
+                self.group_by_row[character.input_coord.row] = []
+            self.group_by_row[character.input_coord.row].append(character)
+        self.pending_chars.clear()
 
     def __next__(self) -> str:
-        if self._group_by_row or self._active_chars or self._pending_chars:
-            if not self._pending_chars and self._group_by_row:
-                self._pending_chars.extend(self._group_by_row.pop(min(self._group_by_row.keys())))  # type: ignore
-            if self._pending_chars:
+        if self.group_by_row or self.active_characters or self.pending_chars:
+            if not self.pending_chars and self.group_by_row:
+                self.pending_chars.extend(self.group_by_row.pop(min(self.group_by_row.keys())))  # type: ignore
+            if self.pending_chars:
                 for _ in range(random.randint(1, 3)):
-                    if self._pending_chars:
-                        next_character = self._pending_chars.pop(random.randint(0, len(self._pending_chars) - 1))
-                        self._terminal.set_character_visibility(next_character, True)
-                        self._active_chars.append(next_character)
+                    if self.pending_chars:
+                        next_character = self.pending_chars.pop(random.randint(0, len(self.pending_chars) - 1))
+                        self.terminal.set_character_visibility(next_character, True)
+                        self.active_characters.append(next_character)
 
                     else:
                         break
-            for character in self._active_chars:
-                character.tick()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Rain(BaseEffect[RainConfig]):
     """Rain characters from the top of the output area.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_random_sequence.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_random_sequence.py`

 * *Files 11% similar despite different names*

```diff
@@ -101,50 +101,43 @@
     def get_effect_class(cls):
         return RandomSequence
 
 
 class RandomSequenceIterator(BaseEffectIterator[RandomSequenceConfig]):
     def __init__(self, effect: "RandomSequence") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._characters_per_tick = max(int(self._config.speed * len(self._terminal._input_characters)), 1)
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.characters_per_tick = max(int(self.config.speed * len(self.terminal._input_characters)), 1)
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            self._terminal.set_character_visibility(character, False)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            self.terminal.set_character_visibility(character, False)
             gradient_scn = character.animation.new_scene()
-            gradient = graphics.Gradient(
-                self._config.starting_color, self._character_final_color_map[character], steps=7
-            )
-            gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self._config.final_gradient_frames)
+            gradient = graphics.Gradient(self.config.starting_color, self.character_final_color_map[character], steps=7)
+            gradient_scn.apply_gradient_to_symbols(gradient, character.input_symbol, self.config.final_gradient_frames)
             character.animation.activate_scene(gradient_scn)
-            self._pending_chars.append(character)
-        random.shuffle(self._pending_chars)
+            self.pending_chars.append(character)
+        random.shuffle(self.pending_chars)
 
     def __next__(self) -> str:
-        if self._pending_chars or self._active_chars:
-            for _ in range(self._characters_per_tick):
-                if self._pending_chars:
-                    next_char = self._pending_chars.pop()
-                    self._terminal.set_character_visibility(next_char, True)
-                    self._active_chars.append(next_char)
-            for character in self._active_chars:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+        if self.pending_chars or self.active_characters:
+            for _ in range(self.characters_per_tick):
+                if self.pending_chars:
+                    next_char = self.pending_chars.pop()
+                    self.terminal.set_character_visibility(next_char, True)
+                    self.active_characters.append(next_char)
+            self.update()
+            return self.frame
         raise StopIteration
 
 
 class RandomSequence(BaseEffect[RandomSequenceConfig]):
     """Prints the input data in a random sequence, one character at a time.
 
     Attributes:
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_rings.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_rings.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     @classmethod
     def get_effect_class(cls):
         return Rings
 
 
 class RingsIterator(BaseEffectIterator[RingsConfig]):
-    class _Ring:
+    class Ring:
         def __init__(
             self,
             config: RingsConfig,
             radius: int,
             origin: Coord,
             ring_coords: list[Coord],
             ring_gap: int,
@@ -217,96 +217,95 @@
                     self.character_last_ring_path[character],
                 )
                 character.motion.activate_path(condense_path)
                 character.animation.activate_scene(character.animation.query_scene("gradient"))
 
     def __init__(self, effect: "Rings") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._ring_chars: list[EffectCharacter] = []
-        self._non_ring_chars: list[EffectCharacter] = []
-        self._rings: dict[int, RingsIterator._Ring] = {}
+        self.pending_chars: list[EffectCharacter] = []
+        self.ring_chars: list[EffectCharacter] = []
+        self.non_ring_chars: list[EffectCharacter] = []
+        self.rings: dict[int, RingsIterator.Ring] = {}
         self.ring_gap = int(
-            max(round(min(self._terminal.output_area.top, self._terminal.output_area.right) * self._config.ring_gap), 1)
+            max(round(min(self.terminal.output_area.top, self.terminal.output_area.right) * self.config.ring_gap), 1)
         )
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
+    def build(self) -> None:
         self.ring_gap = int(
-            max(round(min(self._terminal.output_area.top, self._terminal.output_area.right) * self._config.ring_gap), 1)
+            max(round(min(self.terminal.output_area.top, self.terminal.output_area.right) * self.config.ring_gap), 1)
         )
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
             start_scn = character.animation.new_scene()
-            start_scn.add_frame(character.input_symbol, 1, color=self._character_final_color_map[character])
+            start_scn.add_frame(character.input_symbol, 1, color=self.character_final_color_map[character])
             home_path = character.motion.new_path(speed=0.8, ease=easing.out_quad, id="home")
             home_path.new_waypoint(character.input_coord)
             character.animation.activate_scene(start_scn)
-            self._terminal.set_character_visibility(character, True)
-            self._pending_chars.append(character)
+            self.terminal.set_character_visibility(character, True)
+            self.pending_chars.append(character)
 
-        random.shuffle(self._pending_chars)
+        random.shuffle(self.pending_chars)
         # make rings
-        for radius in range(1, max(self._terminal.output_area.right, self._terminal.output_area.top), self.ring_gap):
+        for radius in range(1, max(self.terminal.output_area.right, self.terminal.output_area.top), self.ring_gap):
             ring_coords = geometry.find_coords_on_circle(
-                self._terminal.output_area.center, radius, 7 * radius, unique=True
+                self.terminal.output_area.center, radius, 7 * radius, unique=True
             )
             # check if any part of the ring is in the output area, if not, stop creating rings
             if (
-                len([coord for coord in ring_coords if self._terminal.output_area.coord_is_in_output_area(coord)])
+                len([coord for coord in ring_coords if self.terminal.output_area.coord_is_in_output_area(coord)])
                 / len(ring_coords)
                 < 0.25
             ):
                 break
 
-            self._rings[radius] = RingsIterator._Ring(
-                self._config,
+            self.rings[radius] = RingsIterator.Ring(
+                self.config,
                 radius,
-                self._terminal.output_area.center,
+                self.terminal.output_area.center,
                 ring_coords,
                 self.ring_gap,
-                self._config.ring_colors[len(self._rings) % len(self._config.ring_colors)],
-                self._character_final_color_map,
+                self.config.ring_colors[len(self.rings) % len(self.config.ring_colors)],
+                self.character_final_color_map,
             )
         # assign characters to rings
         ring_count = 0
-        for ring in self._rings.values():
+        for ring in self.rings.values():
             for _ in ring.counter_clockwise_coords:
-                if self._pending_chars:
-                    next_character = self._pending_chars.pop(0)
+                if self.pending_chars:
+                    next_character = self.pending_chars.pop(0)
                     # set rings to rotate in opposite directions
                     ring.add_character(next_character, clockwise=ring_count % 2)
-                    self._ring_chars.append(next_character)
+                    self.ring_chars.append(next_character)
             ring_count += 1
 
         # make external waypoints for characters not in rings
-        for character in self._terminal.get_characters():
-            if character not in self._ring_chars:
+        for character in self.terminal.get_characters():
+            if character not in self.ring_chars:
                 external_path = character.motion.new_path(id="external", speed=0.8, ease=easing.out_sine)
-                external_path.new_waypoint(self._terminal.output_area.random_coord(outside_scope=True))
+                external_path.new_waypoint(self.terminal.output_area.random_coord(outside_scope=True))
 
-                self._non_ring_chars.append(character)
+                self.non_ring_chars.append(character)
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE,
                     external_path,
                     EventHandler.Action.CALLBACK,
-                    EventHandler.Callback(self._terminal.set_character_visibility, False),
+                    EventHandler.Callback(self.terminal.set_character_visibility, False),
                 )
-        self._rings_list = list(self._rings.values())
+        self._rings_list = list(self.rings.values())
         self._phase = "start"
         self._initial_disperse_complete = False
-        self._spin_time_remaining = self._config.spin_duration
-        self._disperse_time_remaining = self._config.disperse_duration
-        self._cycles_remaining = self._config.spin_disperse_cycles
+        self._spin_time_remaining = self.config.spin_duration
+        self._disperse_time_remaining = self.config.disperse_duration
+        self._cycles_remaining = self.config.spin_disperse_cycles
         self._initial_phase_time_remaining = 100
 
     def __next__(self) -> str:
         if self._phase != "complete":
             if self._phase == "start":
                 if not self._initial_phase_time_remaining:
                     self._phase = "disperse"
@@ -327,59 +326,56 @@
                                 EventHandler.Event.PATH_COMPLETE,
                                 initial_path,
                                 EventHandler.Action.ACTIVATE_PATH,
                                 disperse_path,
                             )
                             character.animation.activate_scene(character.animation.query_scene("disperse"))
                             character.motion.activate_path(initial_path)
-                            self._active_chars.append(character)
+                            self.active_characters.append(character)
 
-                    for character in self._non_ring_chars:
+                    for character in self.non_ring_chars:
                         character.motion.activate_path(character.motion.query_path("external"))
-                        self._active_chars.append(character)
+                        self.active_characters.append(character)
 
                 else:
                     if not self._disperse_time_remaining:
                         self._phase = "spin"
                         self._cycles_remaining -= 1
-                        self._spin_time_remaining = self._config.spin_duration
+                        self._spin_time_remaining = self.config.spin_duration
                         for ring in self._rings_list:
                             ring.spin()
                     else:
                         self._disperse_time_remaining -= 1
 
             elif self._phase == "spin":
                 if not self._spin_time_remaining:
                     if not self._cycles_remaining:
                         self._phase = "final"
-                        for character in self._terminal.get_characters():
-                            self._terminal.set_character_visibility(character, True)
+                        for character in self.terminal.get_characters():
+                            self.terminal.set_character_visibility(character, True)
                             character.motion.activate_path(character.motion.query_path("home"))
-                            self._active_chars.append(character)
+                            self.active_characters.append(character)
                             if "external" in character.motion.paths:
                                 continue
                             character.animation.activate_scene(character.animation.query_scene("disperse"))
                     else:
-                        self._disperse_time_remaining = self._config.disperse_duration
+                        self._disperse_time_remaining = self.config.disperse_duration
                         for ring in self._rings_list:
                             ring.disperse()
                         self._phase = "disperse"
 
                 else:
                     self._spin_time_remaining -= 1
 
             elif self._phase == "final":
-                if not self._active_chars:
+                if not self.active_characters:
                     self._phase = "complete"
 
-            for character in self._active_chars:
-                character.tick()
-            next_frame = self._terminal.get_formatted_output_string()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return next_frame
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Rings(BaseEffect[RingsConfig]):
     """Characters are dispersed and form into spinning rings.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_scattered.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_scattered.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,62 +97,59 @@
     def get_effect_class(cls):
         return Scattered
 
 
 class ScatteredIterator(BaseEffectIterator[ScatteredConfig]):
     def __init__(self, effect: "Scattered") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-            if self._terminal.output_area.right < 2 or self._terminal.output_area.top < 2:
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+            if self.terminal.output_area.right < 2 or self.terminal.output_area.top < 2:
                 character.motion.set_coordinate(Coord(1, 1))
             else:
-                character.motion.set_coordinate(self._terminal.output_area.random_coord())
+                character.motion.set_coordinate(self.terminal.output_area.random_coord())
             input_coord_path = character.motion.new_path(
-                speed=self._config.movement_speed, ease=self._config.movement_easing
+                speed=self.config.movement_speed, ease=self.config.movement_easing
             )
             input_coord_path.new_waypoint(character.input_coord)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_ACTIVATED, input_coord_path, EventHandler.Action.SET_LAYER, 1
             )
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE, input_coord_path, EventHandler.Action.SET_LAYER, 0
             )
             character.motion.activate_path(input_coord_path)
-            self._terminal.set_character_visibility(character, True)
+            self.terminal.set_character_visibility(character, True)
             gradient_scn = character.animation.new_scene()
             char_gradient = graphics.Gradient(
-                final_gradient.spectrum[0], self._character_final_color_map[character], steps=10
+                final_gradient.spectrum[0], self.character_final_color_map[character], steps=10
             )
             gradient_scn.apply_gradient_to_symbols(
-                char_gradient, character.input_symbol, self._config.final_gradient_frames
+                char_gradient, character.input_symbol, self.config.final_gradient_frames
             )
             character.animation.activate_scene(gradient_scn)
-            self._active_chars.append(character)
+            self.active_characters.append(character)
         self._initial_hold_frames = 25
 
     def __next__(self) -> str:
-        if self._pending_chars or self._active_chars:
+        if self.pending_chars or self.active_characters:
             if self._initial_hold_frames:
                 self._initial_hold_frames -= 1
-                return self._terminal.get_formatted_output_string()
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+                return self.frame
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Scattered(BaseEffect[ScatteredConfig]):
     """Text is scattered across the output area and moves into position.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_slide.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_slide.py`

 * *Files 7% similar despite different names*

```diff
@@ -132,123 +132,120 @@
     def get_effect_class(cls):
         return Slide
 
 
 class SlideIterator(BaseEffectIterator[SlideConfig]):
     def __init__(self, effect: "Slide") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._pending_groups: list[list[EffectCharacter]] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.pending_groups: list[list[EffectCharacter]] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
 
         groups: list[list[EffectCharacter]] = []
-        if self._config.grouping == "row":
-            groups = self._terminal.get_characters_grouped(self._terminal.CharacterGroup.ROW_TOP_TO_BOTTOM)
-        elif self._config.grouping == "column":
-            groups = self._terminal.get_characters_grouped(self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT)
-        elif self._config.grouping == "diagonal":
-            groups = self._terminal.get_characters_grouped(
-                self._terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT
+        if self.config.grouping == "row":
+            groups = self.terminal.get_characters_grouped(self.terminal.CharacterGroup.ROW_TOP_TO_BOTTOM)
+        elif self.config.grouping == "column":
+            groups = self.terminal.get_characters_grouped(self.terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT)
+        elif self.config.grouping == "diagonal":
+            groups = self.terminal.get_characters_grouped(
+                self.terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT
             )
         for group in groups:
             for character in group:
                 input_path = character.motion.new_path(
-                    id="input_path", speed=self._config.movement_speed, ease=self._config.movement_easing
+                    id="input_path", speed=self.config.movement_speed, ease=self.config.movement_easing
                 )
                 input_path.new_waypoint(character.input_coord)
 
         for group_index, group in enumerate(groups):
-            if self._config.grouping == "row":
-                if self._config.merge and group_index % 2 == 0:
-                    starting_column = self._terminal.output_area.right + 1
+            if self.config.grouping == "row":
+                if self.config.merge and group_index % 2 == 0:
+                    starting_column = self.terminal.output_area.right + 1
                 else:
                     groups[group_index] = groups[group_index][::-1]
-                    starting_column = self._terminal.output_area.left - 1
-                if self._config.reverse_direction and not self._config.merge:
+                    starting_column = self.terminal.output_area.left - 1
+                if self.config.reverse_direction and not self.config.merge:
                     groups[group_index] = groups[group_index][::-1]
-                    starting_column = self._terminal.output_area.right + 1
+                    starting_column = self.terminal.output_area.right + 1
                 for character in groups[group_index]:
                     character.motion.set_coordinate(geometry.Coord(starting_column, character.input_coord.row))
-            elif self._config.grouping == "column":
-                if self._config.merge and group_index % 2 == 0:
-                    starting_row = self._terminal.output_area.bottom - 1
+            elif self.config.grouping == "column":
+                if self.config.merge and group_index % 2 == 0:
+                    starting_row = self.terminal.output_area.bottom - 1
                 else:
                     groups[group_index] = groups[group_index][::-1]
-                    starting_row = self._terminal.output_area.top + 1
-                if self._config.reverse_direction and not self._config.merge:
+                    starting_row = self.terminal.output_area.top + 1
+                if self.config.reverse_direction and not self.config.merge:
                     groups[group_index] = groups[group_index][::-1]
-                    starting_row = self._terminal.output_area.bottom - 1
+                    starting_row = self.terminal.output_area.bottom - 1
                 for character in groups[group_index]:
                     character.motion.set_coordinate(geometry.Coord(character.input_coord.column, starting_row))
-            if self._config.grouping == "diagonal":
-                distance_from_outside_bottom = group[-1].input_coord.row - (self._terminal.output_area.bottom - 1)
+            if self.config.grouping == "diagonal":
+                distance_from_outside_bottom = group[-1].input_coord.row - (self.terminal.output_area.bottom - 1)
                 starting_coord = geometry.Coord(
                     group[-1].input_coord.column - distance_from_outside_bottom,
                     group[-1].input_coord.row - distance_from_outside_bottom,
                 )
-                if self._config.merge and group_index % 2 == 0:
+                if self.config.merge and group_index % 2 == 0:
                     groups[group_index] = groups[group_index][::-1]
-                    distance_from_outside = (self._terminal.output_area.top + 1) - group[0].input_coord.row
+                    distance_from_outside = (self.terminal.output_area.top + 1) - group[0].input_coord.row
                     starting_coord = geometry.Coord(
                         group[0].input_coord.column + distance_from_outside,
                         group[0].input_coord.row + distance_from_outside,
                     )
-                if self._config.reverse_direction and not self._config.merge:
+                if self.config.reverse_direction and not self.config.merge:
                     groups[group_index] = groups[group_index][::-1]
-                    distance_from_outside = (self._terminal.output_area.top + 1) - group[0].input_coord.row
+                    distance_from_outside = (self.terminal.output_area.top + 1) - group[0].input_coord.row
                     starting_coord = geometry.Coord(
                         group[0].input_coord.column + distance_from_outside,
                         group[0].input_coord.row + distance_from_outside,
                     )
 
                 for character in groups[group_index]:
                     character.motion.set_coordinate(starting_coord)
             for character in group:
                 gradient_scn = character.animation.new_scene()
                 char_gradient = graphics.Gradient(
-                    self._config.final_gradient_stops[0], self._character_final_color_map[character], steps=10
+                    self.config.final_gradient_stops[0], self.character_final_color_map[character], steps=10
                 )
                 gradient_scn.apply_gradient_to_symbols(
-                    char_gradient, character.input_symbol, self._config.final_gradient_frames
+                    char_gradient, character.input_symbol, self.config.final_gradient_frames
                 )
                 character.animation.activate_scene(gradient_scn)
 
-        self._pending_groups = groups
+        self.pending_groups = groups
         self._active_groups: list[list[EffectCharacter]] = []
         self._current_gap = 0
 
     def __next__(self) -> str:
-        if self._pending_groups or self._active_chars or self._active_groups:
-            if self._current_gap == self._config.gap and self._pending_groups:
-                self._active_groups.append(self._pending_groups.pop(0))
+        if self.pending_groups or self.active_characters or self._active_groups:
+            if self._current_gap == self.config.gap and self.pending_groups:
+                self._active_groups.append(self.pending_groups.pop(0))
                 self._current_gap = 0
             else:
-                if self._pending_groups:
+                if self.pending_groups:
                     self._current_gap += 1
             for group in self._active_groups:
                 if group:
                     next_char = group.pop(0)
-                    self._terminal.set_character_visibility(next_char, True)
+                    self.terminal.set_character_visibility(next_char, True)
                     next_char.motion.activate_path(next_char.motion.paths["input_path"])
-                    self._active_chars.append(next_char)
+                    self.active_characters.append(next_char)
             self._active_groups = [group for group in self._active_groups if group]
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Slide(BaseEffect[SlideConfig]):
     """Slides characters into view from outside the terminal.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_spotlights.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_spotlights.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,147 +123,142 @@
     def get_effect_class(cls):
         return Spotlights
 
 
 class SpotlightsIterator(BaseEffectIterator[SpotlightsConfig]):
     def __init__(self, effect: "Spotlights") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._illuminated_chars: set[EffectCharacter] = set()
-        self._character_color_map: dict[EffectCharacter, tuple[graphics.Color, graphics.Color]] = {}  # (bright, dark)
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.illuminated_chars: set[EffectCharacter] = set()
+        self.character_color_map: dict[EffectCharacter, tuple[graphics.Color, graphics.Color]] = {}  # (bright, dark)
+        self.build()
 
-    def _make_spotlights(self, num_spotlights: int) -> list[EffectCharacter]:
+    def make_spotlights(self, num_spotlights: int) -> list[EffectCharacter]:
         spotlights: list[EffectCharacter] = []
-        minimum_distance = self._terminal.output_area.right // 4
+        minimum_distance = self.terminal.output_area.right // 4
         for _ in range(num_spotlights):
-            spotlight = self._terminal.add_character("O", self._terminal.output_area.random_coord(outside_scope=True))
+            spotlight = self.terminal.add_character("O", self.terminal.output_area.random_coord(outside_scope=True))
             spotlights.append(spotlight)
 
             spotlight_target_coords: list[Coord] = []
-            last_coord = self._terminal.output_area.random_coord()
+            last_coord = self.terminal.output_area.random_coord()
             spotlight_target_coords.append(last_coord)
             for _ in range(10):
-                next_coord = self._find_coord_at_minimum_distance(last_coord, minimum_distance)
+                next_coord = self.find_coord_at_minimum_distance(last_coord, minimum_distance)
                 spotlight_target_coords.append(next_coord)
                 last_coord = next_coord
 
             paths: list[motion.Path] = []
             for coord in spotlight_target_coords:
                 path = spotlight.motion.new_path(
-                    speed=random.uniform(self._config.search_speed_range[0], self._config.search_speed_range[1]),
+                    speed=random.uniform(self.config.search_speed_range[0], self.config.search_speed_range[1]),
                     ease=easing.in_out_quad,
                     id=str(len(paths)),
                 )
-                path.new_waypoint(coord, bezier_control=self._terminal.output_area.random_coord(outside_scope=True))
+                path.new_waypoint(coord, bezier_control=self.terminal.output_area.random_coord(outside_scope=True))
                 paths.append(path)
             spotlight.motion.chain_paths(paths, loop=True)
 
             path = spotlight.motion.new_path(speed=0.5, ease=easing.in_out_sine, id="center")
-            path.new_waypoint(self._terminal.output_area.center)
+            path.new_waypoint(self.terminal.output_area.center)
 
         return spotlights
 
-    def _find_coord_at_minimum_distance(self, origin_coord: Coord, minimum_distance: int) -> Coord:
+    def find_coord_at_minimum_distance(self, origin_coord: Coord, minimum_distance: int) -> Coord:
         coord_found = False
         while not coord_found:
-            coord = self._terminal.output_area.random_coord()
+            coord = self.terminal.output_area.random_coord()
             distance = geometry.find_length_of_line(origin_coord, coord)
             if distance >= minimum_distance:
                 coord_found = True
         return coord
 
-    def _illuminate_chars(self, range: int) -> None:
+    def illuminate_chars(self, range: int) -> None:
         coords_in_range: list[Coord] = []
-        for spotlight in self._spotlights:
+        for spotlight in self.spotlights:
             coords_in_range.extend(geometry.find_coords_in_circle(spotlight.motion.current_coord, range))
         chars_in_range: set[EffectCharacter] = set()
         for coord in coords_in_range:
-            character = self._terminal.get_character_by_input_coord(coord)
+            character = self.terminal.get_character_by_input_coord(coord)
             if character and character.symbol != " ":
                 chars_in_range.add(character)
-        chars_no_longer_in_range = self._illuminated_chars - chars_in_range
+        chars_no_longer_in_range = self.illuminated_chars - chars_in_range
         for character in chars_no_longer_in_range:
             character.animation.set_appearance(
                 character.input_symbol,
-                self._character_color_map[character][1],
+                self.character_color_map[character][1],
             )
 
         for character in chars_in_range:
             distance = min(
                 [
                     geometry.find_length_of_line(
                         spotlight.motion.current_coord, character.input_coord, double_row_diff=True
                     )
-                    for spotlight in self._spotlights
+                    for spotlight in self.spotlights
                 ]
             )
 
-            if distance > range * (1 - self._config.beam_falloff):
+            if distance > range * (1 - self.config.beam_falloff):
                 brightness_factor = max(
-                    1 - (distance - range * (1 - self._config.beam_falloff)) / (range * self._config.beam_falloff), 0.2
+                    1 - (distance - range * (1 - self.config.beam_falloff)) / (range * self.config.beam_falloff), 0.2
                 )
                 adjusted_color = animation.Animation.adjust_color_brightness(
-                    self._character_color_map[character][0], brightness_factor
+                    self.character_color_map[character][0], brightness_factor
                 )
             else:
-                adjusted_color = self._character_color_map[character][0]
+                adjusted_color = self.character_color_map[character][0]
             character.animation.set_appearance(character.input_symbol, adjusted_color)
-        self._illuminated_chars = chars_in_range
+        self.illuminated_chars = chars_in_range
 
-    def _build(self) -> None:
-        self._spotlights: list[EffectCharacter] = self._make_spotlights(self._config.spotlight_count)
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        self.spotlights: list[EffectCharacter] = self.make_spotlights(self.config.spotlight_count)
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
+        for character in self.terminal.get_characters():
             color_bright = final_gradient_mapping[character.input_coord]
-            self._terminal.set_character_visibility(character, True)
+            self.terminal.set_character_visibility(character, True)
             color_dark = animation.Animation.adjust_color_brightness(color_bright, 0.2)
-            self._character_color_map[character] = (color_bright, color_dark)
+            self.character_color_map[character] = (color_bright, color_dark)
             character.animation.set_appearance(character.input_symbol, color_dark)
-        self._illuminate_range = int(
+        self.illuminate_range = int(
             max(
-                min(self._terminal.output_area.right, self._terminal.output_area.top) // self._config.beam_width_ratio,
+                min(self.terminal.output_area.right, self.terminal.output_area.top) // self.config.beam_width_ratio,
                 1,
             )
         )
-        self._search_duration = self._config.search_duration
-        self._searching = True
-        self._complete = False
-        for spotlight in self._spotlights:
+        self.search_duration = self.config.search_duration
+        self.searching = True
+        self.complete = False
+        for spotlight in self.spotlights:
             spotlight_path_start = spotlight.motion.query_path("0")
             spotlight.motion.activate_path(spotlight_path_start)
-            self._active_chars.append(spotlight)
+            self.active_characters.append(spotlight)
 
     def __next__(self) -> str:
-        if not self._complete:
-            self._illuminate_chars(self._illuminate_range)
-            if self._searching:
-                self._search_duration -= 1
-                if not self._search_duration:
-                    for spotlight in self._spotlights:
+        if not self.complete:
+            self.illuminate_chars(self.illuminate_range)
+            if self.searching:
+                self.search_duration -= 1
+                if not self.search_duration:
+                    for spotlight in self.spotlights:
                         spotlight_path_center = spotlight.motion.query_path("center")
                         spotlight.motion.activate_path(spotlight_path_center)
-                    self._searching = False
-            if not any([spotlight.motion.active_path for spotlight in self._spotlights]):
-                while len(self._spotlights) > 1:
-                    self._spotlights.pop()
-                self._illuminate_range += 1
-                if (
-                    self._illuminate_range
-                    > max(self._terminal.output_area.right, self._terminal.output_area.top) // 1.5
-                ):
-                    self._complete = True
-
-            for character in self._active_chars:
-                character.tick()
-            return self._terminal.get_formatted_output_string()
+                    self.searching = False
+            if not any([spotlight.motion.active_path for spotlight in self.spotlights]):
+                while len(self.spotlights) > 1:
+                    self.spotlights.pop()
+                self.illuminate_range += 1
+                if self.illuminate_range > max(self.terminal.output_area.right, self.terminal.output_area.top) // 1.5:
+                    self.complete = True
+
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Spotlights(BaseEffect[SpotlightsConfig]):
     """Spotlights search the text area, illuminating characters, before converging in the center and expanding.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_spray.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_spray.py`

 * *Files 24% similar despite different names*

```diff
@@ -108,112 +108,102 @@
 
     @classmethod
     def get_effect_class(cls):
         return Spray
 
 
 class SprayIterator(BaseEffectIterator[SprayConfig]):
-    class _SprayPosition(Enum):
+    class SprayPosition(Enum):
         N = auto()
         NE = auto()
         E = auto()
         SE = auto()
         S = auto()
         SW = auto()
         W = auto()
         NW = auto()
         CENTER = auto()
 
-    def __init__(
-        self,
-        effect: "Spray",
-    ) -> None:
+    def __init__(self, effect: "Spray") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
+    def build(self) -> None:
         self._spray_position = {
-            "n": SprayIterator._SprayPosition.N,
-            "ne": SprayIterator._SprayPosition.NE,
-            "e": SprayIterator._SprayPosition.E,
-            "se": SprayIterator._SprayPosition.SE,
-            "s": SprayIterator._SprayPosition.S,
-            "sw": SprayIterator._SprayPosition.SW,
-            "w": SprayIterator._SprayPosition.W,
-            "nw": SprayIterator._SprayPosition.NW,
-            "center": SprayIterator._SprayPosition.CENTER,
-        }.get(self._config.spray_position, SprayIterator._SprayPosition.E)
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+            "n": SprayIterator.SprayPosition.N,
+            "ne": SprayIterator.SprayPosition.NE,
+            "e": SprayIterator.SprayPosition.E,
+            "se": SprayIterator.SprayPosition.SE,
+            "s": SprayIterator.SprayPosition.S,
+            "sw": SprayIterator.SprayPosition.SW,
+            "w": SprayIterator.SprayPosition.W,
+            "nw": SprayIterator.SprayPosition.NW,
+            "center": SprayIterator.SprayPosition.CENTER,
+        }.get(self.config.spray_position, SprayIterator.SprayPosition.E)
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         spray_origin_map = {
-            SprayIterator._SprayPosition.CENTER: (self._terminal.output_area.center),
-            SprayIterator._SprayPosition.N: Coord(
-                self._terminal.output_area.right // 2, self._terminal.output_area.top
+            SprayIterator.SprayPosition.CENTER: (self.terminal.output_area.center),
+            SprayIterator.SprayPosition.N: Coord(self.terminal.output_area.right // 2, self.terminal.output_area.top),
+            SprayIterator.SprayPosition.NW: Coord(self.terminal.output_area.left, self.terminal.output_area.top),
+            SprayIterator.SprayPosition.W: Coord(self.terminal.output_area.left, self.terminal.output_area.top // 2),
+            SprayIterator.SprayPosition.SW: Coord(self.terminal.output_area.left, self.terminal.output_area.bottom),
+            SprayIterator.SprayPosition.S: Coord(
+                self.terminal.output_area.right // 2, self.terminal.output_area.bottom
             ),
-            SprayIterator._SprayPosition.NW: Coord(self._terminal.output_area.left, self._terminal.output_area.top),
-            SprayIterator._SprayPosition.W: Coord(self._terminal.output_area.left, self._terminal.output_area.top // 2),
-            SprayIterator._SprayPosition.SW: Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
-            SprayIterator._SprayPosition.S: Coord(
-                self._terminal.output_area.right // 2, self._terminal.output_area.bottom
+            SprayIterator.SprayPosition.SE: Coord(
+                self.terminal.output_area.right - 1, self.terminal.output_area.bottom
             ),
-            SprayIterator._SprayPosition.SE: Coord(
-                self._terminal.output_area.right - 1, self._terminal.output_area.bottom
-            ),
-            SprayIterator._SprayPosition.E: Coord(
-                self._terminal.output_area.right - 1, self._terminal.output_area.top // 2
-            ),
-            SprayIterator._SprayPosition.NE: Coord(
-                self._terminal.output_area.right - 1, self._terminal.output_area.top
+            SprayIterator.SprayPosition.E: Coord(
+                self.terminal.output_area.right - 1, self.terminal.output_area.top // 2
             ),
+            SprayIterator.SprayPosition.NE: Coord(self.terminal.output_area.right - 1, self.terminal.output_area.top),
         }
 
-        for character in self._terminal.get_characters():
+        for character in self.terminal.get_characters():
             character.motion.set_coordinate(spray_origin_map[self._spray_position])
             input_coord_path = character.motion.new_path(
-                speed=random.uniform(self._config.movement_speed[0], self._config.movement_speed[1]),
-                ease=self._config.movement_easing,
+                speed=random.uniform(self.config.movement_speed[0], self.config.movement_speed[1]),
+                ease=self.config.movement_easing,
             )
             input_coord_path.new_waypoint(character.input_coord)
             character.event_handler.register_event(
                 EventHandler.Event.PATH_ACTIVATED, input_coord_path, EventHandler.Action.SET_LAYER, 1
             )
             character.event_handler.register_event(
                 EventHandler.Event.PATH_COMPLETE, input_coord_path, EventHandler.Action.SET_LAYER, 0
             )
             droplet_scn = character.animation.new_scene()
             spray_gradient = graphics.Gradient(
-                random.choice(final_gradient.spectrum), self._character_final_color_map[character], steps=7
+                random.choice(final_gradient.spectrum), self.character_final_color_map[character], steps=7
             )
             droplet_scn.apply_gradient_to_symbols(spray_gradient, character.input_symbol, 20)
             character.animation.activate_scene(droplet_scn)
             character.motion.activate_path(input_coord_path)
-            self._pending_chars.append(character)
-        random.shuffle(self._pending_chars)
-        self._volume = max(int(len(self._pending_chars) * self._config.spray_volume), 1)
+            self.pending_chars.append(character)
+        random.shuffle(self.pending_chars)
+        self._volume = max(int(len(self.pending_chars) * self.config.spray_volume), 1)
 
     def __next__(self) -> str:
-        if self._pending_chars or self._active_chars:
-            if self._pending_chars:
+        if self.pending_chars or self.active_characters:
+            if self.pending_chars:
                 for _ in range(random.randint(1, self._volume)):
-                    if self._pending_chars:
-                        next_character = self._pending_chars.pop()
-                        self._terminal.set_character_visibility(next_character, True)
-                        self._active_chars.append(next_character)
-
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+                    if self.pending_chars:
+                        next_character = self.pending_chars.pop()
+                        self.terminal.set_character_visibility(next_character, True)
+                        self.active_characters.append(next_character)
+
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Spray(BaseEffect[SprayConfig]):
     """Sprays the characters from a single point.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_swarm.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_swarm.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,66 +125,63 @@
 
 class SwarmIterator(BaseEffectIterator[SwarmConfig]):
     def __init__(
         self,
         effect: "Swarm",
     ) -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._swarms: list[list[EffectCharacter]] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.swarms: list[list[EffectCharacter]] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _make_swarms(self, swarm_size: int) -> None:
-        unswarmed_characters = list(self._terminal._input_characters[::-1])
+    def make_swarms(self, swarm_size: int) -> None:
+        unswarmed_characters = list(self.terminal._input_characters[::-1])
         while unswarmed_characters:
             new_swarm: list[EffectCharacter] = []
             for _ in range(swarm_size):
                 if unswarmed_characters:
                     new_swarm.append(unswarmed_characters.pop())
                 else:
                     break
-            self._swarms.append(new_swarm)
+            self.swarms.append(new_swarm)
 
-    def _build(self) -> None:
-        swarm_size: int = max(round(len(self._terminal._input_characters) * self._config.swarm_size), 1)
-        self._make_swarms(swarm_size)
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        swarm_size: int = max(round(len(self.terminal._input_characters) * self.config.swarm_size), 1)
+        self.make_swarms(swarm_size)
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        flash_list = [self._config.flash_color for _ in range(10)]
-        for swarm in self._swarms:
-            swarm_gradient = graphics.Gradient(
-                random.choice(self._config.base_color), self._config.flash_color, steps=7
-            )
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        flash_list = [self.config.flash_color for _ in range(10)]
+        for swarm in self.swarms:
+            swarm_gradient = graphics.Gradient(random.choice(self.config.base_color), self.config.flash_color, steps=7)
             swarm_gradient_mirror = list(swarm_gradient) + flash_list + list(swarm_gradient)[::-1]
             swarm_area_coordinate_map: dict[Coord, list[Coord]] = {}
-            swarm_spawn = self._terminal.output_area.random_coord(outside_scope=True)
+            swarm_spawn = self.terminal.output_area.random_coord(outside_scope=True)
             swarm_areas: list[Coord] = []
-            swarm_area_count = random.randint(self._config.swarm_area_count[0], self._config.swarm_area_count[1])
+            swarm_area_count = random.randint(self.config.swarm_area_count[0], self.config.swarm_area_count[1])
             # create areas where characters will swarm
             last_focus_coord = swarm_spawn
-            radius = max(min(self._terminal.output_area.right, self._terminal.output_area.top) // 2, 1)
+            radius = max(min(self.terminal.output_area.right, self.terminal.output_area.top) // 2, 1)
             while len(swarm_areas) < swarm_area_count:
                 potential_focus_coords = geometry.find_coords_on_circle(last_focus_coord, radius)
                 random.shuffle(potential_focus_coords)
                 for coord in potential_focus_coords:
-                    if self._terminal.output_area.coord_is_in_output_area(coord):
+                    if self.terminal.output_area.coord_is_in_output_area(coord):
                         next_focus_coord = coord
                         break
                 else:
-                    next_focus_coord = self._terminal.output_area.random_coord()
+                    next_focus_coord = self.terminal.output_area.random_coord()
                 swarm_areas.append(next_focus_coord)
                 swarm_area_coordinate_map[last_focus_coord] = geometry.find_coords_in_circle(
                     last_focus_coord,
-                    max(min(self._terminal.output_area.right, self._terminal.output_area.top) // 6, 1) * 2,
+                    max(min(self.terminal.output_area.right, self.terminal.output_area.top) // 6, 1) * 2,
                 )
                 last_focus_coord = next_focus_coord
 
             # assign characters waypoints for swarm areas and inner waypoints within the swarm areas
             for character in swarm:
                 swarm_area_count = 0
                 character.motion.set_coordinate(swarm_spawn)
@@ -218,61 +215,59 @@
                         )
                         inner_path.new_waypoint(next_coord, id=str(len(character.motion.paths)))
                 # create landing waypoint and scene
                 input_path = character.motion.new_path(speed=0.3, ease=easing.in_out_quad)
                 input_path.new_waypoint(character.input_coord)
                 input_scn = character.animation.new_scene()
                 for step in graphics.Gradient(
-                    self._config.flash_color, self._character_final_color_map[character], steps=10
+                    self.config.flash_color, self.character_final_color_map[character], steps=10
                 ):
                     input_scn.add_frame(character.input_symbol, 3, color=step)
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE, input_path, EventHandler.Action.ACTIVATE_SCENE, input_scn
                 )
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_COMPLETE, input_path, EventHandler.Action.SET_LAYER, 0
                 )
                 character.event_handler.register_event(
                     EventHandler.Event.PATH_ACTIVATED, input_path, EventHandler.Action.ACTIVATE_SCENE, flash_scn
                 )
                 character.motion.chain_paths(list(character.motion.paths.values()))
-        self._call_next = False
-        self._active_swarm_area = "0_swarm_area"
-        self._current_swarm = self._swarms.pop()
+        self.call_next = False
+        self.active_swarm_area = "0_swarm_area"
+        self.current_swarm = self.swarms.pop()
 
     def __next__(self) -> str:
-        if self._swarms or self._active_chars:
-            if self._swarms and self._call_next:
-                self._call_next = False
-                self._current_swarm = self._swarms.pop()
-                self._active_swarm_area = "0_swarm_area"
-                for character in self._current_swarm:
+        if self.swarms or self.active_characters:
+            if self.swarms and self.call_next:
+                self.call_next = False
+                self.current_swarm = self.swarms.pop()
+                self.active_swarm_area = "0_swarm_area"
+                for character in self.current_swarm:
                     character.motion.activate_path(character.motion.query_path("0_swarm_area"))
-                    self._terminal.set_character_visibility(character, True)
-                    self._active_chars.append(character)
-            for character in self._active_chars:
-                character.tick()
-            if len(self._active_chars) < len(self._current_swarm):
-                self._call_next = True
-            if self._current_swarm:
-                for character in self._current_swarm:
+                    self.terminal.set_character_visibility(character, True)
+                    self.active_characters.append(character)
+            if len(self.active_characters) < len(self.current_swarm):
+                self.call_next = True
+            if self.current_swarm:
+                for character in self.current_swarm:
                     if (
                         character.motion.active_path
-                        and character.motion.active_path.path_id != self._active_swarm_area
+                        and character.motion.active_path.path_id != self.active_swarm_area
                         and "swarm_area" in character.motion.active_path.path_id
-                        and int(character.motion.active_path.path_id[0]) > int(self._active_swarm_area[0])
+                        and int(character.motion.active_path.path_id[0]) > int(self.active_swarm_area[0])
                     ):
-                        self._active_swarm_area = character.motion.active_path.path_id
-                        for other in self._current_swarm:
-                            if other is not character and random.random() < self._config.swarm_coordination:
-                                other.motion.activate_path(other.motion.paths[self._active_swarm_area])
+                        self.active_swarm_area = character.motion.active_path.path_id
+                        for other in self.current_swarm:
+                            if other is not character and random.random() < self.config.swarm_coordination:
+                                other.motion.activate_path(other.motion.paths[self.active_swarm_area])
                         break
 
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Swarm(BaseEffect[SwarmConfig]):
     """Characters are grouped into swarms and move around the terminal before settling into position.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_synthgrid.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_synthgrid.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     "float : Maximum percentage of blocks to have active at any given time."
 
     @classmethod
     def get_effect_class(cls):
         return SynthGrid
 
 
-class _GridLine:
+class GridLine:
     def __init__(
         self,
         terminal: Terminal,
         args: SynthGridConfig,
         origin: Coord,
         direction: str,
         grid_gradient_mapping: dict[geometry.Coord, graphics.Color],
@@ -217,21 +217,20 @@
     def is_collapsed(self) -> bool:
         return not self.extended_characters
 
 
 class SynthGridIterator(BaseEffectIterator[SynthGridConfig]):
     def __init__(self, effect: "SynthGrid") -> None:
         super().__init__(effect)
-        self._pending_groups: list[tuple[int, list[EffectCharacter]]] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._grid_lines: list[_GridLine] = []
-        self._group_tracker: dict[int, int] = {}
-        self._build()
+        self.pending_groups: list[tuple[int, list[EffectCharacter]]] = []
+        self.grid_lines: list[GridLine] = []
+        self.group_tracker: dict[int, int] = {}
+        self.build()
 
-    def _find_even_gap(self, dimension: int) -> int:
+    def find_even_gap(self, dimension: int) -> int:
         """Find the closest even gap to 20% of the longest dimension.
 
         Args:
             dimension (int): The longest dimension.
 
         Returns:
             int: The gap that is closest to 20% of the dimension length.
@@ -243,186 +242,183 @@
         for i in range(dimension, 4, -1):
             if dimension % i <= 1:
                 potential_gaps.append(i)
         if not potential_gaps:
             return 4
         return min(potential_gaps, key=lambda x: abs(x - dimension // 5))
 
-    def _build(self) -> None:
-        grid_gradient = graphics.Gradient(*self._config.grid_gradient_stops, steps=self._config.grid_gradient_steps)
+    def build(self) -> None:
+        grid_gradient = graphics.Gradient(*self.config.grid_gradient_stops, steps=self.config.grid_gradient_steps)
         grid_gradient_mapping = grid_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.grid_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.grid_gradient_direction
         )
-        text_gradient = graphics.Gradient(*self._config.text_gradient_stops, steps=self._config.text_gradient_steps)
+        text_gradient = graphics.Gradient(*self.config.text_gradient_stops, steps=self.config.text_gradient_steps)
         text_gradient_mapping = text_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.text_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.text_gradient_direction
         )
 
-        self._grid_lines.append(
-            _GridLine(
-                self._terminal,
-                self._config,
-                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
+        self.grid_lines.append(
+            GridLine(
+                self.terminal,
+                self.config,
+                Coord(self.terminal.output_area.left, self.terminal.output_area.bottom),
                 "horizontal",
                 grid_gradient_mapping,
             )
         )
-        self._grid_lines.append(
-            _GridLine(
-                self._terminal,
-                self._config,
-                Coord(self._terminal.output_area.left, self._terminal.output_area.top),
+        self.grid_lines.append(
+            GridLine(
+                self.terminal,
+                self.config,
+                Coord(self.terminal.output_area.left, self.terminal.output_area.top),
                 "horizontal",
                 grid_gradient_mapping,
             )
         )
-        self._grid_lines.append(
-            _GridLine(
-                self._terminal,
-                self._config,
-                Coord(self._terminal.output_area.left, self._terminal.output_area.bottom),
+        self.grid_lines.append(
+            GridLine(
+                self.terminal,
+                self.config,
+                Coord(self.terminal.output_area.left, self.terminal.output_area.bottom),
                 "vertical",
                 grid_gradient_mapping,
             )
         )
-        self._grid_lines.append(
-            _GridLine(
-                self._terminal,
-                self._config,
-                Coord(self._terminal.output_area.right, self._terminal.output_area.bottom),
+        self.grid_lines.append(
+            GridLine(
+                self.terminal,
+                self.config,
+                Coord(self.terminal.output_area.right, self.terminal.output_area.bottom),
                 "vertical",
                 grid_gradient_mapping,
             )
         )
         column_indexes: list[int] = []
         row_indexes: list[int] = []
-        if self._terminal.output_area.top > 2 * self._terminal.output_area.right:
-            row_gap = self._find_even_gap(self._terminal.output_area.top) + 1
+        if self.terminal.output_area.top > 2 * self.terminal.output_area.right:
+            row_gap = self.find_even_gap(self.terminal.output_area.top) + 1
             column_gap = row_gap * 2
         else:
-            column_gap = self._find_even_gap(self._terminal.output_area.right) + 1
+            column_gap = self.find_even_gap(self.terminal.output_area.right) + 1
             row_gap = column_gap // 2
 
         for row_index in range(
-            self._terminal.output_area.bottom + row_gap, self._terminal.output_area.top, max(row_gap, 1)
+            self.terminal.output_area.bottom + row_gap, self.terminal.output_area.top, max(row_gap, 1)
         ):
-            if self._terminal.output_area.top - row_index < 2:
+            if self.terminal.output_area.top - row_index < 2:
                 continue
             row_indexes.append(row_index)
-            self._grid_lines.append(
-                _GridLine(
-                    self._terminal,
-                    self._config,
-                    Coord(self._terminal.output_area.left, row_index),
+            self.grid_lines.append(
+                GridLine(
+                    self.terminal,
+                    self.config,
+                    Coord(self.terminal.output_area.left, row_index),
                     "horizontal",
                     grid_gradient_mapping,
                 )
             )
         for column_index in range(
-            self._terminal.output_area.left + column_gap, self._terminal.output_area.right, max(column_gap, 1)
+            self.terminal.output_area.left + column_gap, self.terminal.output_area.right, max(column_gap, 1)
         ):
-            if self._terminal.output_area.right - column_index < 2:
+            if self.terminal.output_area.right - column_index < 2:
                 continue
             column_indexes.append(column_index)
-            self._grid_lines.append(
-                _GridLine(
-                    self._terminal,
-                    self._config,
-                    Coord(column_index, self._terminal.output_area.bottom),
+            self.grid_lines.append(
+                GridLine(
+                    self.terminal,
+                    self.config,
+                    Coord(column_index, self.terminal.output_area.bottom),
                     "vertical",
                     grid_gradient_mapping,
                 )
             )
-        row_indexes.append(self._terminal.output_area.top + 1)
-        column_indexes.append(self._terminal.output_area.right + 1)
+        row_indexes.append(self.terminal.output_area.top + 1)
+        column_indexes.append(self.terminal.output_area.right + 1)
         prev_row_index = 1
         for row_index in row_indexes:
             prev_column_index = 1
             for column_index in column_indexes:
                 coords_in_block: list[Coord] = []
-                if row_index == self._terminal.output_area.top:  # make sure the top row is included
+                if row_index == self.terminal.output_area.top:  # make sure the top row is included
                     row_index += 1
                 for row in range(prev_row_index, row_index):
                     for column in range(prev_column_index, column_index):
                         coords_in_block.append(Coord(column, row))
                 characters_in_block: list[EffectCharacter] = []
                 for coord in coords_in_block:
-                    if coord in self._terminal.character_by_input_coord:
-                        characters_in_block.append(self._terminal.character_by_input_coord[coord])
+                    if coord in self.terminal.character_by_input_coord:
+                        characters_in_block.append(self.terminal.character_by_input_coord[coord])
                 if characters_in_block:
-                    self._pending_groups.append((len(self._pending_groups), characters_in_block))
+                    self.pending_groups.append((len(self.pending_groups), characters_in_block))
                 prev_column_index = column_index
             prev_row_index = row_index
-        for group_number, group in self._pending_groups:
-            self._group_tracker[group_number] = 0
+        for group_number, group in self.pending_groups:
+            self.group_tracker[group_number] = 0
             for character in group:
                 dissolve_scn = character.animation.new_scene()
                 for _ in range(random.randint(15, 30)):
                     dissolve_scn.add_frame(
-                        random.choice(self._config.text_generation_symbols),
+                        random.choice(self.config.text_generation_symbols),
                         3,
                         color=random.choice(text_gradient.spectrum),
                     )
                 dissolve_scn.add_frame(character.input_symbol, 1, color=text_gradient_mapping[character.input_coord])
                 character.animation.activate_scene(dissolve_scn)
                 character.event_handler.register_event(
                     EventHandler.Event.SCENE_COMPLETE,
                     dissolve_scn,
                     EventHandler.Action.CALLBACK,
-                    EventHandler.Callback(self._update_group_tracker, group_number),
+                    EventHandler.Callback(self.update_group_tracker, group_number),
                 )
-        random.shuffle(self._pending_groups)
+        random.shuffle(self.pending_groups)
         self._phase = "grid_expand"
-        self._total_group_count = len(self._pending_groups)
+        self._total_group_count = len(self.pending_groups)
         if not self._total_group_count:
-            for character in self._terminal.get_characters():
-                self._terminal.set_character_visibility(character, True)
-                self._active_chars.append(character)
+            for character in self.terminal.get_characters():
+                self.terminal.set_character_visibility(character, True)
+                self.active_characters.append(character)
         self._active_groups: int = 0
 
-    def _update_group_tracker(self, character: EffectCharacter, *args) -> None:
-        self._group_tracker[args[0]] -= 1
+    def update_group_tracker(self, character: EffectCharacter, *args) -> None:
+        self.group_tracker[args[0]] -= 1
 
     def __next__(self) -> str:
-        if self._pending_groups or self._active_chars or self._phase != "complete":
+        if self.pending_groups or self.active_characters or self._phase != "complete":
             if self._phase == "grid_expand":
-                if not all([grid_line.is_extended() for grid_line in self._grid_lines]):
-                    for grid_line in self._grid_lines:
+                if not all([grid_line.is_extended() for grid_line in self.grid_lines]):
+                    for grid_line in self.grid_lines:
                         if not grid_line.is_extended():
                             grid_line.extend()
                 else:
                     self._phase = "add_chars"
             elif self._phase == "add_chars":
                 if (
-                    self._pending_groups
-                    and self._active_groups < self._total_group_count * self._config.max_active_blocks
+                    self.pending_groups
+                    and self._active_groups < self._total_group_count * self.config.max_active_blocks
                 ):
-                    group_number, next_group = self._pending_groups.pop(0)
+                    group_number, next_group = self.pending_groups.pop(0)
                     for char in next_group:
-                        self._terminal.set_character_visibility(char, True)
-                        self._active_chars.append(char)
-                        self._group_tracker[group_number] += 1
-                if not self._pending_groups and not self._active_chars and not self._active_groups:
+                        self.terminal.set_character_visibility(char, True)
+                        self.active_characters.append(char)
+                        self.group_tracker[group_number] += 1
+                if not self.pending_groups and not self.active_characters and not self._active_groups:
                     self._phase = "collapse"
             elif self._phase == "collapse":
-                if not all([grid_line.is_collapsed() for grid_line in self._grid_lines]):
-                    for grid_line in self._grid_lines:
+                if not all([grid_line.is_collapsed() for grid_line in self.grid_lines]):
+                    for grid_line in self.grid_lines:
                         if not grid_line.is_collapsed():
                             grid_line.collapse()
                 else:
                     self._phase = "complete"
-            for character in self._active_chars:
-                character.tick()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
+            self.update()
             self._active_groups = 0
-            for _, active_count in self._group_tracker.items():
+            for _, active_count in self.group_tracker.items():
                 if active_count:
                     self._active_groups += 1
-            return self._terminal.get_formatted_output_string()
+            return self.frame
         else:
             raise StopIteration
 
 
 class SynthGrid(BaseEffect[SynthGridConfig]):
     """Create a grid which fills with characters dissolving into the final text.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_unstable.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_unstable.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,139 +121,138 @@
     def get_effect_class(cls):
         return Unstable
 
 
 class UnstableIterator(BaseEffectIterator[UnstableConfig]):
     def __init__(self, effect: "Unstable") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._jumbled_coords: dict[EffectCharacter, Coord] = dict()
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.jumbled_coords: dict[EffectCharacter, Coord] = dict()
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
-        character_coords = [character.input_coord for character in self._terminal.get_characters()]
-        for character in self._terminal.get_characters():
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        character_coords = [character.input_coord for character in self.terminal.get_characters()]
+        for character in self.terminal.get_characters():
             pos = random.randint(0, 3)
             match pos:
                 case 0:
-                    col = self._terminal.output_area.left
-                    row = random.randint(1, self._terminal.output_area.top)
+                    col = self.terminal.output_area.left
+                    row = random.randint(1, self.terminal.output_area.top)
                 case 1:
-                    col = self._terminal.output_area.right
-                    row = random.randint(1, self._terminal.output_area.top)
+                    col = self.terminal.output_area.right
+                    row = random.randint(1, self.terminal.output_area.top)
                 case 2:
-                    col = random.randint(1, self._terminal.output_area.right)
-                    row = self._terminal.output_area.bottom
+                    col = random.randint(1, self.terminal.output_area.right)
+                    row = self.terminal.output_area.bottom
                 case 3:
-                    col = random.randint(1, self._terminal.output_area.right)
-                    row = self._terminal.output_area.top
+                    col = random.randint(1, self.terminal.output_area.right)
+                    row = self.terminal.output_area.top
             jumbled_coord = character_coords.pop(random.randint(0, len(character_coords) - 1))
-            self._jumbled_coords[character] = jumbled_coord
+            self.jumbled_coords[character] = jumbled_coord
             character.motion.set_coordinate(jumbled_coord)
-            explosion_path = character.motion.new_path(id="explosion", speed=1.25, ease=self._config.explosion_ease)
+            explosion_path = character.motion.new_path(id="explosion", speed=1.25, ease=self.config.explosion_ease)
             explosion_path.new_waypoint(Coord(col, row))
-            reassembly_path = character.motion.new_path(id="reassembly", speed=0.75, ease=self._config.reassembly_ease)
+            reassembly_path = character.motion.new_path(id="reassembly", speed=0.75, ease=self.config.reassembly_ease)
             reassembly_path.new_waypoint(character.input_coord)
             unstable_gradient = graphics.Gradient(
-                self._character_final_color_map[character], self._config.unstable_color, steps=25
+                self.character_final_color_map[character], self.config.unstable_color, steps=25
             )
             rumble_scn = character.animation.new_scene(id="rumble")
             rumble_scn.apply_gradient_to_symbols(
                 unstable_gradient,
                 character.input_symbol,
                 10,
             )
             final_color = graphics.Gradient(
-                self._config.unstable_color, self._character_final_color_map[character], steps=12
+                self.config.unstable_color, self.character_final_color_map[character], steps=12
             )
             final_scn = character.animation.new_scene(id="final")
             final_scn.apply_gradient_to_symbols(final_color, character.input_symbol, 5)
             character.animation.activate_scene(rumble_scn)
-            self._terminal.set_character_visibility(character, True)
+            self.terminal.set_character_visibility(character, True)
         self._explosion_hold_time = 50
         self.phase = "rumble"
         self._max_rumble_steps = 250
         self._current_rumble_steps = 0
         self._rumble_mod_delay = 20
 
     def __next__(self) -> str:
         next_frame = None
         if self.phase == "rumble":
             if self._current_rumble_steps < self._max_rumble_steps:
                 if self._current_rumble_steps > 30 and self._current_rumble_steps % self._rumble_mod_delay == 0:
                     row_offset = random.choice([-1, 0, 1])
                     column_offset = random.choice([-1, 0, 1])
-                    for character in self._terminal.get_characters():
+                    for character in self.terminal.get_characters():
                         character.motion.set_coordinate(
                             Coord(
                                 character.motion.current_coord.column + column_offset,
                                 character.motion.current_coord.row + row_offset,
                             )
                         )
                         character.animation.step_animation()
-                    next_frame = self._terminal.get_formatted_output_string()
-                    for character in self._terminal.get_characters():
-                        character.motion.set_coordinate(self._jumbled_coords[character])
+                    next_frame = self.terminal.get_formatted_output_string()
+                    for character in self.terminal.get_characters():
+                        character.motion.set_coordinate(self.jumbled_coords[character])
                     self._rumble_mod_delay -= 1
                     self._rumble_mod_delay = max(self._rumble_mod_delay, 1)
                 else:
-                    for character in self._terminal.get_characters():
+                    for character in self.terminal.get_characters():
                         character.animation.step_animation()
-                    next_frame = self._terminal.get_formatted_output_string()
+                    next_frame = self.terminal.get_formatted_output_string()
 
                 self._current_rumble_steps += 1
             else:
                 self.phase = "explosion"
-                for character in self._terminal.get_characters():
+                for character in self.terminal.get_characters():
                     character.motion.activate_path(character.motion.query_path("explosion"))
-                self._active_chars = [character for character in self._terminal.get_characters()]
+                self.active_characters = [character for character in self.terminal.get_characters()]
 
         if self.phase == "explosion":
-            if self._active_chars:
-                for character in self._active_chars:
+            if self.active_characters:
+                for character in self.active_characters:
                     character.tick()
-                self._active_chars = [
+                self.active_characters = [
                     character
-                    for character in self._active_chars
+                    for character in self.active_characters
                     if not character.motion.current_coord == character.motion.query_path("explosion").waypoints[0].coord
                 ]
-                next_frame = self._terminal.get_formatted_output_string()
+                next_frame = self.terminal.get_formatted_output_string()
 
             elif self._explosion_hold_time:
-                for character in self._active_chars:
+                for character in self.active_characters:
                     character.tick()
                 self._explosion_hold_time -= 1
-                next_frame = self._terminal.get_formatted_output_string()
+                next_frame = self.terminal.get_formatted_output_string()
             else:
                 self.phase = "reassembly"
-                for character in self._terminal.get_characters():
+                for character in self.terminal.get_characters():
                     character.animation.activate_scene(character.animation.query_scene("final"))
-                    self._active_chars.append(character)
+                    self.active_characters.append(character)
                     character.motion.activate_path(character.motion.query_path("reassembly"))
 
         if self.phase == "reassembly":
-            if self._active_chars:
-                for character in self._active_chars:
+            if self.active_characters:
+                for character in self.active_characters:
                     character.tick()
-                self._active_chars = [
+                self.active_characters = [
                     character
-                    for character in self._active_chars
+                    for character in self.active_characters
                     if not character.motion.current_coord
                     == character.motion.query_path("reassembly").waypoints[0].coord
                     or not character.animation.active_scene_is_complete()
                 ]
-                next_frame = self._terminal.get_formatted_output_string()
+                next_frame = self.terminal.get_formatted_output_string()
 
         if next_frame is not None:
             return next_frame
         else:
             raise StopIteration
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_verticalslice.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_verticalslice.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,69 +90,66 @@
     def get_effect_class(cls):
         return VerticalSlice
 
 
 class VerticalSliceIterator(BaseEffectIterator[VerticalSliceConfig]):
     def __init__(self, effect: "VerticalSlice") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._new_rows: list[list[EffectCharacter]] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_chars: list[EffectCharacter] = []
+        self.new_rows: list[list[EffectCharacter]] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
             character.animation.set_appearance(
                 character.input_symbol,
-                self._character_final_color_map[character],
+                self.character_final_color_map[character],
             )
 
-        self.rows = self._terminal.get_characters_grouped(grouping=self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP)
+        self.rows = self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.ROW_BOTTOM_TO_TOP)
         lengths = [max([c.input_coord.column for c in row]) for row in self.rows]
         mid_point = sum(lengths) // len(lengths) // 2
         for row_index, row in enumerate(self.rows):
             new_row = []
             left_half = [character for character in row if character.input_coord.column <= mid_point]
             for character in left_half:
-                character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.top))
+                character.motion.set_coordinate(Coord(character.input_coord.column, self.terminal.output_area.top))
                 input_coord_path = character.motion.new_path(
-                    speed=self._config.movement_speed, ease=self._config.movement_easing
+                    speed=self.config.movement_speed, ease=self.config.movement_easing
                 )
                 input_coord_path.new_waypoint(character.input_coord)
                 character.motion.activate_path(input_coord_path)
             opposite_row = self.rows[-(row_index + 1)]
             right_half = [c for c in opposite_row if c.input_coord.column > mid_point]
             for character in right_half:
-                character.motion.set_coordinate(Coord(character.input_coord.column, self._terminal.output_area.bottom))
+                character.motion.set_coordinate(Coord(character.input_coord.column, self.terminal.output_area.bottom))
                 input_coord_path = character.motion.new_path(
-                    speed=self._config.movement_speed, ease=self._config.movement_easing
+                    speed=self.config.movement_speed, ease=self.config.movement_easing
                 )
                 input_coord_path.new_waypoint(character.input_coord)
                 character.motion.activate_path(input_coord_path)
             new_row.extend(left_half)
             new_row.extend(right_half)
-            self._new_rows.append(new_row)
+            self.new_rows.append(new_row)
 
     def __next__(self) -> str:
-        if self._new_rows or self._active_chars:
-            if self._new_rows:
-                next_row = self._new_rows.pop(0)
+        if self.new_rows or self.active_characters:
+            if self.new_rows:
+                next_row = self.new_rows.pop(0)
                 for character in next_row:
-                    self._terminal.set_character_visibility(character, True)
-                self._active_chars.extend(next_row)
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+                    self.terminal.set_character_visibility(character, True)
+                self.active_characters.extend(next_row)
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class VerticalSlice(BaseEffect[VerticalSliceConfig]):
     """Slices the input in half vertically and slides it into place from opposite directions.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_vhstape.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_vhstape.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     @classmethod
     def get_effect_class(cls):
         return VHSTape
 
 
 class VHSTapeIterator(BaseEffectIterator[VHSTapeConfig]):
-    class _Line:
+    class Line:
         def __init__(
             self,
             characters: list[EffectCharacter],
             args: VHSTapeConfig,
             character_final_color_map: dict[EffectCharacter, graphics.Color],
         ) -> None:
             self.characters = characters
@@ -258,160 +258,153 @@
                 character.motion.activate_path(character.motion.query_path(path_id))
 
         def line_movement_complete(self):
             return all(character.motion.movement_is_complete() for character in self.characters)
 
     def __init__(self, effect: "VHSTape") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._lines: dict[int, VHSTapeIterator._Line] = {}
-        self._active_glitch_wave_top: int | None = None
-        self._active_glitch_wave_lines: list[VHSTapeIterator._Line] = []
-        self._active_glitch_lines: list[VHSTapeIterator._Line] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.pending_chars: list[EffectCharacter] = []
+        self.lines: dict[int, VHSTapeIterator.Line] = {}
+        self.active_glitch_wave_top: int | None = None
+        self.active_glitch_wave_lines: list[VHSTapeIterator.Line] = []
+        self.active_glitch_lines: list[VHSTapeIterator.Line] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
         self.build()
 
     def build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         for row_index, characters in enumerate(
-            self._terminal.get_characters_grouped(grouping=self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP)
+            self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.ROW_BOTTOM_TO_TOP)
         ):
-            self._lines[row_index] = VHSTapeIterator._Line(characters, self._config, self._character_final_color_map)
-        for character in self._terminal.get_characters():
-            self._terminal.set_character_visibility(character, True)
+            self.lines[row_index] = VHSTapeIterator.Line(characters, self.config, self.character_final_color_map)
+        for character in self.terminal.get_characters():
+            self.terminal.set_character_visibility(character, True)
             character.animation.activate_scene(character.animation.query_scene("base"))
         self._glitching_steps_elapsed = 0
         self._phase = "glitching"
-        self._to_redraw = list(self._lines.values())
+        self._to_redraw = list(self.lines.values())
         self._redrawing = False
 
-    def _glitch_wave(self) -> None:
-        if not self._active_glitch_wave_top:
-            if self._terminal.output_area.top >= 3:
+    def glitch_wave(self) -> None:
+        if not self.active_glitch_wave_top:
+            if self.terminal.output_area.top >= 3:
                 # choose a wave top index in the top half of the output area or at least 3 rows up
-                self._active_glitch_wave_top = random.randint(
-                    max((3, round(self._terminal.output_area.top * 0.5))), self._terminal.output_area.top
+                self.active_glitch_wave_top = random.randint(
+                    max((3, round(self.terminal.output_area.top * 0.5))), self.terminal.output_area.top
                 )
             else:
                 # not enough room for a wave
                 return
 
         # if all lines have completed movement, proceed to move/restore wave
-        if all(line.line_movement_complete() for line in self._active_glitch_wave_lines):
-            if self._active_glitch_wave_lines:
+        if all(line.line_movement_complete() for line in self.active_glitch_wave_lines):
+            if self.active_glitch_wave_lines:
                 # only move 30% of the time
                 if random.random() < 0.3:
                     # if moving, only move up 10% of the time
                     if random.random() < 0.3:
                         wave_top_delta = 1
                     else:
                         wave_top_delta = -1
                 else:
                     wave_top_delta = 0
-                self._active_glitch_wave_top += wave_top_delta
+                self.active_glitch_wave_top += wave_top_delta
                 # clamp wave top to output area
-                self._active_glitch_wave_top = max(2, min(self._active_glitch_wave_top, self._terminal.output_area.top))
+                self.active_glitch_wave_top = max(2, min(self.active_glitch_wave_top, self.terminal.output_area.top))
             # get the lines for the wave
-            new_wave_lines: list[VHSTapeIterator._Line] = []
-            for line_index in range(self._active_glitch_wave_top - 2, self._active_glitch_wave_top + 1):
-                if line_index in self._lines:
-                    new_wave_lines.append(self._lines[line_index])
+            new_wave_lines: list[VHSTapeIterator.Line] = []
+            for line_index in range(self.active_glitch_wave_top - 2, self.active_glitch_wave_top + 1):
+                if line_index in self.lines:
+                    new_wave_lines.append(self.lines[line_index])
 
             # restore any lines that are no longer part of the wave
-            for line in self._active_glitch_wave_lines:
+            for line in self.active_glitch_wave_lines:
                 if line not in new_wave_lines:
                     line.restore()
-                    self._active_chars.extend(line.characters)
-            self._active_glitch_wave_lines = new_wave_lines
+                    self.active_characters.extend(line.characters)
+            self.active_glitch_wave_lines = new_wave_lines
 
-            if self._active_glitch_wave_top < 3:
+            if self.active_glitch_wave_top < 3:
                 # wave at bottom, restore lines
-                for line in self._active_glitch_wave_lines:
+                for line in self.active_glitch_wave_lines:
                     line.restore()
-                    self._active_chars.extend(line.characters)
-                self._active_glitch_wave_top = None
-                self._active_glitch_wave_lines = []
+                    self.active_characters.extend(line.characters)
+                self.active_glitch_wave_top = None
+                self.active_glitch_wave_lines = []
 
             else:
                 for line, path_id in zip(
-                    self._active_glitch_wave_lines, ("glitch_wave_mid", "glitch_wave_end", "glitch_wave_mid")
+                    self.active_glitch_wave_lines, ("glitch_wave_mid", "glitch_wave_end", "glitch_wave_mid")
                 ):
                     line.activate_path(path_id)
-                    self._active_chars.extend(line.characters)
+                    self.active_characters.extend(line.characters)
 
     def __next__(self) -> str:
-        if self._phase != "complete" or self._active_chars:
+        if self._phase != "complete" or self.active_characters:
             if self._phase == "glitching":
                 # Check if all active glitch wave lines have completed their movement, if so move the wave
-                if not self._active_glitch_wave_lines or all(
-                    line.line_movement_complete() for line in self._active_glitch_wave_lines
+                if not self.active_glitch_wave_lines or all(
+                    line.line_movement_complete() for line in self.active_glitch_wave_lines
                 ):
-                    self._glitch_wave()
+                    self.glitch_wave()
                 # Remove completed glitch lines from active glitch lines
-                self._active_glitch_lines = [
-                    line for line in self._active_glitch_lines if not line.line_movement_complete()
+                self.active_glitch_lines = [
+                    line for line in self.active_glitch_lines if not line.line_movement_complete()
                 ]
                 # Randomly add new glitch lines
-                if random.random() < self._config.glitch_line_chance and len(self._active_glitch_lines) < 3:
-                    glitch_line: VHSTapeIterator._Line = random.choice(list(self._lines.values()))
-                    if (
-                        glitch_line not in self._active_glitch_wave_lines
-                        and glitch_line not in self._active_glitch_lines
-                    ):
+                if random.random() < self.config.glitch_line_chance and len(self.active_glitch_lines) < 3:
+                    glitch_line: VHSTapeIterator.Line = random.choice(list(self.lines.values()))
+                    if glitch_line not in self.active_glitch_wave_lines and glitch_line not in self.active_glitch_lines:
                         glitch_line.set_hold_time(random.randint(30, 120))
-                        self._active_glitch_lines.append(glitch_line)
+                        self.active_glitch_lines.append(glitch_line)
                         glitch_line.glitch()
-                        self._active_chars.extend(glitch_line.characters)
+                        self.active_characters.extend(glitch_line.characters)
                 # Randomly add noise to all lines
-                if random.random() < self._config.noise_chance:
-                    for line in self._lines.values():
+                if random.random() < self.config.noise_chance:
+                    for line in self.lines.values():
                         line.snow()
-                        if line not in self._active_glitch_wave_lines and line not in self._active_glitch_lines:
-                            self._active_chars.extend(line.characters)
+                        if line not in self.active_glitch_wave_lines and line not in self.active_glitch_lines:
+                            self.active_characters.extend(line.characters)
                 self._glitching_steps_elapsed += 1
                 # Check if glitching time has reached the total glitch time
-                if self._glitching_steps_elapsed >= self._config.total_glitch_time:
+                if self._glitching_steps_elapsed >= self.config.total_glitch_time:
                     # Restore glitch wave lines
-                    for line in self._active_glitch_wave_lines:
+                    for line in self.active_glitch_wave_lines:
                         line.restore()
                     # Restore glitch lines
-                    for line in self._active_glitch_lines:
+                    for line in self.active_glitch_lines:
                         line.restore()
                     self._phase = "noise"
 
             elif self._phase == "noise":
                 # Activate final snow animation for all characters
-                if not self._active_chars:
-                    for character in self._terminal.get_characters():
+                if not self.active_characters:
+                    for character in self.terminal.get_characters():
                         character.animation.activate_scene(character.animation.query_scene("final_snow"))
-                        self._active_chars.append(character)
+                        self.active_characters.append(character)
                     self._phase = "redraw"
 
             elif self._phase == "redraw":
                 # Redraw lines one by one
-                if self._redrawing or not self._active_chars:
+                if self._redrawing or not self.active_characters:
                     self._redrawing = True
                     if self._to_redraw:
                         next_line = self._to_redraw.pop()
                         for character in next_line.characters:
                             character.animation.activate_scene(character.animation.query_scene("final_redraw"))
-                            self._active_chars.append(character)
+                            self.active_characters.append(character)
                     else:
                         self._phase = "complete"
-            for character in self._active_chars:
-                character.tick()
-
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class VHSTape(BaseEffect[VHSTapeConfig]):
     """Lines of characters glitch left and right and lose detail like an old VHS tape.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_waves.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_waves.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,60 +128,55 @@
     def get_effect_class(cls):
         return Waves
 
 
 class WavesIterator(BaseEffectIterator[WavesConfig]):
     def __init__(self, effect: "Waves") -> None:
         super().__init__(effect)
-        self._pending_columns: list[list[EffectCharacter]] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
+        self.pending_columns: list[list[EffectCharacter]] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
 
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        wave_gradient = graphics.Gradient(*self._config.wave_gradient_stops, steps=self._config.wave_gradient_steps)
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        wave_gradient = graphics.Gradient(*self.config.wave_gradient_stops, steps=self.config.wave_gradient_steps)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
             wave_scn = character.animation.new_scene()
-            wave_scn.ease = self._config.wave_easing
-            for _ in range(self._config.wave_count):
+            wave_scn.ease = self.config.wave_easing
+            for _ in range(self.config.wave_count):
                 wave_scn.apply_gradient_to_symbols(
-                    wave_gradient, self._config.wave_symbols, duration=self._config.wave_length
+                    wave_gradient, self.config.wave_symbols, duration=self.config.wave_length
                 )
             final_scn = character.animation.new_scene()
             for step in graphics.Gradient(
                 wave_gradient.spectrum[-1],
-                self._character_final_color_map[character],
-                steps=self._config.final_gradient_steps,
+                self.character_final_color_map[character],
+                steps=self.config.final_gradient_steps,
             ):
                 final_scn.add_frame(character.input_symbol, 10, color=step)
             character.event_handler.register_event(
                 EventHandler.Event.SCENE_COMPLETE, wave_scn, EventHandler.Action.ACTIVATE_SCENE, final_scn
             )
             character.animation.activate_scene(wave_scn)
-        for column in self._terminal.get_characters_grouped(
-            grouping=self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT
-        ):
-            self._pending_columns.append(column)
+        for column in self.terminal.get_characters_grouped(grouping=self.terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT):
+            self.pending_columns.append(column)
 
     def __next__(self) -> str:
-        if self._pending_columns or self._active_chars:
-            if self._pending_columns:
-                next_column = self._pending_columns.pop(0)
+        if self.pending_columns or self.active_characters:
+            if self.pending_columns:
+                next_column = self.pending_columns.pop(0)
                 for character in next_column:
-                    self._terminal.set_character_visibility(character, True)
-                    self._active_chars.append(character)
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+                    self.terminal.set_character_visibility(character, True)
+                    self.active_characters.append(character)
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Waves(BaseEffect[WavesConfig]):
     """Creates waves that travel across the terminal, leaving behind the characters.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/effects/effect_wipe.py` & `terminaltexteffects-0.9.1/terminaltexteffects/effects/effect_wipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,67 +114,64 @@
     def get_effect_class(cls):
         return Wipe
 
 
 class WipeIterator(BaseEffectIterator[WipeConfig]):
     def __init__(self, effect: "Wipe") -> None:
         super().__init__(effect)
-        self._pending_groups: list[list[EffectCharacter]] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
-
-    def _build(self) -> None:
-        direction = self._config.wipe_direction
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
+        self.pending_groups: list[list[EffectCharacter]] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
+
+    def build(self) -> None:
+        direction = self.config.wipe_direction
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
         final_gradient_mapping = final_gradient.build_coordinate_color_mapping(
-            self._terminal.output_area.top, self._terminal.output_area.right, self._config.final_gradient_direction
+            self.terminal.output_area.top, self.terminal.output_area.right, self.config.final_gradient_direction
         )
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient_mapping[character.input_coord]
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient_mapping[character.input_coord]
         sort_map = {
-            "column_left_to_right": self._terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
-            "column_right_to_left": self._terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
-            "row_top_to_bottom": self._terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
-            "row_bottom_to_top": self._terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
-            "diagonal_top_left_to_bottom_right": self._terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT,
-            "diagonal_bottom_left_to_top_right": self._terminal.CharacterGroup.DIAGONAL_BOTTOM_LEFT_TO_TOP_RIGHT,
-            "diagonal_top_right_to_bottom_left": self._terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT,
-            "diagonal_bottom_right_to_top_left": self._terminal.CharacterGroup.DIAGONAL_BOTTOM_RIGHT_TO_TOP_LEFT,
+            "column_left_to_right": self.terminal.CharacterGroup.COLUMN_LEFT_TO_RIGHT,
+            "column_right_to_left": self.terminal.CharacterGroup.COLUMN_RIGHT_TO_LEFT,
+            "row_top_to_bottom": self.terminal.CharacterGroup.ROW_TOP_TO_BOTTOM,
+            "row_bottom_to_top": self.terminal.CharacterGroup.ROW_BOTTOM_TO_TOP,
+            "diagonal_top_left_to_bottom_right": self.terminal.CharacterGroup.DIAGONAL_TOP_LEFT_TO_BOTTOM_RIGHT,
+            "diagonal_bottom_left_to_top_right": self.terminal.CharacterGroup.DIAGONAL_BOTTOM_LEFT_TO_TOP_RIGHT,
+            "diagonal_top_right_to_bottom_left": self.terminal.CharacterGroup.DIAGONAL_TOP_RIGHT_TO_BOTTOM_LEFT,
+            "diagonal_bottom_right_to_top_left": self.terminal.CharacterGroup.DIAGONAL_BOTTOM_RIGHT_TO_TOP_LEFT,
         }
-        for group in self._terminal.get_characters_grouped(sort_map[direction]):
+        for group in self.terminal.get_characters_grouped(sort_map[direction]):
             for character in group:
                 wipe_scn = character.animation.new_scene()
                 wipe_gradient = graphics.Gradient(
                     final_gradient.spectrum[0],
-                    self._character_final_color_map[character],
-                    steps=self._config.final_gradient_steps,
+                    self.character_final_color_map[character],
+                    steps=self.config.final_gradient_steps,
                 )
                 wipe_scn.apply_gradient_to_symbols(
-                    wipe_gradient, character.input_symbol, self._config.final_gradient_frames
+                    wipe_gradient, character.input_symbol, self.config.final_gradient_frames
                 )
                 character.animation.activate_scene(wipe_scn)
-            self._pending_groups.append(group)
-        self._wipe_delay = self._config.wipe_delay
+            self.pending_groups.append(group)
+        self._wipe_delay = self.config.wipe_delay
 
     def __next__(self) -> str:
-        if self._pending_groups or self._active_chars:
+        if self.pending_groups or self.active_characters:
             if not self._wipe_delay:
-                if self._pending_groups:
-                    next_group = self._pending_groups.pop(0)
+                if self.pending_groups:
+                    next_group = self.pending_groups.pop(0)
                     for character in next_group:
-                        self._terminal.set_character_visibility(character, True)
-                        self._active_chars.append(character)
-                self._wipe_delay = self._config.wipe_delay
+                        self.terminal.set_character_visibility(character, True)
+                        self.active_characters.append(character)
+                self._wipe_delay = self.config.wipe_delay
             else:
                 self._wipe_delay -= 1
-            for character in self._active_chars:
-                character.tick()
-            self._active_chars = [character for character in self._active_chars if character.is_active]
-            return self._terminal.get_formatted_output_string()
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class Wipe(BaseEffect[WipeConfig]):
     """Performs a wipe across the terminal to reveal characters.
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/engine/animation.py` & `terminaltexteffects-0.9.1/terminaltexteffects/engine/animation.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/engine/base_character.py` & `terminaltexteffects-0.9.1/terminaltexteffects/engine/base_character.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/engine/motion.py` & `terminaltexteffects-0.9.1/terminaltexteffects/engine/motion.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/engine/terminal.py` & `terminaltexteffects-0.9.1/terminaltexteffects/engine/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,23 +69,31 @@
         type_parser=argvalidators.PositiveInt.type_parser,
         default=100,
         help="""Target frame rate for the animation.""",
     )  # type: ignore[assignment]
 
     "float : Minimum time, in seconds, between frames."
 
-    terminal_dimensions: tuple[int, int] = ArgField(
-        cmd_name=["--terminal-dimensions"],
-        type_parser=argvalidators.TerminalDimensions.type_parser,
-        nargs=2,
-        default=(0, 0),
-        help="Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal width.",
+    terminal_width: int = ArgField(
+        cmd_name=["--terminal-width"],
+        type_parser=argvalidators.NonNegativeInt.type_parser,
+        default=0,
+        help="Terminal width, if set to 0 the terminal width is detected automatically.",
     )  # type: ignore[assignment]
 
-    "tuple(int,int) : Terminal dimensions as (width, height), if set to (0,0) the terminal dimensions are detected automatically."
+    "int : Terminal width, if set to 0 the terminal width is detected automatically."
+
+    terminal_height: int = ArgField(
+        cmd_name=["--terminal-height"],
+        type_parser=argvalidators.NonNegativeInt.type_parser,
+        default=0,
+        help="Terminal height, if set to 0 the terminal height is detected automatically.",
+    )  # type: ignore[assignment]
+
+    "int : Terminal height, if set to 0 the terminal height is detected automatically."
 
     ignore_terminal_dimensions: bool = ArgField(
         cmd_name=["--ignore-terminal-dimensions"],
         default=False,
         action="store_true",
         help="Ignore the terminal dimensions and use the input data dimensions for the output area.",
     )  # type: ignore[assignment]
@@ -251,27 +259,32 @@
         if config is None:
             self.config = TerminalConfig()
         else:
             self.config = config
         if not input_data:
             input_data = "No Input."
         self._input_data = input_data.replace("\t", " " * self.config.tab_width)
+        self.detected_terminal_dimensions = self._get_terminal_dimensions()
+        self._width = self.config.terminal_width
+        self._height = self.config.terminal_height
         if self.config.ignore_terminal_dimensions:
             self._width = max([len(line) for line in self._input_data.splitlines()])
             self._height = len(self._input_data.splitlines()) + 1
-        elif self.config.terminal_dimensions == (0, 0):
-            self._width, self._height = self._get_terminal_dimensions()
-        else:
-            self._width, self._height = self.config.terminal_dimensions
+        elif self._width == 0 or self._height == 0:
+            if self._width == 0:
+                self._width = self.detected_terminal_dimensions[0]
+            if self._height == 0:
+                self._height = self.detected_terminal_dimensions[1]
+
         self._next_character_id = 0
         self._input_characters = self._decompose_input(self.config.xterm_colors, self.config.no_color)
         self._added_characters: list[EffectCharacter] = []
         self._input_width = max([character.input_coord.column for character in self._input_characters])
         self._input_height = max([character.input_coord.row for character in self._input_characters])
-        self.output_area = OutputArea(min(self._height - 1, self._input_height), self._input_width)
+        self.output_area = OutputArea(min(max(self._height - 1, 1), self._input_height), self._input_width)
         self._input_characters = [
             character
             for character in self._input_characters
             if character.input_coord.row <= self.output_area.top
             and character.input_coord.column <= self.output_area.right
         ]
         self.character_by_input_coord: dict[Coord, EffectCharacter] = {
@@ -410,15 +423,15 @@
                 rows[row][column] = character.symbol
         terminal_state = ["".join(row) for row in rows]
         self.terminal_state = terminal_state
 
     def prep_outputarea(self) -> None:
         """Prepares the terminal for the effect by adding empty lines and hiding the cursor."""
         sys.stdout.write(ansitools.HIDE_CURSOR())
-        print("\n" * self.output_area.top)
+        print("\n" * (self.output_area.top - 1))
 
     def restore_cursor(self) -> None:
         """Restores the cursor visibility."""
         sys.stdout.write(ansitools.SHOW_CURSOR())
 
     def get_characters(
         self,
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/template/effect_template.py` & `terminaltexteffects-0.9.1/terminaltexteffects/template/effect_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,34 +87,32 @@
     def get_effect_class(cls):
         return NamedEffect
 
 
 class NamedEffectIterator(BaseEffectIterator[EffectConfig]):
     def __init__(self, effect: "NamedEffect") -> None:
         super().__init__(effect)
-        self._pending_chars: list[EffectCharacter] = []
-        self._active_chars: list[EffectCharacter] = []
-        self._character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
-        self._build()
-
-    def _build(self) -> None:
-        final_gradient = graphics.Gradient(*self._config.final_gradient_stops, steps=self._config.final_gradient_steps)
-        for character in self._terminal.get_characters():
-            self._character_final_color_map[character] = final_gradient.get_color_at_fraction(
-                character.input_coord.row / self._terminal.output_area.top
+        self.pending_chars: list[EffectCharacter] = []
+        self.character_final_color_map: dict[EffectCharacter, graphics.Color] = {}
+        self.build()
+
+    def build(self) -> None:
+        final_gradient = graphics.Gradient(*self.config.final_gradient_stops, steps=self.config.final_gradient_steps)
+        for character in self.terminal.get_characters():
+            self.character_final_color_map[character] = final_gradient.get_color_at_fraction(
+                character.input_coord.row / self.terminal.output_area.top
             )
 
             # do something with the data if needed (sort, adjust positions, etc)
 
     def __next__(self) -> str:
-        if self._pending_chars or self._active_chars:
+        if self.pending_chars or self.active_characters:
             # perform effect logic
-            for character in self._active_chars:
-                character.tick()
-            return self._terminal.get_formatted_output_string()
+            self.update()
+            return self.frame
         else:
             raise StopIteration
 
 
 class NamedEffect(BaseEffect[EffectConfig]):
     """Effect description."""
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/utils/ansitools.py` & `terminaltexteffects-0.9.1/terminaltexteffects/utils/ansitools.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/utils/argsdataclass.py` & `terminaltexteffects-0.9.1/terminaltexteffects/utils/argsdataclass.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/utils/argvalidators.py` & `terminaltexteffects-0.9.1/terminaltexteffects/utils/argvalidators.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/utils/colorterm.py` & `terminaltexteffects-0.9.1/terminaltexteffects/utils/colorterm.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/utils/easing.py` & `terminaltexteffects-0.9.1/terminaltexteffects/utils/easing.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/utils/geometry.py` & `terminaltexteffects-0.9.1/terminaltexteffects/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/utils/graphics.py` & `terminaltexteffects-0.9.1/terminaltexteffects/utils/graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,36 +173,45 @@
 
         Returns:
             dict[Coord, str]: A mapping of coordinates to colors.
         """
         gradient_mapping: dict[geometry.Coord, Color] = {}
         if direction == Gradient.Direction.VERTICAL:
             for row_value in range(max_row + 1):
-                fraction = row_value / max_row
+                if max_row == 0:
+                    fraction = 1.0
+                else:
+                    fraction = row_value / max_row
                 color = self.get_color_at_fraction(fraction)
                 for column_value in range(1, max_column + 1):
                     gradient_mapping[geometry.Coord(column_value, row_value)] = color
         elif direction == Gradient.Direction.HORIZONTAL:
             for column_value in range(1, max_column + 1):
-                fraction = column_value / max_column
+                if max_column == 0:
+                    fraction = 1.0
+                else:
+                    fraction = column_value / max_column
                 color = self.get_color_at_fraction(fraction)
                 for row_value in range(max_row + 1):
                     gradient_mapping[geometry.Coord(column_value, row_value)] = color
         elif direction == Gradient.Direction.CENTER:
             for row_value in range(max_row + 1):
                 for column_value in range(1, max_column + 1):
                     distance_from_center = geometry.find_normalized_distance_from_center(
                         max_row, max_column, geometry.Coord(column_value, row_value)
                     )
                     color = self.get_color_at_fraction(distance_from_center)
                     gradient_mapping[geometry.Coord(column_value, row_value)] = color
         elif direction == Gradient.Direction.DIAGONAL:
             for row_value in range(max_row + 1):
                 for column_value in range(1, max_column + 1):
-                    fraction = ((row_value * 2) + column_value) / ((max_row * 2) + max_column)
+                    if max_row == 0 or max_column == 0:
+                        fraction = 1.0
+                    else:
+                        fraction = ((row_value * 2) + column_value) / ((max_row * 2) + max_column)
                     color = self.get_color_at_fraction(fraction)
                     gradient_mapping[geometry.Coord(column_value, row_value)] = color
 
         return gradient_mapping
 
     def __iter__(self) -> Iterator[str]:
         yield from self.spectrum
```

### Comparing `terminaltexteffects-0.9.0/terminaltexteffects/utils/hexterm.py` & `terminaltexteffects-0.9.1/terminaltexteffects/utils/hexterm.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.0/PKG-INFO` & `terminaltexteffects-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminaltexteffects
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of visual effects that can be applied to terminal piped stdin text.
 License: MIT
 Author: Chris
 Author-email: 741258@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -82,31 +82,33 @@
 
 <details>
 
 <summary>TTE Command Line Options</summary>
 
 ```markdown
 options:
--h, --help            show this help message and exit
+  -h, --help            show this help message and exit
   --tab-width (int > 0)
                         Number of spaces to use for a tab character. (default: 4)
   --xterm-colors        Convert any colors specified in RBG hex to the closest XTerm-256 color. (default: False)
   --no-color            Disable all colors in the effect. (default: False)
   --wrap-text           Wrap text wider than the output area width. (default: False)
   --frame-rate FRAME_RATE
                         Target frame rate for the animation. (default: 100)
-  --terminal-dimensions TERMINAL_DIMENSIONS TERMINAL_DIMENSIONS
-                        Use the terminal dimensions to limit the size of the output area and support wrapping. If False, the output area is determined by the input data dimensions and may overflow the terminal
-                        width. (default: (0, 0))
+  --terminal-width TERMINAL_WIDTH
+                        Terminal width, if set to 0 the terminal width is detected automatically. (default: 0)
+  --terminal-height TERMINAL_HEIGHT
+                        Terminal height, if set to 0 the terminal height is detected automatically. (default: 0)
   --ignore-terminal-dimensions
                         Ignore the terminal dimensions and use the input data dimensions for the output area. (default: False)
+
 Effect:
   Name of the effect to apply. Use <effect> -h for effect specific help.
 
-  {beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,dev,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,test,unstable,verticalslice,vhstape,waves,wipe}
+  {beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,unstable,verticalslice,vhstape,waves,wipe}
                         Available Effects
     beams               Create beams which travel over the output area illuminating the characters behind them.
     binarypath          Binary representations of each character move through the terminal towards the home coordinate of the character.
     blackhole           Characters are consumed by a black hole and explode outwards.
     bouncyballs         Characters are bouncy balls falling from the top of the output area.
     bubbles             Characters are formed into bubbles that float down and pop.
     burn                Burns vertically in the output area.
@@ -119,27 +121,27 @@
     orbittingvolley     Four launchers orbit the output area firing volleys of characters inward to build the input text from the center out.
     overflow            Input text overflows ands scrolls the terminal in a random order until eventually appearing ordered.
     pour                Pours the characters into position from the given direction.
     print               Lines are printed one at a time following a print head. Print head performs line feed, carriage return.
     rain                Rain characters from the top of the output area.
     randomsequence      Prints the input data in a random sequence.
     rings               Characters are dispersed and form into spinning rings.
-    scattered           Move the characters into place from random starting locations.
+    scattered           Text is scattered across the output area and moves into position.
     slide               Slide characters into view from outside the terminal.
     spotlights          Spotlights search the text area, illuminating characters, before converging in the center and expanding.
     spray               Draws the characters spawning at varying rates from a single point.
     swarm               Characters are grouped into swarms and move around the terminal before settling into position.
     synthgrid           Create a grid which fills with characters dissolving into the final text.
     unstable            Spawn characters jumbled, explode them to the edge of the output area, then reassemble them in the correct layout.
     verticalslice       Slices the input in half vertically and slides it into place from opposite directions.
     vhstape             Lines of characters glitch left and right and lose detail like an old VHS tape.
     waves               Waves travel across the terminal leaving behind the characters.
     wipe                Wipes the text across the terminal to reveal characters.
 
-Ex: ls -a | tte crumble --final-gradient-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction diagonal
+Ex: ls -a | python -m terminaltexteffects decrypt --typing-speed 2 --ciphertext-colors 008000 00cb00 00ff00 --final-gradient-stops eda000 --final-gradient-steps 12 --final-gradient-direction vertical
 ```
 
 </details>
 
 ```cat your_text | tte <effect> [options]```
 
 OR
@@ -254,31 +256,54 @@
 
 ## In-Development Preview
 
 Any effects shown below are in development and will be available in the next release.
 
 ## Latest Release Notes
 
-## 0.9.0
+## 0.9.1
 
 ---
 
-### New Features (0.9.0)
+### New Features (0.9.1)
+
+---
+
+#### New Engine Features (0.9.1)
+
+* Terminal dimension auto-detection supports automatically detecting a single dimensions.
+
+### Changes (0.9.1)
 
 ---
 
-#### New Engine Features (0.9.0)
+#### Effects Changes (0.9.1)
+
+* All effects have been updated to use the new `update()` method and `frame` property of
+  `base_effect.BaseEffectIterator`. See Engine Changes for more info.
+
+#### Engine Changes (0.9.1)
+
+* `base_effect.BaseEffectIterator` now has an `update()` method which calls the `tick()` method of all active characters
+  and manages the `active_characters` list.
+* `base_effect.BaseEffectIterator` has a `frame` property which calls `Terminal.get_formatted_output_string()` and
+  returns the string.
+* `TerminalConfig.terminal_dimensions` has been split into `TerminalConfig.terminal_width` and
+  `TerminalConfig.terminal_height` to simply the command line argument for dimensions and make it more obvious which
+  dimensions is being specified when interacting with `effect.terminal_config`.
+
+#### Other Changes (0.9.1)
 
-* Linear easing function added.
+* Updated help output for `--terminal-dimensions` argument.
 
-### Changes (0.9.0)
+### Bug Fixes (0.9.1)
 
 ---
 
-#### Other Changes (0.9.0)
+#### Engine Fixes (0.9.1)
 
-* Major re-organization of the codebase and significant documentation changes and additions.
+* Fixed division by zero error when the terminal height was set to 1.
 
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/main/LICENSE.md) for more information.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: terminaltexteffects Version: 0.9.0 Summary: A
+Metadata-Version: 2.1 Name: terminaltexteffects Version: 0.9.1 Summary: A
 collection of visual effects that can be applied to terminal piped stdin text.
 License: MIT Author: Chris Author-email: 741258@pm.me Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Description-Content-Type: text/markdown
                                      _[_T_T_E_]
@@ -45,22 +45,22 @@
 full installation and usage guide. ### Application Quickstart #### Options TTE
 Command Line Options ```markdown options: -h, --help show this help message and
 exit --tab-width (int > 0) Number of spaces to use for a tab character.
 (default: 4) --xterm-colors Convert any colors specified in RBG hex to the
 closest XTerm-256 color. (default: False) --no-color Disable all colors in the
 effect. (default: False) --wrap-text Wrap text wider than the output area
 width. (default: False) --frame-rate FRAME_RATE Target frame rate for the
-animation. (default: 100) --terminal-dimensions TERMINAL_DIMENSIONS
-TERMINAL_DIMENSIONS Use the terminal dimensions to limit the size of the output
-area and support wrapping. If False, the output area is determined by the input
-data dimensions and may overflow the terminal width. (default: (0, 0)) --
-ignore-terminal-dimensions Ignore the terminal dimensions and use the input
-data dimensions for the output area. (default: False) Effect: Name of the
-effect to apply. Use -h for effect specific help.
-{beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,dev,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,test,unstable,verticalslice,vhstape,waves,wipe}
+animation. (default: 100) --terminal-width TERMINAL_WIDTH Terminal width, if
+set to 0 the terminal width is detected automatically. (default: 0) --terminal-
+height TERMINAL_HEIGHT Terminal height, if set to 0 the terminal height is
+detected automatically. (default: 0) --ignore-terminal-dimensions Ignore the
+terminal dimensions and use the input data dimensions for the output area.
+(default: False) Effect: Name of the effect to apply. Use -h for effect
+specific help.
+{beams,binarypath,blackhole,bouncyballs,bubbles,burn,crumble,decrypt,errorcorrect,expand,fireworks,middleout,orbittingvolley,overflow,pour,print,rain,randomsequence,rings,scattered,slide,spotlights,spray,swarm,synthgrid,unstable,verticalslice,vhstape,waves,wipe}
 Available Effects beams Create beams which travel over the output area
 illuminating the characters behind them. binarypath Binary representations of
 each character move through the terminal towards the home coordinate of the
 character. blackhole Characters are consumed by a black hole and explode
 outwards. bouncyballs Characters are bouncy balls falling from the top of the
 output area. bubbles Characters are formed into bubbles that float down and
 pop. burn Burns vertically in the output area. crumble Characters lose color
@@ -73,29 +73,30 @@
 volleys of characters inward to build the input text from the center out.
 overflow Input text overflows ands scrolls the terminal in a random order until
 eventually appearing ordered. pour Pours the characters into position from the
 given direction. print Lines are printed one at a time following a print head.
 Print head performs line feed, carriage return. rain Rain characters from the
 top of the output area. randomsequence Prints the input data in a random
 sequence. rings Characters are dispersed and form into spinning rings.
-scattered Move the characters into place from random starting locations. slide
-Slide characters into view from outside the terminal. spotlights Spotlights
-search the text area, illuminating characters, before converging in the center
-and expanding. spray Draws the characters spawning at varying rates from a
-single point. swarm Characters are grouped into swarms and move around the
-terminal before settling into position. synthgrid Create a grid which fills
+scattered Text is scattered across the output area and moves into position.
+slide Slide characters into view from outside the terminal. spotlights
+Spotlights search the text area, illuminating characters, before converging in
+the center and expanding. spray Draws the characters spawning at varying rates
+from a single point. swarm Characters are grouped into swarms and move around
+the terminal before settling into position. synthgrid Create a grid which fills
 with characters dissolving into the final text. unstable Spawn characters
 jumbled, explode them to the edge of the output area, then reassemble them in
 the correct layout. verticalslice Slices the input in half vertically and
 slides it into place from opposite directions. vhstape Lines of characters
 glitch left and right and lose detail like an old VHS tape. waves Waves travel
 across the terminal leaving behind the characters. wipe Wipes the text across
-the terminal to reveal characters. Ex: ls -a | tte crumble --final-gradient-
-stops 5CE1FF FF8C00 --final-gradient-steps 12 --final-gradient-direction
-diagonal ``` ```cat your_text | tte [options]``` OR ```cat your_text | python -
+the terminal to reveal characters. Ex: ls -a | python -m terminaltexteffects
+decrypt --typing-speed 2 --ciphertext-colors 008000 00cb00 00ff00 --final-
+gradient-stops eda000 --final-gradient-steps 12 --final-gradient-direction
+vertical ``` ```cat your_text | tte [options]``` OR ```cat your_text | python -
 m terminaltexteffects [options]``` * Use ``` -h``` to view options for a
 specific effect, such as color or movement direction. * Ex: ```tte decrypt -
 h``` For more information, view the [Application Usage Guide](https://
 chrisbuilds.github.io/terminaltexteffects/appguide/). ### Library Quickstart
 All effects are iterators which return a string representing the current frame.
 Basic usage is as simple as importing the effect, instantiating it with the
 input text, and iterating over the effect. ```python from
@@ -138,13 +139,25 @@
 057338f4e007) #### Swarm ![swarm_demo](https://github.com/ChrisBuilds/
 terminaltexteffects/assets/57874186/305e8390-a0fb-4edb-a541-7b52cef77c09) ####
 VHSTape ![vhstape_demo](https://github.com/ChrisBuilds/terminaltexteffects/
 assets/57874186/720abbf4-f97d-4ce9-96ee-15ef973488d2) #### Waves ![waves_demo]
 (https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/ea9b04ca-
 e526-4c7e-b98d-a98a42f7137f) ## In-Development Preview Any effects shown below
 are in development and will be available in the next release. ## Latest Release
-Notes ## 0.9.0 --- ### New Features (0.9.0) --- #### New Engine Features
-(0.9.0) * Linear easing function added. ### Changes (0.9.0) --- #### Other
-Changes (0.9.0) * Major re-organization of the codebase and significant
-documentation changes and additions. ## License Distributed under the MIT
-License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/
-main/LICENSE.md) for more information.
+Notes ## 0.9.1 --- ### New Features (0.9.1) --- #### New Engine Features
+(0.9.1) * Terminal dimension auto-detection supports automatically detecting a
+single dimensions. ### Changes (0.9.1) --- #### Effects Changes (0.9.1) * All
+effects have been updated to use the new `update()` method and `frame` property
+of `base_effect.BaseEffectIterator`. See Engine Changes for more info. ####
+Engine Changes (0.9.1) * `base_effect.BaseEffectIterator` now has an `update()`
+method which calls the `tick()` method of all active characters and manages the
+`active_characters` list. * `base_effect.BaseEffectIterator` has a `frame`
+property which calls `Terminal.get_formatted_output_string()` and returns the
+string. * `TerminalConfig.terminal_dimensions` has been split into
+`TerminalConfig.terminal_width` and `TerminalConfig.terminal_height` to simply
+the command line argument for dimensions and make it more obvious which
+dimensions is being specified when interacting with `effect.terminal_config`.
+#### Other Changes (0.9.1) * Updated help output for `--terminal-dimensions`
+argument. ### Bug Fixes (0.9.1) --- #### Engine Fixes (0.9.1) * Fixed division
+by zero error when the terminal height was set to 1. ## License Distributed
+under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/
+terminaltexteffects/blob/main/LICENSE.md) for more information.
```

