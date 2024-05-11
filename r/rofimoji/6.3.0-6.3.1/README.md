# Comparing `tmp/rofimoji-6.3.0.tar.gz` & `tmp/rofimoji-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rofimoji-6.3.0.tar", max compression
+gzip compressed data, was "rofimoji-6.3.1.tar", max compression
```

## Comparing `rofimoji-6.3.0.tar` & `rofimoji-6.3.1.tar`

### file list

```diff
@@ -1,373 +1,373 @@
--rw-r--r--   0        0        0     1075 2024-03-24 10:41:32.767624 rofimoji-6.3.0/LICENSE
--rw-r--r--   0        0        0    19841 2024-04-27 13:42:04.149186 rofimoji-6.3.0/README.md
--rw-r--r--   0        0        0      892 2024-05-01 08:34:01.938166 rofimoji-6.3.0/pyproject.toml
--rw-r--r--   0        0        0       89 2022-12-29 11:56:19.212555 rofimoji-6.3.0/src/picker/__init__.py
--rw-r--r--   0        0        0      259 2024-03-29 09:38:49.773804 rofimoji-6.3.0/src/picker/__main__.py
--rw-r--r--   0        0        0      188 2022-11-13 10:52:07.457219 rofimoji-6.3.0/src/picker/abstractionhelper.py
--rw-r--r--   0        0        0     1204 2024-03-24 10:41:32.767624 rofimoji-6.3.0/src/picker/action.py
--rw-r--r--   0        0        0     5849 2024-03-24 10:41:32.767624 rofimoji-6.3.0/src/picker/argument_parsing.py
--rw-r--r--   0        0        0        0 2022-11-13 10:52:07.457219 rofimoji-6.3.0/src/picker/clipboarder/__init__.py
--rw-r--r--   0        0        0     1127 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/clipboarder.py
--rw-r--r--   0        0        0      677 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/noop.py
--rw-r--r--   0        0        0     1093 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/wl.py
--rw-r--r--   0        0        0     1885 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/xclip.py
--rw-r--r--   0        0        0     1115 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/xsel.py
--rw-r--r--   0        0        0      452 2024-03-24 10:45:56.170300 rofimoji-6.3.0/src/picker/contrib/grid-icons-only.rasi
--rw-r--r--   0        0        0      457 2024-03-24 10:44:13.180796 rofimoji-6.3.0/src/picker/contrib/grid.rasi
--rw-r--r--   0        0        0       23 2023-08-17 09:39:13.406636 rofimoji-6.3.0/src/picker/data/additional/emojis_smileys_emotion.csv
--rw-r--r--   0        0        0     2712 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/adlam.csv
--rw-r--r--   0        0        0     1737 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/aegean_numbers.csv
--rw-r--r--   0        0        0     1470 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/ahom.csv
--rw-r--r--   0        0        0     4551 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/alchemical_symbols.csv
--rw-r--r--   0        0        0     2098 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/alphabetic_presentation_forms.csv
--rw-r--r--   0        0        0    18183 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/anatolian_hieroglyphs.csv
--rw-r--r--   0        0        0     2761 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/ancient_greek_musical_notation.csv
--rw-r--r--   0        0        0     2895 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/ancient_greek_numbers.csv
--rw-r--r--   0        0        0      344 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/ancient_symbols.csv
--rw-r--r--   0        0        0     8311 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/arabic.csv
--rw-r--r--   0        0        0     3561 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/arabic_extended-a.csv
--rw-r--r--   0        0        0     1906 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/arabic_extended-b.csv
--rw-r--r--   0        0        0       98 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/arabic_extended-c.csv
--rw-r--r--   0        0        0     5786 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/arabic_mathematical_alphabetic_symbols.csv
--rw-r--r--   0        0        0    32176 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/arabic_presentation_forms-a.csv
--rw-r--r--   0        0        0     5722 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/arabic_presentation_forms-b.csv
--rw-r--r--   0        0        0     2719 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/arabic_supplement.csv
--rw-r--r--   0        0        0     2715 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/armenian.csv
--rw-r--r--   0        0        0     3689 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/arrows.csv
--rw-r--r--   0        0        0     1729 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/avestan.csv
--rw-r--r--   0        0        0     3904 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/balinese.csv
--rw-r--r--   0        0        0     1870 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/bamum.csv
--rw-r--r--   0        0        0    18380 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/bamum_supplement.csv
--rw-r--r--   0        0        0     1876 2024-04-27 08:12:37.573949 rofimoji-6.3.0/src/picker/data/basic_latin.csv
--rw-r--r--   0        0        0      968 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/bassa_vah.csv
--rw-r--r--   0        0        0     1419 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/batak.csv
--rw-r--r--   0        0        0     2451 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/bengali.csv
--rw-r--r--   0        0        0     2625 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/bhaiksuki.csv
--rw-r--r--   0        0        0      944 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/block_elements.csv
--rw-r--r--   0        0        0      981 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/bopomofo.csv
--rw-r--r--   0        0        0      774 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/bopomofo_extended.csv
--rw-r--r--   0        0        0     5625 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/box_drawing.csv
--rw-r--r--   0        0        0     2950 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/brahmi.csv
--rw-r--r--   0        0        0     7680 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/braille_patterns.csv
--rw-r--r--   0        0        0      716 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/buginese.csv
--rw-r--r--   0        0        0      404 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/buhid.csv
--rw-r--r--   0        0        0    11298 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/byzantine_musical_symbols.csv
--rw-r--r--   0        0        0     1078 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/carian.csv
--rw-r--r--   0        0        0     1885 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/caucasian_albanian.csv
--rw-r--r--   0        0        0     1675 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/chakma.csv
--rw-r--r--   0        0        0     1820 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cham.csv
--rw-r--r--   0        0        0     2166 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/cherokee.csv
--rw-r--r--   0        0        0     2334 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cherokee_supplement.csv
--rw-r--r--   0        0        0     4120 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/chess_symbols.csv
--rw-r--r--   0        0        0      889 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/chorasmian.csv
--rw-r--r--   0        0        0   282678 2024-04-27 08:12:40.473965 rofimoji-6.3.0/src/picker/data/cjk_cantonese.csv
--rw-r--r--   0        0        0     6158 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cjk_compatibility.csv
--rw-r--r--   0        0        0     1463 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/cjk_compatibility_forms.csv
--rw-r--r--   0        0        0    17464 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cjk_compatibility_ideographs.csv
--rw-r--r--   0        0        0    21138 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/cjk_compatibility_ideographs_supplement.csv
--rw-r--r--   0        0        0   164294 2024-04-27 08:12:40.523965 rofimoji-6.3.0/src/picker/data/cjk_japanese_kun.csv
--rw-r--r--   0        0        0   152011 2024-04-27 08:12:40.537299 rofimoji-6.3.0/src/picker/data/cjk_japanese_on.csv
--rw-r--r--   0        0        0    76750 2024-04-27 08:12:40.543966 rofimoji-6.3.0/src/picker/data/cjk_korean.csv
--rw-r--r--   0        0        0   390276 2024-04-27 08:12:40.503965 rofimoji-6.3.0/src/picker/data/cjk_mandarin.csv
--rw-r--r--   0        0        0     3072 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/cjk_radicals_supplement.csv
--rw-r--r--   0        0        0      714 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/cjk_strokes.csv
--rw-r--r--   0        0        0     1919 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/cjk_symbols_and_punctuation.csv
--rw-r--r--   0        0        0    43076 2024-04-27 08:12:40.513965 rofimoji-6.3.0/src/picker/data/cjk_tang.csv
--rw-r--r--   0        0        0    87736 2024-04-27 08:12:40.510632 rofimoji-6.3.0/src/picker/data/cjk_vietnamese.csv
--rw-r--r--   0        0        0     3356 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/combining_diacritical_marks.csv
--rw-r--r--   0        0        0     1141 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_extended.csv
--rw-r--r--   0        0        0     1189 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_for_symbols.csv
--rw-r--r--   0        0        0     2374 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_supplement.csv
--rw-r--r--   0        0        0      581 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/combining_half_marks.csv
--rw-r--r--   0        0        0      347 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/common_indic_number_forms.csv
--rw-r--r--   0        0        0     1104 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/control_pictures.csv
--rw-r--r--   0        0        0     4234 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/coptic.csv
--rw-r--r--   0        0        0      919 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/coptic_epact_numbers.csv
--rw-r--r--   0        0        0      817 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/counting_rod_numerals.csv
--rw-r--r--   0        0        0    30373 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/cuneiform.csv
--rw-r--r--   0        0        0     5019 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/cuneiform_numbers_and_punctuation.csv
--rw-r--r--   0        0        0      556 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/currency_symbols.csv
--rw-r--r--   0        0        0     1535 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/cypriot_syllabary.csv
--rw-r--r--   0        0        0     2873 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/cypro-minoan.csv
--rw-r--r--   0        0        0     9424 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/cyrillic.csv
--rw-r--r--   0        0        0     1116 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/cyrillic_extended-a.csv
--rw-r--r--   0        0        0     3480 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cyrillic_extended-b.csv
--rw-r--r--   0        0        0      338 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/cyrillic_extended-c.csv
--rw-r--r--   0        0        0     2654 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/cyrillic_extended-d.csv
--rw-r--r--   0        0        0     1746 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/cyrillic_supplement.csv
--rw-r--r--   0        0        0     2552 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/deseret.csv
--rw-r--r--   0        0        0     3580 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/devanagari.csv
--rw-r--r--   0        0        0      377 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/devanagari_extended-a.csv
--rw-r--r--   0        0        0     1089 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/devanagari_extended.csv
--rw-r--r--   0        0        0     6632 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/dingbats.csv
--rw-r--r--   0        0        0     2029 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/dives_akuru.csv
--rw-r--r--   0        0        0     1348 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/dogra.csv
--rw-r--r--   0        0        0     3298 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/domino_tiles.csv
--rw-r--r--   0        0        0     4069 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/duployan.csv
--rw-r--r--   0        0        0     7082 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/early_dynastic_cuneiform.csv
--rw-r--r--   0        0        0     1794 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/egyptian_hieroglyph_format_controls.csv
--rw-r--r--   0        0        0    32482 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/egyptian_hieroglyphs.csv
--rw-r--r--   0        0        0      930 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/elbasan.csv
--rw-r--r--   0        0        0      654 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/elymaic.csv
--rw-r--r--   0        0        0     5642 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_activities.csv
--rw-r--r--   0        0        0     7330 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_animals_nature.csv
--rw-r--r--   0        0        0      253 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_component.csv
--rw-r--r--   0        0        0     7284 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_flags.csv
--rw-r--r--   0        0        0     7931 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_food_drink.csv
--rw-r--r--   0        0        0    16393 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_objects.csv
--rw-r--r--   0        0        0    21230 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_people_body.csv
--rw-r--r--   0        0        0    11962 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_smileys_emotion.csv
--rw-r--r--   0        0        0    16126 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_symbols.csv
--rw-r--r--   0        0        0    13690 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_travel_places.csv
--rw-r--r--   0        0        0     2229 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/emoticons.csv
--rw-r--r--   0        0        0     7107 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/enclosed_alphanumeric_supplement.csv
--rw-r--r--   0        0        0     5169 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/enclosed_alphanumerics.csv
--rw-r--r--   0        0        0     7668 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/enclosed_cjk_letters_and_months.csv
--rw-r--r--   0        0        0     2570 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/enclosed_ideographic_supplement.csv
--rw-r--r--   0        0        0     9421 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/ethiopic.csv
--rw-r--r--   0        0        0      868 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/ethiopic_extended-a.csv
--rw-r--r--   0        0        0      903 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/ethiopic_extended-b.csv
--rw-r--r--   0        0        0     2095 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/ethiopic_extended.csv
--rw-r--r--   0        0        0      774 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/ethiopic_supplement.csv
--rw-r--r--   0        0        0    52690 2024-04-27 08:12:41.863973 rofimoji-6.3.0/src/picker/data/fontawesome6.csv
--rw-r--r--   0        0        0     2575 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/general_punctuation.csv
--rw-r--r--   0        0        0     3087 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/geometric_shapes.csv
--rw-r--r--   0        0        0     3236 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/geometric_shapes_extended.csv
--rw-r--r--   0        0        0     2472 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/georgian.csv
--rw-r--r--   0        0        0     1908 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/georgian_extended.csv
--rw-r--r--   0        0        0     1200 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/georgian_supplement.csv
--rw-r--r--   0        0        0     2433 2024-04-27 08:12:41.490638 rofimoji-6.3.0/src/picker/data/gitmoji.csv
--rw-r--r--   0        0        0     3486 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/glagolitic.csv
--rw-r--r--   0        0        0     1500 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/glagolitic_supplement.csv
--rw-r--r--   0        0        0      684 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/gothic.csv
--rw-r--r--   0        0        0     2304 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/grantha.csv
--rw-r--r--   0        0        0     4218 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/greek_and_coptic.csv
--rw-r--r--   0        0        0    11730 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/greek_extended.csv
--rw-r--r--   0        0        0     2334 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/gujarati.csv
--rw-r--r--   0        0        0     1881 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/gunjala_gondi.csv
--rw-r--r--   0        0        0     1908 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/gurmukhi.csv
--rw-r--r--   0        0        0     7414 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/halfwidth_and_fullwidth_forms.csv
--rw-r--r--   0        0        0     2543 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/hangul_compatibility_jamo.csv
--rw-r--r--   0        0        0     7910 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/hangul_jamo.csv
--rw-r--r--   0        0        0      985 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/hangul_jamo_extended-a.csv
--rw-r--r--   0        0        0     2383 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/hangul_jamo_extended-b.csv
--rw-r--r--   0        0        0     1719 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/hanifi_rohingya.csv
--rw-r--r--   0        0        0      538 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/hanunoo.csv
--rw-r--r--   0        0        0      714 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/hatran.csv
--rw-r--r--   0        0        0     2344 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/hebrew.csv
--rw-r--r--   0        0        0     2318 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/hiragana.csv
--rw-r--r--   0        0        0      923 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/ideographic_description_characters.csv
--rw-r--r--   0        0        0      230 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/ideographic_symbols_and_punctuation.csv
--rw-r--r--   0        0        0     1173 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/imperial_aramaic.csv
--rw-r--r--   0        0        0     2591 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/indic_siyaq_numbers.csv
--rw-r--r--   0        0        0     1166 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/inscriptional_pahlavi.csv
--rw-r--r--   0        0        0     1307 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/inscriptional_parthian.csv
--rw-r--r--   0        0        0     3418 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/ipa_extensions.csv
--rw-r--r--   0        0        0     2438 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/javanese.csv
--rw-r--r--   0        0        0     1611 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/kaithi.csv
--rw-r--r--   0        0        0      570 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/kaktovik_numerals.csv
--rw-r--r--   0        0        0     1006 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/kana_extended-a.csv
--rw-r--r--   0        0        0      525 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/kana_extended-b.csv
--rw-r--r--   0        0        0     7167 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/kana_supplement.csv
--rw-r--r--   0        0        0      608 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/kanbun.csv
--rw-r--r--   0        0        0     5434 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/kangxi_radicals.csv
--rw-r--r--   0        0        0     2241 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/kannada.csv
--rw-r--r--   0        0        0    43839 2024-04-27 13:35:29.036304 rofimoji-6.3.0/src/picker/data/kaomoji.csv
--rw-r--r--   0        0        0     2323 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/katakana.csv
--rw-r--r--   0        0        0      464 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/katakana_phonetic_extensions.csv
--rw-r--r--   0        0        0     1997 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/kawi.csv
--rw-r--r--   0        0        0     1121 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/kayah_li.csv
--rw-r--r--   0        0        0     2145 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/kharoshthi.csv
--rw-r--r--   0        0        0    19270 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/khitan_small_script.csv
--rw-r--r--   0        0        0     2849 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/khmer.csv
--rw-r--r--   0        0        0      916 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/khmer_symbols.csv
--rw-r--r--   0        0        0     1526 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/khojki.csv
--rw-r--r--   0        0        0     1793 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/khudawadi.csv
--rw-r--r--   0        0        0     1779 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/lao.csv
--rw-r--r--   0        0        0     2978 2024-04-27 08:12:37.573949 rofimoji-6.3.0/src/picker/data/latin-1_supplement.csv
--rw-r--r--   0        0        0     4762 2024-04-27 08:12:37.573949 rofimoji-6.3.0/src/picker/data/latin_extended-a.csv
--rw-r--r--   0        0        0     7913 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/latin_extended-b.csv
--rw-r--r--   0        0        0     1235 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/latin_extended-c.csv
--rw-r--r--   0        0        0     7236 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/latin_extended-d.csv
--rw-r--r--   0        0        0     2474 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/latin_extended-e.csv
--rw-r--r--   0        0        0     2450 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/latin_extended-f.csv
--rw-r--r--   0        0        0     1799 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/latin_extended-g.csv
--rw-r--r--   0        0        0    11426 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/latin_extended_additional.csv
--rw-r--r--   0        0        0     1765 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/lepcha.csv
--rw-r--r--   0        0        0     1840 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/letterlike_symbols.csv
--rw-r--r--   0        0        0     1538 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/limbu.csv
--rw-r--r--   0        0        0     8429 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/linear_a.csv
--rw-r--r--   0        0        0     3958 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/linear_b_ideograms.csv
--rw-r--r--   0        0        0     2664 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/linear_b_syllabary.csv
--rw-r--r--   0        0        0      995 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/lisu.csv
--rw-r--r--   0        0        0       21 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/lisu_supplement.csv
--rw-r--r--   0        0        0      617 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/lycian.csv
--rw-r--r--   0        0        0      661 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/lydian.csv
--rw-r--r--   0        0        0      964 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/mahajani.csv
--rw-r--r--   0        0        0     1402 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/mahjong_tiles.csv
--rw-r--r--   0        0        0      590 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/makasar.csv
--rw-r--r--   0        0        0     3331 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/malayalam.csv
--rw-r--r--   0        0        0      760 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/mandaic.csv
--rw-r--r--   0        0        0     1695 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/manichaean.csv
--rw-r--r--   0        0        0     1903 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/marchen.csv
--rw-r--r--   0        0        0     2252 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/masaram_gondi.csv
--rw-r--r--   0        0        0    93185 2024-04-27 08:12:41.153969 rofimoji-6.3.0/src/picker/data/math.csv
--rw-r--r--   0        0        0    40125 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/mathematical_alphanumeric_symbols.csv
--rw-r--r--   0        0        0     6216 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/mathematical_operators.csv
--rw-r--r--   0        0        0      510 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/mayan_numerals.csv
--rw-r--r--   0        0        0     2969 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/medefaidrin.csv
--rw-r--r--   0        0        0     1668 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/meetei_mayek.csv
--rw-r--r--   0        0        0      681 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/meetei_mayek_extensions.csv
--rw-r--r--   0        0        0     8499 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/mende_kikakui.csv
--rw-r--r--   0        0        0     3826 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/meroitic_cursive.csv
--rw-r--r--   0        0        0     1298 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/meroitic_hieroglyphs.csv
--rw-r--r--   0        0        0     3532 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/miao.csv
--rw-r--r--   0        0        0     1541 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_mathematical_symbols-a.csv
--rw-r--r--   0        0        0     4228 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_mathematical_symbols-b.csv
--rw-r--r--   0        0        0     5475 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_symbols.csv
--rw-r--r--   0        0        0     9010 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_symbols_and_arrows.csv
--rw-r--r--   0        0        0    16261 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/miscellaneous_symbols_and_pictographs.csv
--rw-r--r--   0        0        0     7975 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_technical.csv
--rw-r--r--   0        0        0     1736 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/modi.csv
--rw-r--r--   0        0        0     1413 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/modifier_tone_letters.csv
--rw-r--r--   0        0        0     4806 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/mongolian.csv
--rw-r--r--   0        0        0      535 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/mongolian_supplement.csv
--rw-r--r--   0        0        0      843 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/mro.csv
--rw-r--r--   0        0        0      893 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/multani.csv
--rw-r--r--   0        0        0     8605 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/musical_symbols.csv
--rw-r--r--   0        0        0     4595 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/myanmar.csv
--rw-r--r--   0        0        0     1000 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/myanmar_extended-a.csv
--rw-r--r--   0        0        0     1001 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/myanmar_extended-b.csv
--rw-r--r--   0        0        0     1272 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/nabataean.csv
--rw-r--r--   0        0        0     1148 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/nag_mundari.csv
--rw-r--r--   0        0        0     1875 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/nandinagari.csv
--rw-r--r--   0        0        0   290162 2023-05-20 08:41:43.841476 rofimoji-6.3.0/src/picker/data/nerd_font.csv
--rw-r--r--   0        0        0     2505 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/new_tai_lue.csv
--rw-r--r--   0        0        0     2148 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/newa.csv
--rw-r--r--   0        0        0     1440 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/nko.csv
--rw-r--r--   0        0        0     1772 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/number_forms.csv
--rw-r--r--   0        0        0    10692 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/nushu.csv
--rw-r--r--   0        0        0     2755 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/nyiakeng_puachue_hmong.csv
--rw-r--r--   0        0        0      673 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/ogham.csv
--rw-r--r--   0        0        0     1158 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/ol_chiki.csv
--rw-r--r--   0        0        0     4348 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_hungarian.csv
--rw-r--r--   0        0        0     1049 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_italic.csv
--rw-r--r--   0        0        0     1200 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_north_arabian.csv
--rw-r--r--   0        0        0     1221 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_permic.csv
--rw-r--r--   0        0        0     1338 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_persian.csv
--rw-r--r--   0        0        0     1434 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/old_sogdian.csv
--rw-r--r--   0        0        0     1228 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_south_arabian.csv
--rw-r--r--   0        0        0     2688 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_turkic.csv
--rw-r--r--   0        0        0      881 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/old_uyghur.csv
--rw-r--r--   0        0        0      227 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/optical_character_recognition.csv
--rw-r--r--   0        0        0     2060 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/oriya.csv
--rw-r--r--   0        0        0     1683 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/ornamental_dingbats.csv
--rw-r--r--   0        0        0     2060 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/osage.csv
--rw-r--r--   0        0        0      947 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/osmanya.csv
--rw-r--r--   0        0        0     2505 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/ottoman_siyaq_numbers.csv
--rw-r--r--   0        0        0     4001 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/pahawh_hmong.csv
--rw-r--r--   0        0        0      988 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/palmyrene.csv
--rw-r--r--   0        0        0     1776 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/pau_cin_hau.csv
--rw-r--r--   0        0        0     1415 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/phags-pa.csv
--rw-r--r--   0        0        0     1455 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/phaistos_disc.csv
--rw-r--r--   0        0        0      889 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/phoenician.csv
--rw-r--r--   0        0        0     4468 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/phonetic_extensions.csv
--rw-r--r--   0        0        0     2620 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/phonetic_extensions_supplement.csv
--rw-r--r--   0        0        0     2562 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/playing_cards.csv
--rw-r--r--   0        0        0     1093 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/psalter_pahlavi.csv
--rw-r--r--   0        0        0      841 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/rejang.csv
--rw-r--r--   0        0        0      881 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/rumi_numeral_symbols.csv
--rw-r--r--   0        0        0     2424 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/runic.csv
--rw-r--r--   0        0        0     1929 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/samaritan.csv
--rw-r--r--   0        0        0     2217 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/saurashtra.csv
--rw-r--r--   0        0        0     2452 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/sharada.csv
--rw-r--r--   0        0        0     1172 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/shavian.csv
--rw-r--r--   0        0        0      140 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/shorthand_format_controls.csv
--rw-r--r--   0        0        0     2805 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/siddham.csv
--rw-r--r--   0        0        0     3060 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/sinhala.csv
--rw-r--r--   0        0        0      679 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/sinhala_archaic_numbers.csv
--rw-r--r--   0        0        0      634 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/small_form_variants.csv
--rw-r--r--   0        0        0      269 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/small_kana_extension.csv
--rw-r--r--   0        0        0     1379 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/sogdian.csv
--rw-r--r--   0        0        0     1012 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/sora_sompeng.csv
--rw-r--r--   0        0        0     2345 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/soyombo.csv
--rw-r--r--   0        0        0     2565 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/spacing_modifier_letters.csv
--rw-r--r--   0        0        0      168 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/specials.csv
--rw-r--r--   0        0        0     1714 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/sundanese.csv
--rw-r--r--   0        0        0      330 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/sundanese_supplement.csv
--rw-r--r--   0        0        0     1147 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/superscripts_and_subscripts.csv
--rw-r--r--   0        0        0      526 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/supplemental_arrows-a.csv
--rw-r--r--   0        0        0     5599 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/supplemental_arrows-b.csv
--rw-r--r--   0        0        0     6639 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/supplemental_arrows-c.csv
--rw-r--r--   0        0        0     8936 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/supplemental_mathematical_operators.csv
--rw-r--r--   0        0        0     2556 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/supplemental_punctuation.csv
--rw-r--r--   0        0        0     4767 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/supplemental_symbols_and_pictographs.csv
--rw-r--r--   0        0        0    31771 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/sutton_signwriting.csv
--rw-r--r--   0        0        0     1281 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/syloti_nagri.csv
--rw-r--r--   0        0        0     1743 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/symbols_and_pictographs_extended-a.csv
--rw-r--r--   0        0        0     8729 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/symbols_for_legacy_computing.csv
--rw-r--r--   0        0        0     2135 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/syriac.csv
--rw-r--r--   0        0        0      385 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/syriac_supplement.csv
--rw-r--r--   0        0        0      524 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/tagalog.csv
--rw-r--r--   0        0        0      418 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/tagbanwa.csv
--rw-r--r--   0        0        0     2575 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/tags.csv
--rw-r--r--   0        0        0      758 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/tai_le.csv
--rw-r--r--   0        0        0     3550 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/tai_tham.csv
--rw-r--r--   0        0        0     1897 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/tai_viet.csv
--rw-r--r--   0        0        0     2517 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/tai_xuan_jing_symbols.csv
--rw-r--r--   0        0        0     1511 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/takri.csv
--rw-r--r--   0        0        0     1534 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/tamil.csv
--rw-r--r--   0        0        0     1535 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/tamil_supplement.csv
--rw-r--r--   0        0        0     2028 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/tangsa.csv
--rw-r--r--   0        0        0    19968 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/tangut_components.csv
--rw-r--r--   0        0        0     2566 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/telugu.csv
--rw-r--r--   0        0        0     1234 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/thaana.csv
--rw-r--r--   0        0        0     2340 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/thai.csv
--rw-r--r--   0        0        0     6455 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/tibetan.csv
--rw-r--r--   0        0        0     1582 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/tifinagh.csv
--rw-r--r--   0        0        0     2049 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/tirhuta.csv
--rw-r--r--   0        0        0      662 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/toto.csv
--rw-r--r--   0        0        0     2229 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/transport_and_map_symbols.csv
--rw-r--r--   0        0        0      791 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/ugaritic.csv
--rw-r--r--   0        0        0    20601 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics.csv
--rw-r--r--   0        0        0      562 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended-a.csv
--rw-r--r--   0        0        0     2167 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended.csv
--rw-r--r--   0        0        0     6238 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/vai.csv
--rw-r--r--   0        0        0      407 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/variation_selectors.csv
--rw-r--r--   0        0        0     6637 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/variation_selectors_supplement.csv
--rw-r--r--   0        0        0     1512 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/vedic_extensions.csv
--rw-r--r--   0        0        0      524 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/vertical_forms.csv
--rw-r--r--   0        0        0     2176 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/vithkuqi.csv
--rw-r--r--   0        0        0     1321 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/wancho.csv
--rw-r--r--   0        0        0     2788 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/warang_citi.csv
--rw-r--r--   0        0        0     1286 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/yezidi.csv
--rw-r--r--   0        0        0     1052 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/yi_radicals.csv
--rw-r--r--   0        0        0    23855 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/yi_syllables.csv
--rw-r--r--   0        0        0     1955 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/yijing_hexagram_symbols.csv
--rw-r--r--   0        0        0     2586 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/zanabazar_square.csv
--rw-r--r--   0        0        0     7873 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/znamenny_musical_notation.csv
--rw-r--r--   0        0        0     5389 2024-05-01 08:34:38.924572 rofimoji-6.3.0/src/picker/docs/rofimoji.1
--rw-r--r--   0        0        0     4620 2024-05-01 08:34:31.074626 rofimoji-6.3.0/src/picker/docs/rofimoji.1.md
--rw-r--r--   0        0        0     1982 2023-09-16 08:10:09.785973 rofimoji-6.3.0/src/picker/emoji_data.py
--rw-r--r--   0        0        0     3130 2024-03-29 09:38:49.797137 rofimoji-6.3.0/src/picker/file_loader.py
--rw-r--r--   0        0        0     1106 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/frecent.py
--rw-r--r--   0        0        0     7720 2024-03-29 09:41:20.083560 rofimoji-6.3.0/src/picker/mode.py
--rw-r--r--   0        0        0     1241 2024-03-29 09:38:49.797137 rofimoji-6.3.0/src/picker/models.py
--rw-r--r--   0        0        0      708 2022-11-13 10:52:07.473886 rofimoji-6.3.0/src/picker/paths.py
--rw-r--r--   0        0        0     1584 2024-03-24 15:38:05.955336 rofimoji-6.3.0/src/picker/recent.py
--rw-r--r--   0        0        0        0 2022-11-13 10:52:07.473886 rofimoji-6.3.0/src/picker/selector/__init__.py
--rw-r--r--   0        0        0     1869 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/bemenu.py
--rw-r--r--   0        0        0     1846 2024-03-24 10:52:21.402810 rofimoji-6.3.0/src/picker/selector/dmenu.py
--rw-r--r--   0        0        0     1964 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/fuzzel.py
--rw-r--r--   0        0        0     4378 2024-03-29 09:38:49.797137 rofimoji-6.3.0/src/picker/selector/rofi.py
--rw-r--r--   0        0        0     2540 2024-03-29 09:38:49.797137 rofimoji-6.3.0/src/picker/selector/selector.py
--rw-r--r--   0        0        0     2081 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/tofi.py
--rw-r--r--   0        0        0     1846 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/wmenu.py
--rw-r--r--   0        0        0     1956 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/wofi.py
--rw-r--r--   0        0        0     3809 2024-04-26 19:41:42.529177 rofimoji-6.3.0/src/picker/standalone.py
--rw-r--r--   0        0        0        0 2022-11-13 10:52:07.473886 rofimoji-6.3.0/src/picker/typer/__init__.py
--rw-r--r--   0        0        0      636 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/typer/noop.py
--rw-r--r--   0        0        0      998 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/typer/typer.py
--rw-r--r--   0        0        0      648 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/typer/wtype.py
--rw-r--r--   0        0        0     1224 2024-04-14 14:51:30.446733 rofimoji-6.3.0/src/picker/typer/xdotool.py
--rw-r--r--   0        0        0    20588 1970-01-01 00:00:00.000000 rofimoji-6.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-24 10:41:32.767624 rofimoji-6.3.1/LICENSE
+-rw-r--r--   0        0        0    19841 2024-04-27 13:42:04.149186 rofimoji-6.3.1/README.md
+-rw-r--r--   0        0        0      892 2024-05-11 14:51:56.641374 rofimoji-6.3.1/pyproject.toml
+-rw-r--r--   0        0        0       89 2022-12-29 11:56:19.212555 rofimoji-6.3.1/src/picker/__init__.py
+-rw-r--r--   0        0        0      259 2024-03-29 09:38:49.773804 rofimoji-6.3.1/src/picker/__main__.py
+-rw-r--r--   0        0        0      188 2022-11-13 10:52:07.457219 rofimoji-6.3.1/src/picker/abstractionhelper.py
+-rw-r--r--   0        0        0     1204 2024-03-24 10:41:32.767624 rofimoji-6.3.1/src/picker/action.py
+-rw-r--r--   0        0        0     5849 2024-03-24 10:41:32.767624 rofimoji-6.3.1/src/picker/argument_parsing.py
+-rw-r--r--   0        0        0        0 2022-11-13 10:52:07.457219 rofimoji-6.3.1/src/picker/clipboarder/__init__.py
+-rw-r--r--   0        0        0     1127 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/clipboarder/clipboarder.py
+-rw-r--r--   0        0        0      677 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/clipboarder/noop.py
+-rw-r--r--   0        0        0     1093 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/clipboarder/wl.py
+-rw-r--r--   0        0        0     1885 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/clipboarder/xclip.py
+-rw-r--r--   0        0        0     1115 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/clipboarder/xsel.py
+-rw-r--r--   0        0        0      452 2024-03-24 10:45:56.170300 rofimoji-6.3.1/src/picker/contrib/grid-icons-only.rasi
+-rw-r--r--   0        0        0      457 2024-03-24 10:44:13.180796 rofimoji-6.3.1/src/picker/contrib/grid.rasi
+-rw-r--r--   0        0        0       23 2023-08-17 09:39:13.406636 rofimoji-6.3.1/src/picker/data/additional/emojis_smileys_emotion.csv
+-rw-r--r--   0        0        0     2712 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/adlam.csv
+-rw-r--r--   0        0        0     1737 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/aegean_numbers.csv
+-rw-r--r--   0        0        0     1470 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/ahom.csv
+-rw-r--r--   0        0        0     4551 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/alchemical_symbols.csv
+-rw-r--r--   0        0        0     2098 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/alphabetic_presentation_forms.csv
+-rw-r--r--   0        0        0    18183 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/anatolian_hieroglyphs.csv
+-rw-r--r--   0        0        0     2761 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/ancient_greek_musical_notation.csv
+-rw-r--r--   0        0        0     2895 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/ancient_greek_numbers.csv
+-rw-r--r--   0        0        0      344 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/ancient_symbols.csv
+-rw-r--r--   0        0        0     8311 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/arabic.csv
+-rw-r--r--   0        0        0     3561 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/arabic_extended-a.csv
+-rw-r--r--   0        0        0     1906 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/arabic_extended-b.csv
+-rw-r--r--   0        0        0       98 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/arabic_extended-c.csv
+-rw-r--r--   0        0        0     5786 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/arabic_mathematical_alphabetic_symbols.csv
+-rw-r--r--   0        0        0    32176 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/arabic_presentation_forms-a.csv
+-rw-r--r--   0        0        0     5722 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/arabic_presentation_forms-b.csv
+-rw-r--r--   0        0        0     2719 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/arabic_supplement.csv
+-rw-r--r--   0        0        0     2715 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/armenian.csv
+-rw-r--r--   0        0        0     3689 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/arrows.csv
+-rw-r--r--   0        0        0     1729 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/avestan.csv
+-rw-r--r--   0        0        0     3904 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/balinese.csv
+-rw-r--r--   0        0        0     1870 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/bamum.csv
+-rw-r--r--   0        0        0    18380 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/bamum_supplement.csv
+-rw-r--r--   0        0        0     1876 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/basic_latin.csv
+-rw-r--r--   0        0        0      968 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/bassa_vah.csv
+-rw-r--r--   0        0        0     1419 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/batak.csv
+-rw-r--r--   0        0        0     2451 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/bengali.csv
+-rw-r--r--   0        0        0     2625 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/bhaiksuki.csv
+-rw-r--r--   0        0        0      944 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/block_elements.csv
+-rw-r--r--   0        0        0      981 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/bopomofo.csv
+-rw-r--r--   0        0        0      774 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/bopomofo_extended.csv
+-rw-r--r--   0        0        0     5625 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/box_drawing.csv
+-rw-r--r--   0        0        0     2950 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/brahmi.csv
+-rw-r--r--   0        0        0     7680 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/braille_patterns.csv
+-rw-r--r--   0        0        0      716 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/buginese.csv
+-rw-r--r--   0        0        0      404 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/buhid.csv
+-rw-r--r--   0        0        0    11298 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/byzantine_musical_symbols.csv
+-rw-r--r--   0        0        0     1078 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/carian.csv
+-rw-r--r--   0        0        0     1885 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/caucasian_albanian.csv
+-rw-r--r--   0        0        0     1675 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/chakma.csv
+-rw-r--r--   0        0        0     1820 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/cham.csv
+-rw-r--r--   0        0        0     2166 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/cherokee.csv
+-rw-r--r--   0        0        0     2334 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/cherokee_supplement.csv
+-rw-r--r--   0        0        0     4120 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/chess_symbols.csv
+-rw-r--r--   0        0        0      889 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/chorasmian.csv
+-rw-r--r--   0        0        0   282678 2024-05-06 17:03:12.984291 rofimoji-6.3.1/src/picker/data/cjk_cantonese.csv
+-rw-r--r--   0        0        0     6158 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/cjk_compatibility.csv
+-rw-r--r--   0        0        0     1463 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/cjk_compatibility_forms.csv
+-rw-r--r--   0        0        0    17464 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/cjk_compatibility_ideographs.csv
+-rw-r--r--   0        0        0    21138 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/cjk_compatibility_ideographs_supplement.csv
+-rw-r--r--   0        0        0   164294 2024-05-06 17:03:13.034291 rofimoji-6.3.1/src/picker/data/cjk_japanese_kun.csv
+-rw-r--r--   0        0        0   152011 2024-05-06 17:03:13.044291 rofimoji-6.3.1/src/picker/data/cjk_japanese_on.csv
+-rw-r--r--   0        0        0    76750 2024-05-06 17:03:13.050957 rofimoji-6.3.1/src/picker/data/cjk_korean.csv
+-rw-r--r--   0        0        0   390276 2024-05-06 17:03:13.010957 rofimoji-6.3.1/src/picker/data/cjk_mandarin.csv
+-rw-r--r--   0        0        0     3072 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/cjk_radicals_supplement.csv
+-rw-r--r--   0        0        0      714 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/cjk_strokes.csv
+-rw-r--r--   0        0        0     1919 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/cjk_symbols_and_punctuation.csv
+-rw-r--r--   0        0        0    43076 2024-05-06 17:03:13.024291 rofimoji-6.3.1/src/picker/data/cjk_tang.csv
+-rw-r--r--   0        0        0    87736 2024-05-06 17:03:13.017624 rofimoji-6.3.1/src/picker/data/cjk_vietnamese.csv
+-rw-r--r--   0        0        0     3356 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/combining_diacritical_marks.csv
+-rw-r--r--   0        0        0     1141 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/combining_diacritical_marks_extended.csv
+-rw-r--r--   0        0        0     1189 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/combining_diacritical_marks_for_symbols.csv
+-rw-r--r--   0        0        0     2374 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/combining_diacritical_marks_supplement.csv
+-rw-r--r--   0        0        0      581 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/combining_half_marks.csv
+-rw-r--r--   0        0        0      347 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/common_indic_number_forms.csv
+-rw-r--r--   0        0        0     1104 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/control_pictures.csv
+-rw-r--r--   0        0        0     4234 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/coptic.csv
+-rw-r--r--   0        0        0      919 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/coptic_epact_numbers.csv
+-rw-r--r--   0        0        0      817 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/counting_rod_numerals.csv
+-rw-r--r--   0        0        0    30373 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/cuneiform.csv
+-rw-r--r--   0        0        0     5019 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/cuneiform_numbers_and_punctuation.csv
+-rw-r--r--   0        0        0      556 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/currency_symbols.csv
+-rw-r--r--   0        0        0     1535 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/cypriot_syllabary.csv
+-rw-r--r--   0        0        0     2873 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/cypro-minoan.csv
+-rw-r--r--   0        0        0     9424 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/cyrillic.csv
+-rw-r--r--   0        0        0     1116 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/cyrillic_extended-a.csv
+-rw-r--r--   0        0        0     3480 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/cyrillic_extended-b.csv
+-rw-r--r--   0        0        0      338 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/cyrillic_extended-c.csv
+-rw-r--r--   0        0        0     2654 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/cyrillic_extended-d.csv
+-rw-r--r--   0        0        0     1746 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/cyrillic_supplement.csv
+-rw-r--r--   0        0        0     2552 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/deseret.csv
+-rw-r--r--   0        0        0     3580 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/devanagari.csv
+-rw-r--r--   0        0        0      377 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/devanagari_extended-a.csv
+-rw-r--r--   0        0        0     1089 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/devanagari_extended.csv
+-rw-r--r--   0        0        0     6632 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/dingbats.csv
+-rw-r--r--   0        0        0     2029 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/dives_akuru.csv
+-rw-r--r--   0        0        0     1348 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/dogra.csv
+-rw-r--r--   0        0        0     3298 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/domino_tiles.csv
+-rw-r--r--   0        0        0     4069 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/duployan.csv
+-rw-r--r--   0        0        0     7082 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/early_dynastic_cuneiform.csv
+-rw-r--r--   0        0        0     1794 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/egyptian_hieroglyph_format_controls.csv
+-rw-r--r--   0        0        0    32482 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/egyptian_hieroglyphs.csv
+-rw-r--r--   0        0        0      930 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/elbasan.csv
+-rw-r--r--   0        0        0      654 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/elymaic.csv
+-rw-r--r--   0        0        0     5642 2024-05-06 17:03:08.227627 rofimoji-6.3.1/src/picker/data/emojis_activities.csv
+-rw-r--r--   0        0        0     7330 2024-05-06 17:03:08.224294 rofimoji-6.3.1/src/picker/data/emojis_animals_nature.csv
+-rw-r--r--   0        0        0      253 2024-05-06 17:03:08.224294 rofimoji-6.3.1/src/picker/data/emojis_component.csv
+-rw-r--r--   0        0        0     7284 2024-05-06 17:03:08.227627 rofimoji-6.3.1/src/picker/data/emojis_flags.csv
+-rw-r--r--   0        0        0     7931 2024-05-06 17:03:08.224294 rofimoji-6.3.1/src/picker/data/emojis_food_drink.csv
+-rw-r--r--   0        0        0    16393 2024-05-06 17:03:08.227627 rofimoji-6.3.1/src/picker/data/emojis_objects.csv
+-rw-r--r--   0        0        0    21230 2024-05-06 17:03:08.224294 rofimoji-6.3.1/src/picker/data/emojis_people_body.csv
+-rw-r--r--   0        0        0    11962 2024-05-06 17:03:08.224294 rofimoji-6.3.1/src/picker/data/emojis_smileys_emotion.csv
+-rw-r--r--   0        0        0    16126 2024-05-06 17:03:08.227627 rofimoji-6.3.1/src/picker/data/emojis_symbols.csv
+-rw-r--r--   0        0        0    13690 2024-05-06 17:03:08.224294 rofimoji-6.3.1/src/picker/data/emojis_travel_places.csv
+-rw-r--r--   0        0        0     2229 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/emoticons.csv
+-rw-r--r--   0        0        0     7107 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/enclosed_alphanumeric_supplement.csv
+-rw-r--r--   0        0        0     5169 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/enclosed_alphanumerics.csv
+-rw-r--r--   0        0        0     7668 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/enclosed_cjk_letters_and_months.csv
+-rw-r--r--   0        0        0     2570 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/enclosed_ideographic_supplement.csv
+-rw-r--r--   0        0        0     9421 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/ethiopic.csv
+-rw-r--r--   0        0        0      868 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/ethiopic_extended-a.csv
+-rw-r--r--   0        0        0      903 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/ethiopic_extended-b.csv
+-rw-r--r--   0        0        0     2095 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/ethiopic_extended.csv
+-rw-r--r--   0        0        0      774 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/ethiopic_supplement.csv
+-rw-r--r--   0        0        0    52690 2024-05-06 17:03:15.550956 rofimoji-6.3.1/src/picker/data/fontawesome6.csv
+-rw-r--r--   0        0        0     2575 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/general_punctuation.csv
+-rw-r--r--   0        0        0     3087 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/geometric_shapes.csv
+-rw-r--r--   0        0        0     3236 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/geometric_shapes_extended.csv
+-rw-r--r--   0        0        0     2472 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/georgian.csv
+-rw-r--r--   0        0        0     1908 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/georgian_extended.csv
+-rw-r--r--   0        0        0     1200 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/georgian_supplement.csv
+-rw-r--r--   0        0        0     2433 2024-05-06 17:03:14.074290 rofimoji-6.3.1/src/picker/data/gitmoji.csv
+-rw-r--r--   0        0        0     3486 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/glagolitic.csv
+-rw-r--r--   0        0        0     1500 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/glagolitic_supplement.csv
+-rw-r--r--   0        0        0      684 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/gothic.csv
+-rw-r--r--   0        0        0     2304 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/grantha.csv
+-rw-r--r--   0        0        0     4218 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/greek_and_coptic.csv
+-rw-r--r--   0        0        0    11730 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/greek_extended.csv
+-rw-r--r--   0        0        0     2334 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/gujarati.csv
+-rw-r--r--   0        0        0     1881 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/gunjala_gondi.csv
+-rw-r--r--   0        0        0     1908 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/gurmukhi.csv
+-rw-r--r--   0        0        0     7414 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/halfwidth_and_fullwidth_forms.csv
+-rw-r--r--   0        0        0     2543 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/hangul_compatibility_jamo.csv
+-rw-r--r--   0        0        0     7910 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/hangul_jamo.csv
+-rw-r--r--   0        0        0      985 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/hangul_jamo_extended-a.csv
+-rw-r--r--   0        0        0     2383 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/hangul_jamo_extended-b.csv
+-rw-r--r--   0        0        0     1719 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/hanifi_rohingya.csv
+-rw-r--r--   0        0        0      538 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/hanunoo.csv
+-rw-r--r--   0        0        0      714 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/hatran.csv
+-rw-r--r--   0        0        0     2344 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/hebrew.csv
+-rw-r--r--   0        0        0     2318 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/hiragana.csv
+-rw-r--r--   0        0        0      923 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/ideographic_description_characters.csv
+-rw-r--r--   0        0        0      230 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/ideographic_symbols_and_punctuation.csv
+-rw-r--r--   0        0        0     1173 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/imperial_aramaic.csv
+-rw-r--r--   0        0        0     2591 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/indic_siyaq_numbers.csv
+-rw-r--r--   0        0        0     1166 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/inscriptional_pahlavi.csv
+-rw-r--r--   0        0        0     1307 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/inscriptional_parthian.csv
+-rw-r--r--   0        0        0     3418 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/ipa_extensions.csv
+-rw-r--r--   0        0        0     2438 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/javanese.csv
+-rw-r--r--   0        0        0     1611 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/kaithi.csv
+-rw-r--r--   0        0        0      570 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/kaktovik_numerals.csv
+-rw-r--r--   0        0        0     1006 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/kana_extended-a.csv
+-rw-r--r--   0        0        0      525 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/kana_extended-b.csv
+-rw-r--r--   0        0        0     7167 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/kana_supplement.csv
+-rw-r--r--   0        0        0      608 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/kanbun.csv
+-rw-r--r--   0        0        0     5434 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/kangxi_radicals.csv
+-rw-r--r--   0        0        0     2241 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/kannada.csv
+-rw-r--r--   0        0        0    43839 2024-05-06 17:03:15.880956 rofimoji-6.3.1/src/picker/data/kaomoji.csv
+-rw-r--r--   0        0        0     2323 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/katakana.csv
+-rw-r--r--   0        0        0      464 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/katakana_phonetic_extensions.csv
+-rw-r--r--   0        0        0     1997 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/kawi.csv
+-rw-r--r--   0        0        0     1121 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/kayah_li.csv
+-rw-r--r--   0        0        0     2145 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/kharoshthi.csv
+-rw-r--r--   0        0        0    19270 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/khitan_small_script.csv
+-rw-r--r--   0        0        0     2849 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/khmer.csv
+-rw-r--r--   0        0        0      916 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/khmer_symbols.csv
+-rw-r--r--   0        0        0     1526 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/khojki.csv
+-rw-r--r--   0        0        0     1793 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/khudawadi.csv
+-rw-r--r--   0        0        0     1779 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/lao.csv
+-rw-r--r--   0        0        0     2978 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/latin-1_supplement.csv
+-rw-r--r--   0        0        0     4762 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/latin_extended-a.csv
+-rw-r--r--   0        0        0     7913 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/latin_extended-b.csv
+-rw-r--r--   0        0        0     1235 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/latin_extended-c.csv
+-rw-r--r--   0        0        0     7236 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/latin_extended-d.csv
+-rw-r--r--   0        0        0     2474 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/latin_extended-e.csv
+-rw-r--r--   0        0        0     2450 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/latin_extended-f.csv
+-rw-r--r--   0        0        0     1799 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/latin_extended-g.csv
+-rw-r--r--   0        0        0    11426 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/latin_extended_additional.csv
+-rw-r--r--   0        0        0     1765 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/lepcha.csv
+-rw-r--r--   0        0        0     1840 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/letterlike_symbols.csv
+-rw-r--r--   0        0        0     1538 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/limbu.csv
+-rw-r--r--   0        0        0     8429 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/linear_a.csv
+-rw-r--r--   0        0        0     3958 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/linear_b_ideograms.csv
+-rw-r--r--   0        0        0     2664 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/linear_b_syllabary.csv
+-rw-r--r--   0        0        0      995 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/lisu.csv
+-rw-r--r--   0        0        0       21 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/lisu_supplement.csv
+-rw-r--r--   0        0        0      617 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/lycian.csv
+-rw-r--r--   0        0        0      661 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/lydian.csv
+-rw-r--r--   0        0        0      964 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/mahajani.csv
+-rw-r--r--   0        0        0     1402 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/mahjong_tiles.csv
+-rw-r--r--   0        0        0      590 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/makasar.csv
+-rw-r--r--   0        0        0     3331 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/malayalam.csv
+-rw-r--r--   0        0        0      760 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/mandaic.csv
+-rw-r--r--   0        0        0     1695 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/manichaean.csv
+-rw-r--r--   0        0        0     1903 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/marchen.csv
+-rw-r--r--   0        0        0     2252 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/masaram_gondi.csv
+-rw-r--r--   0        0        0    93185 2024-05-06 17:03:13.644290 rofimoji-6.3.1/src/picker/data/math.csv
+-rw-r--r--   0        0        0    40125 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/mathematical_alphanumeric_symbols.csv
+-rw-r--r--   0        0        0     6216 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/mathematical_operators.csv
+-rw-r--r--   0        0        0      510 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/mayan_numerals.csv
+-rw-r--r--   0        0        0     2969 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/medefaidrin.csv
+-rw-r--r--   0        0        0     1668 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/meetei_mayek.csv
+-rw-r--r--   0        0        0      681 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/meetei_mayek_extensions.csv
+-rw-r--r--   0        0        0     8499 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/mende_kikakui.csv
+-rw-r--r--   0        0        0     3826 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/meroitic_cursive.csv
+-rw-r--r--   0        0        0     1298 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/meroitic_hieroglyphs.csv
+-rw-r--r--   0        0        0     3532 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/miao.csv
+-rw-r--r--   0        0        0     1541 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/miscellaneous_mathematical_symbols-a.csv
+-rw-r--r--   0        0        0     4228 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/miscellaneous_mathematical_symbols-b.csv
+-rw-r--r--   0        0        0     5475 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/miscellaneous_symbols.csv
+-rw-r--r--   0        0        0     9010 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/miscellaneous_symbols_and_arrows.csv
+-rw-r--r--   0        0        0    16261 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/miscellaneous_symbols_and_pictographs.csv
+-rw-r--r--   0        0        0     7975 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/miscellaneous_technical.csv
+-rw-r--r--   0        0        0     1736 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/modi.csv
+-rw-r--r--   0        0        0     1413 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/modifier_tone_letters.csv
+-rw-r--r--   0        0        0     4806 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/mongolian.csv
+-rw-r--r--   0        0        0      535 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/mongolian_supplement.csv
+-rw-r--r--   0        0        0      843 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/mro.csv
+-rw-r--r--   0        0        0      893 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/multani.csv
+-rw-r--r--   0        0        0     8605 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/musical_symbols.csv
+-rw-r--r--   0        0        0     4595 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/myanmar.csv
+-rw-r--r--   0        0        0     1000 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/myanmar_extended-a.csv
+-rw-r--r--   0        0        0     1001 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/myanmar_extended-b.csv
+-rw-r--r--   0        0        0     1272 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/nabataean.csv
+-rw-r--r--   0        0        0     1148 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/nag_mundari.csv
+-rw-r--r--   0        0        0     1875 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/nandinagari.csv
+-rw-r--r--   0        0        0   290162 2023-05-20 08:41:43.841476 rofimoji-6.3.1/src/picker/data/nerd_font.csv
+-rw-r--r--   0        0        0     2505 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/new_tai_lue.csv
+-rw-r--r--   0        0        0     2148 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/newa.csv
+-rw-r--r--   0        0        0     1440 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/nko.csv
+-rw-r--r--   0        0        0     1772 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/number_forms.csv
+-rw-r--r--   0        0        0    10692 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/nushu.csv
+-rw-r--r--   0        0        0     2755 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/nyiakeng_puachue_hmong.csv
+-rw-r--r--   0        0        0      673 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/ogham.csv
+-rw-r--r--   0        0        0     1158 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/ol_chiki.csv
+-rw-r--r--   0        0        0     4348 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/old_hungarian.csv
+-rw-r--r--   0        0        0     1049 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/old_italic.csv
+-rw-r--r--   0        0        0     1200 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/old_north_arabian.csv
+-rw-r--r--   0        0        0     1221 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/old_permic.csv
+-rw-r--r--   0        0        0     1338 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/old_persian.csv
+-rw-r--r--   0        0        0     1434 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/old_sogdian.csv
+-rw-r--r--   0        0        0     1228 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/old_south_arabian.csv
+-rw-r--r--   0        0        0     2688 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/old_turkic.csv
+-rw-r--r--   0        0        0      881 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/old_uyghur.csv
+-rw-r--r--   0        0        0      227 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/optical_character_recognition.csv
+-rw-r--r--   0        0        0     2060 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/oriya.csv
+-rw-r--r--   0        0        0     1683 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/ornamental_dingbats.csv
+-rw-r--r--   0        0        0     2060 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/osage.csv
+-rw-r--r--   0        0        0      947 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/osmanya.csv
+-rw-r--r--   0        0        0     2505 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/ottoman_siyaq_numbers.csv
+-rw-r--r--   0        0        0     4001 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/pahawh_hmong.csv
+-rw-r--r--   0        0        0      988 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/palmyrene.csv
+-rw-r--r--   0        0        0     1776 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/pau_cin_hau.csv
+-rw-r--r--   0        0        0     1415 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/phags-pa.csv
+-rw-r--r--   0        0        0     1455 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/phaistos_disc.csv
+-rw-r--r--   0        0        0      889 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/phoenician.csv
+-rw-r--r--   0        0        0     4468 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/phonetic_extensions.csv
+-rw-r--r--   0        0        0     2620 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/phonetic_extensions_supplement.csv
+-rw-r--r--   0        0        0     2562 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/playing_cards.csv
+-rw-r--r--   0        0        0     1093 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/psalter_pahlavi.csv
+-rw-r--r--   0        0        0      841 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/rejang.csv
+-rw-r--r--   0        0        0      881 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/rumi_numeral_symbols.csv
+-rw-r--r--   0        0        0     2424 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/runic.csv
+-rw-r--r--   0        0        0     1929 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/samaritan.csv
+-rw-r--r--   0        0        0     2217 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/saurashtra.csv
+-rw-r--r--   0        0        0     2452 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/sharada.csv
+-rw-r--r--   0        0        0     1172 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/shavian.csv
+-rw-r--r--   0        0        0      140 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/shorthand_format_controls.csv
+-rw-r--r--   0        0        0     2805 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/siddham.csv
+-rw-r--r--   0        0        0     3060 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/sinhala.csv
+-rw-r--r--   0        0        0      679 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/sinhala_archaic_numbers.csv
+-rw-r--r--   0        0        0      634 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/small_form_variants.csv
+-rw-r--r--   0        0        0      269 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/small_kana_extension.csv
+-rw-r--r--   0        0        0     1379 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/sogdian.csv
+-rw-r--r--   0        0        0     1012 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/sora_sompeng.csv
+-rw-r--r--   0        0        0     2345 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/soyombo.csv
+-rw-r--r--   0        0        0     2565 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/spacing_modifier_letters.csv
+-rw-r--r--   0        0        0      168 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/specials.csv
+-rw-r--r--   0        0        0     1714 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/sundanese.csv
+-rw-r--r--   0        0        0      330 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/sundanese_supplement.csv
+-rw-r--r--   0        0        0     1147 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/superscripts_and_subscripts.csv
+-rw-r--r--   0        0        0      526 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/supplemental_arrows-a.csv
+-rw-r--r--   0        0        0     5599 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/supplemental_arrows-b.csv
+-rw-r--r--   0        0        0     6639 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/supplemental_arrows-c.csv
+-rw-r--r--   0        0        0     8936 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/supplemental_mathematical_operators.csv
+-rw-r--r--   0        0        0     2556 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/supplemental_punctuation.csv
+-rw-r--r--   0        0        0     4767 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/supplemental_symbols_and_pictographs.csv
+-rw-r--r--   0        0        0    31771 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/sutton_signwriting.csv
+-rw-r--r--   0        0        0     1281 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/syloti_nagri.csv
+-rw-r--r--   0        0        0     1743 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/symbols_and_pictographs_extended-a.csv
+-rw-r--r--   0        0        0     8729 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/symbols_for_legacy_computing.csv
+-rw-r--r--   0        0        0     2135 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/syriac.csv
+-rw-r--r--   0        0        0      385 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/syriac_supplement.csv
+-rw-r--r--   0        0        0      524 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/tagalog.csv
+-rw-r--r--   0        0        0      418 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/tagbanwa.csv
+-rw-r--r--   0        0        0     2575 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/tags.csv
+-rw-r--r--   0        0        0      758 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/tai_le.csv
+-rw-r--r--   0        0        0     3550 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/tai_tham.csv
+-rw-r--r--   0        0        0     1897 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/tai_viet.csv
+-rw-r--r--   0        0        0     2517 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/tai_xuan_jing_symbols.csv
+-rw-r--r--   0        0        0     1511 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/takri.csv
+-rw-r--r--   0        0        0     1534 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/tamil.csv
+-rw-r--r--   0        0        0     1535 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/tamil_supplement.csv
+-rw-r--r--   0        0        0     2028 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/tangsa.csv
+-rw-r--r--   0        0        0    19968 2024-05-06 17:03:09.684293 rofimoji-6.3.1/src/picker/data/tangut_components.csv
+-rw-r--r--   0        0        0     2566 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/telugu.csv
+-rw-r--r--   0        0        0     1234 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/thaana.csv
+-rw-r--r--   0        0        0     2340 2024-05-06 17:03:09.664293 rofimoji-6.3.1/src/picker/data/thai.csv
+-rw-r--r--   0        0        0     6455 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/tibetan.csv
+-rw-r--r--   0        0        0     1582 2024-05-06 17:03:09.670960 rofimoji-6.3.1/src/picker/data/tifinagh.csv
+-rw-r--r--   0        0        0     2049 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/tirhuta.csv
+-rw-r--r--   0        0        0      662 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/toto.csv
+-rw-r--r--   0        0        0     2229 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/transport_and_map_symbols.csv
+-rw-r--r--   0        0        0      791 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/ugaritic.csv
+-rw-r--r--   0        0        0    20601 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/unified_canadian_aboriginal_syllabics.csv
+-rw-r--r--   0        0        0      562 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/unified_canadian_aboriginal_syllabics_extended-a.csv
+-rw-r--r--   0        0        0     2167 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/unified_canadian_aboriginal_syllabics_extended.csv
+-rw-r--r--   0        0        0     6238 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/vai.csv
+-rw-r--r--   0        0        0      407 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/variation_selectors.csv
+-rw-r--r--   0        0        0     6637 2024-05-06 17:03:09.690960 rofimoji-6.3.1/src/picker/data/variation_selectors_supplement.csv
+-rw-r--r--   0        0        0     1512 2024-05-06 17:03:09.667626 rofimoji-6.3.1/src/picker/data/vedic_extensions.csv
+-rw-r--r--   0        0        0      524 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/vertical_forms.csv
+-rw-r--r--   0        0        0     2176 2024-05-06 17:03:09.677626 rofimoji-6.3.1/src/picker/data/vithkuqi.csv
+-rw-r--r--   0        0        0     1321 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/wancho.csv
+-rw-r--r--   0        0        0     2788 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/warang_citi.csv
+-rw-r--r--   0        0        0     1286 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/yezidi.csv
+-rw-r--r--   0        0        0     1052 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/yi_radicals.csv
+-rw-r--r--   0        0        0    23855 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/yi_syllables.csv
+-rw-r--r--   0        0        0     1955 2024-05-06 17:03:09.674293 rofimoji-6.3.1/src/picker/data/yijing_hexagram_symbols.csv
+-rw-r--r--   0        0        0     2586 2024-05-06 17:03:09.680960 rofimoji-6.3.1/src/picker/data/zanabazar_square.csv
+-rw-r--r--   0        0        0     7873 2024-05-06 17:03:09.687626 rofimoji-6.3.1/src/picker/data/znamenny_musical_notation.csv
+-rw-r--r--   0        0        0     5387 2024-05-11 14:51:43.921469 rofimoji-6.3.1/src/picker/docs/rofimoji.1
+-rw-r--r--   0        0        0     4620 2024-05-11 14:51:39.461503 rofimoji-6.3.1/src/picker/docs/rofimoji.1.md
+-rw-r--r--   0        0        0     1982 2023-09-16 08:10:09.785973 rofimoji-6.3.1/src/picker/emoji_data.py
+-rw-r--r--   0        0        0     3331 2024-05-06 16:08:16.276068 rofimoji-6.3.1/src/picker/file_loader.py
+-rw-r--r--   0        0        0     1106 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/frecent.py
+-rw-r--r--   0        0        0     7720 2024-03-29 09:41:20.083560 rofimoji-6.3.1/src/picker/mode.py
+-rw-r--r--   0        0        0     1258 2024-05-06 16:08:16.276068 rofimoji-6.3.1/src/picker/models.py
+-rw-r--r--   0        0        0      708 2022-11-13 10:52:07.473886 rofimoji-6.3.1/src/picker/paths.py
+-rw-r--r--   0        0        0     1657 2024-05-06 16:48:42.299637 rofimoji-6.3.1/src/picker/recent.py
+-rw-r--r--   0        0        0        0 2022-11-13 10:52:07.473886 rofimoji-6.3.1/src/picker/selector/__init__.py
+-rw-r--r--   0        0        0     1869 2024-03-24 10:52:21.399476 rofimoji-6.3.1/src/picker/selector/bemenu.py
+-rw-r--r--   0        0        0     1846 2024-03-24 10:52:21.402810 rofimoji-6.3.1/src/picker/selector/dmenu.py
+-rw-r--r--   0        0        0     1964 2024-03-24 10:52:21.399476 rofimoji-6.3.1/src/picker/selector/fuzzel.py
+-rw-r--r--   0        0        0     4378 2024-03-29 09:38:49.797137 rofimoji-6.3.1/src/picker/selector/rofi.py
+-rw-r--r--   0        0        0     2540 2024-03-29 09:38:49.797137 rofimoji-6.3.1/src/picker/selector/selector.py
+-rw-r--r--   0        0        0     2081 2024-03-24 10:52:21.399476 rofimoji-6.3.1/src/picker/selector/tofi.py
+-rw-r--r--   0        0        0     1846 2024-03-24 10:52:21.399476 rofimoji-6.3.1/src/picker/selector/wmenu.py
+-rw-r--r--   0        0        0     1956 2024-03-24 10:52:21.399476 rofimoji-6.3.1/src/picker/selector/wofi.py
+-rw-r--r--   0        0        0     3809 2024-04-26 19:41:42.529177 rofimoji-6.3.1/src/picker/standalone.py
+-rw-r--r--   0        0        0        0 2022-11-13 10:52:07.473886 rofimoji-6.3.1/src/picker/typer/__init__.py
+-rw-r--r--   0        0        0      636 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/typer/noop.py
+-rw-r--r--   0        0        0      998 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/typer/typer.py
+-rw-r--r--   0        0        0      648 2024-03-24 10:41:32.770958 rofimoji-6.3.1/src/picker/typer/wtype.py
+-rw-r--r--   0        0        0     1224 2024-04-14 14:51:30.446733 rofimoji-6.3.1/src/picker/typer/xdotool.py
+-rw-r--r--   0        0        0    20588 1970-01-01 00:00:00.000000 rofimoji-6.3.1/PKG-INFO
```

### Comparing `rofimoji-6.3.0/LICENSE` & `rofimoji-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/README.md` & `rofimoji-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/pyproject.toml` & `rofimoji-6.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rofimoji"
-version = "6.3.0"
+version = "6.3.1"
 description = "Simple character picker using rofi"
 authors = ["Fabian Winter <5821180+fdw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fdw/rofimoji"
 repository = "https://github.com/fdw/rofimoji"
 packages =[
@@ -21,17 +21,17 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ConfigArgParse = "^1.3"
 
 [tool.poetry.group.dev.dependencies]
 beautifulsoup4 = "^4.12.3"
-lxml = "^4.9.4"
+lxml = "^5.2.1"
 requests = "^2.31.0"
-tqdm = "^4.66.2"
+tqdm = "^4.66.4"
 black = "^24.3.0"
 isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rofimoji-6.3.0/src/picker/action.py` & `rofimoji-6.3.1/src/picker/action.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/argument_parsing.py` & `rofimoji-6.3.1/src/picker/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/clipboarder/clipboarder.py` & `rofimoji-6.3.1/src/picker/clipboarder/clipboarder.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/clipboarder/noop.py` & `rofimoji-6.3.1/src/picker/clipboarder/noop.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/clipboarder/wl.py` & `rofimoji-6.3.1/src/picker/clipboarder/wl.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/clipboarder/xclip.py` & `rofimoji-6.3.1/src/picker/clipboarder/xclip.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/clipboarder/xsel.py` & `rofimoji-6.3.1/src/picker/clipboarder/xsel.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/adlam.csv` & `rofimoji-6.3.1/src/picker/data/adlam.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/aegean_numbers.csv` & `rofimoji-6.3.1/src/picker/data/aegean_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ahom.csv` & `rofimoji-6.3.1/src/picker/data/ahom.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/alchemical_symbols.csv` & `rofimoji-6.3.1/src/picker/data/alchemical_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/alphabetic_presentation_forms.csv` & `rofimoji-6.3.1/src/picker/data/alphabetic_presentation_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/anatolian_hieroglyphs.csv` & `rofimoji-6.3.1/src/picker/data/anatolian_hieroglyphs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ancient_greek_musical_notation.csv` & `rofimoji-6.3.1/src/picker/data/ancient_greek_musical_notation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ancient_greek_numbers.csv` & `rofimoji-6.3.1/src/picker/data/ancient_greek_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/arabic.csv` & `rofimoji-6.3.1/src/picker/data/arabic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/arabic_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/arabic_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/arabic_extended-b.csv` & `rofimoji-6.3.1/src/picker/data/arabic_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/arabic_mathematical_alphabetic_symbols.csv` & `rofimoji-6.3.1/src/picker/data/arabic_mathematical_alphabetic_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/arabic_presentation_forms-a.csv` & `rofimoji-6.3.1/src/picker/data/arabic_presentation_forms-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/arabic_presentation_forms-b.csv` & `rofimoji-6.3.1/src/picker/data/arabic_presentation_forms-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/arabic_supplement.csv` & `rofimoji-6.3.1/src/picker/data/arabic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/armenian.csv` & `rofimoji-6.3.1/src/picker/data/armenian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/arrows.csv` & `rofimoji-6.3.1/src/picker/data/arrows.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/avestan.csv` & `rofimoji-6.3.1/src/picker/data/avestan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/balinese.csv` & `rofimoji-6.3.1/src/picker/data/balinese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/bamum.csv` & `rofimoji-6.3.1/src/picker/data/bamum.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/bamum_supplement.csv` & `rofimoji-6.3.1/src/picker/data/bamum_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/basic_latin.csv` & `rofimoji-6.3.1/src/picker/data/basic_latin.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/bassa_vah.csv` & `rofimoji-6.3.1/src/picker/data/bassa_vah.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/batak.csv` & `rofimoji-6.3.1/src/picker/data/batak.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/bengali.csv` & `rofimoji-6.3.1/src/picker/data/bengali.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/bhaiksuki.csv` & `rofimoji-6.3.1/src/picker/data/bhaiksuki.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/block_elements.csv` & `rofimoji-6.3.1/src/picker/data/block_elements.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/bopomofo.csv` & `rofimoji-6.3.1/src/picker/data/bopomofo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/bopomofo_extended.csv` & `rofimoji-6.3.1/src/picker/data/bopomofo_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/box_drawing.csv` & `rofimoji-6.3.1/src/picker/data/box_drawing.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/brahmi.csv` & `rofimoji-6.3.1/src/picker/data/brahmi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/braille_patterns.csv` & `rofimoji-6.3.1/src/picker/data/braille_patterns.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/buginese.csv` & `rofimoji-6.3.1/src/picker/data/buginese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/byzantine_musical_symbols.csv` & `rofimoji-6.3.1/src/picker/data/byzantine_musical_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/carian.csv` & `rofimoji-6.3.1/src/picker/data/carian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/caucasian_albanian.csv` & `rofimoji-6.3.1/src/picker/data/caucasian_albanian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/chakma.csv` & `rofimoji-6.3.1/src/picker/data/chakma.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cham.csv` & `rofimoji-6.3.1/src/picker/data/cham.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cherokee.csv` & `rofimoji-6.3.1/src/picker/data/cherokee.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cherokee_supplement.csv` & `rofimoji-6.3.1/src/picker/data/cherokee_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/chess_symbols.csv` & `rofimoji-6.3.1/src/picker/data/chess_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/chorasmian.csv` & `rofimoji-6.3.1/src/picker/data/chorasmian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_cantonese.csv` & `rofimoji-6.3.1/src/picker/data/cjk_cantonese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_compatibility.csv` & `rofimoji-6.3.1/src/picker/data/cjk_compatibility.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_compatibility_forms.csv` & `rofimoji-6.3.1/src/picker/data/cjk_compatibility_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_compatibility_ideographs.csv` & `rofimoji-6.3.1/src/picker/data/cjk_compatibility_ideographs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_compatibility_ideographs_supplement.csv` & `rofimoji-6.3.1/src/picker/data/cjk_compatibility_ideographs_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_japanese_kun.csv` & `rofimoji-6.3.1/src/picker/data/cjk_japanese_kun.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_japanese_on.csv` & `rofimoji-6.3.1/src/picker/data/cjk_japanese_on.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_korean.csv` & `rofimoji-6.3.1/src/picker/data/cjk_korean.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_mandarin.csv` & `rofimoji-6.3.1/src/picker/data/cjk_mandarin.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_radicals_supplement.csv` & `rofimoji-6.3.1/src/picker/data/cjk_radicals_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_strokes.csv` & `rofimoji-6.3.1/src/picker/data/cjk_strokes.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_symbols_and_punctuation.csv` & `rofimoji-6.3.1/src/picker/data/cjk_symbols_and_punctuation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_tang.csv` & `rofimoji-6.3.1/src/picker/data/cjk_tang.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cjk_vietnamese.csv` & `rofimoji-6.3.1/src/picker/data/cjk_vietnamese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/combining_diacritical_marks.csv` & `rofimoji-6.3.1/src/picker/data/combining_diacritical_marks.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_extended.csv` & `rofimoji-6.3.1/src/picker/data/combining_diacritical_marks_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_for_symbols.csv` & `rofimoji-6.3.1/src/picker/data/combining_diacritical_marks_for_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_supplement.csv` & `rofimoji-6.3.1/src/picker/data/combining_diacritical_marks_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/combining_half_marks.csv` & `rofimoji-6.3.1/src/picker/data/combining_half_marks.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/control_pictures.csv` & `rofimoji-6.3.1/src/picker/data/control_pictures.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/coptic.csv` & `rofimoji-6.3.1/src/picker/data/coptic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/coptic_epact_numbers.csv` & `rofimoji-6.3.1/src/picker/data/coptic_epact_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/counting_rod_numerals.csv` & `rofimoji-6.3.1/src/picker/data/counting_rod_numerals.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cuneiform.csv` & `rofimoji-6.3.1/src/picker/data/cuneiform.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cuneiform_numbers_and_punctuation.csv` & `rofimoji-6.3.1/src/picker/data/cuneiform_numbers_and_punctuation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/currency_symbols.csv` & `rofimoji-6.3.1/src/picker/data/currency_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cypriot_syllabary.csv` & `rofimoji-6.3.1/src/picker/data/cypriot_syllabary.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cypro-minoan.csv` & `rofimoji-6.3.1/src/picker/data/cypro-minoan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cyrillic.csv` & `rofimoji-6.3.1/src/picker/data/cyrillic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cyrillic_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/cyrillic_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cyrillic_extended-b.csv` & `rofimoji-6.3.1/src/picker/data/cyrillic_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cyrillic_extended-d.csv` & `rofimoji-6.3.1/src/picker/data/cyrillic_extended-d.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/cyrillic_supplement.csv` & `rofimoji-6.3.1/src/picker/data/cyrillic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/deseret.csv` & `rofimoji-6.3.1/src/picker/data/deseret.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/devanagari.csv` & `rofimoji-6.3.1/src/picker/data/devanagari.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/devanagari_extended.csv` & `rofimoji-6.3.1/src/picker/data/devanagari_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/dingbats.csv` & `rofimoji-6.3.1/src/picker/data/dingbats.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/dives_akuru.csv` & `rofimoji-6.3.1/src/picker/data/dives_akuru.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/dogra.csv` & `rofimoji-6.3.1/src/picker/data/dogra.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/domino_tiles.csv` & `rofimoji-6.3.1/src/picker/data/domino_tiles.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/duployan.csv` & `rofimoji-6.3.1/src/picker/data/duployan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/early_dynastic_cuneiform.csv` & `rofimoji-6.3.1/src/picker/data/early_dynastic_cuneiform.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/egyptian_hieroglyph_format_controls.csv` & `rofimoji-6.3.1/src/picker/data/egyptian_hieroglyph_format_controls.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/egyptian_hieroglyphs.csv` & `rofimoji-6.3.1/src/picker/data/egyptian_hieroglyphs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/elbasan.csv` & `rofimoji-6.3.1/src/picker/data/elbasan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/elymaic.csv` & `rofimoji-6.3.1/src/picker/data/elymaic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_activities.csv` & `rofimoji-6.3.1/src/picker/data/emojis_activities.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_animals_nature.csv` & `rofimoji-6.3.1/src/picker/data/emojis_animals_nature.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_flags.csv` & `rofimoji-6.3.1/src/picker/data/emojis_flags.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_food_drink.csv` & `rofimoji-6.3.1/src/picker/data/emojis_food_drink.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_objects.csv` & `rofimoji-6.3.1/src/picker/data/emojis_objects.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_people_body.csv` & `rofimoji-6.3.1/src/picker/data/emojis_people_body.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_smileys_emotion.csv` & `rofimoji-6.3.1/src/picker/data/emojis_smileys_emotion.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_symbols.csv` & `rofimoji-6.3.1/src/picker/data/emojis_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emojis_travel_places.csv` & `rofimoji-6.3.1/src/picker/data/emojis_travel_places.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/emoticons.csv` & `rofimoji-6.3.1/src/picker/data/emoticons.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/enclosed_alphanumeric_supplement.csv` & `rofimoji-6.3.1/src/picker/data/enclosed_alphanumeric_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/enclosed_alphanumerics.csv` & `rofimoji-6.3.1/src/picker/data/enclosed_alphanumerics.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/enclosed_cjk_letters_and_months.csv` & `rofimoji-6.3.1/src/picker/data/enclosed_cjk_letters_and_months.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/enclosed_ideographic_supplement.csv` & `rofimoji-6.3.1/src/picker/data/enclosed_ideographic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ethiopic.csv` & `rofimoji-6.3.1/src/picker/data/ethiopic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ethiopic_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/ethiopic_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ethiopic_extended-b.csv` & `rofimoji-6.3.1/src/picker/data/ethiopic_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ethiopic_extended.csv` & `rofimoji-6.3.1/src/picker/data/ethiopic_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ethiopic_supplement.csv` & `rofimoji-6.3.1/src/picker/data/ethiopic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/fontawesome6.csv` & `rofimoji-6.3.1/src/picker/data/fontawesome6.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/general_punctuation.csv` & `rofimoji-6.3.1/src/picker/data/general_punctuation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/geometric_shapes.csv` & `rofimoji-6.3.1/src/picker/data/geometric_shapes.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/geometric_shapes_extended.csv` & `rofimoji-6.3.1/src/picker/data/geometric_shapes_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/georgian.csv` & `rofimoji-6.3.1/src/picker/data/georgian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/georgian_extended.csv` & `rofimoji-6.3.1/src/picker/data/georgian_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/georgian_supplement.csv` & `rofimoji-6.3.1/src/picker/data/georgian_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/gitmoji.csv` & `rofimoji-6.3.1/src/picker/data/gitmoji.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/glagolitic.csv` & `rofimoji-6.3.1/src/picker/data/glagolitic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/glagolitic_supplement.csv` & `rofimoji-6.3.1/src/picker/data/glagolitic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/gothic.csv` & `rofimoji-6.3.1/src/picker/data/gothic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/grantha.csv` & `rofimoji-6.3.1/src/picker/data/grantha.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/greek_and_coptic.csv` & `rofimoji-6.3.1/src/picker/data/greek_and_coptic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/greek_extended.csv` & `rofimoji-6.3.1/src/picker/data/greek_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/gujarati.csv` & `rofimoji-6.3.1/src/picker/data/gujarati.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/gunjala_gondi.csv` & `rofimoji-6.3.1/src/picker/data/gunjala_gondi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/gurmukhi.csv` & `rofimoji-6.3.1/src/picker/data/gurmukhi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/halfwidth_and_fullwidth_forms.csv` & `rofimoji-6.3.1/src/picker/data/halfwidth_and_fullwidth_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hangul_compatibility_jamo.csv` & `rofimoji-6.3.1/src/picker/data/hangul_compatibility_jamo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hangul_jamo.csv` & `rofimoji-6.3.1/src/picker/data/hangul_jamo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hangul_jamo_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/hangul_jamo_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hangul_jamo_extended-b.csv` & `rofimoji-6.3.1/src/picker/data/hangul_jamo_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hanifi_rohingya.csv` & `rofimoji-6.3.1/src/picker/data/hanifi_rohingya.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hanunoo.csv` & `rofimoji-6.3.1/src/picker/data/hanunoo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hatran.csv` & `rofimoji-6.3.1/src/picker/data/hatran.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hebrew.csv` & `rofimoji-6.3.1/src/picker/data/hebrew.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/hiragana.csv` & `rofimoji-6.3.1/src/picker/data/hiragana.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ideographic_description_characters.csv` & `rofimoji-6.3.1/src/picker/data/ideographic_description_characters.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/imperial_aramaic.csv` & `rofimoji-6.3.1/src/picker/data/imperial_aramaic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/indic_siyaq_numbers.csv` & `rofimoji-6.3.1/src/picker/data/indic_siyaq_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/inscriptional_pahlavi.csv` & `rofimoji-6.3.1/src/picker/data/inscriptional_pahlavi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/inscriptional_parthian.csv` & `rofimoji-6.3.1/src/picker/data/inscriptional_parthian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ipa_extensions.csv` & `rofimoji-6.3.1/src/picker/data/ipa_extensions.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/javanese.csv` & `rofimoji-6.3.1/src/picker/data/javanese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kaithi.csv` & `rofimoji-6.3.1/src/picker/data/kaithi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kaktovik_numerals.csv` & `rofimoji-6.3.1/src/picker/data/kaktovik_numerals.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kana_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/kana_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kana_extended-b.csv` & `rofimoji-6.3.1/src/picker/data/kana_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kana_supplement.csv` & `rofimoji-6.3.1/src/picker/data/kana_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kanbun.csv` & `rofimoji-6.3.1/src/picker/data/kanbun.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kangxi_radicals.csv` & `rofimoji-6.3.1/src/picker/data/kangxi_radicals.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kannada.csv` & `rofimoji-6.3.1/src/picker/data/kannada.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kaomoji.csv` & `rofimoji-6.3.1/src/picker/data/kaomoji.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/katakana.csv` & `rofimoji-6.3.1/src/picker/data/katakana.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kawi.csv` & `rofimoji-6.3.1/src/picker/data/kawi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kayah_li.csv` & `rofimoji-6.3.1/src/picker/data/kayah_li.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/kharoshthi.csv` & `rofimoji-6.3.1/src/picker/data/kharoshthi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/khitan_small_script.csv` & `rofimoji-6.3.1/src/picker/data/khitan_small_script.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/khmer.csv` & `rofimoji-6.3.1/src/picker/data/khmer.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/khmer_symbols.csv` & `rofimoji-6.3.1/src/picker/data/khmer_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/khojki.csv` & `rofimoji-6.3.1/src/picker/data/khojki.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/khudawadi.csv` & `rofimoji-6.3.1/src/picker/data/khudawadi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/lao.csv` & `rofimoji-6.3.1/src/picker/data/lao.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin-1_supplement.csv` & `rofimoji-6.3.1/src/picker/data/latin-1_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/latin_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin_extended-b.csv` & `rofimoji-6.3.1/src/picker/data/latin_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin_extended-c.csv` & `rofimoji-6.3.1/src/picker/data/latin_extended-c.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin_extended-d.csv` & `rofimoji-6.3.1/src/picker/data/latin_extended-d.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin_extended-e.csv` & `rofimoji-6.3.1/src/picker/data/latin_extended-e.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin_extended-f.csv` & `rofimoji-6.3.1/src/picker/data/latin_extended-f.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin_extended-g.csv` & `rofimoji-6.3.1/src/picker/data/latin_extended-g.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/latin_extended_additional.csv` & `rofimoji-6.3.1/src/picker/data/latin_extended_additional.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/lepcha.csv` & `rofimoji-6.3.1/src/picker/data/lepcha.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/letterlike_symbols.csv` & `rofimoji-6.3.1/src/picker/data/letterlike_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/limbu.csv` & `rofimoji-6.3.1/src/picker/data/limbu.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/linear_a.csv` & `rofimoji-6.3.1/src/picker/data/linear_a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/linear_b_ideograms.csv` & `rofimoji-6.3.1/src/picker/data/linear_b_ideograms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/linear_b_syllabary.csv` & `rofimoji-6.3.1/src/picker/data/linear_b_syllabary.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/lisu.csv` & `rofimoji-6.3.1/src/picker/data/lisu.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/lycian.csv` & `rofimoji-6.3.1/src/picker/data/lycian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/lydian.csv` & `rofimoji-6.3.1/src/picker/data/lydian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mahajani.csv` & `rofimoji-6.3.1/src/picker/data/mahajani.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mahjong_tiles.csv` & `rofimoji-6.3.1/src/picker/data/mahjong_tiles.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/makasar.csv` & `rofimoji-6.3.1/src/picker/data/makasar.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/malayalam.csv` & `rofimoji-6.3.1/src/picker/data/malayalam.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mandaic.csv` & `rofimoji-6.3.1/src/picker/data/mandaic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/manichaean.csv` & `rofimoji-6.3.1/src/picker/data/manichaean.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/marchen.csv` & `rofimoji-6.3.1/src/picker/data/marchen.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/masaram_gondi.csv` & `rofimoji-6.3.1/src/picker/data/masaram_gondi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/math.csv` & `rofimoji-6.3.1/src/picker/data/math.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mathematical_alphanumeric_symbols.csv` & `rofimoji-6.3.1/src/picker/data/mathematical_alphanumeric_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mathematical_operators.csv` & `rofimoji-6.3.1/src/picker/data/mathematical_operators.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/medefaidrin.csv` & `rofimoji-6.3.1/src/picker/data/medefaidrin.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/meetei_mayek.csv` & `rofimoji-6.3.1/src/picker/data/meetei_mayek.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/meetei_mayek_extensions.csv` & `rofimoji-6.3.1/src/picker/data/meetei_mayek_extensions.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mende_kikakui.csv` & `rofimoji-6.3.1/src/picker/data/mende_kikakui.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/meroitic_cursive.csv` & `rofimoji-6.3.1/src/picker/data/meroitic_cursive.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/meroitic_hieroglyphs.csv` & `rofimoji-6.3.1/src/picker/data/meroitic_hieroglyphs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/miao.csv` & `rofimoji-6.3.1/src/picker/data/miao.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/miscellaneous_mathematical_symbols-a.csv` & `rofimoji-6.3.1/src/picker/data/miscellaneous_mathematical_symbols-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/miscellaneous_mathematical_symbols-b.csv` & `rofimoji-6.3.1/src/picker/data/miscellaneous_mathematical_symbols-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/miscellaneous_symbols.csv` & `rofimoji-6.3.1/src/picker/data/miscellaneous_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/miscellaneous_symbols_and_arrows.csv` & `rofimoji-6.3.1/src/picker/data/miscellaneous_symbols_and_arrows.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/miscellaneous_symbols_and_pictographs.csv` & `rofimoji-6.3.1/src/picker/data/miscellaneous_symbols_and_pictographs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/miscellaneous_technical.csv` & `rofimoji-6.3.1/src/picker/data/miscellaneous_technical.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/modi.csv` & `rofimoji-6.3.1/src/picker/data/modi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/modifier_tone_letters.csv` & `rofimoji-6.3.1/src/picker/data/modifier_tone_letters.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mongolian.csv` & `rofimoji-6.3.1/src/picker/data/mongolian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mongolian_supplement.csv` & `rofimoji-6.3.1/src/picker/data/mongolian_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/mro.csv` & `rofimoji-6.3.1/src/picker/data/mro.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/multani.csv` & `rofimoji-6.3.1/src/picker/data/multani.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/musical_symbols.csv` & `rofimoji-6.3.1/src/picker/data/musical_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/myanmar.csv` & `rofimoji-6.3.1/src/picker/data/myanmar.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/myanmar_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/myanmar_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/myanmar_extended-b.csv` & `rofimoji-6.3.1/src/picker/data/myanmar_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/nabataean.csv` & `rofimoji-6.3.1/src/picker/data/nabataean.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/nag_mundari.csv` & `rofimoji-6.3.1/src/picker/data/nag_mundari.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/nandinagari.csv` & `rofimoji-6.3.1/src/picker/data/nandinagari.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/nerd_font.csv` & `rofimoji-6.3.1/src/picker/data/nerd_font.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/new_tai_lue.csv` & `rofimoji-6.3.1/src/picker/data/new_tai_lue.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/newa.csv` & `rofimoji-6.3.1/src/picker/data/newa.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/nko.csv` & `rofimoji-6.3.1/src/picker/data/nko.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/number_forms.csv` & `rofimoji-6.3.1/src/picker/data/number_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/nushu.csv` & `rofimoji-6.3.1/src/picker/data/nushu.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/nyiakeng_puachue_hmong.csv` & `rofimoji-6.3.1/src/picker/data/nyiakeng_puachue_hmong.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ogham.csv` & `rofimoji-6.3.1/src/picker/data/ogham.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ol_chiki.csv` & `rofimoji-6.3.1/src/picker/data/ol_chiki.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_hungarian.csv` & `rofimoji-6.3.1/src/picker/data/old_hungarian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_italic.csv` & `rofimoji-6.3.1/src/picker/data/old_italic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_north_arabian.csv` & `rofimoji-6.3.1/src/picker/data/old_north_arabian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_permic.csv` & `rofimoji-6.3.1/src/picker/data/old_permic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_persian.csv` & `rofimoji-6.3.1/src/picker/data/old_persian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_sogdian.csv` & `rofimoji-6.3.1/src/picker/data/old_sogdian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_south_arabian.csv` & `rofimoji-6.3.1/src/picker/data/old_south_arabian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_turkic.csv` & `rofimoji-6.3.1/src/picker/data/old_turkic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/old_uyghur.csv` & `rofimoji-6.3.1/src/picker/data/old_uyghur.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/oriya.csv` & `rofimoji-6.3.1/src/picker/data/oriya.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ornamental_dingbats.csv` & `rofimoji-6.3.1/src/picker/data/ornamental_dingbats.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/osage.csv` & `rofimoji-6.3.1/src/picker/data/osage.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/osmanya.csv` & `rofimoji-6.3.1/src/picker/data/osmanya.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ottoman_siyaq_numbers.csv` & `rofimoji-6.3.1/src/picker/data/ottoman_siyaq_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/pahawh_hmong.csv` & `rofimoji-6.3.1/src/picker/data/pahawh_hmong.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/palmyrene.csv` & `rofimoji-6.3.1/src/picker/data/palmyrene.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/pau_cin_hau.csv` & `rofimoji-6.3.1/src/picker/data/pau_cin_hau.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/phags-pa.csv` & `rofimoji-6.3.1/src/picker/data/phags-pa.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/phaistos_disc.csv` & `rofimoji-6.3.1/src/picker/data/phaistos_disc.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/phoenician.csv` & `rofimoji-6.3.1/src/picker/data/phoenician.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/phonetic_extensions.csv` & `rofimoji-6.3.1/src/picker/data/phonetic_extensions.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/phonetic_extensions_supplement.csv` & `rofimoji-6.3.1/src/picker/data/phonetic_extensions_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/playing_cards.csv` & `rofimoji-6.3.1/src/picker/data/playing_cards.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/psalter_pahlavi.csv` & `rofimoji-6.3.1/src/picker/data/psalter_pahlavi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/rejang.csv` & `rofimoji-6.3.1/src/picker/data/rejang.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/rumi_numeral_symbols.csv` & `rofimoji-6.3.1/src/picker/data/rumi_numeral_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/runic.csv` & `rofimoji-6.3.1/src/picker/data/runic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/samaritan.csv` & `rofimoji-6.3.1/src/picker/data/samaritan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/saurashtra.csv` & `rofimoji-6.3.1/src/picker/data/saurashtra.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/sharada.csv` & `rofimoji-6.3.1/src/picker/data/sharada.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/shavian.csv` & `rofimoji-6.3.1/src/picker/data/shavian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/siddham.csv` & `rofimoji-6.3.1/src/picker/data/siddham.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/sinhala.csv` & `rofimoji-6.3.1/src/picker/data/sinhala.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/sinhala_archaic_numbers.csv` & `rofimoji-6.3.1/src/picker/data/sinhala_archaic_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/small_form_variants.csv` & `rofimoji-6.3.1/src/picker/data/small_form_variants.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/sogdian.csv` & `rofimoji-6.3.1/src/picker/data/sogdian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/sora_sompeng.csv` & `rofimoji-6.3.1/src/picker/data/sora_sompeng.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/soyombo.csv` & `rofimoji-6.3.1/src/picker/data/soyombo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/spacing_modifier_letters.csv` & `rofimoji-6.3.1/src/picker/data/spacing_modifier_letters.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/sundanese.csv` & `rofimoji-6.3.1/src/picker/data/sundanese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/superscripts_and_subscripts.csv` & `rofimoji-6.3.1/src/picker/data/superscripts_and_subscripts.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/supplemental_arrows-a.csv` & `rofimoji-6.3.1/src/picker/data/supplemental_arrows-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/supplemental_arrows-b.csv` & `rofimoji-6.3.1/src/picker/data/supplemental_arrows-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/supplemental_arrows-c.csv` & `rofimoji-6.3.1/src/picker/data/supplemental_arrows-c.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/supplemental_mathematical_operators.csv` & `rofimoji-6.3.1/src/picker/data/supplemental_mathematical_operators.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/supplemental_punctuation.csv` & `rofimoji-6.3.1/src/picker/data/supplemental_punctuation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/supplemental_symbols_and_pictographs.csv` & `rofimoji-6.3.1/src/picker/data/supplemental_symbols_and_pictographs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/sutton_signwriting.csv` & `rofimoji-6.3.1/src/picker/data/sutton_signwriting.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/syloti_nagri.csv` & `rofimoji-6.3.1/src/picker/data/syloti_nagri.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/symbols_and_pictographs_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/symbols_and_pictographs_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/symbols_for_legacy_computing.csv` & `rofimoji-6.3.1/src/picker/data/symbols_for_legacy_computing.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/syriac.csv` & `rofimoji-6.3.1/src/picker/data/syriac.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tagalog.csv` & `rofimoji-6.3.1/src/picker/data/tagalog.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tags.csv` & `rofimoji-6.3.1/src/picker/data/tags.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tai_le.csv` & `rofimoji-6.3.1/src/picker/data/tai_le.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tai_tham.csv` & `rofimoji-6.3.1/src/picker/data/tai_tham.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tai_viet.csv` & `rofimoji-6.3.1/src/picker/data/tai_viet.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tai_xuan_jing_symbols.csv` & `rofimoji-6.3.1/src/picker/data/tai_xuan_jing_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/takri.csv` & `rofimoji-6.3.1/src/picker/data/takri.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tamil.csv` & `rofimoji-6.3.1/src/picker/data/tamil.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tamil_supplement.csv` & `rofimoji-6.3.1/src/picker/data/tamil_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tangsa.csv` & `rofimoji-6.3.1/src/picker/data/tangsa.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tangut_components.csv` & `rofimoji-6.3.1/src/picker/data/tangut_components.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/telugu.csv` & `rofimoji-6.3.1/src/picker/data/telugu.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/thaana.csv` & `rofimoji-6.3.1/src/picker/data/thaana.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/thai.csv` & `rofimoji-6.3.1/src/picker/data/thai.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tibetan.csv` & `rofimoji-6.3.1/src/picker/data/tibetan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tifinagh.csv` & `rofimoji-6.3.1/src/picker/data/tifinagh.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/tirhuta.csv` & `rofimoji-6.3.1/src/picker/data/tirhuta.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/toto.csv` & `rofimoji-6.3.1/src/picker/data/toto.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/transport_and_map_symbols.csv` & `rofimoji-6.3.1/src/picker/data/transport_and_map_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/ugaritic.csv` & `rofimoji-6.3.1/src/picker/data/ugaritic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics.csv` & `rofimoji-6.3.1/src/picker/data/unified_canadian_aboriginal_syllabics.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended-a.csv` & `rofimoji-6.3.1/src/picker/data/unified_canadian_aboriginal_syllabics_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended.csv` & `rofimoji-6.3.1/src/picker/data/unified_canadian_aboriginal_syllabics_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/vai.csv` & `rofimoji-6.3.1/src/picker/data/vai.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/variation_selectors_supplement.csv` & `rofimoji-6.3.1/src/picker/data/variation_selectors_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/vedic_extensions.csv` & `rofimoji-6.3.1/src/picker/data/vedic_extensions.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/vertical_forms.csv` & `rofimoji-6.3.1/src/picker/data/vertical_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/vithkuqi.csv` & `rofimoji-6.3.1/src/picker/data/vithkuqi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/wancho.csv` & `rofimoji-6.3.1/src/picker/data/wancho.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/warang_citi.csv` & `rofimoji-6.3.1/src/picker/data/warang_citi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/yezidi.csv` & `rofimoji-6.3.1/src/picker/data/yezidi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/yi_radicals.csv` & `rofimoji-6.3.1/src/picker/data/yi_radicals.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/yi_syllables.csv` & `rofimoji-6.3.1/src/picker/data/yi_syllables.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/yijing_hexagram_symbols.csv` & `rofimoji-6.3.1/src/picker/data/yijing_hexagram_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/zanabazar_square.csv` & `rofimoji-6.3.1/src/picker/data/zanabazar_square.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/data/znamenny_musical_notation.csv` & `rofimoji-6.3.1/src/picker/data/znamenny_musical_notation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/docs/rofimoji.1` & `rofimoji-6.3.1/src/picker/docs/rofimoji.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-.\" Automatically generated by Pandoc 3.1.12.2
+.\" Automatically generated by Pandoc 3.1.13
 .\"
-.TH "ROFIMOJI" "1" "May 01, 2024" "Version 6.3.0" "Rofi Third\-party Add\-on Documentation"
+.TH "ROFIMOJI" "1" "May 11, 2024" "Version 6.3.1" "Rofi Third\-party Add\-on Documentation"
 .SH NAME
 \f[B]rofimoji\f[R] \- An emoji and general character picker for rofi and
 rofi\-likes
 .SH SYNOPSIS
 .PP
 \f[B]rofimoji\f[R] [\f[B]\-h\f[R]] [\f[B]\-\-version\f[R]]
 [\f[B]\-\-action\f[R]
```

### Comparing `rofimoji-6.3.0/src/picker/docs/rofimoji.1.md` & `rofimoji-6.3.1/src/picker/docs/rofimoji.1.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% ROFIMOJI(1) Version 6.3.0 | Rofi Third-party Add-on Documentation
+% ROFIMOJI(1) Version 6.3.1 | Rofi Third-party Add-on Documentation
 % Fabian Winter
-% May 01, 2024
+% May 11, 2024
 
 # NAME
 
 
 **rofimoji** \- An emoji and general character picker for rofi and rofi-likes
 
 # SYNOPSIS
```

### Comparing `rofimoji-6.3.0/src/picker/emoji_data.py` & `rofimoji-6.3.1/src/picker/emoji_data.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/file_loader.py` & `rofimoji-6.3.1/src/picker/file_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 
     for character in frecent:
         all_characters[character] = CharacterEntry(character)
 
     for file in __resolve_all_filenames(files, use_additional):
         characters_from_file = __load_from_file(file)
         for character_entry in characters_from_file:
-            all_characters.setdefault(character_entry.character, character_entry)
+            if character_entry.character in all_characters:
+                all_characters[character_entry.character].merge(character_entry)
+            else:
+                all_characters[character_entry.character] = character_entry
 
-    return list(all_characters.values())
+    return [character for character in all_characters.values() if character.description]
 
 
 def __resolve_all_filenames(file_names: List[str], use_additional: bool) -> List[Path]:
     resolved_file_names = []
     for file_name in file_names:
         resolved_file_names += __resolve_filename(file_name, use_additional)
```

### Comparing `rofimoji-6.3.0/src/picker/frecent.py` & `rofimoji-6.3.1/src/picker/frecent.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/mode.py` & `rofimoji-6.3.1/src/picker/mode.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/models.py` & `rofimoji-6.3.1/src/picker/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,22 +34,25 @@
 class Shortcut:
     index: int
 
 
 @dataclass
 class CharacterEntry:
     character: str
-    description: str
+    description: str | None
 
     def __init__(self, character: str, description: str | None = None):
         self.character = character
-        self.description = description if description else ""
+        self.description = description
 
     def merge(self, other: "CharacterEntry"):
+        if self == other:
+            return self
+
         if self.character != other.character:
             raise Exception("Cannot merge different characters")
 
-        if len(other.description) > 0:
-            if len(self.description) > 0:
+        if other.description:
+            if self.description:
                 self.description = f"{self.description}, {other.description}"
             else:
                 self.description = other.description
```

### Comparing `rofimoji-6.3.0/src/picker/paths.py` & `rofimoji-6.3.1/src/picker/paths.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/recent.py` & `rofimoji-6.3.1/src/picker/recent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 from typing import List
 
 from .paths import *
 
 
 def load_recent_characters(max_recent: int, files: List[str]) -> List[str]:
     try:
@@ -41,8 +42,8 @@
         except FileNotFoundError:
             pass
 
     new_file_name.rename(old_file_name)
 
 
 def __filename_for(files: List[str]) -> Path:
-    return recents_file_location / "-".join(files)
+    return recents_file_location / hashlib.sha256(b"\0".join(f.encode() for f in sorted(files))).hexdigest()
```

### Comparing `rofimoji-6.3.0/src/picker/selector/bemenu.py` & `rofimoji-6.3.1/src/picker/selector/bemenu.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/selector/dmenu.py` & `rofimoji-6.3.1/src/picker/selector/dmenu.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/selector/fuzzel.py` & `rofimoji-6.3.1/src/picker/selector/fuzzel.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/selector/rofi.py` & `rofimoji-6.3.1/src/picker/selector/rofi.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/selector/selector.py` & `rofimoji-6.3.1/src/picker/selector/selector.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/selector/tofi.py` & `rofimoji-6.3.1/src/picker/selector/tofi.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/selector/wmenu.py` & `rofimoji-6.3.1/src/picker/selector/wmenu.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/selector/wofi.py` & `rofimoji-6.3.1/src/picker/selector/wofi.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/standalone.py` & `rofimoji-6.3.1/src/picker/standalone.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/typer/noop.py` & `rofimoji-6.3.1/src/picker/typer/noop.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/typer/typer.py` & `rofimoji-6.3.1/src/picker/typer/typer.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/typer/wtype.py` & `rofimoji-6.3.1/src/picker/typer/wtype.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/src/picker/typer/xdotool.py` & `rofimoji-6.3.1/src/picker/typer/xdotool.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.3.0/PKG-INFO` & `rofimoji-6.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rofimoji
-Version: 6.3.0
+Version: 6.3.1
 Summary: Simple character picker using rofi
 Home-page: https://github.com/fdw/rofimoji
 License: MIT
 Author: Fabian Winter
 Author-email: 5821180+fdw@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

