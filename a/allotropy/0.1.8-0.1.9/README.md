# Comparing `tmp/allotropy-0.1.8.tar.gz` & `tmp/allotropy-0.1.9.tar.gz`

## Comparing `allotropy-0.1.8.tar` & `allotropy-0.1.9.tar`

### file list

```diff
@@ -1,262 +1,268 @@
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 allotropy-0.1.8/.flake8
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 allotropy-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 allotropy-0.1.8/CODEOWNERS
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 allotropy-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 allotropy-0.1.8/GOVERNANCE.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 allotropy-0.1.8/mypy.ini
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 allotropy-0.1.8/ruff.toml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 allotropy-0.1.8/.idea/.gitignore
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 allotropy-0.1.8/.idea/allotropy.iml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 allotropy-0.1.8/.idea/misc.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 allotropy-0.1.8/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 allotropy-0.1.8/.idea/vcs.xml
--rw-r--r--   0        0        0    20951 2020-02-02 00:00:00.000000 allotropy-0.1.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 allotropy-0.1.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 allotropy-0.1.8/.vscode/settings.json
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 allotropy-0.1.8/scripts/generate_schemas.py
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 allotropy-0.1.8/scripts/pre-push-hook
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/constants.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parser_factory.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/py.typed
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/to_allotrope.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/__init__.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/allotrope.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/__init__.py
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/cell_counting_benchling_2023_09_cell_counting.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/cell_culture_analyzer_benchling_2023_09_cell_culture_analyzer.py
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/fluorescence_benchling_2023_09_fluorescence.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/liquid_chromatography_rec_2023_03_liquid_chromatography.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/luminescence_benchling_2023_09_luminescence.py
--rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/pcr_benchling_2023_09_dpcr.py
--rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/pcr_benchling_2023_09_qpcr.py
--rw-r--r--   0        0        0    21597 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/plate_reader_rec_2023_09_plate_reader.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/ultraviolet_absorbance_benchling_2023_09_ultraviolet_absorbance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/shared/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/shared/components/__init__.py
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/shared/components/liquid_chromatography.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/shared/components/plate_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/shared/definitions/__init__.py
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/shared/definitions/custom.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/shared/definitions/definitions.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/models/shared/definitions/units.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schema_parser/__init__.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schema_parser/generate_schemas.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schema_parser/model_class_editor.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schema_parser/schema_model.py
--rw-r--r--   0        0        0    24956 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/cell-counting/BENCHLING/2023/09/cell-counting.json
--rw-r--r--   0        0        0    15395 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/cell-culture-analyzer/BENCHLING/2023/09/cell-culture-analyzer.json
--rw-r--r--   0        0        0    17858 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/fluorescence/BENCHLING/2023/09/fluorescence.json
--rw-r--r--   0        0        0    63509 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/liquid-chromatography/REC/2023/03/liquid-chromatography.json
--rw-r--r--   0        0        0    17296 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/luminescence/BENCHLING/2023/09/luminescence.json
--rw-r--r--   0        0        0    29955 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/pcr/BENCHLING/2023/09/dpcr.json
--rw-r--r--   0        0        0    37667 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/pcr/BENCHLING/2023/09/qpcr.json
--rw-r--r--   0        0        0    67914 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/plate-reader/REC/2023/09/plate-reader.json
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/components/liquid_chromatography.json
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/components/plate_reader.json
--rw-r--r--   0        0        0     9720 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/definitions/custom.json
--rw-r--r--   0        0        0    14875 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/definitions/definitions.json
--rw-r--r--   0        0        0     8475 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/definitions/units.json
--rw-r--r--   0        0        0    16844 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/allotrope/schemas/ultraviolet-absorbance/BENCHLING/2023/09/ultraviolet-absorbance.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/__init__.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/lines_reader.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/vendor_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/absorbance_data_point.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/absorbance_plate_data.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/agilent_gen5_parser.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/constants.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/create_plate_data.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/data_point.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/fluorescence_data_point.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/fluorescence_plate_data.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/luminescence_data_point.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/luminescence_plate_data.py
--rw-r--r--   0        0        0    14854 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/plate_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_absolute_q/__init__.py
--rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_absolute_q/appbio_absolute_q_parser.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_absolute_q/appbio_absolute_q_reader.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_absolute_q/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/__init__.py
--rw-r--r--   0        0        0    25344 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_builders.py
--rw-r--r--   0        0        0    18664 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_calculated_documents.py
--rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_parser.py
--rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_structure.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_views.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/calculated_document.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/decorators.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/referenceable.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_blu/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_blu/constants.py
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_blu/vi_cell_blu_parser.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_blu/vi_cell_blu_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_xr/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_xr/constants.py
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_xr/vi_cell_xr_parser.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_xr/vi_cell_xr_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/__init__.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/absorbance_plate_block.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/block_factory.py
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/fluorescence_plate_block.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/luminescence_plate_block.py
--rw-r--r--   0        0        0    14555 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/plate_block.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/softmax_pro_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/novabio_flex2/__init__.py
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/novabio_flex2/constants.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/novabio_flex2/novabio_flex2_parser.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/novabio_flex2/novabio_flex2_structure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/perkin_elmer_envision/__init__.py
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/perkin_elmer_envision/perkin_elmer_envision_parser.py
--rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/perkin_elmer_envision/perkin_elmer_envision_structure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/__init__.py
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/constants.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_parser.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_reader.py
--rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_structure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/utils/__init__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/utils/timestamp_parser.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 allotropy-0.1.8/src/allotropy/parsers/utils/values.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/__init__.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/allotrope_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/models/shared/__init__.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/models/shared/definitions_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/schema_parser/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/schema_parser/generate_schemas_test.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/schema_parser/model_class_editor_test.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/allotrope/schema_parser/schema_model_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/__init__.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/lines_reader_test.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/__init__.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/to_allotrope_test.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/garbage.txt
--rw-r--r--   0        0        0   236555 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_pathlength_correct_singleplate.json
--rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_pathlength_correct_singleplate.txt
--rw-r--r--   0        0        0   370326 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_multiplate.json
--rw-r--r--   0        0        0    26342 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_multiplate.txt
--rw-r--r--   0        0        0   123885 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate.json
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate.txt
--rw-r--r--   0        0        0   123139 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate_2.json
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate_2.txt
--rw-r--r--   0        0        0   483029 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_helper_gene_growth_curve.json
--rw-r--r--   0        0        0   123352 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_helper_gene_growth_curve.txt
--rw-r--r--   0        0        0   697333 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_multiplate.json
--rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_multiplate.txt
--rw-r--r--   0        0        0   232916 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_singleplate.json
--rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_singleplate.txt
--rw-r--r--   0        0        0   438246 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_multiplate.json
--rw-r--r--   0        0        0    16660 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_multiplate.txt
--rw-r--r--   0        0        0   146578 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_singleplate.json
--rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_singleplate.txt
--rw-r--r--   0        0        0   309799 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_multiplate.json
--rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_multiplate.txt
--rw-r--r--   0        0        0   103848 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_singleplate.json
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_singleplate.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/appbio_absolute_q_parser_test.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example01.csv
--rw-r--r--   0        0        0    58862 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example01.json
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example02.csv
--rw-r--r--   0        0        0    37735 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example02.json
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example03.csv
--rw-r--r--   0        0        0    52169 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example03.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example04.csv
--rw-r--r--   0        0        0    37735 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example04.json
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example05.csv
--rw-r--r--   0        0        0   110062 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example05.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/__init__.py
--rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/appbio_quantstudio_builders_test.py
--rw-r--r--   0        0        0   203732 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/appbio_quantstudio_data.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/appbio_quantstudio_parser_test.py
--rw-r--r--   0        0        0 10778434 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example01.json
--rw-r--r--   0        0        0  3721779 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example01.txt
--rw-r--r--   0        0        0  5542898 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example02.json
--rw-r--r--   0        0        0   734530 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example02.txt
--rw-r--r--   0        0        0  3176114 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example03.json
--rw-r--r--   0        0        0   309495 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example03.txt
--rw-r--r--   0        0        0   127208 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example04.txt
--rw-r--r--   0        0        0   233048 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example05.txt
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example06.txt
--rw-r--r--   0        0        0   290340 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example07.txt
--rw-r--r--   0        0        0   290340 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example08.txt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test01.txt
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test02.txt
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test03.txt
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test04.txt
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test05.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/__init__.py
--rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/vi_cell_blu_data.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/vi_cell_blu_parser_test.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example01.csv
--rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example01.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example02.csv
--rw-r--r--   0        0        0    19364 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example02.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/__init__.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/vi_cell_xr_parser_test.py
--rw-r--r--   0        0        0    79872 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example02_instrumentOutput.xls
--rw-r--r--   0        0        0   101834 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example03_instrumentOutput.json
--rw-r--r--   0        0        0    43008 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example03_instrumentOutput.xls
--rw-r--r--   0        0        0   546028 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example01_instrumentOutput.json
--rw-r--r--   0        0        0    30502 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example01_instrumentOutput.xlsx
--rw-r--r--   0        0        0    47237 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example04_instrumentOutput.json
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example04_instrumentOutput.xlsx
--rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example05_instrumentOutput.json
--rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example05_instrumentOutput.xlsx
--rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example06_instrumentOutput.json
--rw-r--r--   0        0        0    33709 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example06_instrumentOutput.xlsx
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/__init__.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/to_allotrope_test.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/abs_endpoint_plates.txt
--rw-r--r--   0        0        0   141758 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/expected_abs_endpoint.json
--rw-r--r--   0        0        0   315001 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/expected_fl_kinetic.json
--rw-r--r--   0        0        0   326874 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/expected_lum_spectrum.json
--rw-r--r--   0        0        0    18134 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/fl_kinetic_plates.txt
--rw-r--r--   0        0        0    31660 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/lum_spectrum_columns.txt
--rw-r--r--   0        0        0    22065 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/trf_well_scan_plates.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/novabio_flex2/__init__.py
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/novabio_flex2/novabio_flex2_data.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/novabio_flex2/novabio_flex2_parser_test.py
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/novabio_flex2/novabio_flex2_structure_test.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/novabio_flex2/testdata/SampleResults2022-06-28_142558.csv
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/novabio_flex2/testdata/SampleResults2022-06-28_142558.json
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/novabio_flex2/testdata/SampleResultsDEVICE1232021-02-18_104838.csv
--rw-r--r--   0        0        0    21901 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/novabio_flex2/testdata/SampleResultsDEVICE1232021-02-18_104838.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/__init__.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_data.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_parser_test.py
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_structure_test.py
--rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_absorbance_example01.csv
--rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01.csv
--rw-r--r--   0        0        0   216571 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01.json
--rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01_v2.json
--rw-r--r--   0        0        0    16247 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example02.csv
--rw-r--r--   0        0        0   837086 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example02.json
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example03.csv
--rw-r--r--   0        0        0   474169 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example03.json
--rw-r--r--   0        0        0    15646 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example04.csv
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_luminescence_example01.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/__init__.py
--rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_data.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_parser_test.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_reader_test.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_structure_test.py
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example01.json
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example01.txt
--rw-r--r--   0        0        0   337296 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example02.json
--rw-r--r--   0        0        0    93706 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example02.txt
--rw-r--r--   0        0        0   595846 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example03.json
--rw-r--r--   0        0        0   140886 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example03.txt
--rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example04.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example04.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/utils/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 allotropy-0.1.8/tests/parsers/utils/timestamp_parser_test.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 allotropy-0.1.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 allotropy-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 allotropy-0.1.8/README.md
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 allotropy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 allotropy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 allotropy-0.1.9/.flake8
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 allotropy-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 allotropy-0.1.9/CODEOWNERS
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 allotropy-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 allotropy-0.1.9/GOVERNANCE.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 allotropy-0.1.9/mypy.ini
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 allotropy-0.1.9/ruff.toml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 allotropy-0.1.9/.idea/.gitignore
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 allotropy-0.1.9/.idea/allotropy.iml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 allotropy-0.1.9/.idea/misc.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 allotropy-0.1.9/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 allotropy-0.1.9/.idea/vcs.xml
+-rw-r--r--   0        0        0    20951 2020-02-02 00:00:00.000000 allotropy-0.1.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 allotropy-0.1.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 allotropy-0.1.9/.vscode/settings.json
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 allotropy-0.1.9/scripts/generate_schemas.py
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 allotropy-0.1.9/scripts/pre-push-hook
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/__init__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/constants.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parser_factory.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/py.typed
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/to_allotrope.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/__init__.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/allotrope.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/__init__.py
+-rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/cell_counting_benchling_2023_09_cell_counting.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/cell_culture_analyzer_benchling_2023_09_cell_culture_analyzer.py
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/fluorescence_benchling_2023_09_fluorescence.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/liquid_chromatography_rec_2023_03_liquid_chromatography.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/luminescence_benchling_2023_09_luminescence.py
+-rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/pcr_benchling_2023_09_dpcr.py
+-rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/pcr_benchling_2023_09_qpcr.py
+-rw-r--r--   0        0        0    21665 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/plate_reader_benchling_2023_09_plate_reader.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/ultraviolet_absorbance_benchling_2023_09_ultraviolet_absorbance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/shared/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/shared/components/__init__.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/shared/components/liquid_chromatography.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/shared/components/plate_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/shared/definitions/__init__.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/shared/definitions/custom.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/shared/definitions/definitions.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/models/shared/definitions/units.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schema_parser/__init__.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schema_parser/generate_schemas.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schema_parser/model_class_editor.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schema_parser/schema_model.py
+-rw-r--r--   0        0        0    24956 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/cell-counting/BENCHLING/2023/09/cell-counting.json
+-rw-r--r--   0        0        0    15395 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/cell-culture-analyzer/BENCHLING/2023/09/cell-culture-analyzer.json
+-rw-r--r--   0        0        0    17858 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/fluorescence/BENCHLING/2023/09/fluorescence.json
+-rw-r--r--   0        0        0    63509 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/liquid-chromatography/REC/2023/03/liquid-chromatography.json
+-rw-r--r--   0        0        0    17296 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/luminescence/BENCHLING/2023/09/luminescence.json
+-rw-r--r--   0        0        0    29955 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/pcr/BENCHLING/2023/09/dpcr.json
+-rw-r--r--   0        0        0    37667 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/pcr/BENCHLING/2023/09/qpcr.json
+-rw-r--r--   0        0        0    67768 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/plate-reader/BENCHLING/2023/09/plate-reader.json
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/components/liquid_chromatography.json
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/components/plate_reader.json
+-rw-r--r--   0        0        0     9713 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/definitions/custom.json
+-rw-r--r--   0        0        0    14875 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/definitions/definitions.json
+-rw-r--r--   0        0        0     8475 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/definitions/units.json
+-rw-r--r--   0        0        0    16844 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/allotrope/schemas/ultraviolet-absorbance/BENCHLING/2023/09/ultraviolet-absorbance.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/__init__.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/lines_reader.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/vendor_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/absorbance_data_point.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/absorbance_plate_data.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/agilent_gen5_parser.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/constants.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/create_plate_data.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/data_point.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/fluorescence_data_point.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/fluorescence_plate_data.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/luminescence_data_point.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/luminescence_plate_data.py
+-rw-r--r--   0        0        0    14854 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/plate_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_absolute_q/__init__.py
+-rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_absolute_q/appbio_absolute_q_parser.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_absolute_q/appbio_absolute_q_reader.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_absolute_q/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/__init__.py
+-rw-r--r--   0        0        0    24978 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_builders.py
+-rw-r--r--   0        0        0    18664 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_calculated_documents.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_parser.py
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_structure.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_views.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/calculated_document.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/decorators.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/referenceable.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_blu/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_blu/constants.py
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_blu/vi_cell_blu_parser.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_blu/vi_cell_blu_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_xr/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_xr/constants.py
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_xr/vi_cell_xr_parser.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_xr/vi_cell_xr_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/__init__.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/absorbance_plate_block.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/block_factory.py
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/fluorescence_plate_block.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/luminescence_plate_block.py
+-rw-r--r--   0        0        0    14555 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/plate_block.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/softmax_pro_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/novabio_flex2/__init__.py
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/novabio_flex2/constants.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/novabio_flex2/novabio_flex2_parser.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/novabio_flex2/novabio_flex2_structure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/perkin_elmer_envision/__init__.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/perkin_elmer_envision/perkin_elmer_envision_parser.py
+-rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/perkin_elmer_envision/perkin_elmer_envision_structure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/__init__.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/constants.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_parser.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_reader.py
+-rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_structure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/utils/__init__.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/utils/timestamp_parser.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/parsers/utils/values.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/src/allotropy/testing/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/__init__.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/allotrope_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/models/shared/__init__.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/models/shared/definitions_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/schema_parser/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/schema_parser/generate_schemas_test.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/schema_parser/model_class_editor_test.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/allotrope/schema_parser/schema_model_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/lines_reader_test.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/__init__.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/to_allotrope_test.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/garbage.txt
+-rw-r--r--   0        0        0   236555 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_pathlength_correct_singleplate.json
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_pathlength_correct_singleplate.txt
+-rw-r--r--   0        0        0   370326 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_multiplate.json
+-rw-r--r--   0        0        0    26342 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_multiplate.txt
+-rw-r--r--   0        0        0   123885 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate.json
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate.txt
+-rw-r--r--   0        0        0   123139 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate_2.json
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate_2.txt
+-rw-r--r--   0        0        0   483029 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_helper_gene_growth_curve.json
+-rw-r--r--   0        0        0   123352 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_helper_gene_growth_curve.txt
+-rw-r--r--   0        0        0   697333 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_multiplate.json
+-rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_multiplate.txt
+-rw-r--r--   0        0        0   232916 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_singleplate.json
+-rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_singleplate.txt
+-rw-r--r--   0        0        0   438246 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_multiplate.json
+-rw-r--r--   0        0        0    16660 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_multiplate.txt
+-rw-r--r--   0        0        0   146578 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_singleplate.json
+-rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_singleplate.txt
+-rw-r--r--   0        0        0   309799 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_multiplate.json
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_multiplate.txt
+-rw-r--r--   0        0        0   103848 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_singleplate.json
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_singleplate.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/appbio_absolute_q_parser_test.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example01.csv
+-rw-r--r--   0        0        0    58862 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example01.json
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example02.csv
+-rw-r--r--   0        0        0    37735 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example02.json
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example03.csv
+-rw-r--r--   0        0        0    52169 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example03.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example04.csv
+-rw-r--r--   0        0        0    37735 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example04.json
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example05.csv
+-rw-r--r--   0        0        0   110062 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example05.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/__init__.py
+-rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/appbio_quantstudio_builders_test.py
+-rw-r--r--   0        0        0   203732 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/appbio_quantstudio_data.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/appbio_quantstudio_parser_test.py
+-rw-r--r--   0        0        0 10778434 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example01.json
+-rw-r--r--   0        0        0  3721779 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example01.txt
+-rw-r--r--   0        0        0  5542898 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example02.json
+-rw-r--r--   0        0        0   734530 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example02.txt
+-rw-r--r--   0        0        0  3176114 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example03.json
+-rw-r--r--   0        0        0   309495 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example03.txt
+-rw-r--r--   0        0        0  1333877 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example04.json
+-rw-r--r--   0        0        0   127208 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example04.txt
+-rw-r--r--   0        0        0  1740374 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example05.json
+-rw-r--r--   0        0        0   233048 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example05.txt
+-rw-r--r--   0        0        0    89399 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example06.json
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example06.txt
+-rw-r--r--   0        0        0  1803603 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example07.json
+-rw-r--r--   0        0        0   290340 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example07.txt
+-rw-r--r--   0        0        0  1803603 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example08.json
+-rw-r--r--   0        0        0   290340 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example08.txt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test01.txt
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test02.txt
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test03.txt
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test04.txt
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test05.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/__init__.py
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/vi_cell_blu_data.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/vi_cell_blu_parser_test.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example01.csv
+-rw-r--r--   0        0        0    38139 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example01.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example02.csv
+-rw-r--r--   0        0        0    19364 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example02.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/__init__.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/vi_cell_xr_parser_test.py
+-rw-r--r--   0        0        0    79872 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example02_instrumentOutput.xls
+-rw-r--r--   0        0        0   101834 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example03_instrumentOutput.json
+-rw-r--r--   0        0        0    43008 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example03_instrumentOutput.xls
+-rw-r--r--   0        0        0   546028 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example01_instrumentOutput.json
+-rw-r--r--   0        0        0    30502 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example01_instrumentOutput.xlsx
+-rw-r--r--   0        0        0    47237 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example04_instrumentOutput.json
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example04_instrumentOutput.xlsx
+-rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example05_instrumentOutput.json
+-rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example05_instrumentOutput.xlsx
+-rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example06_instrumentOutput.json
+-rw-r--r--   0        0        0    33709 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example06_instrumentOutput.xlsx
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/__init__.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/to_allotrope_test.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/abs_endpoint_plates.txt
+-rw-r--r--   0        0        0   141758 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/expected_abs_endpoint.json
+-rw-r--r--   0        0        0   315001 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/expected_fl_kinetic.json
+-rw-r--r--   0        0        0   326874 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/expected_lum_spectrum.json
+-rw-r--r--   0        0        0    18134 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/fl_kinetic_plates.txt
+-rw-r--r--   0        0        0    31660 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/lum_spectrum_columns.txt
+-rw-r--r--   0        0        0    22065 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/trf_well_scan_plates.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/novabio_flex2/__init__.py
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/novabio_flex2/novabio_flex2_data.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/novabio_flex2/novabio_flex2_parser_test.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/novabio_flex2/novabio_flex2_structure_test.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/novabio_flex2/testdata/SampleResults2022-06-28_142558.csv
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/novabio_flex2/testdata/SampleResults2022-06-28_142558.json
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/novabio_flex2/testdata/SampleResultsDEVICE1232021-02-18_104838.csv
+-rw-r--r--   0        0        0    21901 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/novabio_flex2/testdata/SampleResultsDEVICE1232021-02-18_104838.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/__init__.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_data.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_parser_test.py
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_structure_test.py
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_absorbance_example01.csv
+-rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01.csv
+-rw-r--r--   0        0        0   216571 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01.json
+-rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01_v2.json
+-rw-r--r--   0        0        0    16247 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example02.csv
+-rw-r--r--   0        0        0   837086 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example02.json
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example03.csv
+-rw-r--r--   0        0        0   474169 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example03.json
+-rw-r--r--   0        0        0    15646 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example04.csv
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_luminescence_example01.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/__init__.py
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_data.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_parser_test.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_reader_test.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_structure_test.py
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example01.json
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example01.txt
+-rw-r--r--   0        0        0   337296 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example02.json
+-rw-r--r--   0        0        0    93706 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example02.txt
+-rw-r--r--   0        0        0   595846 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example03.json
+-rw-r--r--   0        0        0   140886 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example03.txt
+-rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example04.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example04.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/utils/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 allotropy-0.1.9/tests/parsers/utils/timestamp_parser_test.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 allotropy-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 allotropy-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 allotropy-0.1.9/README.md
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 allotropy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 allotropy-0.1.9/PKG-INFO
```

