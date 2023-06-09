# Comparing `tmp/dsptoolbox-0.2.4.tar.gz` & `tmp/dsptoolbox-0.2.5.tar.gz`

## Comparing `dsptoolbox-0.2.4.tar` & `dsptoolbox-0.2.5.tar`

### file list

```diff
@@ -1,85 +1,92 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/.gitattributes
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/.readthedocs.yaml
--rw-r--r--   0        0        0     9689 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/CHANGELOG.rst
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/requirements.txt
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/Makefile
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/__rdme.rst
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/classes.rst
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/conf.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/index.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/make.bat
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules.rst
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/readme.rst
--rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/logo/logo.png
--rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/logo/logo2.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.audio_io.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.beamforming.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.distances.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.filterbanks.rst
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.generators.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.plots.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.room_acoustics.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.special.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.standard_functions.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/docs/modules/dsptoolbox.transfer_functions.rst
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/__init__.py
--rw-r--r--   0        0        0    22294 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/_general_helpers.py
--rw-r--r--   0        0        0    30530 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/_standard.py
--rw-r--r--   0        0        0    42665 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/standard_functions.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/audio_io/__init__.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/audio_io/_audio_io.py
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/audio_io/audio_io.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/beamforming/__init__.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/beamforming/_beamforming.py
--rw-r--r--   0        0        0    63085 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/beamforming/beamforming.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/classes/__init__.py
--rw-r--r--   0        0        0    20613 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/classes/_filter.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/classes/_plots.py
--rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/classes/filter_class.py
--rw-r--r--   0        0        0    27757 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/classes/filterbank.py
--rw-r--r--   0        0        0    13664 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/classes/multibandsignal.py
--rw-r--r--   0        0        0    47885 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/classes/signal_class.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/distances/__init__.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/distances/_distances.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/distances/distances.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/experimental/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/experimental/experimental.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/filterbanks/__init__.py
--rw-r--r--   0        0        0    44829 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/filterbanks/_filterbank.py
--rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/filterbanks/filterbanks.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/generators/__init__.py
--rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/generators/generators.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/plots/__init__.py
--rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/plots/plots.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/room_acoustics/__init__.py
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/room_acoustics/_room_acoustics.py
--rw-r--r--   0        0        0    20855 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/room_acoustics/room_acoustics.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/special/__init__.py
--rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/special/special.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/transfer_functions/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/transfer_functions/_transfer_functions.py
--rw-r--r--   0        0        0    23524 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/dsptoolbox/transfer_functions/transfer_functions.py
--rw-r--r--   0        0        0   948939 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/examples/general.ipynb
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/examples/data/array.xml
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/examples/data/chirp.wav
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/examples/data/chirp_mono.wav
--rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/examples/data/chirp_stereo.wav
--rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/examples/data/rir.wav
--rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/examples/data/speech.flac
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/manual_filter_testing.py
--rw-r--r--   0        0        0    29084 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/manual_testing.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_audio_io.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_beamforming.py
--rw-r--r--   0        0        0    30055 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_classes.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_distances.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_filterbanks.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_generators.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_room_acoustics.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_special.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_standard.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/tests/test_transfer_functions.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/LICENSE
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/README.rst
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 dsptoolbox-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/.gitattributes
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/.readthedocs.yaml
+-rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/CHANGELOG.rst
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/requirements.txt
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/Makefile
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/__rdme.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/classes.rst
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/conf.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/index.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/make.bat
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules.rst
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/readme.rst
+-rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/logo/logo.png
+-rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/logo/logo2.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.audio_io.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.beamforming.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.distances.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.filterbanks.rst
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.generators.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.plots.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.room_acoustics.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.special.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.standard_functions.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.transfer_functions.rst
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/__init__.py
+-rw-r--r--   0        0        0    23326 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/_general_helpers.py
+-rw-r--r--   0        0        0    30953 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/_standard.py
+-rw-r--r--   0        0        0    42692 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/standard_functions.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/audio_io/__init__.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/audio_io/_audio_io.py
+-rw-r--r--   0        0        0    14816 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/audio_io/audio_io.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/beamforming/__init__.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/beamforming/_beamforming.py
+-rw-r--r--   0        0        0    61951 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/beamforming/beamforming.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/__init__.py
+-rw-r--r--   0        0        0    20613 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/_filter.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/_plots.py
+-rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/filter_class.py
+-rw-r--r--   0        0        0    27757 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/filterbank.py
+-rw-r--r--   0        0        0    13664 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/multibandsignal.py
+-rw-r--r--   0        0        0    48334 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/signal_class.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/distances/__init__.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/distances/_distances.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/distances/distances.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/filterbanks/__init__.py
+-rw-r--r--   0        0        0    45051 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/filterbanks/_filterbank.py
+-rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/filterbanks/filterbanks.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/generators/__init__.py
+-rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/generators/generators.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/plots/__init__.py
+-rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/plots/plots.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/room_acoustics/__init__.py
+-rw-r--r--   0        0        0    33500 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/room_acoustics/_room_acoustics.py
+-rw-r--r--   0        0        0    20850 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/room_acoustics/room_acoustics.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/special/__init__.py
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/special/special.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/transfer_functions/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/transfer_functions/_transfer_functions.py
+-rw-r--r--   0        0        0    23751 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/transfer_functions/transfer_functions.py
+-rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/audio_io_module.ipynb
+-rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/beamforming_module.ipynb
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/distances_module.ipynb
+-rw-r--r--   0        0        0   403706 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/filterbanks_module.ipynb
+-rw-r--r--   0        0        0   948939 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/general.ipynb
+-rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/generators_module.ipynb
+-rw-r--r--   0        0        0   330277 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/room_acoustics_module.ipynb
+-rw-r--r--   0        0        0  1536113 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/special_module.ipynb
+-rw-r--r--   0        0        0    47577 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/standard_module.ipynb
+-rw-r--r--   0        0        0   209919 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/transfer_function_module.ipynb
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/array.xml
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/chirp.wav
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/chirp_mono.wav
+-rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/chirp_stereo.wav
+-rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/rir.wav
+-rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/speech.flac
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/manual_filter_testing.py
+-rw-r--r--   0        0        0    29360 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/manual_testing.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_audio_io.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_beamforming.py
+-rw-r--r--   0        0        0    30055 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_classes.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_distances.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_filterbanks.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_generators.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_room_acoustics.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_special.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_standard.py
+-rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_transfer_functions.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/README.rst
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/PKG-INFO
```

### Comparing `dsptoolbox-0.2.4/.readthedocs.yaml` & `dsptoolbox-0.2.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/CHANGELOG.rst` & `dsptoolbox-0.2.5/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,34 @@
 
 `To Do's for future releases`_
 ------------------------------
 
 - Validation for results from tests in every module (so far many tests are
   only regarding functionality)
 
+`0.2.5 <https://pypi.org/project/dsptoolbox/0.2.5>`_ - 
+---------------------
+
+Added
+~~~~~~
+- mel-frequency cepstral coefficients ``mfcc`` in ``special`` module
+- spectrogram of a signal can now be plotted with a selected dynamic range
+- ``audio_io`` has now more port functionalities to ``sounddevice``
+
+Bugfix
+~~~~~~~
+- plotting for the ``qmf`` Crossover is now possible without downsampling
+- Linkwitz-Riley crossovers plotting functions have been updated and corrected
+- corrected some tests
+
+Misc
+~~~~~
+- docstrings corrected and extended
+- computation of steering vectors in ``beamforming`` has been optimized
+
 `0.2.4 <https://pypi.org/project/dsptoolbox/0.2.4>`_ - 
 ---------------------
 
 Added
 ~~~~~~
 - ``rms`` function
 - ``constrain_amplitude`` property to signal class is now used to enable
```

### Comparing `dsptoolbox-0.2.4/requirements.txt` & `dsptoolbox-0.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/docs/Makefile` & `dsptoolbox-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/docs/classes.rst` & `dsptoolbox-0.2.5/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/docs/conf.py` & `dsptoolbox-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/docs/index.rst` & `dsptoolbox-0.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/docs/make.bat` & `dsptoolbox-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/docs/readme.rst` & `dsptoolbox-0.2.5/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/docs/logo/logo.png` & `dsptoolbox-0.2.5/docs/logo/logo.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/docs/logo/logo2.png` & `dsptoolbox-0.2.5/docs/logo/logo2.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/__init__.py` & `dsptoolbox-0.2.5/dsptoolbox/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,11 +24,11 @@
     'resample', 'activity_detector', 'normalize',
     'fractional_delay', 'true_peak_level', 'ir_to_filter', 'erb_frequencies',
     'load_pkl_object', 'fractional_octave_frequencies', 'filter_to_ir',
     'detrend', 'rms', 'CalibrationData',
 
     # Modules
     'transfer_functions', 'distances', 'room_acoustics', 'plots', 'generators',
-    'filterbanks', 'special', 'audio_io', 'beamforming',
+    'filterbanks', 'special', 'audio_io', 'beamforming'
 ]
 
-__version__ = '0.2.4'
+__version__ = '0.2.5'
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/_general_helpers.py` & `dsptoolbox-0.2.5/dsptoolbox/_general_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 
 def _get_normalized_spectrum(f, spectra: np.ndarray, mode='standard',
                              f_range_hz=[20, 20000], normalize: str = None,
                              smoothe: int = 0, phase=False,
                              calibrated_data: bool = False) \
         -> tuple[np.ndarray, np.ndarray, np.ndarray]:
-    """This function gives a normalized magnitude spectrum with frequency
+    """This function gives a normalized magnitude spectrum in dB with frequency
     vector for a given range. It is also smoothed. Use `None` for the
     spectrum without f_range_hz.
 
     Parameters
     ----------
     f : `np.ndarray`
         Frequency vector.
@@ -701,7 +701,41 @@
     format = format.split('.')
     if len(format) != 1:
         assert format[-1] == desired_format, \
             f'{format[-1]} is not the desired format'
     else:
         path += f'.{desired_format}'
     return path
+
+
+def _get_next_power_2(number, mode: str = 'closest') -> int:
+    """This function returns the power of 2 closest to the given number.
+
+    Parameters
+    ----------
+    number : int, float
+        Number for which to find the closest power of 2.
+    mode : str {'closest', 'floor', 'ceil'}, optional
+        `'closest'` gives the closest value. `'floor'` returns the next smaller
+        power of 2 and `'ceil'` the next larger. Default: `'closest'`.
+
+    Returns
+    -------
+    number_2 : int
+        Next power of 2 according to the selected mode.
+
+    """
+    assert number > 0, 'Only positive numbers are valid'
+    mode = mode.lower()
+    assert mode in ('closest', 'floor', 'ceil'), \
+        'Mode must be either closest, floor or ceil'
+
+    p = np.log2(number)
+    if mode == 'closest':
+        remainder = p - int(p)
+        mode == 'floor' if remainder < 0.5 else 'ceil'
+
+    if mode == 'floor':
+        p = np.floor(p).astype(int)
+    elif mode == 'ceil':
+        p = np.ceil(p).astype(int)
+    return int(2**p)
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/_standard.py` & `dsptoolbox-0.2.5/dsptoolbox/_standard.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,61 +133,37 @@
         x_frames -= np.mean(x_frames, axis=0)
         y_frames -= np.mean(y_frames, axis=0)
 
     # Combine
     sp_frames = np.fft.rfft(x_frames, axis=0).conjugate() * \
         np.fft.rfft(y_frames, axis=0)
 
-    # ==== Averaging of magnitude and unwrapped phase much slower...
-    # # Get magnitude and phase
-    # magnitude = np.abs(sp_frames)
-    # phase = np.unwrap(np.angle(sp_frames), axis=0)
-
-    # # mean without first and last arrays
-    # if average == 'mean':
-    #     magnitude = np.mean(magnitude[:, 1:-1], axis=-1)
-    #     phase = np.mean(phase[:, 1:-1], axis=-1)
-    # else:
-    #     magnitude = np.median(magnitude[:, 1:-1], axis=-1)
-    #     phase = np.median(phase[:, 1:-1], axis=-1)
-
-    # # Cross spectral density
-    # csd = magnitude * np.exp(1j*phase)
-
     # Direct averaging much faster
     if average == 'mean':
         csd = np.mean(sp_frames, axis=-1)
     else:
         csd = np.median(sp_frames.real, axis=-1) + 1j * \
             np.median(sp_frames.imag, axis=-1)
         # Bias according to reference
         n = sp_frames.shape[1] if sp_frames.shape[1] % 2 == 1 else \
             sp_frames.shape[1] - 1
         bias = np.sum((-1)**(n+1)/n)
-        # This is taken from scipy, it is somewhat different to the paper
-        # ii_2 = 2 * np.arange(1., (n-1) // 2 + 1)
-        # bias = 1 + np.sum(1. / (ii_2 + 1) - 1. / ii_2)
         csd /= bias
 
     # Weightning (with 2 because one-sided)
     if scaling in ('power spectrum', 'amplitude spectrum'):
         factor = 2 / np.sum(window)**2
     elif scaling in ('power spectral density', 'amplitude spectral density'):
         factor = 2 / (window @ window) / fs_hz
         # With this factor, energy can be regained by integrating the psd
         # while taking into account the frequency step
-        # =====================================
-        # This is not consistent with scipy or the reference paper but does
-        # arrive at the right energy when summing over the psd (without taking
-        # frequency step into account)
-        # factor = 2 / (window @ window) / window_length_samples
     else:
         factor = 1
 
-    # Zero frequency fix when detrending
+    # Zero frequency fix when detrending (especially useful for dB plotting)
     if detrend:
         csd[0] = csd[1]
 
     csd *= factor
     csd[0] /= 2
     csd[-1] /= 2
 
@@ -346,16 +322,14 @@
     if detrend:
         time_x -= np.mean(time_x, axis=0)
     # Spectra
     stft = np.fft.rfft(time_x, axis=0, n=fft_length_samples)
     # Scaling
     if scaling:
         factor = np.sqrt(2 / np.sum(window)**2)
-        # factor = 2 / np.sum(window**2) / window_length_samples
-        # factor = 2 / np.sum(window)**2 / fs_hz * window_length_samples
     else:
         factor = 1
     stft *= factor
 
     time_s = np.linspace(0, len(x)/fs_hz, stft.shape[1])
     freqs_hz = np.fft.rfftfreq(len(window), 1/fs_hz)
     return time_s, freqs_hz, stft
@@ -777,15 +751,15 @@
     time_power -= time_power[max_ind]
 
     # All indexes above threshold
     indexes_above_0 = time_power > threshold_dbfs
     indexes_above = np.zeros_like(indexes_above_0).astype(bool)
 
     # Apply release and attack
-    for ind in range(len(indexes_above)):
+    for ind in np.arange(len(indexes_above)):
         # Attack after certain amount of samples surpass threshold
         ind_attack = 0 if ind-attack_samples < 0 else ind-attack_samples
         if np.all(indexes_above_0[ind_attack:ind]):
             indexes_above[ind:ind+release_samples] = True
     return indexes_above
 
 
@@ -831,7 +805,55 @@
         x = x[..., None]
     elif x.ndim == 2:
         pass
     else:
         raise ValueError('Shape of array is not valid. Only 2D-Arrays ' +
                          'are valid')
     return np.sqrt(np.mean(x**2, axis=0))
+
+
+def _get_framed_signal(td: np.ndarray, window_length_samples: int,
+                       step_size: int, keep_last_frame: bool = True) \
+        -> np.ndarray:
+    """This method computes a framed version of a signal and returns it.
+
+    Parameters
+    ----------
+    td : `np.ndarray`
+        Signal with shape (time samples, channels).
+    window_length_samples : int
+        Window length in samples.
+    step_size : int
+        Step size (also called hop length) in samples.
+    keep_last_frame : bool, optional
+        When `True`, the last frame (probably with padded zeroes) is kept.
+        Otherwise, it is not returned and hence the signal is cropped.
+        Default: `True`.
+
+    Returns
+    -------
+    td_framed : `np.ndarray`
+        Framed signal with shape (time samples, frames, channels).
+
+    """
+    # Force casting to integers
+    if type(window_length_samples) != int:
+        window_length_samples = int(window_length_samples)
+    if type(step_size) != int:
+        step_size = int(step_size)
+
+    # Start Parameters
+    n_frames, padding_samp = \
+        _compute_number_frames(window_length_samples, step_size, td.shape[0])
+    td = _pad_trim(td, td.shape[0] + padding_samp)
+    td_framed = np.zeros((window_length_samples, n_frames, td.shape[1]),
+                         dtype='float')
+
+    # Create time frames
+    start = 0
+    for n in range(n_frames):
+        td_framed[:, n, :] = td[start:start+window_length_samples, :].copy()
+        start += step_size
+
+    if not keep_last_frame:
+        td_framed = td_framed[:, :-1, :]
+    return td_framed
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/standard_functions.py` & `dsptoolbox-0.2.5/dsptoolbox/standard_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,15 @@
     each_channel : bool, optional
         When `True`, each channel on its own is normalized. When `False`,
         the peak value for all channels is regarded. Default: `False`.
 
     Returns
     -------
     new_sig : `Signal` or `MultiBandSignal`
+        Normalized signal.
 
     """
     if type(sig) == Signal:
         new_sig = sig.copy()
         new_time_data = np.empty_like(sig.time_data)
         if each_channel:
             for n in range(sig.number_of_channels):
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/audio_io/__init__.py` & `dsptoolbox-0.2.5/dsptoolbox/audio_io/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,22 @@
 References
 ----------
 - https://pypi.org/project/sounddevice/
 
 """
 from .audio_io import (play, play_and_record, set_device, record,
                        print_device_info, play_through_stream, CallbackStop,
-                       standard_callback, sleep, output_stream)
+                       standard_callback, sleep, output_stream, default_config)
 
 __all__ = [
     'play',
     'play_and_record',
     'set_device',
     'record',
     'print_device_info',
     'play_through_stream',
     'CallbackStop',
     'standard_callback',
     'sleep',
     'output_stream',
+    'default_config',
 ]
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/audio_io/_audio_io.py` & `dsptoolbox-0.2.5/dsptoolbox/audio_io/_audio_io.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/audio_io/audio_io.py` & `dsptoolbox-0.2.5/dsptoolbox/audio_io/audio_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,63 +3,101 @@
 measurements and testing audio streams
 """
 import sounddevice as sd
 from dsptoolbox import Signal
 from dsptoolbox._general_helpers import _normalize
 from ._audio_io import standard_callback
 
+default_config = sd.default
+
 
 def print_device_info(device_number: int = None):
     """Prints available audio devices or information about a certain device
     when the device number is given.
 
     Parameters
     ----------
     device_number : int, optional
         Prints information about the specific device and returns it as
         a dictionary. Use `None` to only print information about all devices
         without returning anything. Default: `None`.
 
     Returns
     -------