### Comparing `allotropy-0.1.8/CHANGELOG.md` & `allotropy-0.1.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 ### Added
 ### Fixed
 ### Changed
 ### Deprecated
 ### Removed
 ### Security
 
+## [0.1.9] - 2023-11-03
+### Added
+- Add missing example outputs for AppBio Quantstudio tests
+### Fixed
+- Update plate-reader schema to be compatible with current supported adapters and change REC -> BENCHLING
 
 ## [0.1.8] - 2023-10-30
 ### Added
 - Allow lines reader to accept or infer encoding
 ### Fixed
 - Use fuzzy=True for timestamp parsing to handle non-standard cases (e.g. mixing 24h time and AM/PM)
```

### Comparing `allotropy-0.1.8/CONTRIBUTING.md` & `allotropy-0.1.9/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - [Tell Git about your signing key](https://docs.github.com/en/authentication/managing-commit-signature-verification/telling-git-about-your-signing-key).
   - Follow up until step 5.
 
 To configure commits to be signed by default within this repo, run `git config commit.gpgsign true`.
 
 # Adding a new converter
 
-Determine if the ASM schemas you need are in [the schema folder](../src/allotropy/allotrope/schemas). We keep a copy of published ASM schemas here as well as our proposed changes that are yet to be taken up by the Allotrope Foundation. We expect this to be eventually consistent with the public ASM schemas.
+Determine if the ASM schemas you need are in [the schema folder](src/allotropy/allotrope/schemas). We keep a copy of published ASM schemas here as well as our proposed changes that are yet to be taken up by the Allotrope Foundation. We expect this to be eventually consistent with the public ASM schemas.
 
 ## If the ASM schema you need is available
 
 In this case we already have some code in the library to handle instruments of this type and you should look at those for examples of how to structure your own code. Each converter consists of two main pieces:
 1. A `Parser` class -- this implements [`VendorParser`](src/allotropy/parsers/vendor_parser.py) and does most of the work converting the instrument data to ASM.
 2. Either:
   - A `Structure` file that the `Parser` uses to build an in memory representation of the instrument data that can be serialized to ASM.
```

### Comparing `allotropy-0.1.8/GOVERNANCE.md` & `allotropy-0.1.9/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/.idea/allotropy.iml` & `allotropy-0.1.9/.idea/allotropy.iml`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/.idea/inspectionProfiles/Project_Default.xml` & `allotropy-0.1.9/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/.vscode/settings.json` & `allotropy-0.1.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parser_factory.py` & `allotropy-0.1.9/src/allotropy/parser_factory.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/to_allotrope.py` & `allotropy-0.1.9/src/allotropy/to_allotrope.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/allotrope.py` & `allotropy-0.1.9/src/allotropy/allotrope/allotrope.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 class AllotropyError(Exception):
     pass
 
 
 # TODO: gather exceptions when parsing models from schema and publish them in model
 SPECIAL_KEYS = {
     "manifest": "$asm.manifest",
+    "field_asm_manifest": "$asm.manifest",
     "cube_structure": "cube-structure",
     "field_componentDatatype": "@componentDatatype",
     "field_asm_fill_value": "$asm.fill-value",
     "field_type": "@type",
     "field_index": "@index",
     "scan_position_setting__plate_reader_": "scan position setting (plate reader)",
     "detector_distance_setting__plate_reader_": "detector distance setting (plate reader)",
```

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas.py` & `allotropy-0.1.9/src/allotropy/allotrope/schemas.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/cell_counting_benchling_2023_09_cell_counting.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/cell_counting_benchling_2023_09_cell_counting.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/cell_culture_analyzer_benchling_2023_09_cell_culture_analyzer.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/cell_culture_analyzer_benchling_2023_09_cell_culture_analyzer.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/fluorescence_benchling_2023_09_fluorescence.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/fluorescence_benchling_2023_09_fluorescence.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/liquid_chromatography_rec_2023_03_liquid_chromatography.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/liquid_chromatography_rec_2023_03_liquid_chromatography.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/luminescence_benchling_2023_09_luminescence.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/luminescence_benchling_2023_09_luminescence.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/pcr_benchling_2023_09_dpcr.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/pcr_benchling_2023_09_dpcr.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/pcr_benchling_2023_09_qpcr.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/pcr_benchling_2023_09_qpcr.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/plate_reader_rec_2023_09_plate_reader.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/plate_reader_benchling_2023_09_plate_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  plate-reader.json
-#   timestamp: 2023-10-24T10:28:46+00:00
+#   timestamp: 2023-11-02T19:59:01+00:00
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Optional, Union
 
@@ -317,17 +317,17 @@
     equipment_serial_number: Optional[TStringValue] = None
     firmware_version: Optional[TStringValue] = None
     field_index: Optional[int] = None
 
 
 @dataclass
 class DeviceSystemDocument:
-    asset_management_identifier: TStringValue
     device_identifier: TStringValue
     model_number: TStringValue
+    asset_management_identifier: Optional[TStringValue] = None
     description: Optional[Any] = None
     brand_name: Optional[TStringValue] = None
     product_manufacturer: Optional[TStringValue] = None
     equipment_serial_number: Optional[TStringValue] = None
     firmware_version: Optional[TStringValue] = None
     device_document: Optional[list[DeviceDocumentItem]] = None
 
@@ -476,63 +476,63 @@
 
 
 @dataclass
 class FluorescencePointDetectionMeasurementDocumentItems:
     measurement_identifier: TStringValue
     device_control_aggregate_document: FluorescencePointDetectionDeviceControlAggregateDocument
     sample_document: SampleDocument
-    compartment_temperature: TQuantityValueDegreeCelsius
     fluorescence: TRelativeFluorescenceUnit
     measurement_time: Optional[TDateTimeStampValue] = None
     detection_type: Optional[TStringValue] = None
     processed_data_aggregate_document: Optional[
         ProcessedDataAggregateDocumentModel
     ] = None
     calculated_data_aggregate_document: Optional[
         CalculatedDataAggregateDocumentModel
     ] = None
     statistics_aggregate_document: Optional[StatisticsAggregateDocument] = None
+    compartment_temperature: Optional[TQuantityValueDegreeCelsius] = None
     mass_concentration: Optional[TQuantityValuePicogramPerMilliliter] = None
 
 
 @dataclass
 class LuminescencePointDetectionMeasurementDocumentItems:
     measurement_identifier: TStringValue
     device_control_aggregate_document: LuminescencePointDetectionDeviceControlAggregateDocument
     sample_document: SampleDocument
-    compartment_temperature: TQuantityValueDegreeCelsius
     luminescence: TRelativeLightUnit
     measurement_time: Optional[TDateTimeStampValue] = None
     detection_type: Optional[TStringValue] = None
     processed_data_aggregate_document: Optional[
         ProcessedDataAggregateDocumentModel
     ] = None
     calculated_data_aggregate_document: Optional[
         CalculatedDataAggregateDocumentModel
     ] = None
     statistics_aggregate_document: Optional[StatisticsAggregateDocument] = None
+    compartment_temperature: Optional[TQuantityValueDegreeCelsius] = None
     mass_concentration: Optional[TQuantityValuePicogramPerMilliliter] = None
 
 
 @dataclass
 class UltravioletAbsorbancePointDetectionMeasurementDocumentItems:
     measurement_identifier: TStringValue
     device_control_aggregate_document: UltravioletAbsorbancePointDetectionDeviceControlAggregateDocument
     sample_document: SampleDocument
-    compartment_temperature: TQuantityValueDegreeCelsius
     absorbance: TQuantityValueMilliAbsorbanceUnit
     measurement_time: Optional[TDateTimeStampValue] = None
     detection_type: Optional[TStringValue] = None
     processed_data_aggregate_document: Optional[
         ProcessedDataAggregateDocumentModel
     ] = None
     calculated_data_aggregate_document: Optional[
         CalculatedDataAggregateDocumentModel
     ] = None
     statistics_aggregate_document: Optional[StatisticsAggregateDocument] = None
+    compartment_temperature: Optional[TQuantityValueDegreeCelsius] = None
     mass_concentration: Optional[TQuantityValuePicogramPerMilliliter] = None
 
 
 @dataclass
 class MeasurementAggregateDocument:
     measurement_time: TDateTimeStampValue
     plate_well_count: TQuantityValueNumber
```

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/ultraviolet_absorbance_benchling_2023_09_ultraviolet_absorbance.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/ultraviolet_absorbance_benchling_2023_09_ultraviolet_absorbance.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/shared/components/liquid_chromatography.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/shared/components/liquid_chromatography.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/shared/components/plate_reader.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/shared/components/plate_reader.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/shared/definitions/custom.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/shared/definitions/custom.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/shared/definitions/definitions.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/shared/definitions/definitions.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/models/shared/definitions/units.py` & `allotropy-0.1.9/src/allotropy/allotrope/models/shared/definitions/units.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schema_parser/generate_schemas.py` & `allotropy-0.1.9/src/allotropy/allotrope/schema_parser/generate_schemas.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schema_parser/model_class_editor.py` & `allotropy-0.1.9/src/allotropy/allotrope/schema_parser/model_class_editor.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schema_parser/schema_model.py` & `allotropy-0.1.9/src/allotropy/allotrope/schema_parser/schema_model.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/cell-counting/BENCHLING/2023/09/cell-counting.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/cell-counting/BENCHLING/2023/09/cell-counting.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/cell-culture-analyzer/BENCHLING/2023/09/cell-culture-analyzer.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/cell-culture-analyzer/BENCHLING/2023/09/cell-culture-analyzer.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/fluorescence/BENCHLING/2023/09/fluorescence.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/fluorescence/BENCHLING/2023/09/fluorescence.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/liquid-chromatography/REC/2023/03/liquid-chromatography.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/liquid-chromatography/REC/2023/03/liquid-chromatography.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/luminescence/BENCHLING/2023/09/luminescence.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/luminescence/BENCHLING/2023/09/luminescence.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/pcr/BENCHLING/2023/09/dpcr.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/pcr/BENCHLING/2023/09/dpcr.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/pcr/BENCHLING/2023/09/qpcr.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/pcr/BENCHLING/2023/09/qpcr.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/plate-reader/REC/2023/09/plate-reader.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/plate-reader/BENCHLING/2023/09/plate-reader.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8998193627450981%*

 * *Differences: {"'$defs'": "{'ultravioletAbsorbancePointDetectionMeasurementDocumentItems': {'required': {delete: "*

 * *            "[4]}}, 'fluorescencePointDetectionMeasurementDocumentItems': {'required': {delete: "*

 * *            "[4]}}, 'luminescencePointDetectionMeasurementDocumentItems': {'required': {delete: "*

 * *            '[4]}}}',*

 * * "'$id'": "'http://purl.allotrope.org/json-schemas/adm/plate-reader/BENCHLING/2023/09/plate-reader.schema'",*

 * * "'allOf'": "{0: {'properties': {'plate reader aggregate document': {'properties': { […]*

```diff
@@ -365,16 +365,15 @@
                     "$ref": "#/$defs/statisticsAggregateDocument"
                 }
             },
             "required": [
                 "fluorescence",
                 "sample document",
                 "device control aggregate document",
-                "measurement identifier",
-                "compartment temperature"
+                "measurement identifier"
             ],
             "type": "object"
         },
         "luminescencePointDetectionDeviceControlAggregateDocument": {
             "$asm.pattern": "aggregate datum",
             "$asm.property-class": "http://purl.allotrope.org/ontologies/result#AFR_0002722",
             "properties": {
@@ -480,16 +479,15 @@
                     "$ref": "#/$defs/statisticsAggregateDocument"
                 }
             },
             "required": [
                 "luminescence",
                 "sample document",
                 "device control aggregate document",
-                "measurement identifier",
-                "compartment temperature"
+                "measurement identifier"
             ],
             "type": "object"
         },
         "manifest": {
             "$id": "http://purl.allotrope.org/json-schemas/adm/core/REC/2023/09/manifest.schema",
             "properties": {
                 "@id": {
@@ -1030,21 +1028,20 @@
                     "$ref": "#/$defs/statisticsAggregateDocument"
                 }
             },
             "required": [
                 "absorbance",
                 "sample document",
                 "device control aggregate document",
-                "measurement identifier",
-                "compartment temperature"
+                "measurement identifier"
             ],
             "type": "object"
         }
     },