-    d : dict
-        Only when `device_number is not None`.
+    d : dict or `sounddevice.DeviceList`
+        dict of a device when device number is passed or DeviceList when `None`
+        is passed.
 
     """
     if device_number is None:
-        print(sd.query_devices())
+        d = sd.query_devices()
+        print(d)
+        return d
     else:
         d = sd.query_devices(device_number)
         print(d)
         return d
 
 
-def set_device(device_number: int = None):
-    """Takes in a device number to set it as the default. If `None` is passed,
-    the available devices are first shown and then the user is asked for
-    input to set the device.
+def set_device(device_numbers: list = None, sampling_rate_hz: int = None):
+    """Takes in a device number to set it as the default for the input and the
+    output. If `None` is passed, the available devices are first shown and
+    then the user is asked for input to set the device two values separated by
+    a comma "input_int, output_int".
 
     Parameters
     ----------
-    device_number : int, optional
-        Sets the device as default. Use `None` to be prompted with the
-        options. Default: `None`.
+    device_number : list with length 2, optional
+        Sets the input and output devices from two integers, e.g. [1, 2].
+        Use `None` to be prompted with the options and pass only two values
+        separated by a comma, e.g., `1, 2`. Default: `None`.
+    sampling_rate_hz : int, optional
+        Pass a default sampling rate to the devices. Pass `None` to ignore.
+        Default: `None`.
+
+    Returns
+    -------
+    device_list : `sounddevice.DeviceList`
+        Device List with dictionaries containing information about each
+        available device.
 
     """
-    if device_number is None:
+    if device_numbers is None:
         txt = 'List of available devices'
         print(txt+'\n'+'-'*len(txt))
         print(sd.query_devices())
         print('-'*len(txt))
-        device_number = int(input(
+        device_numbers = input(
             'Which device should be set as default? Between ' +
-            f'0 and {len(sd.query_devices())-1}: '))
-    d = sd.query_devices(device_number)['name']
-    print(f"""{d} will be used!""")
-    sd.default.device = d
+            f'0 and {len(sd.query_devices())-1}: ')
+        device_numbers = \
+            [int(d) for d in device_numbers.split(',')]
+        if len(device_numbers) == 1:
+            device_numbers = device_numbers[0]
+    device_list = sd.query_devices()
+    if type(device_numbers) == int:
+        d = device_list[device_numbers]['name']
+        print(f"""{d} will be used for input and output!""")
+        sd.default.device = device_numbers
+    elif type(device_numbers) == list:
+        assert len(device_numbers) == 2, \
+            'List with device numbers must be exactly 2'
+        d = device_list[device_numbers[0]]['name']
+        print(f"""{d} will be used for input!""")
+
+        d = device_list[device_numbers[1]]['name']
+        print(f"""{d} will be used for output!""")
+        sd.default.device = device_numbers
+    else:
+        raise TypeError('device_number must be either a list or an int')
+
+    # Sampling rate
+    if sampling_rate_hz is not None:
+        sd.default.samplerate = sampling_rate_hz
+    return sd.query_devices()
 
 
 def play_and_record(signal: Signal, duration_seconds: float = None,
                     normalized_dbfs: float = -6, device: str = None,
                     play_channels=None, rec_channels=[1]) -> Signal:
     """Play and record using some available device. Note that the channel
     numbers start here with 1.
@@ -121,31 +159,31 @@
     if normalized_dbfs is not None:
         assert normalized_dbfs <= 0, 'Only values beneath 0 dBFS are allowed'
         play_data = _normalize(play_data, dbfs=normalized_dbfs, mode='peak')
 
     if device is not None:
         sd.default.device = device
 
-    print('\nReproduction and recording have started ' +
+    print('Playback and recording have started ' +
           f'({duration_seconds:.1f} s)...')
     rec_time_data = \
         sd.playrec(
             data=play_data,
             samplerate=signal.sampling_rate_hz,
             input_mapping=rec_channels,
             output_mapping=play_channels)
     sd.wait()
-    print('Reproduction and recording have ended\n')
+    print('Playback and recording have ended\n')
 
     rec_sig = Signal(None, rec_time_data, signal.sampling_rate_hz)
     return rec_sig
 
 
 def record(duration_seconds: float = 5, sampling_rate_hz: int = 48000,
-           device: str = None, rec_channels=[1]) -> Signal:
+           device: str | int = None, rec_channels=[1]) -> Signal:
     """Record using some available device. Note that the channel numbers
     start here with 1.
 
     Parameters
     ----------
     duration_seconds : float, optional
         Duration of recording in seconds. Default: 5.
@@ -229,21 +267,21 @@
     if normalized_dbfs is not None:
         assert normalized_dbfs <= 0, 'Only values beneath 0 dBFS are allowed'
         play_data = _normalize(play_data, dbfs=normalized_dbfs, mode='peak')
     #
     if device is not None:
         sd.default.device = device
 
-    print(f'\nReproduction started ({duration_seconds:.1f} s)...')
+    print(f'Playback started ({duration_seconds:.1f} s)...')
     sd.play(
         data=play_data,
         samplerate=signal.sampling_rate_hz,
         mapping=play_channels)
     sd.wait()
-    print('Reproduction has ended\n')
+    print('Playback has ended\n')
 
 
 def play_through_stream(signal: Signal, blocksize: int = 2048,
                         audio_callback: callable = standard_callback,
                         device: str = None):
     """Plays a signal using a stream and a callback function.
     See `sounddevice.OutputStream` for extensive information about
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/beamforming/__init__.py` & `dsptoolbox-0.2.5/dsptoolbox/beamforming/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/beamforming/_beamforming.py` & `dsptoolbox-0.2.5/dsptoolbox/beamforming/_beamforming.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Backend for beamforming module
 """
 import numpy as np
+from scipy.spatial import distance_matrix
 import matplotlib.pyplot as plt
 from seaborn import set_style
 set_style('whitegrid')
 
 
 class BasePoints():
     """This is a base class for saving point data (like grids or mic arrays).
@@ -84,48 +85,30 @@
     def get_distances_to_point(self, point: np.ndarray) -> np.ndarray:
         """Compute distances (euclidean) from given point to all points of the
         object efficiently.
 
         Parameters
         ----------
         point : `np.ndarray`
-            Point to which to compute the distances from all points saved in.
+            Point or points to which to compute the distances from all other
+            points. Its shape should be (point, coordinate).
 
         Returns
         -------
         distances : `np.ndarray`
-            Distances with shape (points).
+            Distances with shape (points, new_points).
 
         """
-        assert len(point) == self.coordinates.shape[1], \
+        if type(point) != np.ndarray:
+            point = np.asarray(point)
+        if point.ndim == 1:
+            point = point[None, ...]
+        assert point.shape[1] == self.coordinates.shape[1], \
             f'Invalid shapes: {point.shape}, {self.coordinates.shape}'
-        # Make helper matrix if needed
-        if not hasattr(self, 'distance_helper_matrix'):
-            self._compute_distance_helper_matrix()
-        if self._distance_helper_matrix is None:
-            self._compute_distance_helper_matrix()
-        distances = self.coordinates - point
-        return (distances.flatten()**2 @ self._distance_helper_matrix)**0.5
-
-    # Helper matrix for vectorized computation
-    def _compute_distance_helper_matrix(self):
-        """Compute helper matrix for euclidean distances. Only intended as an
-        internal method.
-
-        """
-        helper_matrix = \
-            np.zeros((self.coordinates.shape[0]*self.coordinates.shape[1], 1))
-        helper_matrix[:self.coordinates.shape[1], 0] = 1
-        for _ in range(1, self.coordinates.shape[0]):
-            helper_matrix = np.append(
-                helper_matrix,
-                np.roll(helper_matrix[:, -1],
-                        self.coordinates.shape[1])[..., None],
-                axis=-1)
-        self._distance_helper_matrix = helper_matrix
+        return distance_matrix(self.coordinates, point, p=2).squeeze()
 
     # ======== Plotting =======================================================
     def plot_points(self, projection: str = None):
         """Plot points in 2D or 3D plot depending on the actual points.
 
         Parameters
         ----------
@@ -287,15 +270,15 @@
 
         if remove_diagonal_csm:
             np.fill_diagonal(G, 0)
 
         for gind in range(len(map)):
             # Clean map
             map[gind] -= np.linalg.multi_dot([
-                h_H[gind, :], G, h[:, gind]]) * safety_factor
+                h_H[gind, :], G, h[:, gind]]).real * safety_factor
 
         # Swap degraded CSM
         temp = D[1, :, :].copy()
         D[1, :, :] = D[1, :, :] - safety_factor * G
         D[0, :, :] = temp
 
     return second_map
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/beamforming/beamforming.py` & `dsptoolbox-0.2.5/dsptoolbox/beamforming/beamforming.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,27 +493,19 @@
         return self.__array_center_channel_number
 
     def __compute_aperture_min_distance(self):
         """Method to trigger the computation for the array's aperture and
         minimum distance between microphones.
 
         """
-        # Initialize values
-        min_value = 1e20
-        max_value = -1
-        for i1 in range(self.coordinates.shape[0]):
-            # Get distances from point i1 to all other points
-            distances = self.get_distances_to_point(self.coordinates[i1, :])
-            # Prune 0 value (distance for point with itself)
-            distances = distances[distances != 0]
-            # Get min and max values
-            max_value = max(max_value, np.max(distances))
-            min_value = min(min_value, np.min(distances))
-        self.__min_distance = min_value
-        self.__aperture = max_value
+        distances = self.get_distances_to_point(self.coordinates)
+        np.fill_diagonal(distances, np.inf)
+        self.__min_distance = np.min(distances)
+        np.fill_diagonal(distances, -np.inf)
+        self.__aperture = np.max(distances)
 
     def __compute_array_center(self):
         """Returns array center mic's coordinates and number.
 
         Parameters
         ----------
         coord : `np.ndarray`
@@ -903,15 +895,15 @@
     """
     beamformer_type = 'CleanSC'
 
     def get_beamformer_map(self, center_frequency_hz: float,
                            octave_fraction: int = 3,
                            maximum_iterations: int = None,
                            safety_factor: float = 0.5,
-                           remove_diagonal_csm: bool = False) -> np.ndarray:
+                           remove_csm_diagonal: bool = False) -> np.ndarray:
         """Returns a deconvolved beaforming map.
 
         Parameters
         ----------
         center_frequenc_hz : float
             Center frequency for which to compute map.
         octave_fraction : int, optional
@@ -922,15 +914,15 @@
             If `None` is passed, the double of the number of microphones is
             taken as the maximum iteration number. The stopping criterion
             given in [1] is always checked. Default: `None`.
         safety_factor : float, optional
             Also called loop gain, the safety factor dampens the result from
             each iteration during deconvolution. Should be between 0 and 1.
             See [1] for more details. Default: 0.5.
-        remove_diagonal_csm : bool, optional
+        remove_csm_diagonal : bool, optional
             When `True`, the main diagonal of the CSM is removed for a cleaner
             map (source powers might be wrongly estimated). Default: `False`.
 
         Returns
         -------
         map : `np.ndarray`
             Beamformer map.
@@ -978,30 +970,30 @@
         wave_numbers = f * np.pi * 2 / self.c
         h = self.st_vec.get_vector(
             wave_numbers, grid=self.grid, mic=self.mics)
         h_H = np.swapaxes(h, 1, 2).conjugate()
         self.f_range_hz = np.array([f[0], f[-1]])
 
         # Remove diagonal CSM
-        if remove_diagonal_csm:
+        if remove_csm_diagonal:
             for find in range(len(f)):
                 np.fill_diagonal(csm[find, :, :], 0)
 
         print('...Create and deconvolve map...')
         map = np.zeros((self.grid.number_of_points,
                         number_frequency_bins))
         for find in range(len(f)):
             for gind in range(self.grid.number_of_points):
                 # Create initial map
                 map[gind, find] = np.linalg.multi_dot(
                     [h_H[find, gind, :], csm[find, :, :],
                      h[find, :, gind]]).real
-            map = _clean_sc_deconvolve(
+            map[:, find] = _clean_sc_deconvolve(
                 map[:, find], csm[find, :, :], h[find, :, :], h_H[find, :, :],
-                maximum_iterations, remove_diagonal_csm, safety_factor).real
+                maximum_iterations, remove_csm_diagonal, safety_factor).real
 
         # Integrate over all frequencies
         if number_frequency_bins > 1:
             map = simpson(map, dx=f[1]-f[0], axis=1)
         else:
             map = map.squeeze()
         self.map = self.grid.reconstruct_map_shape(map)
@@ -1339,42 +1331,38 @@
         print('\n'+txt)
         print('-'*len(txt))
         print('...get delays...')
         # Start Signal from one channel
         out_sig = self.signal.get_channels(0)
 
         # Get maximal distance in order to delay all signals to that
-        r0 = -1
-        min_distance = 1e20
-        for gp in self.grid.coordinates:
-            ds = self.mics.get_distances_to_point(gp)
-            r0 = max(r0, np.max(ds))
-            min_distance = min(min_distance, np.min(ds))
+        ds = self.mics.get_distances_to_point(self.grid.coordinates)
+        min_distance = np.min(ds)
+        r0 = np.max(ds)
 
         # Get longest delay in order to pad all signals accordingly
         longest_delay_samples = \
             (r0 - min_distance)/self.c * self.signal.sampling_rate_hz
         longest_delay_samples = int(longest_delay_samples + 2)
         total_length_samples = \
             out_sig.time_data.shape[0] + longest_delay_samples
         out_sig = pad_trim(out_sig, total_length_samples)
 
         # Start computation for each grid point
         print('...grid focusing...')
         for ig in range(self.grid.number_of_points):
             if ig == self.grid.number_of_points//2:
                 print(r'...50% grid done...')
-            ds = self.mics.get_distances_to_point(self.grid.coordinates[ig, :])
-            delays = (r0 - ds)/self.c
+            delays = (r0 - ds[:, ig])/self.c
             # Accumulator
             new_time_data = np.zeros((total_length_samples, 1))
             for im in range(self.mics.number_of_points):
                 ntd = fractional_delay(
                     self.signal.get_channels(im), delays[im]).time_data *\
-                        ds[im]
+                        ds[im, ig]
                 new_time_data += _pad_trim(ntd, total_length_samples)
             new_time_data *= (4*np.pi/self.mics.number_of_points)
             out_sig.add_channel(None, new_time_data, out_sig.sampling_rate_hz)
         out_sig.remove_channel(0)
         return out_sig
 
 
@@ -1518,23 +1506,21 @@
 
     """
     wave_number = np.atleast_1d(wave_number)
     assert wave_number.ndim == 1, \
         'Wave number should be a 1D-array'
     # Number of mics and grid points
     N = mic.number_of_points
-    NGrid = grid.number_of_points
 
     # rt0 with shape (ngrid)
     rt0 = grid.get_distances_to_point(mic.array_center_coordinates)
 
     # rti matrix with shape (nmic, ngrid)
-    rti = np.zeros((N, NGrid))
-    for i in range(N):
-        rti[i, :] = grid.get_distances_to_point(mic.coordinates[i, :])
+    rti = grid.get_distances_to_point(mic.coordinates).T
+    # Transpose because output is always (grid, other points)
 
     return 1/N * np.exp(
         -1j*wave_number[:, nxs, nxs] * (rti[nxs, :, :] - rt0[nxs, nxs, :]))
 
 
 def inverse_steering(wave_number: np.ndarray, grid: Grid,
                      mic: MicArray) -> np.ndarray:
@@ -1563,23 +1549,20 @@
 
     """
     wave_number = np.atleast_1d(wave_number)
     assert wave_number.ndim == 1, \
         'Wave number should be a 1D-array'
     # Number of mics and grid points
     N = mic.number_of_points
-    NGrid = grid.number_of_points
 
     # rt0 with shape (ngrid)
     rt0 = grid.get_distances_to_point(mic.array_center_coordinates)
 
     # rti matrix with shape (nmic, ngrid)
-    rti = np.zeros((N, NGrid))
-    for i in range(N):
-        rti[i, :] = grid.get_distances_to_point(mic.coordinates[i, :])
+    rti = grid.get_distances_to_point(mic.coordinates).T
 
     # Formulate vector
     return rti[nxs, :, :] / N / rt0[nxs, nxs, :] * \
         np.exp(-1j * wave_number[:, nxs, nxs] *
                (rti[nxs, :, :] - rt0[nxs, nxs, :]))
 
 
@@ -1608,31 +1591,23 @@
       with Different Beamforming Steering Vector Formulations. Advances in
       Acoustics and Vibration. 2012. 10.1155/2012/292695.
 
     """
     wave_number = np.atleast_1d(wave_number)
     assert wave_number.ndim == 1, \
         'Wave number should be a 1D-array'
-    # Number of mics and grid points
-    N = mic.number_of_points
-    NGrid = grid.number_of_points
 
     # rt0 with shape (ngrid)
     rt0 = grid.get_distances_to_point(mic.array_center_coordinates)
 
     # rti matrix with shape (nmic, ngrid)
-    rti = np.zeros((N, NGrid))
-    for i in range(N):
-        rti[i, :] = grid.get_distances_to_point(mic.coordinates[i, :])
+    rti = grid.get_distances_to_point(mic.coordinates).T
 
     # rtj vector with shape (ngrid)
-    rtj = np.zeros((NGrid))
-    for i in range(NGrid):
-        all_distances = mic.get_distances_to_point(grid.coordinates[i, :])
-        rtj[i] = np.sum(1/all_distances**2)
+    rtj = np.sum(1/mic.get_distances_to_point(grid.coordinates)**2, axis=0)
 
     # Formulate vector
     return 1 / rt0[nxs, nxs, :] / rti[nxs, :, :] / rtj[nxs, nxs, :] * \
         np.exp(-1j * wave_number[:, nxs, nxs] *
                (rti[nxs, :, :] - rt0[nxs, nxs, :]))
 
 