-    "$id": "http://purl.allotrope.org/json-schemas/adm/plate-reader/REC/2023/09/plate-reader.schema",
+    "$id": "http://purl.allotrope.org/json-schemas/adm/plate-reader/BENCHLING/2023/09/plate-reader.schema",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "properties": {
                 "plate reader aggregate document": {
                     "$asm.pattern": "aggregate datum",
                     "$asm.property-class": "http://purl.allotrope.org/ontologies/result#AFR_0002845",
@@ -1286,15 +1283,14 @@
                                     "$asm.pattern": "value datum",
                                     "$asm.property-class": "http://purl.allotrope.org/ontologies/result#AFR_0001258",
                                     "$asm.type": "http://www.w3.org/2001/XMLSchema#string",
                                     "$ref": "#/$defs/tStringValue"
                                 }
                             },
                             "required": [
-                                "asset management identifier",
                                 "device identifier",
                                 "model number"
                             ],
                             "type": "object"
                         },
                         "plate reader document": {
                             "items": {
```

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/components/liquid_chromatography.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/components/liquid_chromatography.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/components/plate_reader.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/components/plate_reader.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/definitions/custom.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/definitions/custom.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'tRelativeLightUnit'": "{'allOf': {0: {'$ref': '#/$defs/RelativeLightUnit'}}}"}*

```diff
@@ -408,15 +408,15 @@
                 "$ref": "#/$defs/tQuantityValue"
             }
         ]
     },
     "tRelativeLightUnit": {
         "allOf": [
             {
-                "$ref": "#/$defs/RelativeFluorescenceUnit"
+                "$ref": "#/$defs/RelativeLightUnit"
             },
             {
                 "$ref": "#/$defs/tQuantityValue"
             }
         ]
     }
 }