@@ -1663,26 +1638,20 @@
 
     """
     wave_number = np.atleast_1d(wave_number)
     assert wave_number.ndim == 1, \
         'Wave number should be a 1D-array'
     # Number of mics and grid points
     N = mic.number_of_points
-    NGrid = grid.number_of_points
 
     # rt0 with shape (ngrid)
     rt0 = grid.get_distances_to_point(mic.array_center_coordinates)
 
     # rti matrix with shape (nmic, ngrid)
-    rti = np.zeros((N, NGrid))
-    for i in range(N):
-        rti[i, :] = grid.get_distances_to_point(mic.coordinates[i, :])
+    rti = grid.get_distances_to_point(mic.coordinates).T
 
     # rtj vector with shape (ngrid)
-    rtj = np.zeros((NGrid))
-    for i in range(NGrid):
-        all_distances = mic.get_distances_to_point(grid.coordinates[i, :])
-        rtj[i] = N * np.sum(1/all_distances**2)
+    rtj = N * np.sum(1/mic.get_distances_to_point(grid.coordinates)**2, axis=0)
 
     return 1 / rti[nxs, :, :] / np.sqrt(rtj[nxs, nxs, :]) * \
         np.exp(-1j * wave_number[:, nxs, nxs] *
                (rti[nxs, :, :] - rt0[nxs, nxs, :]))
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/classes/__init__.py` & `dsptoolbox-0.2.5/dsptoolbox/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/classes/_filter.py` & `dsptoolbox-0.2.5/dsptoolbox/classes/_filter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/classes/_plots.py` & `dsptoolbox-0.2.5/dsptoolbox/classes/_plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/classes/filter_class.py` & `dsptoolbox-0.2.5/dsptoolbox/classes/filter_class.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/classes/filterbank.py` & `dsptoolbox-0.2.5/dsptoolbox/classes/filterbank.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/classes/multibandsignal.py` & `dsptoolbox-0.2.5/dsptoolbox/classes/multibandsignal.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/classes/signal_class.py` & `dsptoolbox-0.2.5/dsptoolbox/classes/signal_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,25 +945,32 @@
             f, gd*1e3, range_hz,
             labels=[f'Channel {n}' for n in range(self.number_of_channels)],
             ylabel='Group delay / ms',
             returns=True)
         return fig, ax
 
     def plot_spectrogram(self, channel_number: int = 0,
-                         logfreqs: bool = True) -> tuple[Figure, Axes]:
+                         logfreqs: bool = True,
+                         dynamic_range_db: float = 50) -> tuple[Figure, Axes]:
         """Plots STFT matrix of the given channel. The levels in the plot can
         go down until -400 dB.
 
         Parameters
         ----------
         channel_number : int, optional
             Selected channel to plot spectrogram. Default: 0 (first).
         logfreqs : bool, optional
             When `True`, frequency axis is plotted logarithmically.
             Default: `True`.
+        dynamic_range_db : float, optional
+            This sets the dynamic range to show for the spectrogram. The
+            plotted colormap goes from the maximum down to maximum minus
+            dynamic range. For example, dynamic_range_db=50 plots for a peak
+            value of 30 dB the colormap of the spectrogram between
+            [30, -20] dB. Default: 50.
 
         Returns
         -------
         fig : `matplotlib.figure.Figure`
             Figure.
         ax : `matplotlib.axes.Axes`
             Axes.
@@ -979,15 +986,15 @@
         stft_db = np.nan_to_num(stft_db, nan=np.min(stft_db))
         if self._spectrogram_parameters['scaling']:
             zlabel = 'dB (Pa$^2$/Hz)'
         else:
             zlabel = 'dB (No Scaling)'
         fig, ax = general_matrix_plot(
             matrix=stft_db, range_x=(t[0], t[-1]),
-            range_y=(f[0], f[-1]), range_z=50,
+            range_y=(f[0], f[-1]), range_z=np.abs(dynamic_range_db),
             xlabel='Time / s', ylabel='Frequency / Hz',
             zlabel=zlabel,
             xlog=False, ylog=logfreqs,
             colorbar=True, returns=True)
         return fig, ax
 
     def plot_coherence(self) -> tuple[Figure, Axes]:
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/distances/_distances.py` & `dsptoolbox-0.2.5/dsptoolbox/distances/_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/distances/distances.py` & `dsptoolbox-0.2.5/dsptoolbox/distances/distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/filterbanks/__init__.py` & `dsptoolbox-0.2.5/dsptoolbox/filterbanks/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/filterbanks/_filterbank.py` & `dsptoolbox-0.2.5/dsptoolbox/filterbanks/_filterbank.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,76 +284,74 @@
         s_h = sosfilt(self.sos[f_number][1], x=s_h, axis=0)
         if split:
             return s_l, s_h
         else:
             return s_l + s_h
 
     # ======== IR =============================================================
-    def get_ir(self, test_zi: bool = False):
+    def get_ir(self, length_samples: int = 1024, test_zi: bool = False):
         """Returns impulse response from the filter bank. For this filter
         bank only `mode='parallel'` is valid and there is no zero phase
         filtering.
 
         Parameters
         ----------
-        mode : str, optional
-            Way to apply filter bank to the signal. Supported modes are:
-            `'parallel'`, `'summed'`. Default: `'parallel'`.
+        length_samples : int, optional
+            Impulse length in samples. This defines the resolution of the
+            plot. Default: 2048.
         test_zi : bool, optional
             When `True`, filtering is done while updating filters' initial
             values. Default: `False`.
 
         Returns
         -------
         ir : `MultiBandSignal` or `Signal`
             Impulse response of the filter bank.
 
         """
-        d = dirac(
-            length_samples=1024,
-            number_of_channels=1)
-        ir = self.filter_signal(
-            d, activate_zi=test_zi)
+        d = dirac(length_samples=length_samples, number_of_channels=1)
+        ir = self.filter_signal(d, activate_zi=test_zi)
         return ir
 
     # ======== Prints and plots ===============================================
     def plot_magnitude(self, range_hz=[20, 20e3], mode: str = 'parallel',
-                       test_zi: bool = False, zero_phase: bool = False,
-                       returns: bool = False):
+                       length_samples: int = 2048, test_zi: bool = False,
+                       zero_phase: bool = False):
         """Plots the magnitude response of each filter. Only `'parallel'`
         mode is supported, thus no mode parameter can be set.
 
         Parameters
         ----------
         range_hz : array_like, optional
             Range of Hz to plot. Default: [20, 20e3].
         mode : str, optional
             Way to apply filter bank to the signal. Supported modes are:
             `'parallel'`. Default: `'parallel'`.
+        length_samples : int, optional
+            Impulse length in samples. This defines the resolution of the
+            plot. Default: 2048.
         zero_phase : bool, optional
             Activates zero phase filtering. Default: `False`.
         test_zi : bool, optional
             Uses the zi's of each filter to test the FilterBank's output.
             Default: `False`.
-        returns : bool, optional
-            When `True`, the figure and axis are returned. Default: `False`.
 
         Returns
         -------
         fig, ax
-            Returned only when `returns=True`.
+            Figure and axes of the plot
 
         """
         mode = mode.lower()
         if mode != 'parallel':
             warn('Plotting for LRFilterBank is only supported with parallel ' +
                  'mode. Setting to parallel')
         d = dirac(
-            length_samples=1024, number_of_channels=1,
-            sampling_rate_hz=48000)
+            length_samples=length_samples, number_of_channels=1,
+            sampling_rate_hz=self.sampling_rate_hz)
         bs = self.filter_signal(d, mode='parallel', activate_zi=test_zi,
                                 zero_phase=zero_phase)
         specs = []
         f = bs.bands[0].get_spectrum()[0]
         summed = []
         for b in bs.bands:
             b.set_spectrum_parameters(method='standard')
@@ -377,52 +375,52 @@
             _get_normalized_spectrum(
                 f, sp_summed,
                 f_range_hz=range_hz,
                 normalize=None)
         ax.plot(f_s, sp_summed, alpha=0.7, linestyle='dashed',
                 label='Summed signal')
         ax.legend()
-        if returns:
-            return fig, ax
+        return fig, ax
 
     def plot_phase(self, range_hz=[20, 20e3], mode: str = 'parallel',
+                   length_samples: int = 2048,
                    test_zi: bool = False, zero_phase: bool = True,
-                   unwrap: bool = False, returns: bool = False):
+                   unwrap: bool = False):
         """Plots the phase response of each filter.
 
         Parameters
         ----------
+        range_hz : array-like, optional
+            Range of Hz to plot. Default: [20, 20e3].
         mode : str, optional
             Way to apply filter bank to the signal. Supported modes are:
             `'parallel'`. Default: `'parallel'`.
-        range_hz : array-like, optional
-            Range of Hz to plot. Default: [20, 20e3].
+        length_samples : int, optional
+            Impulse length in samples. This defines the resolution of the
+            plot. Default: 2048.
         test_zi : bool, optional
             Uses the zi's of each filter to test the FilterBank's output.
             Default: `False`.
         zero_phase : bool, optional
             Activates zero phase filtering. Default: `False`.
         unwrap : bool, optional
             When `True`, unwrapped phase is plotted. Default: `False`.
-        returns : bool, optional
-            When `True`, the figure and axis are returned. Default: `False`.
 
         Returns
         -------
         fig, ax
-            Returned only when `returns=True`.
+            Figure and axes of the plot
 
         """
         mode = mode.lower()
         assert mode in ('parallel', 'summed'), \
             f'{mode} is not supported. Use either parallel or summed'
-        length_samples = 1024
         d = dirac(
             length_samples=length_samples,
-            number_of_channels=1, sampling_rate_hz=48000)
+            number_of_channels=1, sampling_rate_hz=self.sampling_rate_hz)
 
         if mode == 'parallel':
             bs = self.filter_signal(d, mode='parallel', activate_zi=test_zi,
                                     zero_phase=zero_phase)
             phase = []
             f = bs.bands[0].get_spectrum()[0]
             for b in bs.bands:
@@ -437,29 +435,32 @@
             labels = ['Summed']
 
         if unwrap:
             phase = np.unwrap(phase, axis=0)
         fig, ax = general_plot(f, phase, range_hz, ylabel='Phase / rad',
                                returns=True,
                                labels=labels)
-        if returns:
-            return fig, ax
+        return fig, ax
 
     def plot_group_delay(self, range_hz=[20, 20e3], mode: str = 'parallel',
+                         length_samples: int = 2048,
                          test_zi: bool = False, zero_phase: bool = False,
                          returns: bool = False):
         """Plots the phase response of each filter.
 
         Parameters
         ----------
+        range_hz : array-like, optional
+            Range of Hz to plot. Default: [20, 20e3].
         mode : str, optional
             Way to apply filter bank to the signal. Supported modes are:
             `'parallel'`. Default: `'parallel'`.
-        range_hz : array-like, optional
-            Range of Hz to plot. Default: [20, 20e3].
+        length_samples : int, optional
+            Impulse length in samples. This defines the resolution of the
+            plot. Default: 2048.
         test_zi : bool, optional
             Uses the zi's of each filter to test the FilterBank's output.
             Default: `False`.
         zero_phase : bool, optional
             Activates zero phase filtering. Default: `False`.
         returns : bool, optional
             When `True`, the figure and axis are returned. Default: `False`.
@@ -469,18 +470,17 @@
         fig, ax
             Returned only when `returns=True`.
 
         """
         mode = mode.lower()
         assert mode in ('parallel', 'summed'), \
             f'{mode} is not supported. Use either parallel or summed'
-        length_samples = 1024
         d = dirac(
             length_samples=length_samples,
-            number_of_channels=1, sampling_rate_hz=48000)
+            number_of_channels=1, sampling_rate_hz=self.sampling_rate_hz)
         if mode == 'parallel':
             bs = self.filter_signal(d, mode='parallel', activate_zi=test_zi,
                                     zero_phase=zero_phase)
             gd = []
             f = bs.bands[0].get_spectrum()[0]
             for b in bs.bands:
                 gd.append(_group_delay_direct(
@@ -744,15 +744,15 @@
             'Two synthesis filters are needed in a crossover'
         assert all([type(n) == Filter for n in new_filters]), \
             'Filters have to be of type Filter'
         self.__filters_synthesis = new_filters
 
     # ======== Filtering ======================================================
     def filter_signal(self, signal: Signal, mode: str = 'parallel',
-                      activate_zi: bool = False, downsample: bool = True) \
+                      activate_zi: bool = False, downsample: bool = False) \
             -> Signal | MultiBandSignal:
         if not downsample:
             return super().filter_signal(
                 signal, mode, activate_zi, zero_phase=False)
         # ========== In case of downsampling while filtering ==================
         mode = mode.lower()
         assert mode in ('parallel', 'sequential', 'summed'), \
@@ -764,27 +764,27 @@
                 self.initialize_zi(signal.number_of_channels)
         new_sig = _crossover_downsample(
             signal, self.filters, mode=mode, down_factor=2)
         return new_sig
 
     # ======== Reconstructing =================================================
     def reconstruct_signal(self, signal: MultiBandSignal,
-                           upsample: bool = True):
+                           upsample: bool = False):
         """Reconstructs a two band signal using the synthesis filters of the
         crossover.
 
         Parameters
         ----------
         signal : `MultiBandSignal`
             Multi-band signal containing two bands from which to reconstruct
             the original signal. It is assumed that the first band is the
             low-frequency content.
         upsample : bool, optional
             When `True`, the signal's sampling rate is doubled.
-            Default: `True`.
+            Default: `False`.
 
         Returns
         -------
         reconstructed : `Signal`
             Reconstructed signal.
 
         """
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/filterbanks/filterbanks.py` & `dsptoolbox-0.2.5/dsptoolbox/filterbanks/filterbanks.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,27 +32,27 @@
         internal methods.
 
     """
     return LRFilterBank(crossover_frequencies_hz, order, sampling_rate_hz)
 
 
 def reconstructing_fractional_octave_bands(
-        octave_fraction: int = 1, frequency_range_hz=[63, 16000],
+        frequency_range_hz=[63, 16000], octave_fraction: int = 1,
         overlap: float = 1, slope: int = 0, n_samples: int = 2**11,
         sampling_rate_hz: int = None) -> FilterBank:
     """Create a perfect reconstruction filter bank with linear-phase
     characteristics. According to (Antoni J., 2010). This implementation is
     taken from the pyfar package. See references for more information about it.
 
     Parameters
     ----------
-    octave_fraction : int, optional
-        Octave fraction used to define bandwidth. Default: 1.
     frequency_range_hz : tuple, optional
         Frequency range in Hz. Default:[ 63, 16e3].
+    octave_fraction : int, optional
+        Octave fraction used to define bandwidth. Default: 1.
     overlap : float, optional
         Band overlap of the filter slopes between 0 and 1. Smaller values yield
         wider pass-bands and steeper filter slopes. Default: 1.
     slope : int, optional
         Number > 0 that defines the width and steepness of the filter slopes.
         Larger values yield wider pass-bands and steeper filter slopes.
         Default: 0.
@@ -263,15 +263,15 @@
     Parameters
     ----------
     lowpass : `Filter`
         Lowpass filter prototype with which to create the other filters.
 
     Returns
     -------
-    fb : `QMFilterBank`
+    fb : `QMFCrossover`
         Quadrature mirror filters crossover.
 
     References
     ----------
     - https://ccrma.stanford.edu/~jos/sasp/Quadrature_Mirror_Filters_QMF.html
 
     """
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/generators/generators.py` & `dsptoolbox-0.2.5/dsptoolbox/generators/generators.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/plots/plots.py` & `dsptoolbox-0.2.5/dsptoolbox/plots/plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/room_acoustics/__init__.py` & `dsptoolbox-0.2.5/dsptoolbox/room_acoustics/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/room_acoustics/_room_acoustics.py` & `dsptoolbox-0.2.5/dsptoolbox/room_acoustics/_room_acoustics.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,15 +513,15 @@
 
         Returns
         -------
         modes : np.ndarray
             Array containing the frequencies of the room modes as well as
             their characteristics (orders in each room dimension. This is
             necessary to know if it is an axial, a tangential or oblique mode).
-            Its shape is (frequency, order x, order y, order z)
+            Its shape is (mode, frequency and order xyz).
 
         """
         max_order += 1
         modes = np.zeros((max_order**3, 4))
         counter = 0
 
         max_order_loop = np.arange(max_order)
@@ -566,15 +566,15 @@
 
         Returns
         -------
         p : `np.ndarray`
             Complex transfer function, non-normalized.
         modes : `np.ndarray`
             Modes for which the transfer function was computed. It has shape
-            (frequency_hz, order x, order y, order z) and it is sorted by
+            (mode, frequency and order xyz) and it is sorted by
             frequency.
         plot : tuple
             When `generate_plot=True`, this is a tuple containing two entries:
             `(matplotlib.figure.Figure, matplotlib.axes.Axes)`. When `False`,
             `None` is returned as the content of the tuple
 
         """
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/room_acoustics/room_acoustics.py` & `dsptoolbox-0.2.5/dsptoolbox/room_acoustics/room_acoustics.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 
     Parameters
     ----------
     rir : `Signal` or `MultiBandSignal`
         Room impulse response. If it is a multi-channel signal, the descriptor
         given back has the shape (channel). If it is a `MultiBandSignal`,
         the descriptor has shape (band, channel).
-    mode : {'d50', 'c80', 'br', 'ts', 'g'} str, optional
+    mode : {'d50', 'c80', 'br', 'ts'} str, optional
         This defines the descriptor to be computed. Options are:
         - `'d50'`: Definition. It takes values between [0, 1] and should
           correlate (positively) with speech inteligibility.
         - `'c80'`: Clarity. It is a value in dB. The higher, the more energy
           arrives in the early part of the RIR compared to the later part.
         - `'br'`: Bass-ratio. It exposes the ratio of reverberation times
           of the lower-frequency octave bands (125, 250) to the higher ones
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/special/__init__.py` & `dsptoolbox-0.2.5/dsptoolbox/special/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,16 @@
   with mel frequency axis)
 - `mel_filterbank()` (returns matrix with triangular mel filters used to
   convert spectrograms' frequency axis from Hz into mel)
 - `plot_waterfall()` (creates and returns a waterfall plot)
 
 """
 from .special import (cepstrum, log_mel_spectrogram, mel_filterbank,
-                      plot_waterfall)
+                      plot_waterfall, mfcc)
 
 __all__ = [
     'cepstrum',
     'log_mel_spectrogram',
     'mel_filterbank',
     'plot_waterfall',
+    'mfcc',
 ]
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/special/special.py` & `dsptoolbox-0.2.5/dsptoolbox/special/special.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Here are methods considered as somewhat special or less common.
 """
 from dsptoolbox.classes.signal_class import Signal
 from dsptoolbox.plots import general_matrix_plot
 from dsptoolbox._general_helpers import _hz2mel, _mel2hz
 
 import numpy as np
+from scipy.fft import dct
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes
 from seaborn import set_style
 set_style('whitegrid')
 
 
@@ -139,16 +140,16 @@
         When `True`, the bands are area normalized for preserving approximately
         same energy in each band. Default: `True`.
 
     Returns
     -------
     mel_filters : `np.ndarray`
         Mel filters matrix with shape (bands, frequency).
-    bands_mel : `np.ndarray`
-        Vector containing mel bands that correspond to the filters.
+    mel_center_freqs : `np.ndarray`
+        Vector containing mel center frequencies.
 
     """
     f_hz = np.squeeze(f_hz)
     assert f_hz.ndim == 1, \
         'f_hz should be a 1D-array'
     n_bands = int(n_bands)
 
@@ -164,19 +165,19 @@
             f'Upper frequency in range {range_hz[-1]} is bigger than ' +\
             f'nyquist frequency {f_hz[-1]}'
         assert range_hz[0] >= 0, \
             'Lower frequency in range must be positive'
 
     # Compute band center frequencies in mel
     range_mel = _hz2mel(range_hz)