```

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/definitions/definitions.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/definitions/definitions.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/shared/definitions/units.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/shared/definitions/units.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/allotrope/schemas/ultraviolet-absorbance/BENCHLING/2023/09/ultraviolet-absorbance.json` & `allotropy-0.1.9/src/allotropy/allotrope/schemas/ultraviolet-absorbance/BENCHLING/2023/09/ultraviolet-absorbance.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/lines_reader.py` & `allotropy-0.1.9/src/allotropy/parsers/lines_reader.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/vendor_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/vendor_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/absorbance_data_point.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/absorbance_data_point.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/absorbance_plate_data.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/absorbance_plate_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/agilent_gen5_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/agilent_gen5_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/constants.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/constants.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/create_plate_data.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/create_plate_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/data_point.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/data_point.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/fluorescence_data_point.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/fluorescence_data_point.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/fluorescence_plate_data.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/fluorescence_plate_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/luminescence_data_point.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/luminescence_data_point.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/luminescence_plate_data.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/luminescence_plate_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/agilent_gen5/plate_data.py` & `allotropy-0.1.9/src/allotropy/parsers/agilent_gen5/plate_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_absolute_q/appbio_absolute_q_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_absolute_q/appbio_absolute_q_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_absolute_q/constants.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_absolute_q/constants.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_builders.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,46 +72,36 @@
 
 
 class HeaderBuilder:
     @staticmethod
     def build(reader: LinesReader) -> Header:
         data = HeaderBuilder.get_data(reader)
 
-        device_identifier = get_str(data, "Instrument Name")
-        if device_identifier is None:
-            msg = "Unable to get device identifier"
-            raise AllotropeConversionError(msg)
-
         model_number = get_str(data, "Instrument Type")
         if model_number is None:
             msg = "Unable to get model number"
             raise AllotropeConversionError(msg)
 
-        device_serial_number = get_str(data, "Instrument Serial Number")
-        if device_serial_number is None:
-            msg = "Unable to get device serial number"
-            raise AllotropeConversionError(msg)
-
         measurement_method_identifier = get_str(data, "Quantification Cycle Method")
         if measurement_method_identifier is None:
             msg = "Unable to get measurement method identifier"
             raise AllotropeConversionError(msg)
 
         pcr_detection_chemistry = get_str(data, "Chemistry")
         if pcr_detection_chemistry is None:
             msg = "Unable to get PCR detection chemistry"
             raise AllotropeConversionError(msg)
 
         return Header(
             measurement_time=HeaderBuilder.get_measurement_time(data),
             plate_well_count=HeaderBuilder.get_plate_well_count(data),
             experiment_type=HeaderBuilder.get_experiment_type(data),
-            device_identifier=device_identifier,
+            device_identifier=get_str(data, "Instrument Name") or "NA",
             model_number=model_number,
-            device_serial_number=device_serial_number,
+            device_serial_number=get_str(data, "Instrument Serial Number") or "NA",
             measurement_method_identifier=measurement_method_identifier,
             pcr_detection_chemistry=pcr_detection_chemistry,
             passive_reference_dye_setting=get_str(data, "Passive Reference"),
             barcode=get_str(data, "Experiment Barcode"),
             analyst=get_str(data, "Experiment User Name"),
             experimental_data_identifier=get_str(data, "Experiment Name"),
         )
```

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_calculated_documents.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_calculated_documents.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_structure.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_structure.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_views.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/appbio_quantstudio_views.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/calculated_document.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/calculated_document.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/appbio_quantstudio/views.py` & `allotropy-0.1.9/src/allotropy/parsers/appbio_quantstudio/views.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_blu/vi_cell_blu_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_blu/vi_cell_blu_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_blu/vi_cell_blu_reader.py` & `allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_blu/vi_cell_blu_reader.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_xr/vi_cell_xr_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_xr/vi_cell_xr_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/beckman_vi_cell_xr/vi_cell_xr_reader.py` & `allotropy-0.1.9/src/allotropy/parsers/beckman_vi_cell_xr/vi_cell_xr_reader.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/absorbance_plate_block.py` & `allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/absorbance_plate_block.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/block_factory.py` & `allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/block_factory.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/fluorescence_plate_block.py` & `allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/fluorescence_plate_block.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/luminescence_plate_block.py` & `allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/luminescence_plate_block.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/plate_block.py` & `allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/plate_block.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/moldev_softmax_pro/softmax_pro_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/moldev_softmax_pro/softmax_pro_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/novabio_flex2/constants.py` & `allotropy-0.1.9/src/allotropy/parsers/novabio_flex2/constants.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/novabio_flex2/novabio_flex2_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/novabio_flex2/novabio_flex2_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/novabio_flex2/novabio_flex2_structure.py` & `allotropy-0.1.9/src/allotropy/parsers/novabio_flex2/novabio_flex2_structure.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/perkin_elmer_envision/perkin_elmer_envision_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/perkin_elmer_envision/perkin_elmer_envision_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/perkin_elmer_envision/perkin_elmer_envision_structure.py` & `allotropy-0.1.9/src/allotropy/parsers/perkin_elmer_envision/perkin_elmer_envision_structure.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/constants.py` & `allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/constants.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_reader.py` & `allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_reader.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_structure.py` & `allotropy-0.1.9/src/allotropy/parsers/roche_cedex_bioht/roche_cedex_bioht_structure.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/utils/timestamp_parser.py` & `allotropy-0.1.9/src/allotropy/parsers/utils/timestamp_parser.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/src/allotropy/parsers/utils/values.py` & `allotropy-0.1.9/src/allotropy/parsers/utils/values.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/allotrope/allotrope_test.py` & `allotropy-0.1.9/tests/allotrope/allotrope_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/allotrope/models/shared/definitions_test.py` & `allotropy-0.1.9/tests/allotrope/models/shared/definitions_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/allotrope/schema_parser/model_class_editor_test.py` & `allotropy-0.1.9/tests/allotrope/schema_parser/model_class_editor_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/allotrope/schema_parser/schema_model_test.py` & `allotropy-0.1.9/tests/allotrope/schema_parser/schema_model_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/lines_reader_test.py` & `allotropy-0.1.9/tests/parsers/lines_reader_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/test_utils.py` & `allotropy-0.1.9/tests/parsers/test_utils.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/to_allotrope_test.py` & `allotropy-0.1.9/tests/parsers/agilent_gen5/to_allotrope_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_pathlength_correct_singleplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_pathlength_correct_singleplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_pathlength_correct_singleplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_pathlength_correct_singleplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_multiplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_multiplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_multiplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_multiplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate_2.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate_2.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate_2.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/endpoint_stdcurve_singleplate_2.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_helper_gene_growth_curve.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_helper_gene_growth_curve.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_helper_gene_growth_curve.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_helper_gene_growth_curve.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_multiplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_multiplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_multiplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_multiplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_singleplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_singleplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_singleplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/absorbance/kinetic_singleplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_multiplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_multiplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_multiplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_multiplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_singleplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_singleplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_singleplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/fluorescence/endpoint_singleplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_multiplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_multiplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_multiplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_multiplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_singleplate.json` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_singleplate.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_singleplate.txt` & `allotropy-0.1.9/tests/parsers/agilent_gen5/testdata/luminescence/endpoint_singleplate.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/appbio_absolute_q_parser_test.py` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/appbio_absolute_q_parser_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example01.csv` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example01.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example01.json` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example01.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example02.csv` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example02.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example02.json` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example02.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example03.csv` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example03.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example03.json` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example03.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example04.csv` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example04.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example04.json` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example04.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example05.csv` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example05.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example05.json` & `allotropy-0.1.9/tests/parsers/appbio_absolute_q/testdata/Appbio_AbsoluteQ_example05.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/appbio_quantstudio_builders_test.py` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/appbio_quantstudio_builders_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,15 @@
         experimental_data_identifier=experimental_data_identifier,
     )
 
 
 @pytest.mark.parametrize(
     "parameter,expected_error",
     [
-        ("device_identifier", "Unable to get device identifier"),
         ("model_number", "Unable to get model number"),
-        ("device_serial_number", "Unable to get device serial number"),
         (
             "measurement_method_identifier",
             "Unable to get measurement method identifier",
         ),
         ("pcr_detection_chemistry", "Unable to get PCR detection chemistry"),
         ("plate_well_count", "Unable to interpret plate well count"),
     ],
```

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/appbio_quantstudio_data.py` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/appbio_quantstudio_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/appbio_quantstudio_parser_test.py` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/appbio_quantstudio_parser_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 )
 from tests.parsers.test_utils import from_file, validate_contents, validate_schema
 
 output_files = (
     "appbio_quantstudio_example01",
     "appbio_quantstudio_example02",
     "appbio_quantstudio_example03",
+    "appbio_quantstudio_example04",
+    "appbio_quantstudio_example05",
+    "appbio_quantstudio_example06",
+    "appbio_quantstudio_example07",
+    "appbio_quantstudio_example08",
 )
 
 VENDOR_TYPE = Vendor.APPBIO_QUANTSTUDIO
 
 
 @pytest.mark.parametrize("output_file", output_files)
 def test_parse_appbio_quantstudio_to_asm_schema(output_file: str) -> None:
```

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example01.json` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example01.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example01.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example01.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example02.json` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example02.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example02.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example02.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example03.json` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example03.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example03.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example03.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example04.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example04.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example05.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example05.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example06.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example06.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example07.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example07.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example08.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_example08.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test01.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test01.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test02.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test02.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test03.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test03.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test04.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test04.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test05.txt` & `allotropy-0.1.9/tests/parsers/appbio_quantstudio/testdata/appbio_quantstudio_test05.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/vi_cell_blu_data.py` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/vi_cell_blu_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/vi_cell_blu_parser_test.py` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/vi_cell_blu_parser_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example01.csv` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example01.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example01.json` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example01.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example02.csv` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example02.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example02.json` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_blu/testdata/Beckman_Vi-Cell-BLU_example02.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/vi_cell_xr_parser_test.py` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/vi_cell_xr_parser_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example02_instrumentOutput.xls` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example02_instrumentOutput.xls`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example03_instrumentOutput.json` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example03_instrumentOutput.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example03_instrumentOutput.xls` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.04/Beckman_Vi-Cell-XR_example03_instrumentOutput.xls`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example01_instrumentOutput.json` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example01_instrumentOutput.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example01_instrumentOutput.xlsx` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example01_instrumentOutput.xlsx`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example04_instrumentOutput.json` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example04_instrumentOutput.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example04_instrumentOutput.xlsx` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example04_instrumentOutput.xlsx`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example05_instrumentOutput.json` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example05_instrumentOutput.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example05_instrumentOutput.xlsx` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example05_instrumentOutput.xlsx`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example06_instrumentOutput.json` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example06_instrumentOutput.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example06_instrumentOutput.xlsx` & `allotropy-0.1.9/tests/parsers/beckman_vi_cell_xr/testdata/v2.06/Beckman_Vi-Cell-XR_example06_instrumentOutput.xlsx`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/moldev_softmax_pro/to_allotrope_test.py` & `allotropy-0.1.9/tests/parsers/moldev_softmax_pro/to_allotrope_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/abs_endpoint_plates.txt` & `allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/abs_endpoint_plates.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/expected_abs_endpoint.json` & `allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/expected_abs_endpoint.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/expected_fl_kinetic.json` & `allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/expected_fl_kinetic.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/expected_lum_spectrum.json` & `allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/expected_lum_spectrum.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/fl_kinetic_plates.txt` & `allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/fl_kinetic_plates.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/lum_spectrum_columns.txt` & `allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/lum_spectrum_columns.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/moldev_softmax_pro/testdata/trf_well_scan_plates.txt` & `allotropy-0.1.9/tests/parsers/moldev_softmax_pro/testdata/trf_well_scan_plates.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/novabio_flex2/novabio_flex2_data.py` & `allotropy-0.1.9/tests/parsers/novabio_flex2/novabio_flex2_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/novabio_flex2/novabio_flex2_parser_test.py` & `allotropy-0.1.9/tests/parsers/novabio_flex2/novabio_flex2_parser_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/novabio_flex2/novabio_flex2_structure_test.py` & `allotropy-0.1.9/tests/parsers/novabio_flex2/novabio_flex2_structure_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/novabio_flex2/testdata/SampleResults2022-06-28_142558.csv` & `allotropy-0.1.9/tests/parsers/novabio_flex2/testdata/SampleResults2022-06-28_142558.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/novabio_flex2/testdata/SampleResults2022-06-28_142558.json` & `allotropy-0.1.9/tests/parsers/novabio_flex2/testdata/SampleResults2022-06-28_142558.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/novabio_flex2/testdata/SampleResultsDEVICE1232021-02-18_104838.csv` & `allotropy-0.1.9/tests/parsers/novabio_flex2/testdata/SampleResultsDEVICE1232021-02-18_104838.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/novabio_flex2/testdata/SampleResultsDEVICE1232021-02-18_104838.json` & `allotropy-0.1.9/tests/parsers/novabio_flex2/testdata/SampleResultsDEVICE1232021-02-18_104838.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_data.py` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_parser_test.py` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_parser_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_structure_test.py` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/perkin_elmer_envision_structure_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_absorbance_example01.csv` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_absorbance_example01.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01.csv` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01.json` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01_v2.json` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example01_v2.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example02.csv` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example02.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example02.json` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example02.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example03.csv` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example03.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example03.json` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example03.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example04.csv` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_fluorescence_example04.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_luminescence_example01.csv` & `allotropy-0.1.9/tests/parsers/perkin_elmer_envision/testdata/PE_Envision_luminescence_example01.csv`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_data.py` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_data.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_parser_test.py` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_parser_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_structure_test.py` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/roche_cedex_bioht_structure_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example01.json` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example01.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example01.txt` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example01.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example02.json` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example02.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example02.txt` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example02.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example03.json` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example03.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example03.txt` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example03.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example04.json` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example04.json`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example04.txt` & `allotropy-0.1.9/tests/parsers/roche_cedex_bioht/testdata/roche_cedex_bioht_example04.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/tests/parsers/utils/timestamp_parser_test.py` & `allotropy-0.1.9/tests/parsers/utils/timestamp_parser_test.py`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/.gitignore` & `allotropy-0.1.9/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -209,7 +209,10 @@
 .idea/httpRequests
 
 # Android studio 3.1+ serialized cache file
 .idea/caches/build_file_checksums.ser
 
 # MacOS
 .DS_Store
+
+# Emacs
+*~
```

### Comparing `allotropy-0.1.8/LICENSE.txt` & `allotropy-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/README.md` & `allotropy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `allotropy-0.1.8/pyproject.toml` & `allotropy-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 description = 'Converts to ASM (Allotrope Simple Model) from various file formats.'
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
 keywords = ["allotropy", "allotrope", "asm", "benchling", "converters"]
 authors = [
   { name = "Benchling Open Source", email = "opensource@benchling.com" },
-  { name = "Alejando Salgado", email = "alejando.salgado@benchling.com" },
-  { name = "Brian Worth", email = "brian@benchling.com" },
-  { name = "Greg Wilson", email = "greg@deepgenomics.com" },
-  { name = "Joe Negri", email = "joe.negri@benchling.com" },
+  { name = "Lukas Boelling", email = "lukas.boelling@deepgenomics.com" },
   { name = "Kathy Garcia", email = "kathy@benchling.com" },
+  { name = "Trevor Halum", email = "trevor.halum@deepgenomics.com" },
+  { name = "Sebastian Lopez", email = "sebastian.cardona@benchling.com" },
   { name = "Mindren Lu", email = "mindren.lu@benchling.com" },
+  { name = "Joe Negri", email = "joe.negri@benchling.com" },
+  { name = "Alejando Salgado", email = "alejando.salgado@benchling.com" },
   { name = "Nathan Stender", email = "nathan.stender@benchling.com" },
-  { name = "Sebastian Lopez", email = "sebastian.cardona@benchling.com" },
+  { name = "Eihab Syed", email = "eihabsyed@gmail.com" },
+  { name = "Yukthi Wickramarachchi", email = "yukthi.wickramarachchi@deepgenomics.com" },
+  { name = "Greg Wilson", email = "gvwilson@third-bit.com" },
   { name = "Stephen Worlow", email = "stephen.worlow@benchling.com" },
+  { name = "Brian Worth", email = "brian@benchling.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
```

### Comparing `allotropy-0.1.8/PKG-INFO` & `allotropy-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: allotropy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Converts to ASM (Allotrope Simple Model) from various file formats.
 Project-URL: Documentation, https://github.com/Benchling-Open-Source/allotropy#readme
 Project-URL: Issues, https://github.com/Benchling-Open-Source/allotropy/issues
 Project-URL: Source, https://github.com/Benchling-Open-Source/allotropy
-Author-email: Benchling Open Source <opensource@benchling.com>, Alejando Salgado <alejando.salgado@benchling.com>, Brian Worth <brian@benchling.com>, Greg Wilson <greg@deepgenomics.com>, Joe Negri <joe.negri@benchling.com>, Kathy Garcia <kathy@benchling.com>, Mindren Lu <mindren.lu@benchling.com>, Nathan Stender <nathan.stender@benchling.com>, Sebastian Lopez <sebastian.cardona@benchling.com>, Stephen Worlow <stephen.worlow@benchling.com>
+Author-email: Benchling Open Source <opensource@benchling.com>, Lukas Boelling <lukas.boelling@deepgenomics.com>, Kathy Garcia <kathy@benchling.com>, Trevor Halum <trevor.halum@deepgenomics.com>, Sebastian Lopez <sebastian.cardona@benchling.com>, Mindren Lu <mindren.lu@benchling.com>, Joe Negri <joe.negri@benchling.com>, Alejando Salgado <alejando.salgado@benchling.com>, Nathan Stender <nathan.stender@benchling.com>, Eihab Syed <eihabsyed@gmail.com>, Yukthi Wickramarachchi <yukthi.wickramarachchi@deepgenomics.com>, Greg Wilson <gvwilson@third-bit.com>, Stephen Worlow <stephen.worlow@benchling.com>, Brian Worth <brian@benchling.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: allotrope,allotropy,asm,benchling,converters
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