-    bands_mel = np.linspace(
+    mel_center_freqs = np.linspace(
         range_mel[0], range_mel[1], n_bands+2, endpoint=True)
 
     # Center frequencies in Hz
-    bands_hz = _mel2hz(bands_mel)
+    bands_hz = _mel2hz(mel_center_freqs)
 
     # Find indexes for frequencies
     inds = np.empty_like(bands_hz, dtype=int)
     for ind, b in enumerate(bands_hz):
         inds[ind] = np.argmin(np.abs(b - f_hz))
 
     # Create triangle filters
@@ -185,15 +186,15 @@
         ni = n+1
         mel_filters[n, inds[ni-1]:inds[ni]] = \
             np.linspace(0, 1, inds[ni]-inds[ni-1], endpoint=False)
         mel_filters[n, inds[ni]:inds[ni+1]] = \
             np.linspace(1, 0, inds[ni+1] - inds[ni], endpoint=False)
         if normalize:
             mel_filters[n, :] /= np.sum(mel_filters[n, :])
-    return mel_filters, bands_mel
+    return mel_filters, mel_center_freqs[1:-1]
 
 
 def plot_waterfall(sig: Signal, channel: int = 0,
                    dynamic_range_db: float = 40,
                    stft_parameters: dict = None) -> tuple[Figure, Axes]:
     """Generates and returns a waterfall plot from a signal. The settings
     for the spectrogram saved in the signal are the ones used for the plot
@@ -240,7 +241,96 @@
     ax.plot_surface(tt, ff, 20*np.log10(stft), cmap='magma')
     ax.set_xlabel('Time / s')
     ax.set_ylabel('Frequency / Hz')
     ax.set_zlabel('dB'+z_label_extra)
     fig.tight_layout()
     # fig.colorbar(surface, ax=ax, shrink=0.4, aspect=10)
     return fig, ax
+
+
+def mfcc(signal: Signal, channel: int = 0,
+         mel_filters: np.ndarray = None, generate_plot: bool = True,
+         stft_parameters: dict = None):
+    """Mel-frequency cepstral coefficients for a windowed signal are computed
+    and returned using the discrete cosine transform of type 2 (see
+    `scipy.fft.dct` for more details).
+
+    Parameters
+    ----------
+    signal : `Signal`
+        The signal for which to compute the mel-frequency cepstral
+        coefficients.
+    channel : int, optional
+        Channel of the signal for which to compute the MFCC. Default: 0.
+    mel_filters : `np.ndarray`, optional
+        Hz-to-Mel transformation matrix with shape (mel band, frequency Hz).
+        It can be created using `mel_filterbank`. If `None` is passed, the
+        filters are automatically computed regarding the whole
+        available spectrum and dividing it in 40 bands (with normalized
+        amplitudes for energy preserving filters, see `mel_filterbank` for
+        details). Default: `None`.
+    generate_plot : bool, optional
+        When `True`, a plot of the MFCC is generated and returned.
+        Default: `True`.
+    stft_parameters : dict, optional
+        Pass arguments to define computation of STFT. If `None` is passed, the
+        parameters already set in the signal will be used. Refer to
+        `Signal.set_spectrogram_parameters()` for details. Default: `None`.
+
+    Returns
+    -------
+    time_s : `np.ndarray`
+        Time vector.
+    f_mel : `np.ndarray`
+        Frequency vector in mel. If `mel_filters` is passed, this is only a
+        list with entries [0, n_mel_filters].
+    mfcc : `np.ndarray`
+        Mel-frequency cepstral coefficients
+
+    When `generate_plot=True`:
+
+    time_s : `np.ndarray`
+        Time vector.
+    f_mel : `np.ndarray`
+        Frequency vector in mel. If `mel_filters` is passed, this is only a
+        list with entries [0, n_mel_filters].
+    log_mel_sp : `np.ndarray`
+        Log mel spectrogram.
+    fig : `matplotlib.figure.Figure`
+        Figure.
+    ax : `matplotlib.axes.Axes`
+        Axes.
+
+    """
+    if stft_parameters is not None:
+        signal.set_spectrogram_parameters(**stft_parameters)
+    time_s, f, sp = signal.get_spectrogram(channel_number=channel)
+
+    # Get Log power spectrum
+    log_sp = 2*np.log(np.abs(sp))
+
+    # Mel filters
+    if mel_filters is None:
+        mel_filters, f_mel = mel_filterbank(f, None, n_bands=40)
+    else:
+        assert mel_filters.shape[1] == log_sp.shape[0], \
+            f'Shape of the mel filter matrix {mel_filters.shape} does ' +\
+            f'not match the STFT {log_sp.shape}'
+        f_mel = [0, mel_filters.shape[0]]
+
+    # Convert from Hz to Mel
+    log_sp = mel_filters @ log_sp
+
+    # Discrete cosine transform
+    mfcc = np.abs(dct(log_sp, type=2, axis=0))
+
+    # Prune nans
+    np.nan_to_num(mfcc, copy=False, nan=0)
+
+    # Plot and return
+    if generate_plot:
+        fig, ax = general_matrix_plot(
+            mfcc, range_x=[time_s[0], time_s[-1]],
+            range_y=[f_mel[0], f_mel[-1]],
+            xlabel='Time / s', ylabel='Cepstral coefficients', returns=True)
+        return time_s, f_mel, mfcc, fig, ax
+    return time_s, f_mel, mfcc
```

### Comparing `dsptoolbox-0.2.4/dsptoolbox/transfer_functions/__init__.py` & `dsptoolbox-0.2.5/dsptoolbox/transfer_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/transfer_functions/_transfer_functions.py` & `dsptoolbox-0.2.5/dsptoolbox/transfer_functions/_transfer_functions.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/dsptoolbox/transfer_functions/transfer_functions.py` & `dsptoolbox-0.2.5/dsptoolbox/transfer_functions/transfer_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,17 @@
         if keep_original_length:
             new_sig.time_data = _pad_trim(new_sig.time_data, original_length)
     return new_sig
 
 
 def window_ir(signal: Signal, constant_percentage=0.75, exp2_trim: int = 13,
               window_type='hann', at_start: bool = True) -> Signal:
-    """Windows an IR with trimming and selection of constant valued length.
+    """Windows an IR in time while trimming or padding it to an expected
+    length. One half of the window is used for the start and the other for
+    the end.
 
     Parameters
     ----------
     signal: `Signal`
         Signal to window
     constant_percentage: float, optional
         Percentage (between 0 and 1) of the window's length that should be
@@ -136,16 +138,16 @@
     window_type: str, optional
         Window function to be used. Available selection from
         scipy.signal.windows: `barthann`, `bartlett`, `blackman`,
         `boxcar`, `cosine`, `hamming`, `hann`, `flattop`, `nuttall` and
         others. Pass a tuple with window type and extra parameters if needed.
         Default: `hann`.
     at_start: bool, optional
-        Windows the start with a rising window as well as the end.
-        Default: `True`.
+        When `True`, the start is windowed as well as the end. When `False`,
+        only the end is windowed. Default: `True`.
 
     Returns
     -------
     new_sig : `Signal`
         Windowed signal. The used window is also saved under `new_sig.window`.
 
     """
@@ -174,15 +176,15 @@
     new_sig.set_window(window)
     return new_sig
 
 
 def compute_transfer_function(output: Signal, input: Signal, mode='h2',
                               window_length_samples: int = 1024,
                               spectrum_parameters: dict = None) -> \
-        Signal:
+        tuple[Signal, np.ndarray]:
     """Gets transfer function H1, H2 or H3 (for stochastic signals).
     H1: for noise in the output signal. `Gxy/Gxx`.
     H2: for noise in the input signal. `Gyy/Gyx`.
     H3: for noise in both signals. `G_xy / abs(G_xy) * (G_yy/G_xx)**0.5`.
     If the input signal only has one channel, it is assumed to be the input
     for all of the channels of the output.
 
@@ -201,17 +203,19 @@
     spectrum_parameters : dict, optional
         Extra parameters for the computation of the cross spectral densities
         using welch's method. See `Signal.set_spectrum_parameters()`
         for details. Default: empty dictionary.
 
     Returns
     -------
-    tf : `Signal`
+    tf_sig : `Signal`
         Transfer functions as `Signal` object. Coherences are also computed
         and saved in the `Signal` object.
+    tf : `np.ndarray`
+        Complex transfer function as type `np.ndarray`.
 
     """
     mode = mode.casefold()
     assert mode in \
         ('h1'.casefold(), 'h2'.casefold(), 'h3'.casefold()), \
         f'{mode} is not a valid mode. Use H1, H2 or H3'
     assert input.sampling_rate_hz == output.sampling_rate_hz, \
@@ -225,17 +229,18 @@
     else:
         multichannel = True
     if spectrum_parameters is None:
         spectrum_parameters = {}
     assert type(spectrum_parameters) == dict, \
         'Spectrum parameters should be passed as a dictionary'
 
-    H_time = np.zeros((window_length_samples, output.number_of_channels))
     coherence = np.zeros((window_length_samples//2 + 1,
                           output.number_of_channels))
+    tf = np.zeros((window_length_samples//2 + 1,
+                   output.number_of_channels), dtype='cfloat')
     if multichannel:
         G_xx = _welch(
             input.time_data[:, 0],
             input.time_data[:, 0],
             input.sampling_rate_hz,
             window_length_samples=window_length_samples,
             **spectrum_parameters)
@@ -267,25 +272,24 @@
             input.time_data[:, n_input],
             output.time_data[:, n],
             output.sampling_rate_hz,
             window_length_samples=window_length_samples,
             **spectrum_parameters)
 
         if mode == 'h1'.casefold():
-            H_time[:, n] = np.fft.irfft(G_xy / G_xx)
+            tf[:, n] = G_xy / G_xx
         elif mode == 'h2'.casefold():
-            H_time[:, n] = np.fft.irfft(G_yy / G_yx)
+            tf[:, n] = G_yy / G_yx
         elif mode == 'h3'.casefold():
-            H_time[:, n] = np.fft.irfft(
-                G_xy / np.abs(G_xy) * (G_yy/G_xx)**0.5)
+            tf[:, n] = G_xy / np.abs(G_xy) * (G_yy/G_xx)**0.5
         coherence[:, n] = np.abs(G_xy)**2 / G_xx / G_yy
-    tf = Signal(None, H_time, output.sampling_rate_hz,
-                signal_type=mode.lower())
-    tf.set_coherence(coherence)
-    return tf
+    tf_sig = Signal(None, np.fft.irfft(tf, axis=0), output.sampling_rate_hz,
+                    signal_type=mode.lower())
+    tf_sig.set_coherence(coherence)
+    return tf_sig, tf
 
 
 def spectral_average(signal: Signal) -> Signal:
     """Averages all channels of a given IR using their magnitude and
     phase spectra and returns the averaged IR.
 
     Parameters
```

### Comparing `dsptoolbox-0.2.4/examples/general.ipynb` & `dsptoolbox-0.2.5/examples/general.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/examples/data/array.xml` & `dsptoolbox-0.2.5/examples/data/array.xml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/examples/data/chirp.wav` & `dsptoolbox-0.2.5/examples/data/chirp.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/examples/data/chirp_mono.wav` & `dsptoolbox-0.2.5/examples/data/chirp_mono.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/examples/data/chirp_stereo.wav` & `dsptoolbox-0.2.5/examples/data/chirp_stereo.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/examples/data/rir.wav` & `dsptoolbox-0.2.5/examples/data/rir.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/examples/data/speech.flac` & `dsptoolbox-0.2.5/examples/data/speech.flac`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/tests/manual_filter_testing.py` & `dsptoolbox-0.2.5/tests/manual_filter_testing.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/tests/manual_testing.py` & `dsptoolbox-0.2.5/tests/manual_testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,20 +518,20 @@
     # g.plot_points()
 
     # Steering vector
     st = dsp.beamforming.SteeringVector(formulation='classic')
     k = np.linspace(800, 1000, 10) * 2 * np.pi / 343
     h = st.get_vector(k, g, ma)
     print(h.shape)
-    st = dsp.beamforming.SteeringVector(formulation='inverse')
+    st = dsp.beamforming.SteeringVector(formulation='true power')
     h = st.get_vector(k, g, ma)
     print(h.shape)
-    # print('Grid: ', g.coordinates.shape)
-    # print('Mics: ', ma.coordinates.shape)
-    # print('k: ', k.shape)
+    print('Grid: ', g.coordinates.shape)
+    print('Mics: ', ma.coordinates.shape)
+    print('k: ', k.shape)
 
     # Beamformer
     noise = dsp.generators.noise(
         number_of_channels=ma.number_of_points, sampling_rate_hz=20_000)
     bf = dsp.beamforming.BeamformerDASFrequency(noise, ma, g, st)
     bf.plot_setting()
     bf.show_info()
@@ -782,15 +782,15 @@
     grid = dsp.beamforming.Regular2DGrid(line, line, ('x', 'y'), ap)
     st = dsp.beamforming.SteeringVector('true power')
 
     bf = dsp.beamforming.BeamformerCleanSC(s_out, ma, grid, st)
     bf.plot_setting()
     map = bf.get_beamformer_map(
         center_frequency_hz=1500, octave_fraction=0, maximum_iterations=100,
-        safety_factor=0.5, remove_diagonal_csm=True)
+        safety_factor=0.5, remove_csm_diagonal=True)
     grid.plot_map(map, range_db=60)
     bf = dsp.beamforming.BeamformerDASFrequency(s_out, ma, grid, st)
     map = bf.get_beamformer_map(center_frequency_hz=1500, octave_fraction=0)
     grid.plot_map(map, range_db=60)
     bf = dsp.beamforming.BeamformerOrthogonal(s_out, ma, grid, st)
     map = bf.get_beamformer_map(center_frequency_hz=1500, octave_fraction=0)
     grid.plot_map(map, range_db=60)
@@ -829,14 +829,24 @@
     mb = fb.filter_signal(s, mode='parallel')
     for n in mb:
         print(type(n))
     for n in fb:
         print(type(n))
 
 
+def mfcc():
+    sp = dsp.Signal(join('examples', 'data', 'speech.flac'))
+    t, f, s = sp.get_spectrogram()
+
+    mels, _ = dsp.special.mel_filterbank(f, [20, 10e3], n_bands=40)
+    t, mel, mf, fig, ax = dsp.special.mfcc(sp, mel_filters=mels)
+
+    dsp.plots.show()
+
+
 if __name__ == '__main__':
     # transfer_function_test()
     # new_transfer_functions()
     # welch_method()
     # csm()
     # group_delay()
     # stft()
@@ -868,10 +878,11 @@
     # beamforming_complete_test_2D()
     # beamforming_complete_test_time()
     # cepstrum()
     # beamforming_3d_grid()
     # beamforming_frequency_formulations()
     # detrending()
     # iterators()
+    # mfcc()
 
     # Next
     print()
```

### Comparing `dsptoolbox-0.2.4/tests/test_beamforming.py` & `dsptoolbox-0.2.5/tests/test_beamforming.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             assert False
 
         # Create beamformer and plot setting
         bf = dsp.beamforming.BeamformerCleanSC(s, ma, g, st)
         # Get and show map
         bf.get_beamformer_map(
             2000, 0, maximum_iterations=10, safety_factor=0.5,
-            remove_diagonal_csm=True)
+            remove_csm_diagonal=True)
 
     def test_beamformer_time(self):
         # Only functionality
         # Mic Array
         ma = self.points_uniform.copy()
         ma['z'] = np.zeros(len(ma['x']))
         ma = dsp.beamforming.MicArray(ma)
```

### Comparing `dsptoolbox-0.2.4/tests/test_classes.py` & `dsptoolbox-0.2.5/tests/test_classes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -199,20 +199,20 @@
         f, csm = s.get_csm()
 
     def test_get_stft(self):
         s = dsp.Signal(time_data=self.time_vec, sampling_rate_hz=self.fs)
         # Use parameters just like librosa for validation
         s.set_spectrogram_parameters(
             channel_number=0, window_length_samples=1024,
-            window_type='hann', overlap_percent=50, fft_length_samples=None,
+            window_type='hann', overlap_percent=50, fft_length_samples=4096,
             detrend=False, padding=False, scaling=False)
         t, f, stft = s.get_spectrogram()
         s.set_spectrogram_parameters(
             channel_number=0, window_length_samples=1024,
-            window_type='hann', overlap_percent=50, fft_length_samples=4096,
+            window_type='hann', overlap_percent=50, fft_length_samples=None,
             detrend=False, padding=False, scaling=False)
         t, f, stft = s.get_spectrogram()
 
         # Validate result with librosa library if installed
         try:
             import librosa
             y = librosa.stft(
```

### Comparing `dsptoolbox-0.2.4/tests/test_distances.py` & `dsptoolbox-0.2.5/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/tests/test_filterbanks.py` & `dsptoolbox-0.2.5/tests/test_filterbanks.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/tests/test_generators.py` & `dsptoolbox-0.2.5/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/tests/test_room_acoustics.py` & `dsptoolbox-0.2.5/tests/test_room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/tests/test_special.py` & `dsptoolbox-0.2.5/tests/test_special.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,7 +48,15 @@
     def test_plot_waterfall(self):
         # Only functionality
         dsp.special.plot_waterfall(self.speech)
         with pytest.raises(AssertionError):
             dsp.special.plot_waterfall(self.speech, dynamic_range_db=-10)
         dsp.special.plot_waterfall(
             self.speech, stft_parameters=dict(window_type=('chebwin', 40)))
+
+    def test_mfcc(self):
+        # Only functionality
+        t, f, s = self.speech.get_spectrogram()
+
+        mels, _ = dsp.special.mel_filterbank(f, [20, 10e3], n_bands=4)
+        t, mel, mf, fig, ax = dsp.special.mfcc(self.speech, mel_filters=mels)
+        t, mel, mf = dsp.special.mfcc(self.speech, generate_plot=False)
```

### Comparing `dsptoolbox-0.2.4/tests/test_standard.py` & `dsptoolbox-0.2.5/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/tests/test_transfer_functions.py` & `dsptoolbox-0.2.5/tests/test_transfer_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             self.y_st, self.x, mode='H1', window_length_samples=1024,
             spectrum_parameters=None)
         # Single-channel with other windows
         h = dsp.transfer_functions.compute_transfer_function(
             self.y_m, self.x, mode='H2', window_length_samples=1024,
             spectrum_parameters=dict(window_type=('chebwin', 40)))
         # Check that coherence is saved
-        h.get_coherence()
+        h[0].get_coherence()
 
     def test_spectral_average(self):
         # Only functionality is tested
         h = dsp.transfer_functions.spectral_deconvolve(self.y_st, self.x)
         h.plot_phase()
         h = dsp.transfer_functions.spectral_average(h)
         h.plot_phase()
```

### Comparing `dsptoolbox-0.2.4/LICENSE` & `dsptoolbox-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/README.rst` & `dsptoolbox-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/pyproject.toml` & `dsptoolbox-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.4/PKG-INFO` & `dsptoolbox-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsptoolbox
-Version: 0.2.4
+Version: 0.2.5
 Summary: Collection of dsp algorithms to be used for analysis of audio signals
 Project-URL: Homepage, https://github.com/nico-franco-gomez/dsptoolbox
 Project-URL: Bug Tracker, https://github.com/nico-franco-gomez/dsptoolbox/issues
 Project-URL: Documentation, https://dsptoolbox.readthedocs.io/en/latest/
 Author: Nicolas Franco-Gomez
 License-Expression: MIT
 License-File: LICENSE
```

