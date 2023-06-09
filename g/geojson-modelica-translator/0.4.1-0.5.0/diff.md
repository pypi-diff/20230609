# Comparing `tmp/geojson_modelica_translator-0.4.1.tar.gz` & `tmp/geojson_modelica_translator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson_modelica_translator-0.4.1.tar", max compression
+gzip compressed data, was "geojson_modelica_translator-0.5.0.tar", max compression
```

## Comparing `geojson_modelica_translator-0.4.1.tar` & `geojson_modelica_translator-0.5.0.tar`

### file list

```diff
@@ -1,187 +1,202 @@
--rw-r--r--   0        0        0     5501 2023-03-13 19:30:06.533373 geojson_modelica_translator-0.4.1/LICENSE.md
--rw-r--r--   0        0        0     5912 2022-07-18 20:07:47.609250 geojson_modelica_translator-0.4.1/README.rst
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.602417 geojson_modelica_translator-0.4.1/geojson_modelica_translator/__init__.py
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.608869 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/__init__.py
--rw-r--r--   0        0        0    21238 2022-04-27 21:48:45.736618 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/building_properties.json
--rw-r--r--   0        0        0     4477 2022-04-18 22:19:44.856964 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/district_system_properties.json
--rw-r--r--   0        0        0     5820 2022-04-18 22:19:44.857230 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/electrical_connector_properties.json
--rw-r--r--   0        0        0     1679 2021-03-23 22:50:43.555533 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/electrical_junction_properties.json
--rw-r--r--   0        0        0     2326 2021-03-22 17:09:40.711956 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/region_properties.json
--rw-r--r--   0        0        0     2510 2022-04-18 22:19:44.857555 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/site_properties.json
--rw-r--r--   0        0        0     2869 2021-03-23 22:50:43.555931 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/thermal_connector_properties.json
--rw-r--r--   0        0        0     2236 2021-03-23 22:50:43.556356 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/thermal_junction_properties.json
--rw-r--r--   0        0        0     1676 2023-03-13 19:30:06.539032 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/schemas.py
--rw-r--r--   0        0        0     3260 2023-03-13 19:30:06.539626 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/urbanopt_geojson.py
--rw-r--r--   0        0        0     5847 2023-03-13 19:30:06.540335 geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson_modelica_translator.py
--rw-r--r--   0        0        0      287 2023-03-13 19:30:06.541020 geojson_modelica_translator-0.4.1/geojson_modelica_translator/jinja_filters.py
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.596404 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/__init__.py
--rw-r--r--   0        0        0     2214 2022-11-07 14:12:33.904938 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0     1218 2022-11-07 14:12:33.905170 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0      273 2023-03-13 19:30:06.541737 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/__init__.py
--rw-r--r--   0        0        0     7109 2023-03-13 19:30:06.542467 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/coupling.py
--rw-r--r--   0        0        0    21075 2023-03-13 19:30:06.543266 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/diagram.py
--rw-r--r--   0        0        0     5112 2023-03-13 19:30:06.543845 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/graph.py
--rw-r--r--   0        0        0       70 2021-03-14 00:14:54.963794 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_Network2Pipe/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      470 2021-03-14 00:14:54.964070 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_Network2Pipe/ConnectStatements.mopt
--rw-r--r--   0        0        0      388 2021-03-14 00:14:54.964356 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_NetworkChilledWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      460 2021-03-14 00:14:54.964580 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_NetworkChilledWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0       70 2021-03-14 00:14:54.965478 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_Network2Pipe/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      472 2021-03-14 00:14:54.965633 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_Network2Pipe/ConnectStatements.mopt
--rw-r--r--   0        0        0      488 2021-03-14 00:14:54.965822 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_NetworkHeatedWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      457 2021-03-14 00:14:54.965961 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_NetworkHeatedWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0       46 2021-03-14 00:14:54.966128 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      946 2021-03-14 00:14:54.966237 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ConnectStatements.mopt
--rw-r--r--   0        0        0      914 2022-11-07 13:45:19.274215 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      759 2021-03-14 00:14:54.966508 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ConnectStatements.mopt
--rw-r--r--   0        0        0      439 2022-07-18 20:07:47.614321 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ComponentDefinitions.mopt
--rw-r--r--   0        0        0     1183 2022-07-18 20:07:47.614452 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ConnectStatements.mopt
--rw-r--r--   0        0        0     1003 2022-11-07 13:45:19.274477 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ComponentDefinitions.mopt
--rw-r--r--   0        0        0     1133 2022-07-18 20:07:47.614785 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ConnectStatements.mopt
--rw-r--r--   0        0        0     1353 2022-07-18 20:07:47.615510 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      636 2022-04-27 21:48:45.742594 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      265 2021-05-06 14:53:19.413863 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      541 2021-03-14 00:14:54.966779 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0      265 2021-03-14 00:14:54.966937 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      540 2021-03-14 00:14:54.967052 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0     1440 2022-07-18 20:07:47.615776 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      633 2022-04-27 21:48:45.743210 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0     1360 2022-07-18 20:07:47.615997 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      639 2022-04-27 21:48:45.743822 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      265 2021-05-06 14:53:20.732123 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      544 2021-03-14 00:14:54.967320 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0      265 2021-05-06 14:52:26.050913 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      543 2021-03-14 00:14:54.967575 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0     1443 2022-07-18 20:07:47.616197 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      635 2022-04-27 21:48:45.744794 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      562 2022-07-18 20:07:47.616508 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      546 2021-03-14 00:14:54.967864 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      610 2022-07-18 20:07:47.616719 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      542 2021-03-14 00:14:54.968121 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0     1310 2022-11-07 13:45:16.520801 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      682 2021-03-14 00:14:54.968406 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      246 2022-11-07 13:45:16.521273 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      541 2022-11-07 14:12:33.906104 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0      292 2022-11-07 13:45:16.521689 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      540 2021-03-14 00:14:54.968920 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0     1453 2022-11-07 13:45:16.522323 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      682 2022-11-07 14:12:33.906568 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0     3618 2023-03-13 19:30:06.544501 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/utils.py
--rw-r--r--   0        0        0      226 2023-03-13 19:30:06.545033 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/districts/__init__.py
--rw-r--r--   0        0        0     6559 2023-03-13 19:30:06.546205 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/districts/district.py
--rw-r--r--   0        0        0     1883 2022-11-07 14:12:33.907384 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem.mot
--rw-r--r--   0        0        0     2125 2022-11-07 14:12:33.907581 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem5G.mot
--rw-r--r--   0        0        0      427 2023-03-13 19:30:06.547411 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/__init__.py
--rw-r--r--   0        0        0     2998 2023-03-13 19:30:06.548009 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/cooling_indirect.py
--rw-r--r--   0        0        0      698 2023-03-13 19:30:06.548545 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/energy_transfer_base.py
--rw-r--r--   0        0        0     1098 2023-03-13 19:30:06.549448 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_cold_water_stub.py
--rw-r--r--   0        0        0     1142 2023-03-13 19:30:06.550615 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_hot_water_stub.py
--rw-r--r--   0        0        0     2998 2023-03-13 19:30:06.551345 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/heating_indirect.py
--rw-r--r--   0        0        0    16170 2023-03-01 22:57:24.166459 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect.mot
--rw-r--r--   0        0        0      740 2021-03-14 00:14:54.973713 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect_Instance.mopt
--rw-r--r--   0        0        0      554 2021-03-14 00:14:54.973843 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsColdWaterStub_Instance.mopt
--rw-r--r--   0        0        0      554 2021-03-14 00:14:54.973955 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsHotWaterStub_Instance.mopt
--rw-r--r--   0        0        0    15552 2023-03-01 22:57:24.123438 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect.mot
--rw-r--r--   0        0        0      702 2021-03-14 00:14:54.974692 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect_Instance.mopt
--rw-r--r--   0        0        0      381 2023-03-13 19:30:06.551862 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/__init__.py
--rw-r--r--   0        0        0    12733 2023-03-13 19:30:06.552178 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/load_base.py
--rw-r--r--   0        0        0    11737 2023-03-13 19:30:06.552632 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/spawn.py
--rw-r--r--   0        0        0    32876 2023-03-13 19:30:02.200061 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/teaser.py
--rw-r--r--   0        0        0     3283 2021-03-14 00:14:54.976624 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/RunSpawnCouplingBuilding.most
--rw-r--r--   0        0        0     1606 2021-03-14 00:14:54.977435 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/RunTeaserCouplingBuilding.most
--rw-r--r--   0        0        0    12800 2023-03-01 22:57:24.774790 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnBuilding.mot
--rw-r--r--   0        0        0     5179 2023-03-01 22:57:24.647993 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnCouplingBuilding.mot
--rw-r--r--   0        0        0      747 2022-07-18 20:07:47.623647 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/Spawn_Instance.mopt
--rw-r--r--   0        0        0     8397 2023-03-01 22:57:24.840870 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserBuilding.mot
--rw-r--r--   0        0        0     4925 2023-03-01 22:57:24.735168 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserCouplingBuilding.mot
--rw-r--r--   0        0        0      257 2021-03-14 00:14:54.978638 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/Teaser_Instance.mopt
--rw-r--r--   0        0        0    17143 2023-03-01 22:57:24.685624 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuilding.mot
--rw-r--r--   0        0        0     5827 2023-03-01 22:57:24.711031 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuildingWithETS.mot
--rw-r--r--   0        0        0      116 2021-03-14 00:14:54.979175 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMFT_Instance.mopt
--rw-r--r--   0        0        0     8618 2023-03-01 22:57:24.812245 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMassFlowTemperatures.mot
--rw-r--r--   0        0        0      733 2023-03-13 19:30:02.200330 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeries_Instance.mopt
--rw-r--r--   0        0        0     3183 2023-03-01 22:57:24.856467 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/getPeakMassFlowRate.mo
--rw-r--r--   0        0        0    11839 2023-03-13 19:30:02.201120 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/time_series.py
--rw-r--r--   0        0        0     6821 2023-03-13 19:30:06.553050 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/time_series_mft_ets_coupling.py
--rw-r--r--   0        0        0     7697 2023-03-13 19:30:06.553477 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/model_base.py
--rw-r--r--   0        0        0     1949 2023-03-13 19:30:02.202978 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/__init__.py
--rw-r--r--   0        0        0      893 2023-03-13 19:30:06.553864 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_2_pipe.py
--rw-r--r--   0        0        0      878 2023-03-13 19:30:06.554241 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_ambient_water_stub.py
--rw-r--r--   0        0        0      532 2023-03-13 19:30:06.555175 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_base.py
--rw-r--r--   0        0        0      878 2023-03-13 19:30:06.555907 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_chilled_water_stub.py
--rw-r--r--   0        0        0      875 2023-03-13 19:30:06.556381 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_heated_water_stub.py
--rw-r--r--   0        0        0     1918 2022-07-18 20:07:47.627799 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/templates/Network2Pipe_Instance.mopt
--rw-r--r--   0        0        0      934 2022-11-07 14:12:33.910459 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/templates/NetworkAmbientWaterStub_Instance.mopt
--rw-r--r--   0        0        0      729 2022-11-07 14:12:33.910744 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/templates/NetworkChilledWaterStub_Instance.mopt
--rw-r--r--   0        0        0      935 2022-11-07 14:12:33.911009 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/templates/NetworkHeatedWaterStub_Instance.mopt
--rw-r--r--   0        0        0      294 2023-03-13 19:30:06.556779 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/__init__.py
--rw-r--r--   0        0        0     5224 2023-03-13 19:30:06.557044 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/chp.py
--rw-r--r--   0        0        0     7475 2023-03-13 19:30:06.557732 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/cooling_plant.py
--rw-r--r--   0        0        0      524 2023-03-13 19:30:06.558122 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/plant_base.py
--rw-r--r--   0        0        0     8784 2023-03-01 22:57:24.617004 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/BoilerStage.mo
--rw-r--r--   0        0        0     4805 2023-03-01 22:57:24.473206 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel.mo
--rw-r--r--   0        0        0    20268 2023-03-01 22:57:24.444231 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CentralCoolingPlant.mot
--rw-r--r--   0        0        0    13293 2023-03-01 22:57:24.313411 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CentralHeatingPlant.mo
--rw-r--r--   0        0        0     4440 2023-03-01 22:57:24.267863 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/ChilledWaterPumpSpeed.mo
--rw-r--r--   0        0        0     6161 2023-03-01 22:57:24.348152 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/ChillerStage.mo
--rw-r--r--   0        0        0     3163 2022-07-18 20:07:47.632116 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CoolingPlant_Instance.mopt
--rw-r--r--   0        0        0    10525 2023-03-01 22:57:24.238137 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerParallel.mo
--rw-r--r--   0        0        0    14122 2023-03-01 22:57:24.536678 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerWithBypass.mo
--rw-r--r--   0        0        0    15897 2023-03-01 22:57:24.583743 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlantWithCHP.mot
--rw-r--r--   0        0        0     2060 2022-07-18 20:07:47.633512 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlant_Instance.mopt
--rw-r--r--   0        0        0     6783 2023-03-01 22:57:24.197924 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/HeatingWaterPumpSpeed.mo
--rw-r--r--   0        0        0     2874 2023-03-01 22:57:24.393202 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel.mo
--rw-r--r--   0        0        0      899 2023-03-01 22:57:24.495228 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallelInterface.mo
--rw-r--r--   0        0        0     4245 2023-03-01 22:57:24.371276 geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/ValveParameters.mo
--rw-r--r--   0        0        0     1429 2022-07-18 20:07:47.634451 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mo
--rw-r--r--   0        0        0     1898 2022-07-18 20:07:47.634583 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mos
--rw-r--r--   0        0        0     1659 2022-07-18 20:07:47.634736 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mot
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.634910 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.634988 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACDCConverter.py
--rw-r--r--   0        0        0     2147 2022-11-07 13:45:19.285507 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/ACLine.mot
--rw-r--r--   0        0        0     1911 2023-03-13 19:30:06.558713 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/Lines.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.635434 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.635504 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/capacitors.py
--rw-r--r--   0        0        0     1264 2022-07-18 20:07:47.635668 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/PVPanels.mot
--rw-r--r--   0        0        0     1372 2022-07-18 20:07:47.636161 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/WindTurbine.mot
--rw-r--r--   0        0        0     1156 2022-07-18 20:07:47.636337 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/community_pv.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.636404 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/generators.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.636491 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/grid.py
--rw-r--r--   0        0        0     1788 2022-11-07 14:12:33.911571 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/wind_turbines.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.636777 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/Battery.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.636990 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/DC/Loads/Conductor.py
--rw-r--r--   0        0        0     3754 2022-07-18 20:07:47.637256 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/RenewableSources.mot
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.618734 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/__init__.py
--rw-r--r--   0        0        0     8103 2023-03-13 19:30:06.559223 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/csv_modelica.py
--rw-r--r--   0        0        0    15169 2023-03-13 19:30:06.560097 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/input_parser.py
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.607601 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/__init__.py
--rw-r--r--   0        0        0     4897 2022-11-07 13:45:19.289042 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/runner/Dockerfile
--rw-r--r--   0        0        0     2862 2022-11-07 13:45:19.290384 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/runner/README.md
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.613657 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/runner/__init__.py
--rw-r--r--   0        0        0      243 2022-11-07 13:45:19.292721 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/runner/docker-compose.yml
--rw-r--r--   0        0        0     5354 2023-03-13 19:30:06.560732 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/runner/fmu_runner.py
--rw-r--r--   0        0        0     2125 2022-11-07 13:45:19.294310 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/runner/make.inc
--rw-r--r--   0        0        0     4406 2022-11-07 13:45:19.294631 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/runner/spawn.py
--rwxr-xr-x   0        0        0     3614 2023-03-13 19:30:06.561260 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/lib/runner/spawn_docker.sh
--rw-r--r--   0        0        0      959 2020-09-30 19:56:12.680802 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/model_connectors/templates/RunSpawnBuilding.mot
--rw-r--r--   0        0        0     3060 2022-07-18 20:07:47.638320 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/model_connectors/templates/spawn_fmu.mot
--rw-r--r--   0        0        0    12176 2023-03-13 19:30:06.562069 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/modelica_runner.py
--rw-r--r--   0        0        0     1060 2023-03-13 19:30:06.562685 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/simple_gmt_base.py
--rw-r--r--   0        0        0       85 2020-06-18 17:45:51.984105 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/templates/package.mot
--rw-r--r--   0        0        0      160 2022-11-07 13:45:19.297904 geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/templates/package_base.mot
--rw-r--r--   0        0        0     3040 2023-03-13 19:30:06.563685 geojson_modelica_translator-0.4.1/geojson_modelica_translator/scaffold.py
--rwxr-xr-x   0        0        0    40209 2022-11-07 13:45:19.298965 geojson_modelica_translator-0.4.1/geojson_modelica_translator/system_parameters/schema.json
--rw-r--r--   0        0        0    35776 2023-03-13 19:30:06.564163 geojson_modelica_translator-0.4.1/geojson_modelica_translator/system_parameters/system_parameters.py
--rw-r--r--   0        0        0     3128 2022-11-07 13:45:19.299807 geojson_modelica_translator-0.4.1/geojson_modelica_translator/system_parameters/time_series_microgrid_template.json
--rw-r--r--   0        0        0     2774 2022-11-07 13:45:19.300056 geojson_modelica_translator-0.4.1/geojson_modelica_translator/system_parameters/time_series_template.json
--rw-r--r--   0        0        0     4977 2023-03-13 19:30:06.564971 geojson_modelica_translator-0.4.1/geojson_modelica_translator/utils.py
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.593171 geojson_modelica_translator-0.4.1/management/__init__.py
--rw-r--r--   0        0        0     9963 2023-03-13 19:30:06.565467 geojson_modelica_translator-0.4.1/management/check_sys_params.py
--rw-r--r--   0        0        0     2634 2022-07-18 20:07:47.641868 geojson_modelica_translator-0.4.1/management/data/baseline_geojson.json
--rw-r--r--   0        0        0     5678 2022-11-07 13:45:19.300334 geojson_modelica_translator-0.4.1/management/data/baseline_sys_params.json
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.642053 geojson_modelica_translator-0.4.1/management/data/baseline_time_series.mos
--rw-r--r--   0        0        0  1148813 2022-07-18 20:07:47.647980 geojson_modelica_translator-0.4.1/management/data/baseline_weather.mos
--rw-r--r--   0        0        0     6648 2023-03-13 19:30:06.566021 geojson_modelica_translator-0.4.1/management/format_modelica_files.py
--rw-r--r--   0        0        0     6858 2023-03-13 19:30:06.566660 geojson_modelica_translator-0.4.1/management/uo_des.py
--rw-r--r--   0        0        0     1280 2023-03-13 19:30:06.567076 geojson_modelica_translator-0.4.1/management/update_schemas.py
--rw-r--r--   0        0        0     2706 2023-03-13 19:30:06.569228 geojson_modelica_translator-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7455 1970-01-01 00:00:00.000000 geojson_modelica_translator-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     5237 2023-06-09 02:59:16.640290 geojson_modelica_translator-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     5912 2022-07-18 20:07:47.609250 geojson_modelica_translator-0.5.0/README.rst
+-rw-r--r--   0        0        0        0 2020-06-18 17:43:32.602417 geojson_modelica_translator-0.5.0/geojson_modelica_translator/__init__.py
+-rw-r--r--   0        0        0        0 2020-06-18 17:43:32.608869 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/__init__.py
+-rw-r--r--   0        0        0    21238 2022-04-27 21:48:45.736618 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/building_properties.json
+-rw-r--r--   0        0        0     4477 2022-04-18 22:19:44.856964 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/district_system_properties.json
+-rw-r--r--   0        0        0     5820 2022-04-18 22:19:44.857230 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/electrical_connector_properties.json
+-rw-r--r--   0        0        0     1679 2021-03-23 22:50:43.555533 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/electrical_junction_properties.json
+-rw-r--r--   0        0        0     2326 2021-03-22 17:09:40.711956 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/region_properties.json
+-rw-r--r--   0        0        0     2510 2022-04-18 22:19:44.857555 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/site_properties.json
+-rw-r--r--   0        0        0     2869 2021-03-23 22:50:43.555931 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/thermal_connector_properties.json
+-rw-r--r--   0        0        0     2236 2021-03-23 22:50:43.556356 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/thermal_junction_properties.json
+-rw-r--r--   0        0        0     1681 2023-06-09 02:59:16.642371 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/schemas.py
+-rw-r--r--   0        0        0     3260 2023-03-13 19:30:06.539626 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/urbanopt_geojson.py
+-rw-r--r--   0        0        0     5847 2023-03-13 19:30:06.540335 geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson_modelica_translator.py
+-rw-r--r--   0        0        0      287 2023-03-13 19:30:06.541020 geojson_modelica_translator-0.5.0/geojson_modelica_translator/jinja_filters.py
+-rw-r--r--   0        0        0        0 2020-06-18 17:43:32.596404 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-09 02:59:16.642933 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkAmbientWaterStub_Borefield/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      376 2023-06-09 02:59:16.643166 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkAmbientWaterStub_Borefield/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1913 2023-06-09 02:59:16.643531 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0     1294 2023-06-09 02:59:16.643843 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0      273 2023-03-13 19:30:06.541737 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/__init__.py
+-rw-r--r--   0        0        0     7109 2023-03-13 19:30:06.542467 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/coupling.py
+-rw-r--r--   0        0        0    21075 2023-03-13 19:30:06.543266 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/diagram.py
+-rw-r--r--   0        0        0     5112 2023-03-13 19:30:06.543845 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/graph.py
+-rw-r--r--   0        0        0       70 2021-03-14 00:14:54.963794 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_Network2Pipe/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      470 2021-03-14 00:14:54.964070 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_Network2Pipe/ConnectStatements.mopt
+-rw-r--r--   0        0        0      388 2021-03-14 00:14:54.964356 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_NetworkChilledWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      460 2021-03-14 00:14:54.964580 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_NetworkChilledWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0       70 2021-03-14 00:14:54.965478 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_Network2Pipe/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      472 2021-03-14 00:14:54.965633 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_Network2Pipe/ConnectStatements.mopt
+-rw-r--r--   0        0        0      488 2021-03-14 00:14:54.965822 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_NetworkHeatedWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      457 2021-03-14 00:14:54.965961 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_NetworkHeatedWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0       46 2021-03-14 00:14:54.966128 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      946 2021-03-14 00:14:54.966237 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ConnectStatements.mopt
+-rw-r--r--   0        0        0      914 2022-11-07 13:45:19.274215 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      759 2021-03-14 00:14:54.966508 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ConnectStatements.mopt
+-rw-r--r--   0        0        0      439 2022-07-18 20:07:47.614321 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0     1183 2022-07-18 20:07:47.614452 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1003 2022-11-07 13:45:19.274477 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0     1133 2022-07-18 20:07:47.614785 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1353 2022-07-18 20:07:47.615510 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      636 2022-04-27 21:48:45.742594 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      265 2021-05-06 14:53:19.413863 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      541 2021-03-14 00:14:54.966779 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0      265 2021-03-14 00:14:54.966937 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      540 2021-03-14 00:14:54.967052 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1440 2022-07-18 20:07:47.615776 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      633 2022-04-27 21:48:45.743210 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1360 2022-07-18 20:07:47.615997 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      639 2022-04-27 21:48:45.743822 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      265 2021-05-06 14:53:20.732123 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      544 2021-03-14 00:14:54.967320 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0      265 2021-05-06 14:52:26.050913 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      543 2021-03-14 00:14:54.967575 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1443 2022-07-18 20:07:47.616197 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      635 2022-04-27 21:48:45.744794 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      562 2022-07-18 20:07:47.616508 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      542 2023-06-09 02:59:16.644146 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      610 2022-07-18 20:07:47.616719 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      529 2023-06-09 02:59:16.644529 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1310 2022-11-07 13:45:16.520801 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      682 2021-03-14 00:14:54.968406 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      246 2022-11-07 13:45:16.521273 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      541 2022-11-07 14:12:33.906104 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0      292 2022-11-07 13:45:16.521689 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      540 2021-03-14 00:14:54.968920 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1453 2022-11-07 13:45:16.522323 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      682 2022-11-07 14:12:33.906568 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0     3618 2023-03-13 19:30:06.544501 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/utils.py
+-rw-r--r--   0        0        0      226 2023-03-13 19:30:06.545033 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/districts/__init__.py
+-rw-r--r--   0        0        0     7130 2023-06-09 02:59:16.645388 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/districts/district.py
+-rw-r--r--   0        0        0     1925 2023-06-09 02:59:16.645829 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem.mot
+-rw-r--r--   0        0        0     2212 2023-06-09 02:59:16.646190 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem5G.mot
+-rw-r--r--   0        0        0      427 2023-03-13 19:30:06.547411 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/__init__.py
+-rw-r--r--   0        0        0     2998 2023-03-13 19:30:06.548009 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/cooling_indirect.py
+-rw-r--r--   0        0        0      698 2023-03-13 19:30:06.548545 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/energy_transfer_base.py
+-rw-r--r--   0        0        0     1098 2023-03-13 19:30:06.549448 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_cold_water_stub.py
+-rw-r--r--   0        0        0     1142 2023-03-13 19:30:06.550615 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_hot_water_stub.py
+-rw-r--r--   0        0        0     2998 2023-03-13 19:30:06.551345 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/heating_indirect.py
+-rw-r--r--   0        0        0    16350 2023-06-09 02:59:16.646654 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect.mot
+-rw-r--r--   0        0        0      738 2023-06-09 02:59:16.647026 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect_Instance.mopt
+-rw-r--r--   0        0        0      554 2021-03-14 00:14:54.973843 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsColdWaterStub_Instance.mopt
+-rw-r--r--   0        0        0      554 2021-03-14 00:14:54.973955 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsHotWaterStub_Instance.mopt
+-rw-r--r--   0        0        0    15722 2023-06-09 02:59:16.647357 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect.mot
+-rw-r--r--   0        0        0      700 2023-06-09 02:59:16.647707 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect_Instance.mopt
+-rw-r--r--   0        0        0      381 2023-03-13 19:30:06.551862 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/__init__.py
+-rw-r--r--   0        0        0    10507 2023-06-09 02:59:16.648674 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/load_base.py
+-rw-r--r--   0        0        0    11737 2023-03-13 19:30:06.552632 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/spawn.py
+-rw-r--r--   0        0        0    30617 2023-06-09 02:59:16.649613 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/teaser.py
+-rw-r--r--   0        0        0     3283 2021-03-14 00:14:54.976624 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/RunSpawnCouplingBuilding.most
+-rw-r--r--   0        0        0     1606 2021-03-14 00:14:54.977435 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/RunTeaserCouplingBuilding.most
+-rw-r--r--   0        0        0    12856 2023-06-09 02:59:16.650266 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnBuilding.mot
+-rw-r--r--   0        0        0     5179 2023-06-08 21:28:32.405825 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnCouplingBuilding.mot
+-rw-r--r--   0        0        0      777 2023-06-09 02:59:16.650701 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/Spawn_Instance.mopt
+-rw-r--r--   0        0        0     8397 2023-06-08 21:28:32.637430 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserBuilding.mot
+-rw-r--r--   0        0        0     4925 2023-06-08 21:28:32.522062 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserCouplingBuilding.mot
+-rw-r--r--   0        0        0      257 2021-03-14 00:14:54.978638 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/Teaser_Instance.mopt
+-rw-r--r--   0        0        0    17163 2023-06-09 02:59:16.651133 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuilding.mot
+-rw-r--r--   0        0        0     5864 2023-06-09 02:59:16.651488 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuildingWithETS.mot
+-rw-r--r--   0        0        0      116 2021-03-14 00:14:54.979175 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMFT_Instance.mopt
+-rw-r--r--   0        0        0     9486 2023-06-09 02:59:16.651832 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMassFlowTemperatures.mot
+-rw-r--r--   0        0        0      917 2023-06-09 02:59:16.652150 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeries_Instance.mopt
+-rw-r--r--   0        0        0     3233 2023-06-09 02:59:16.652645 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/getPeakMassFlowRate.mot
+-rw-r--r--   0        0        0     9612 2023-06-09 02:59:16.653464 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/time_series.py
+-rw-r--r--   0        0        0     7163 2023-06-09 02:59:16.653900 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/time_series_mft_ets_coupling.py
+-rw-r--r--   0        0        0     7832 2023-06-09 02:59:16.654326 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/model_base.py
+-rw-r--r--   0        0        0      390 2023-06-09 02:59:16.655120 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/__init__.py
+-rw-r--r--   0        0        0      893 2023-03-13 19:30:06.553864 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_2_pipe.py
+-rw-r--r--   0        0        0      878 2023-03-13 19:30:06.554241 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_ambient_water_stub.py
+-rw-r--r--   0        0        0      532 2023-03-13 19:30:06.555175 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_base.py
+-rw-r--r--   0        0        0      878 2023-03-13 19:30:06.555907 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_chilled_water_stub.py
+-rw-r--r--   0        0        0      875 2023-03-13 19:30:06.556381 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_heated_water_stub.py
+-rw-r--r--   0        0        0     1917 2023-06-09 02:59:16.655491 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/templates/Network2Pipe_Instance.mopt
+-rw-r--r--   0        0        0     1263 2023-06-09 02:59:16.656225 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkAmbientWaterStub_Instance.mopt
+-rw-r--r--   0        0        0      729 2022-11-07 14:12:33.910744 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkChilledWaterStub_Instance.mopt
+-rw-r--r--   0        0        0      935 2022-11-07 14:12:33.911009 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkHeatedWaterStub_Instance.mopt
+-rw-r--r--   0        0        0      294 2023-03-13 19:30:06.556779 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/__init__.py
+-rw-r--r--   0        0        0     9921 2023-06-09 02:59:16.656523 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/borefield.py
+-rw-r--r--   0        0        0     5359 2023-06-09 02:59:16.656859 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/chp.py
+-rw-r--r--   0        0        0     7475 2023-03-13 19:30:06.557732 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/cooling_plant.py
+-rw-r--r--   0        0        0      524 2023-03-13 19:30:06.558122 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/plant_base.py
+-rw-r--r--   0        0        0     8784 2023-06-08 21:28:32.370696 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/BoilerStage.mo
+-rw-r--r--   0        0        0     4815 2023-06-09 02:59:16.657150 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel.mo
+-rw-r--r--   0        0        0    16131 2023-06-09 02:59:16.657646 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/BorefieldOneUTube.mot
+-rw-r--r--   0        0        0    16131 2023-06-09 02:59:16.657846 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/BorefieldTwoUTubes.mot
+-rw-r--r--   0        0        0      133 2023-06-09 02:59:16.658004 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/Borefield_Instance.mopt
+-rw-r--r--   0        0        0    20277 2023-06-09 02:59:16.658311 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CentralCoolingPlant.mot
+-rw-r--r--   0        0        0    13292 2023-06-09 02:59:16.658662 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CentralHeatingPlant.mo
+-rw-r--r--   0        0        0     4455 2023-06-09 02:59:16.659034 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/ChilledWaterPumpSpeed.mo
+-rw-r--r--   0        0        0     6161 2023-06-08 21:28:32.020819 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/ChillerStage.mo
+-rw-r--r--   0        0        0     3189 2023-06-09 02:59:16.659311 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingPlant_Instance.mopt
+-rw-r--r--   0        0        0    10560 2023-06-09 02:59:16.659666 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerParallel.mo
+-rw-r--r--   0        0        0    14157 2023-06-09 02:59:16.659936 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerWithBypass.mo
+-rw-r--r--   0        0        0    16335 2023-06-09 02:59:16.660148 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/GroundTemperatureResponse.mo
+-rw-r--r--   0        0        0    15906 2023-06-09 02:59:16.660512 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlantWithCHP.mot
+-rw-r--r--   0        0        0     2060 2022-07-18 20:07:47.633512 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlant_Instance.mopt
+-rw-r--r--   0        0        0     6798 2023-06-09 02:59:16.660803 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingWaterPumpSpeed.mo
+-rw-r--r--   0        0        0     2874 2023-06-08 21:28:32.115823 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel.mo
+-rw-r--r--   0        0        0      899 2023-06-08 21:28:32.231351 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallelInterface.mo
+-rw-r--r--   0        0        0     4245 2023-06-08 21:28:32.045435 geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/ValveParameters.mo
+-rw-r--r--   0        0        0     1377 2023-06-09 02:59:16.661511 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mo
+-rw-r--r--   0        0        0     1898 2022-07-18 20:07:47.634583 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mos
+-rw-r--r--   0        0        0     1600 2023-06-09 02:59:16.661760 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mot
+-rw-r--r--   0        0        0    14862 2023-06-09 02:59:16.662992 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_partial.mot
+-rw-r--r--   0        0        0     4316 2023-06-09 02:59:16.663974 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.mot
+-rw-r--r--   0        0        0     5320 2023-06-09 02:59:16.665404 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.py
+-rw-r--r--   0        0        0        0 2022-07-18 20:07:47.634910 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.py
+-rw-r--r--   0        0        0        0 2022-07-18 20:07:47.634988 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACDCConverter.py
+-rw-r--r--   0        0        0     2043 2023-06-09 02:59:16.665777 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/ACLine.mot
+-rw-r--r--   0        0        0     1911 2023-03-13 19:30:06.558713 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/Lines.py
+-rw-r--r--   0        0        0     1148 2023-06-09 02:59:16.665929 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Capacitor.mot
+-rw-r--r--   0        0        0     1092 2023-06-09 02:59:16.666056 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.mot
+-rw-r--r--   0        0        0     1354 2023-06-09 02:59:16.666272 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.py
+-rw-r--r--   0        0        0      935 2023-06-09 02:59:16.666399 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/capacitor.py
+-rw-r--r--   0        0        0     1202 2023-06-09 02:59:16.666574 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Generator.mot
+-rw-r--r--   0        0        0     1088 2023-06-09 02:59:16.666860 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Grid.mot
+-rw-r--r--   0        0        0     1228 2023-06-09 02:59:16.667220 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/PVPanels.mot
+-rw-r--r--   0        0        0     1333 2023-06-09 02:59:16.667461 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/WindTurbine.mot
+-rw-r--r--   0        0        0     1156 2022-07-18 20:07:47.636337 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/community_pv.py
+-rw-r--r--   0        0        0     1483 2023-06-09 02:59:16.667679 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/generators.py
+-rw-r--r--   0        0        0      958 2023-06-09 02:59:16.667963 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/grid.py
+-rw-r--r--   0        0        0     1788 2022-11-07 14:12:33.911571 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/wind_turbines.py
+-rw-r--r--   0        0        0     1040 2023-06-09 02:59:16.668147 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/AcBattery.mot
+-rw-r--r--   0        0        0     1179 2023-06-09 02:59:16.668362 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/Battery.py
+-rw-r--r--   0        0        0        0 2022-07-18 20:07:47.636990 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/DC/Loads/Conductor.py
+-rw-r--r--   0        0        0     3754 2022-07-18 20:07:47.637256 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/RenewableSources.mot
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:45.425849 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/__init__.py
+-rw-r--r--   0        0        0     8103 2023-03-13 19:30:06.559223 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/csv_modelica.py
+-rw-r--r--   0        0        0    15380 2023-06-09 02:59:16.669182 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/input_parser.py
+-rw-r--r--   0        0        0        0 2020-06-18 17:43:32.607601 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/lib/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-09 02:59:16.669488 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/lib/runner/Dockerfile
+-rw-r--r--   0        0        0      996 2023-06-09 02:59:16.669756 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/lib/runner/README.md
+-rw-r--r--   0        0        0        0 2020-06-18 17:43:32.613657 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/lib/runner/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-09 02:59:16.669975 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/lib/runner/compile_fmu.most
+-rw-r--r--   0        0        0     6045 2023-06-09 02:59:16.670462 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/lib/runner/om.py
+-rwxr-xr-x   0        0        0     4175 2023-06-09 02:59:16.670611 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/lib/runner/om_docker.sh
+-rw-r--r--   0        0        0      522 2023-06-09 02:59:16.670733 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/lib/runner/simulate.most
+-rw-r--r--   0        0        0      959 2020-09-30 19:56:12.680802 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/model_connectors/templates/RunSpawnBuilding.mot
+-rw-r--r--   0        0        0     3060 2022-07-18 20:07:47.638320 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/model_connectors/templates/spawn_fmu.mot
+-rw-r--r--   0        0        0     3691 2023-06-09 02:59:16.671287 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/modelica_mos_file.py
+-rw-r--r--   0        0        0    14455 2023-06-09 02:59:16.671716 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/modelica_runner.py
+-rw-r--r--   0        0        0     3031 2023-06-09 02:59:16.672352 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/simple_gmt_base.py
+-rw-r--r--   0        0        0       85 2020-06-18 17:45:51.984105 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/templates/package.mot
+-rw-r--r--   0        0        0      160 2022-11-07 13:45:19.297904 geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/templates/package_base.mot
+-rw-r--r--   0        0        0     3802 2023-06-09 02:59:16.672705 geojson_modelica_translator-0.5.0/geojson_modelica_translator/scaffold.py
+-rwxr-xr-x   0        0        0    52826 2023-06-09 02:59:16.673652 geojson_modelica_translator-0.5.0/geojson_modelica_translator/system_parameters/schema.json
+-rw-r--r--   0        0        0    36705 2023-06-09 02:59:16.674943 geojson_modelica_translator-0.5.0/geojson_modelica_translator/system_parameters/system_parameters.py
+-rw-r--r--   0        0        0     3164 2023-06-09 02:59:16.675852 geojson_modelica_translator-0.5.0/geojson_modelica_translator/system_parameters/time_series_microgrid_template.json
+-rw-r--r--   0        0        0     2810 2023-06-09 02:59:16.676142 geojson_modelica_translator-0.5.0/geojson_modelica_translator/system_parameters/time_series_template.json
+-rw-r--r--   0        0        0     4977 2023-03-13 19:30:06.564971 geojson_modelica_translator-0.5.0/geojson_modelica_translator/utils.py
+-rw-r--r--   0        0        0        0 2020-06-18 17:43:32.593171 geojson_modelica_translator-0.5.0/management/__init__.py
+-rw-r--r--   0        0        0     9963 2023-03-13 19:30:06.565467 geojson_modelica_translator-0.5.0/management/check_sys_params.py
+-rw-r--r--   0        0        0     2634 2022-07-18 20:07:47.641868 geojson_modelica_translator-0.5.0/management/data/baseline_geojson.json
+-rw-r--r--   0        0        0     5678 2022-11-07 13:45:19.300334 geojson_modelica_translator-0.5.0/management/data/baseline_sys_params.json
+-rw-r--r--   0        0        0        0 2022-07-18 20:07:47.642053 geojson_modelica_translator-0.5.0/management/data/baseline_time_series.mos
+-rw-r--r--   0        0        0  1148813 2022-07-18 20:07:47.647980 geojson_modelica_translator-0.5.0/management/data/baseline_weather.mos
+-rw-r--r--   0        0        0     6648 2023-03-13 19:30:06.566021 geojson_modelica_translator-0.5.0/management/format_modelica_files.py
+-rw-r--r--   0        0        0     6977 2023-06-09 02:59:16.676452 geojson_modelica_translator-0.5.0/management/uo_des.py
+-rw-r--r--   0        0        0     1280 2023-03-13 19:30:06.567076 geojson_modelica_translator-0.5.0/management/update_schemas.py
+-rw-r--r--   0        0        0     2723 2023-06-09 02:59:16.678389 geojson_modelica_translator-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7315 1970-01-01 00:00:00.000000 geojson_modelica_translator-0.5.0/PKG-INFO
```

### Comparing `geojson_modelica_translator-0.4.1/LICENSE.md` & `geojson_modelica_translator-0.5.0/LICENSE.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 URBANopt™, Copyright (c) 2019, 2023 Alliance for Sustainable Energy, LLC, and other contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted
 provided that the following conditions are met:
 
-Redistributions of source code must retain the above copyright notice, this list of conditions
+(1) Redistributions of source code must retain the above copyright notice, this list of conditions
 and the following disclaimer.
 
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions
+(2) Redistributions in binary form must reproduce the above copyright notice, this list of conditions
 and the following disclaimer in the documentation and/or other materials provided with the
 distribution.
 
-Neither the name of the copyright holder nor the names of its contributors may be used to endorse
+(3) Neither the name of the copyright holder nor the names of its contributors may be used to endorse
 or promote products derived from this software without specific prior written permission.
 
-Redistribution of this software, without modification, must refer to the software by the same
-designation. Redistribution of a modified version of this software (i) may not refer to the
-modified version by the same designation, or by any confusingly similar designation, and
-(ii) must refer to the underlying software originally provided by Alliance as “URBANopt”. Except
-to comply with the foregoing, the term “URBANopt”, or any confusingly similar designation may
-not be used to refer to any modified version of this software or any modified version of the
-underlying software originally provided by Alliance without the prior written consent of Alliance.
+(4) Other than as required in clauses (1) and (2), distributions in any form of modifications or
+other derivative works (i) may not use the "URBANopt" trademark, or any other confusingly
+similar designation without specific prior written permission from Alliance for Sustainable
+Energy, LLC., and (ii) must refer to the underlying software originally provided by
+Alliance as “URBANopt”.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
 IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
 FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
 CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
 OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-
 ---
 This library also uses some examples and components from the Modelica Buildings Library.
 
 Modelica Buildings Library. Copyright (c) 1998-2019
 Modelica Association,
 International Building Performance Simulation Association (IBPSA),
 The Regents of the University of California, through Lawrence Berkeley National Laboratory
```

### Comparing `geojson_modelica_translator-0.4.1/README.rst` & `geojson_modelica_translator-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/building_properties.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/building_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/district_system_properties.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/district_system_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/electrical_connector_properties.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/electrical_connector_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/electrical_junction_properties.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/electrical_junction_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/region_properties.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/region_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/site_properties.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/site_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/thermal_connector_properties.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/thermal_connector_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/data/schemas/thermal_junction_properties.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/data/schemas/thermal_junction_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/schemas.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import json
 import os
 
-from jsonschema.validators import _LATEST_VERSION as LatestValidator
+from jsonschema.validators import Draft202012Validator as LatestValidator
 
 
 class Schemas(object):
     """
     Class to hold the various schemas
     """
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson/urbanopt_geojson.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson/urbanopt_geojson.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/geojson_modelica_translator.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/geojson_modelica_translator.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ComponentDefinitions.mopt`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,21 @@
   // TimeSeries 5G Component Definitions
   // TODO: the components below need to be fixed!
   parameter Modelica.Units.SI.MassFlowRate mDis_flow_nominal_{{ coupling.id }}={{ coupling.load.id }}.bui.mHeaWat_flow_nominal*{{ globals.delHeaWatTemBui }}/{{ globals.delHeaWatTemDis }}
     "Nominal mass flow rate of primary (district) district heating side";
   parameter Modelica.Units.SI.MassFlowRate mBui_flow_nominal_{{ coupling.id }}={{ coupling.load.id }}.bui.mHeaWat_flow_nominal
     "Nominal mass flow rate of secondary (building) district heating side";
   parameter Modelica.Units.SI.HeatFlowRate Q_flow_nominal_{{ coupling.id }}=({{ coupling.load.id }}.bui.QHea_flow_nominal);
-  // Modelica.Fluid.Sources.FixedBoundary pressure_source_{{ coupling.id }}(
-  //   redeclare package Medium={{ globals.medium_w }},
-  //   use_T=false,
-  //   nPorts=1)
-  //   "Pressure source"
-  //   annotation (Placement({{ diagram.transformation.pressure_source.fixed_boundary }}));
-    Modelica.Blocks.Sources.RealExpression secMasFloRat_{{ coupling.id }}(
-    // TODO: avoid reaching into other coupling!
-    // Removed the unexplained *5/7.5, and added a multiplier of 15, to have a flow rate closer to the datDes nominal value
-    y=15*mDis_flow_nominal_{{ graph.couplings_by_type(coupling.load.id).network_couplings[0].id }})
-    "Secondary loop conditioned water flow rate."
-    annotation (Placement({{ diagram.transformation.sec_mas_flo_rat.real_expression }}));
-    // TODO: move THeaWatSet (and its connection) into a specific template file (this component does not depend on the coupling)
+  Modelica.Blocks.Sources.RealExpression secMasFloRat_{{ coupling.id }}(
+  // TODO: avoid reaching into other coupling!
+  // Removed the unexplained *5/7.5, and added a multiplier of 15, to have a flow rate closer to the datDes nominal value
+  y=15*mDis_flow_nominal_{{ graph.couplings_by_type(coupling.load.id).network_couplings[0].id }})
+  "Secondary loop conditioned water flow rate."
+  annotation (Placement({{ diagram.transformation.sec_mas_flo_rat.real_expression }}));
+  // TODO: move THeaWatSet (and its connection) into a specific template file (this component does not depend on the coupling)
   Modelica.Blocks.Sources.RealExpression THeaWatSet_{{ coupling.id }}(
     y=273.15+{{ sys_params.building.load_model_parameters.time_series.temp_hw_supply }})
     "Secondary loop (Building side) heating setpoint temperature."
     annotation (Placement({{ diagram.transformation.t_hea_wat_set.real_expression }}));
   Modelica.Blocks.Sources.RealExpression TCooWatSet_{{ coupling.id }}(
     y=273.15+{{ sys_params.building.load_model_parameters.time_series.temp_chw_supply }})
     "Secondary loop (Building side) cooling setpoint temperature."
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ConnectStatements.mopt`

 * *Files 10% similar despite different names*

```diff
@@ -5,13 +5,13 @@
   annotation ({{ diagram.line.ts_load.t_hea_wat_max_set.t_hea_wat_set.y }});
 connect({{ coupling.load.id }}.THotWatSupSet, THeaWatSet_{{ coupling.id }}.y)
   annotation ({{ diagram.line.ts_load.t_hot_wat_set.t_hea_wat_set.y }});
 connect({{ coupling.load.id }}.TChiWatSupSet, THeaWatSet_{{ coupling.id }}.y)
   annotation ({{ diagram.line.ts_load.t_chi_wat_set.t_hea_wat_set.y }});
 connect(TCooWatSet_{{ coupling.id }}.y, {{ coupling.load.id }}.TColWat)
   annotation ({{ diagram.line.t_coo_wat_set.y.ts_load.t_col_wat }});
-connect(secMasFloRat_{{ coupling.id }}.y, supHeaWat.m_flow_in)
+connect(secMasFloRat_{{ coupling.id }}.y, supHeaWat_{{ sys_params.load_num }}.m_flow_in)
   annotation ({{ diagram.line.sec_mas_flo_rat.y.sup_hea_wat.m_flow_in }});
-connect(supHeaWat.ports[1], {{ coupling.load.id }}.port_aSerAmb)
+connect(supHeaWat_{{ sys_params.load_num }}.ports[1], {{ coupling.load.id }}.port_aSerAmb)
   annotation ({{ diagram.line.sup_hea_wat.ports.ts_load.port_a_amb }});
-connect({{ coupling.load.id }}.port_bSerAmb, sinHeaWat.ports[1])
+connect({{ coupling.load.id }}.port_bSerAmb, sinHeaWat.ports[{{ sys_params.load_num }}])
   annotation ({{ diagram.line.ts_load.port_b_amb.sin_hea_wat.ports }});
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/coupling.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/coupling.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/diagram.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/diagram.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/graph.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/graph.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ConnectStatements.mopt`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
   connect(TChWSET_{{ coupling.id }}.y,{{ coupling.ets.id }}.TSetBuiSup)
     annotation ({{ diagram.line.t_ch_w_set.y.coo_ets.t_set_bui_sup }});
-  connect({{ coupling.load.id }}.buiMasTem.y[4],TChWSET_{{ coupling.id }}.u);
+  connect({{ coupling.load.id }}.realOutput,TChWSET_{{ coupling.id }}.u);
   connect({{ coupling.load.id }}.ports_aChiWat[1],{{ coupling.ets.id }}.port_b2)
     annotation ({{ diagram.line.ts_mft_load.ports_a_chi_wat.coo_ets.port_b2 }});
   connect({{ coupling.ets.id }}.port_a2,{{ coupling.load.id }}.ports_bChiWat[1])
     annotation ({{ diagram.line.coo_ets.port_a2.ts_mft_load.ports_b_chi_wat }});
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ConnectStatements.mopt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-  connect(THWSET_{{ coupling.id }}.y,{{ coupling.ets.id }}.TSetBuiSup)
-    annotation ({{ diagram.line.t_hw_set.y.hea_ets.t_set_bui_sup }});
-  connect({{ coupling.load.id }}.buiMasTem.y[2],THWSET_{{ coupling.id }}.u);
-  connect({{ coupling.load.id }}.ports_aHeaWat[1],{{ coupling.ets.id }}.port_b2)
-    annotation ({{ diagram.line.ts_mft_load.ports_a_hea_wat.hea_ets.port_b2 }});
-  connect({{ coupling.load.id }}.ports_bHeaWat[1],{{ coupling.ets.id }}.port_a2)
-    annotation ({{ diagram.line.ts_mft_load.ports_b_hea_wat.hea_ets.port_a2 }});
+  // time series, ets hot water stub connections
+  connect(supHeaWat_{{ coupling.ets.id }}.T_in,THeaWatSup_{{ coupling.id }}.y)
+    annotation ({{ diagram.line.sup_hea_wat.t_in.t_hea_wat_sup.y }});
+  connect(supHeaWat_{{ coupling.ets.id }}.ports[1],{{ coupling.load.id }}.ports_aHeaWat[1])
+    annotation ({{ diagram.line.sup_hea_wat.ports.ts_load.ports_a_hea_wat }});
+  connect(sinHeaWat_{{ coupling.ets.id }}.ports[1],{{ coupling.load.id }}.ports_bHeaWat[1])
+    annotation ({{ diagram.line.sin_hea_wat.ports.ts_load.ports_b_hea_wat }});
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/couplings/utils.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/couplings/utils.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/districts/district.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/districts/district.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,41 +69,49 @@
         # construct graph of visual components
         diagram = Diagram(self._coupling_graph)
 
         district_template_params = {
             "district_within_path": '.'.join([self._scaffold.project_name, 'Districts']),
             "diagram": diagram,
             "couplings": [],
-            "models": []
+            "models": [],
+            "is_ghe_district": self.system_parameters.get_param('$.district_system.fifth_generation.ghe_parameters')
         }
         common_template_params = {
             'globals': {
                 'medium_w': 'MediumW',
                 'delChiWatTemBui': 'delChiWatTemBui',
                 'delChiWatTemDis': 'delChiWatTemDis',
                 'delHeaWatTemBui': 'delHeaWatTemBui',
                 'delHeaWatTemDis': 'delHeaWatTemDis',
             },
             'graph': self._coupling_graph,
             'sys_params': {
-                'district_system': self.system_parameters.get_param('$.district_system')
+                'district_system': self.system_parameters.get_param('$.district_system'),
+                # num_buildings counts the ports required for 5G systems
+                "num_buildings": len(self.system_parameters.get_param('$.buildings')),
             }
         }
 
         # render each coupling
+        load_num = 1
         for coupling in self._coupling_graph.couplings:
             template_context = {
                 'diagram': diagram.to_dict(coupling.id, is_coupling=True),
             }
             template_context.update(**common_template_params)
 
             coupling_load = coupling.get_load()
             if coupling_load is not None:
+                # read sys params file for the load
                 building_sys_params = self.system_parameters.get_param_by_building_id(coupling_load.building_id, '$')
                 template_context['sys_params']['building'] = building_sys_params
+                # Note which load is being used, so ports connect properly in couplings/5G_templates/ConnectStatements
+                template_context['sys_params']['load_num'] = load_num
+                load_num += 1
 
             templated_result = coupling.render_templates(template_context)
             district_template_params['couplings'].append({
                 'id': coupling.id,
                 'component_definitions': templated_result['component_definitions'],
                 'connect_statements': templated_result['connect_statements'],
                 'coupling_definitions_template_path': templated_result['component_definitions_template_path'],
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem.mot`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "Load side medium";
 
   // TODO: dehardcode these
   parameter Modelica.Units.SI.TemperatureDifference delChiWatTemDis(displayUnit="degC")=7;
   parameter Modelica.Units.SI.TemperatureDifference delChiWatTemBui(displayUnit="degC")=5;
   parameter Modelica.Units.SI.TemperatureDifference delHeaWatTemDis(displayUnit="degC")=12;
   parameter Modelica.Units.SI.TemperatureDifference delHeaWatTemBui(displayUnit="degC")=5;
+  parameter Integer numberofchillers = 2;
 
   // Models
 {% for model in models %}
   //
   // Begin Model Instance for {{ model.id }}
   // Source template: {{ model.instance_template_path }}
   //
```

#### html2text {}

```diff
@@ -3,20 +3,20 @@
 MediumW=Buildings.Media.Water "Source side medium"; package
 MediumA=Buildings.Media.Air "Load side medium"; // TODO: dehardcode these
 parameter Modelica.Units.SI.TemperatureDifference delChiWatTemDis
 (displayUnit="degC")=7; parameter Modelica.Units.SI.TemperatureDifference
 delChiWatTemBui(displayUnit="degC")=5; parameter
 Modelica.Units.SI.TemperatureDifference delHeaWatTemDis(displayUnit="degC")=12;
 parameter Modelica.Units.SI.TemperatureDifference delHeaWatTemBui
-(displayUnit="degC")=5; // Models {% for model in models %} // // Begin Model
-Instance for {{ model.id }} // Source template: {{ model.instance_template_path
-}} // {{ model.instance }} // // End Model Instance for {{ model.id }} // {%
-endfor %} // Model dependencies {% for coupling in couplings %} // // Begin
-Component Definitions for {{ coupling.id }} // Source template: {
-{ coupling.coupling_definitions_template_path }} // {
+(displayUnit="degC")=5; parameter Integer numberofchillers = 2; // Models {%
+for model in models %} // // Begin Model Instance for {{ model.id }} // Source
+template: {{ model.instance_template_path }} // {{ model.instance }} // // End
+Model Instance for {{ model.id }} // {% endfor %} // Model dependencies {% for
+coupling in couplings %} // // Begin Component Definitions for {{ coupling.id
+}} // Source template: {{ coupling.coupling_definitions_template_path }} // {
 { coupling.component_definitions }} // // End Component Definitions for {
 { coupling.id }} // {% endfor %} equation // Connections {% for coupling in
 couplings %} // // Begin Connect Statements for {{ coupling.id }} // Source
 template: {{ coupling.connect_statements_template_path }} // {
 { coupling.connect_statements }} // // End Connect Statements for {
 { coupling.id }} // {% endfor %} annotation( experiment( StopTime=86400,
 Interval=3600, Tolerance=1e-06), Diagram( coordinateSystem
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem5G.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem5G.mot`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 within {{ district_within_path }};
 model DistrictEnergySystem
   extends Modelica.Icons.Example;
   // District Parameters
   package MediumW=Buildings.Media.Water
     "Source side medium";
+  {% if not is_ghe_district %}
   package MediumA=Buildings.Media.Air
     "Load side medium";
   // TODO: dehardcode these
   parameter Modelica.Units.SI.TemperatureDifference delChiWatTemDis(displayUnit="degC")=7;
   parameter Modelica.Units.SI.TemperatureDifference delChiWatTemBui(displayUnit="degC")=5;
   parameter Modelica.Units.SI.TemperatureDifference delHeaWatTemDis(displayUnit="degC")=12;
   parameter Modelica.Units.SI.TemperatureDifference delHeaWatTemBui(displayUnit="degC")=5;
+  parameter Integer numberofchillers = 2;
   inner parameter Buildings.Experimental.DHC.Examples.Combined.BaseClasses.DesignDataSeries datDes(
     nBui=1,
     mPumDis_flow_nominal=95,
     mPipDis_flow_nominal=95,
     dp_length_nominal=250,
     epsPla=0.935,
     final mCon_flow_nominal={18})
     "Design data";
+  {% endif %}
   // Models
   {% for model in models %}
   //
   // Begin Model Instance for {{ model.id }}
   // Source template: {{ model.instance_template_path }}
   //
   {{ model.instance }}
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 within {{ district_within_path }}; model DistrictEnergySystem extends
 Modelica.Icons.Example; // District Parameters package
-MediumW=Buildings.Media.Water "Source side medium"; package
-MediumA=Buildings.Media.Air "Load side medium"; // TODO: dehardcode these
-parameter Modelica.Units.SI.TemperatureDifference delChiWatTemDis
+MediumW=Buildings.Media.Water "Source side medium"; {% if not is_ghe_district
+%} package MediumA=Buildings.Media.Air "Load side medium"; // TODO: dehardcode
+these parameter Modelica.Units.SI.TemperatureDifference delChiWatTemDis
 (displayUnit="degC")=7; parameter Modelica.Units.SI.TemperatureDifference
 delChiWatTemBui(displayUnit="degC")=5; parameter
 Modelica.Units.SI.TemperatureDifference delHeaWatTemDis(displayUnit="degC")=12;
 parameter Modelica.Units.SI.TemperatureDifference delHeaWatTemBui
-(displayUnit="degC")=5; inner parameter
+(displayUnit="degC")=5; parameter Integer numberofchillers = 2; inner parameter
 Buildings.Experimental.DHC.Examples.Combined.BaseClasses.DesignDataSeries
 datDes( nBui=1, mPumDis_flow_nominal=95, mPipDis_flow_nominal=95,
 dp_length_nominal=250, epsPla=0.935, final mCon_flow_nominal={18}) "Design
-data"; // Models {% for model in models %} // // Begin Model Instance for {
-{ model.id }} // Source template: {{ model.instance_template_path }} // {
-{ model.instance }} // // End Model Instance for {{ model.id }} // {% endfor %}
-// Model dependencies {% for coupling in couplings %} // // Begin Component
-Definitions for {{ coupling.id }} // Source template: {
+data"; {% endif %} // Models {% for model in models %} // // Begin Model
+Instance for {{ model.id }} // Source template: {{ model.instance_template_path
+}} // {{ model.instance }} // // End Model Instance for {{ model.id }} // {%
+endfor %} // Model dependencies {% for coupling in couplings %} // // Begin
+Component Definitions for {{ coupling.id }} // Source template: {
 { coupling.coupling_definitions_template_path }} // {
 { coupling.component_definitions }} // // End Component Definitions for {
 { coupling.id }} // {% endfor %} equation // Connections {% for coupling in
 couplings %} // // Begin Connect Statements for {{ coupling.id }} // Source
 template: {{ coupling.connect_statements_template_path }} // {
 { coupling.connect_statements }} // // End Connect Statements for {
 { coupling.id }} // {% endfor %} annotation ( experiment( StopTime=86400,
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/cooling_indirect.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/cooling_indirect.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/energy_transfer_base.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/energy_transfer_base.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_cold_water_stub.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_cold_water_stub.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_hot_water_stub.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_hot_water_stub.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/heating_indirect.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/heating_indirect.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect.mot`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 within {{ project_name }}.Substations;
 model {{ model_filename }}
-  {% raw %} "Indirect cooling energy transfer station for district energy systems"
+  {% raw %} "Indirect heating energy transfer station for district energy systems"
   extends Buildings.Fluid.Interfaces.PartialFourPortInterface(
     redeclare final package Medium1=Medium,
     redeclare final package Medium2=Medium,
     final m1_flow_nominal=mDis_flow_nominal,
     final m2_flow_nominal=mBui_flow_nominal,
-    show_T=true);
+    show_T=false);
   replaceable package Medium=Modelica.Media.Interfaces.PartialMedium
     "Medium in the component";
   // mass flow rates
   parameter Modelica.Units.SI.MassFlowRate mDis_flow_nominal(
     final min=0,
     {% endraw %}start={{ets_data["nominal_mass_flow_district"]}})
-    {% raw %} "Nominal mass flow rate of primary (district) cooling side";
+    {% raw %} "Nominal mass flow rate of primary (district) heating side";
   parameter Modelica.Units.SI.MassFlowRate mBui_flow_nominal(
     final min=0,
     {% endraw %}start={{ets_data["nominal_mass_flow_building"]}})
-    {% raw %} "Nominal mass flow rate of secondary (building) cooling side";
+    {% raw %} "Nominal mass flow rate of secondary (building) heating side";
   // Primary supply control valve
   parameter Modelica.Units.SI.PressureDifference dpValve_nominal(
     final min=0,
     {% endraw %}final displayUnit="Pa")={{ ets_data["valve_pressure_drop"] }}
     {% raw %} "Nominal pressure drop of fully open control valve";
   // Heat exchanger
   parameter Modelica.Units.SI.PressureDifference dp1_nominal(
@@ -43,22 +43,22 @@
     final min=0,
     {% endraw %}start={{ ets_data["heat_flow_nominal"]  }})
     {% raw %} "Nominal heat transfer"
     annotation (Dialog(group="Heat exchanger"));
   parameter Modelica.Units.SI.Temperature T_a1_nominal(
     min=0+273,
     max=100+273.15,
-    {% endraw %}start={{ets_data["temp_setpoint_chw"]}}+273.15,
+    {% endraw %}start={{ets_data["temp_setpoint_hhw"]}}+273.15,
     {% raw %}final displayUnit="K")
     "Nominal temperature at port a1"
     annotation (Dialog(group="Heat exchanger"));
   parameter Modelica.Units.SI.Temperature T_a2_nominal(
     min=0+273,
     max=100+273.15,
-    {% endraw %}start={{ets_data["cooling_supply_water_temperature_building"]}}+273.15,
+    {% endraw %}start={{ets_data["heating_supply_water_temperature_building"]}}+273.15,
     {% raw  %}final displayUnit="K")
     "Nominal temperature at port a2"
     annotation (Dialog(group="Heat exchanger"));
   parameter Modelica.Units.SI.Efficiency eta(
     final min=0,
     {% endraw %}final max=0.8)={{  ets_data["heat_exchanger_efficiency"]  }}
     {% raw %} "Constant effectiveness"
@@ -77,30 +77,30 @@
     "Time constant of integrator block"
     annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PI or controllerType == Modelica.Blocks.Types.SimpleController.PID));
   parameter Modelica.Units.SI.Time Td(
     final min=0)=0.1
     "Time constant of derivative block"
     annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID));
   parameter Real yMax(
-    {% endraw %}start=1)={{ ets_data["cooling_controller_y_max"] }}
+    {% endraw %}start=1)={{ ets_data["heating_controller_y_max"] }}
     {% raw %} "Upper limit of output"
     annotation (Dialog(tab="Controller"));
-  {% endraw %}parameter Real yMin={{ ets_data["cooling_controller_y_min"] }}
+  {% endraw %}parameter Real yMin={{ ets_data["heating_controller_y_min"] }}
     {% raw %} "Lower limit of output"
     annotation (Dialog(tab="Controller"));
   parameter Real wp(
     final min=0)=1
     "Set-point weight for Proportional block (0..1)"
     annotation (Dialog(tab="Controller"));
   parameter Real wd(
     final min=0)=0
     "Set-point weight for Derivative block (0..1)"
     annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID));
   parameter Real Ni(
-    min=100*Modelica.Constants.eps)=0.8
+    min=100*Modelica.Constants.eps)=0.9
     "Ni*Ti is time constant of anti-windup compensation"
     annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PI or controllerType == Modelica.Blocks.Types.SimpleController.PID));
   parameter Real Nd(
     min=100*Modelica.Constants.eps)=10
     "The higher Nd, the more ideal the derivative block"
     annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID));
   parameter Modelica.Blocks.Types.Init initType=Modelica.Blocks.Types.Init.InitialOutput
@@ -111,64 +111,65 @@
     annotation (Dialog(group="Initialization",tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PI or controllerType == Modelica.Blocks.Types.SimpleController.PID));
   parameter Real xd_start=0
     "Initial or guess value for state of derivative block"
     annotation (Dialog(group="Initialization",tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID));
   parameter Real yCon_start=0
     "Initial value of output from the controller"
     annotation (Dialog(group="Initialization",tab="Controller",enable=initType == Modelica.Blocks.Types.Init.InitialOutput));
-  parameter Boolean reverseActing=false
-    "Set to true for throttling the water flow rate through a cooling coil controller"
+  parameter Boolean reverseActing=true
     annotation (Dialog(tab="Controller"));
   Modelica.Blocks.Interfaces.RealInput TSetBuiSup(
-    final quantity="ThermodynamicTemperature",
-    final unit="K")
+    each final quantity="ThermodynamicTemperature",
+    each final unit="K")
     "Setpoint temperature for building supply"
     annotation (Placement(transformation(extent={{-140,-20},{-100,20}})));
   Modelica.Blocks.Interfaces.RealOutput Q_flow(
-    final quantity="Power",
-    final unit="W",
-    final displayUnit="kW")
+    each final quantity="Power",
+    each final unit="W",
+    each final displayUnit="kW")
     "Measured power demand at the ETS"
     annotation (Placement(transformation(extent={{100,140},{120,160}})));
   Modelica.Blocks.Interfaces.RealOutput Q(
-    final quantity="Energy",
-    final unit="J",
-    final displayUnit="kWh")
+    each final quantity="Energy",
+    each final unit="J",
+    each final displayUnit="kWh")
     "Measured energy consumption at the ETS"
     annotation (Placement(transformation(extent={{100,100},{120,120}})));
   Buildings.Fluid.HeatExchangers.PlateHeatExchangerEffectivenessNTU hex(
     redeclare final package Medium1=Medium,
     redeclare final package Medium2=Medium,
-    final m1_flow_nominal=mDis_flow_nominal,
-    final m2_flow_nominal=mBui_flow_nominal,
-    final dp1_nominal=dp1_nominal,
-    final dp2_nominal=dp2_nominal,
-    final configuration=Buildings.Fluid.Types.HeatExchangerConfiguration.CounterFlow,
-    final use_Q_flow_nominal=true,
-    final Q_flow_nominal=Q_flow_nominal,
-    final T_a1_nominal=T_a1_nominal,
-    final T_a2_nominal=T_a2_nominal)
-    "Indirect cooling heat exchanger"
+    each final m1_flow_nominal=mDis_flow_nominal,
+    each final m2_flow_nominal=mBui_flow_nominal,
+    each final dp1_nominal=dp1_nominal,
+    each final dp2_nominal=dp2_nominal,
+    each final configuration=Buildings.Fluid.Types.HeatExchangerConfiguration.CounterFlow,
+    each final use_Q_flow_nominal=true,
+    each final Q_flow_nominal=Q_flow_nominal,
+    each final T_a1_nominal=T_a1_nominal,
+    each final T_a2_nominal=T_a2_nominal)
+    "Indirect heating heat exchanger"
     annotation (Placement(transformation(extent={{20,-10},{40,10}})));
   Buildings.Controls.Continuous.LimPID con(
-    final controllerType=Modelica.Blocks.Types.SimpleController.PI,
-    final k=k,
-    final Td=Td,
-    final yMax=yMax,
-    final yMin=yMin,
-    final Ti=Ti,
-    final wp=wp,
-    final wd=wd,
-    final Ni=Ni,
-    final Nd=Nd,
-    final initType=Modelica.Blocks.Types.Init.InitialOutput,
-    final xi_start=xi_start,
-    final xd_start=xd_start,
-    final y_start=yCon_start,
-    final reverseActing=reverseActing)
+    each final controllerType=Modelica.Blocks.Types.SimpleController.PI,
+    each final k=k,
+    each final Td=Td,
+    each final yMax=yMax,
+    each final yMin=yMin,
+    each final Ti=Ti,
+    each final wp=wp,
+    each final wd=wd,
+    each final Ni=Ni,
+    each final Nd=Nd,
+    each final initType=Modelica.Blocks.Types.Init.InitialOutput,
+    each final xi_start=xi_start,
+    each final xd_start=xd_start,
+    each final y_start=yCon_start,
+    each final reverseActing=reverseActing,
+    reset=Buildings.Types.Reset.Disabled,
+    y_reset=0)
     "Controller"
     annotation (Placement(transformation(extent={{-90,-10},{-70,10}})));
   Buildings.Fluid.Sensors.TemperatureTwoPort senTDisSup(
     redeclare final package Medium=Medium,
     final m_flow_nominal=mDis_flow_nominal)
     "District-side (primary) supply temperature sensor"
     annotation (Placement(transformation(extent={{-90,50},{-70,70}})));
@@ -182,26 +183,24 @@
     "Integration"
     annotation (Placement(transformation(extent={{60,120},{80,100}})));
   Buildings.Fluid.Sensors.MassFlowRate senMasFlo(
     redeclare package Medium=Medium)
     annotation (Placement(transformation(extent={{-60,50},{-40,70}})));
   Buildings.Fluid.Sensors.TemperatureTwoPort senTBuiSup(
     redeclare final package Medium=Medium,
-    final m_flow_nominal=mBui_flow_nominal,
-    tau=10)
+    final m_flow_nominal=mBui_flow_nominal)
     "Building-side (secondary) supply temperature"
     annotation (Placement(transformation(extent={{-70,-70},{-90,-50}})));
   Buildings.Fluid.Actuators.Valves.TwoWayEqualPercentage val(
     redeclare final package Medium=Medium,
-    final m_flow_nominal=mDis_flow_nominal,
-    final dpValve_nominal=dpValve_nominal,
+    each final m_flow_nominal=mDis_flow_nominal,
+    each final dpValve_nominal=dpValve_nominal,
     riseTime(
       displayUnit="s")=60,
-    y_start=0,
-    l=0.005)
+    y_start=0)
     "District-side (primary) control valve"
     annotation (Placement(transformation(extent={{-30,70},{-10,50}})));
   Modelica.Blocks.Math.Gain cp(
     final k=cp_default)
     "Specifc heat multiplier to calculate heat flow rate"
     annotation (Placement(transformation(extent={{20,100},{40,120}})));
   Modelica.Blocks.Math.Product pro
@@ -259,15 +258,15 @@
   connect(senTBuiSup.port_a,hex.port_b2)
     annotation (Line(points={{-70,-60},{0,-60},{0,-6},{20,-6}},color={0,127,255}));
   connect(senTBuiSup.T,con.u_m)
     annotation (Line(points={{-80,-49},{-80,-12}},color={0,0,127}));
   connect(port_b2,senTBuiSup.port_b)
     annotation (Line(points={{-100,-60},{-90,-60}},color={0,127,255}));
   annotation (
-    defaultComponentName="cooEts",
+    defaultComponentName="heaEts",
     Icon(
       coordinateSystem(
         preserveAspectRatio=false),
       graphics={
         Rectangle(
           extent={{-100,-56},{100,-64}},
           fillColor={0,0,0},
@@ -277,15 +276,15 @@
           extent={{-100,64},{100,56}},
           fillColor={0,0,0},
           fillPattern=FillPattern.Solid,
           pattern=LinePattern.None),
         Rectangle(
           extent={{-80,80},{80,-80}},
           lineColor={175,175,175},
-          fillColor={35,138,255},
+          fillColor={238,46,47},
           fillPattern=FillPattern.Solid),
         Rectangle(
           extent={{-62,80},{-58,-80}},
           lineColor={0,0,255},
           pattern=LinePattern.None,
           fillColor={0,0,0},
           fillPattern=FillPattern.Solid),
@@ -304,57 +303,49 @@
         Rectangle(
           extent={{58,80},{62,-80}},
           lineColor={0,0,255},
           pattern=LinePattern.None,
           fillColor={0,0,0},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-80,65},{80,54}},
+          extent={{-80,65},{-4,56}},
+          lineColor={0,0,255},
+          pattern=LinePattern.None,
+          fillColor={255,0,0},
+          fillPattern=FillPattern.Solid),
+        Rectangle(
+          extent={{-4,66},{80,56}},
           lineColor={0,0,255},
           pattern=LinePattern.None,
           fillColor={0,0,255},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-80,-55},{80,-66}},
+          extent={{-80,-55},{-4,-64}},
+          lineColor={0,0,255},
+          pattern=LinePattern.None,
+          fillColor={255,0,0},
+          fillPattern=FillPattern.Solid),
+        Rectangle(
+          extent={{-4,-54},{80,-64}},
           lineColor={0,0,255},
           pattern=LinePattern.None,
           fillColor={0,0,255},
-          fillPattern=FillPattern.Solid)}),
+          fillPattern=FillPattern.Solid),
+        Rectangle(
+          extent={{-80,-56},{-4,-64}},
+          lineColor={0,0,255},
+          pattern=LinePattern.None)}),
     Diagram(
       coordinateSystem(
         preserveAspectRatio=false,
         extent={{-100,-100},{100,160}})),
     Documentation(
       info="<html>
-<p>
-Indirect cooling energy transfer station (ETS) model that controls
-the building chilled water supply temperature by modulating a
-primary control valve on the district supply side. The design is
-based on a typical district cooling ETS described in ASHRAE's
-<a href=\"https://www.ashrae.org/technical-resources/bookstore/district-heating-and-cooling-guides\">
-District Cooling Guide</a>.
-As shown in the figure below, the building pumping design (constant,
-variable) is specified on the building side, not within the ETS.
-</p>
-<p align=\"center\">
-<img src=\"modelica://Buildings/Resources/Images/Applications/DHC/EnergyTransferStations/CoolingIndirect.png\" alt=\"DHC.ETS.CoolingIndirect\"/>
-</p>
-<h4>Reference</h4>
-<p>
-American Society of Heating, Refrigeration and Air-Conditioning
-Engineers. (2013). Chapter 5: End User Interface. In
-<i>District Cooling Guide</i>. 1st Edition.
-</p>
-</html>",
+      </html>",
       revisions="<html>
-<ul>
-<li>
-December 10, 2019 by Kathryn Hinkelman:<br/>
-Updated model to use control valve <a href=\"modelica://Buildings.Fluid.Actuators.Valves.TwoWayEqualPercentage\">
-TwoWayEqualPercentage</a>.
-</li>
-<li>
-November 1, 2019, by Kathryn Hinkelman:<br/>
-First implementation. </li>
-</ul>
-</html>"));
+  <li>
+  August 1, 2020, by Hagar Elarga:<br/>
+  First implementation.
+  </li>
+  </ul>
+  </html>"));
 {% endraw %}end {{ model_filename }};
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect_Instance.mopt`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-  // cooling indirect instance
+  // heating indirect instance
   {{ model.modelica_type }} {{ model.id }}(
+    allowFlowReversal1=true,
+    allowFlowReversal2=true,
+    show_T=true,
     redeclare package Medium={{ globals.medium_w }},
-    allowFlowReversal1=false,
-    allowFlowReversal2=false,
     mDis_flow_nominal=mDis_flow_nominal_{{ couplings.load_couplings[0].id }},
     mBui_flow_nominal=mBui_flow_nominal_{{ couplings.load_couplings[0].id }},
+    dpValve_nominal=6000,
     dp1_nominal=500,
     dp2_nominal=500,
-    dpValve_nominal=7000,
     use_Q_flow_nominal=true,
     Q_flow_nominal=Q_flow_nominal_{{ couplings.load_couplings[0].id }},
-    // TODO: dehardcode the nominal temperatures?
-    T_a1_nominal=273.15+5,
-    T_a2_nominal=273.15+13)
-    "Indirect cooling energy transfer station ETS."
-    annotation (Placement({{ diagram.transformation.coo_ets.ets }}));
+    T_a1_nominal=55+273.15,
+    T_a2_nominal=35+273.15,
+    k=0.1,
+    Ti=60,
+    reverseActing=true)
+    annotation (Placement({{ diagram.transformation.hea_ets.ets }}));
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsColdWaterStub_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsColdWaterStub_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsHotWaterStub_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsHotWaterStub_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerWithBypass.mo`

 * *Files 17% similar despite different names*

```diff
@@ -1,351 +1,381 @@
-within {{ project_name }}.Substations;
-model {{ model_filename }}
-  {% raw %} "Indirect heating energy transfer station for district energy systems"
-  extends Buildings.Fluid.Interfaces.PartialFourPortInterface(
-    redeclare final package Medium1=Medium,
-    redeclare final package Medium2=Medium,
-    final m1_flow_nominal=mDis_flow_nominal,
-    final m2_flow_nominal=mBui_flow_nominal,
-    show_T=false);
-  replaceable package Medium=Modelica.Media.Interfaces.PartialMedium
-    "Medium in the component";
-  // mass flow rates
-  parameter Modelica.Units.SI.MassFlowRate mDis_flow_nominal(
-    final min=0,
-    {% endraw %}start={{ets_data["nominal_mass_flow_district"]}})
-    {% raw %} "Nominal mass flow rate of primary (district) heating side";
-  parameter Modelica.Units.SI.MassFlowRate mBui_flow_nominal(
-    final min=0,
-    {% endraw %}start={{ets_data["nominal_mass_flow_building"]}})
-    {% raw %} "Nominal mass flow rate of secondary (building) heating side";
-  // Primary supply control valve
-  parameter Modelica.Units.SI.PressureDifference dpValve_nominal(
-    final min=0,
-    {% endraw %}final displayUnit="Pa")={{ ets_data["valve_pressure_drop"] }}
-    {% raw %} "Nominal pressure drop of fully open control valve";
-  // Heat exchanger
-  parameter Modelica.Units.SI.PressureDifference dp1_nominal(
-    final min=0,
-    {% endraw %}start={{ ets_data["heat_exchanger_primary_pressure_drop"] }},
-    {% raw %}final displayUnit="Pa")
-    "Nominal pressure difference on primary side"
-    annotation (Dialog(group="Heat exchanger"));
-  parameter Modelica.Units.SI.PressureDifference dp2_nominal(
-    final min=0,
-    {% endraw %}start={{  ets_data["heat_exchanger_secondary_pressure_drop"] }},
-    {% raw %}final displayUnit="Pa")
-    "Nominal pressure difference on secondary side"
-    annotation (Dialog(group="Heat exchanger"));
-  parameter Boolean use_Q_flow_nominal=true
-    "Set to true to specify Q_flow_nominal and temperatures, or to false to specify effectiveness"
-    annotation (Dialog(group="Heat exchanger"));
-  parameter Modelica.Units.SI.HeatFlowRate Q_flow_nominal(
-    final min=0,
-    {% endraw %}start={{ ets_data["heat_flow_nominal"]  }})
-    {% raw %} "Nominal heat transfer"
-    annotation (Dialog(group="Heat exchanger"));
-  parameter Modelica.Units.SI.Temperature T_a1_nominal(
-    min=0+273,
-    max=100+273.15,
-    {% endraw %}start={{ets_data["temp_setpoint_hhw"]}}+273.15,
-    {% raw %}final displayUnit="K")
-    "Nominal temperature at port a1"
-    annotation (Dialog(group="Heat exchanger"));
-  parameter Modelica.Units.SI.Temperature T_a2_nominal(
-    min=0+273,
-    max=100+273.15,
-    {% endraw %}start={{ets_data["heating_supply_water_temperature_building"]}}+273.15,
-    {% raw  %}final displayUnit="K")
-    "Nominal temperature at port a2"
-    annotation (Dialog(group="Heat exchanger"));
-  parameter Modelica.Units.SI.Efficiency eta(
-    final min=0,
-    {% endraw %}final max=0.8)={{  ets_data["heat_exchanger_efficiency"]  }}
-    {% raw %} "Constant effectiveness"
-    annotation (Dialog(group="Heat exchanger"));
-  // Controller parameters
+within geojson_modelica_translator.model_connectors.templates;
+model CoolingTowerWithBypass
+  "Cooling tower system with bypass valve"
+  replaceable package Medium=Buildings.Media.Water
+    "Condenser water medium";
+  parameter Integer num(
+    min=1)=2
+    "Number of cooling towers";
+  parameter Boolean show_T=true
+    "= true, if actual temperature at port is computed"
+    annotation (Dialog(tab="Advanced",group="Diagnostics"));
+  parameter Modelica.Units.SI.MassFlowRate m_flow_nominal
+    "Total nominal mass flow rate of condenser water"
+    annotation (Dialog(group="Nominal condition"));
+  parameter Modelica.Units.SI.Pressure dp_nominal
+    "Nominal pressure difference of the tower"
+    annotation (Dialog(group="Nominal condition"));
+  parameter Real ratWatAir_nominal(
+    min=0,
+    unit="1")=0.625
+    "Design water-to-air ratio"
+    annotation (Dialog(group="Nominal condition"));
+  parameter Modelica.Units.SI.Temperature TAirInWB_nominal
+    "Nominal outdoor (air inlet) wetbulb temperature"
+    annotation (Dialog(group="Heat transfer"));
+  parameter Modelica.Units.SI.Temperature TWatIn_nominal
+    "Nominal water inlet temperature"
+    annotation (Dialog(group="Heat transfer"));
+  parameter Modelica.Units.SI.TemperatureDifference dT_nominal
+    "Temperature difference between inlet and outlet of the tower"
+    annotation (Dialog(group="Heat transfer"));
+  parameter Modelica.Units.SI.Power PFan_nominal
+    "Fan power"
+    annotation (Dialog(group="Fan"));
+  parameter Modelica.Units.SI.TemperatureDifference dTApp=3
+    "Approach temperature"
+    annotation (Dialog(group="Control Settings"));
+  parameter Modelica.Units.SI.Temperature TMin
+    "Minimum allowed water temperature entering chiller"
+    annotation (Dialog(group="Control Settings"));
   parameter Modelica.Blocks.Types.SimpleController controllerType=Modelica.Blocks.Types.SimpleController.PI
-    "Type of controller"
-    annotation (Dialog(tab="Controller"));
+    "Type of fan speed controller"
+    annotation (Dialog(group="Control Settings"));
   parameter Real k(
-    final min=0,
-    final unit="1")=1
-    "Gain of controller"
-    annotation (Dialog(tab="Controller"));
+    unit="1",
+    min=0)=1
+    "Gain of the tower PID controller"
+    annotation (Dialog(group="Control Settings"));
   parameter Modelica.Units.SI.Time Ti(
-    min=Modelica.Constants.small)=120
-    "Time constant of integrator block"
-    annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PI or controllerType == Modelica.Blocks.Types.SimpleController.PID));
+    min=Modelica.Constants.small)=60
+    "Integrator time constant of the tower PID controller"
+    annotation (Dialog(enable=(controllerType == Modelica.Blocks.Types.SimpleController.PI or controllerType == Modelica.Blocks.Types.SimpleController.PID),group="Control Settings"));
   parameter Modelica.Units.SI.Time Td(
-    final min=0)=0.1
-    "Time constant of derivative block"
-    annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID));
-  parameter Real yMax(
-    {% endraw %}start=1)={{ ets_data["heating_controller_y_max"] }}
-    {% raw %} "Upper limit of output"
-    annotation (Dialog(tab="Controller"));
-  {% endraw %}parameter Real yMin={{ ets_data["heating_controller_y_min"] }}
-    {% raw %} "Lower limit of output"
-    annotation (Dialog(tab="Controller"));
-  parameter Real wp(
-    final min=0)=1
-    "Set-point weight for Proportional block (0..1)"
-    annotation (Dialog(tab="Controller"));
-  parameter Real wd(
-    final min=0)=0
-    "Set-point weight for Derivative block (0..1)"
-    annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID));
-  parameter Real Ni(
-    min=100*Modelica.Constants.eps)=0.9
-    "Ni*Ti is time constant of anti-windup compensation"
-    annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PI or controllerType == Modelica.Blocks.Types.SimpleController.PID));
-  parameter Real Nd(
-    min=100*Modelica.Constants.eps)=10
-    "The higher Nd, the more ideal the derivative block"
-    annotation (Dialog(tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID));
-  parameter Modelica.Blocks.Types.Init initType=Modelica.Blocks.Types.Init.InitialOutput
-    "Type of initialization (1: NoInit, 2: SteadyState, 3: InitialState, 4: InitialOutput)"
-    annotation (Evaluate=true,Dialog(group="Initialization",tab="Controller"));
-  parameter Real xi_start=0
-    "Initial or guess value value for integrator output (= integrator state)"
-    annotation (Dialog(group="Initialization",tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PI or controllerType == Modelica.Blocks.Types.SimpleController.PID));
-  parameter Real xd_start=0
-    "Initial or guess value for state of derivative block"
-    annotation (Dialog(group="Initialization",tab="Controller",enable=controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID));
-  parameter Real yCon_start=0
-    "Initial value of output from the controller"
-    annotation (Dialog(group="Initialization",tab="Controller",enable=initType == Modelica.Blocks.Types.Init.InitialOutput));
-  parameter Boolean reverseActing=true
-    annotation (Dialog(tab="Controller"));
-  Modelica.Blocks.Interfaces.RealInput TSetBuiSup(
-    final quantity="ThermodynamicTemperature",
-    final unit="K")
-    "Setpoint temperature for building supply"
-    annotation (Placement(transformation(extent={{-140,-20},{-100,20}})));
-  Modelica.Blocks.Interfaces.RealOutput Q_flow(
-    final quantity="Power",
-    final unit="W",
-    final displayUnit="kW")
-    "Measured power demand at the ETS"
-    annotation (Placement(transformation(extent={{100,140},{120,160}})));
-  Modelica.Blocks.Interfaces.RealOutput Q(
-    final quantity="Energy",
-    final unit="J",
-    final displayUnit="kWh")
-    "Measured energy consumption at the ETS"
-    annotation (Placement(transformation(extent={{100,100},{120,120}})));
-  Buildings.Fluid.HeatExchangers.PlateHeatExchangerEffectivenessNTU hex(
-    redeclare final package Medium1=Medium,
-    redeclare final package Medium2=Medium,
-    final m1_flow_nominal=mDis_flow_nominal,
-    final m2_flow_nominal=mBui_flow_nominal,
-    final dp1_nominal=dp1_nominal,
-    final dp2_nominal=dp2_nominal,
-    final configuration=Buildings.Fluid.Types.HeatExchangerConfiguration.CounterFlow,
-    final use_Q_flow_nominal=true,
-    final Q_flow_nominal=Q_flow_nominal,
-    final T_a1_nominal=T_a1_nominal,
-    final T_a2_nominal=T_a2_nominal)
-    "Indirect heating heat exchanger"
-    annotation (Placement(transformation(extent={{20,-10},{40,10}})));
-  Buildings.Controls.Continuous.LimPID con(
-    final controllerType=Modelica.Blocks.Types.SimpleController.PI,
-    final k=k,
-    final Td=Td,
-    final yMax=yMax,
-    final yMin=yMin,
-    final Ti=Ti,
-    final wp=wp,
-    final wd=wd,
-    final Ni=Ni,
-    final Nd=Nd,
-    final initType=Modelica.Blocks.Types.Init.InitialOutput,
-    final xi_start=xi_start,
-    final xd_start=xd_start,
-    final y_start=yCon_start,
-    final reverseActing=reverseActing,
-    reset=Buildings.Types.Reset.Disabled,
-    y_reset=0)
-    "Controller"
-    annotation (Placement(transformation(extent={{-90,-10},{-70,10}})));
-  Buildings.Fluid.Sensors.TemperatureTwoPort senTDisSup(
-    redeclare final package Medium=Medium,
-    final m_flow_nominal=mDis_flow_nominal)
-    "District-side (primary) supply temperature sensor"
-    annotation (Placement(transformation(extent={{-90,50},{-70,70}})));
-  Buildings.Fluid.Sensors.TemperatureTwoPort senTDisRet(
-    redeclare final package Medium=Medium,
-    final m_flow_nominal=mDis_flow_nominal)
-    "District-side (primary) return temperature sensor"
-    annotation (Placement(transformation(extent={{70,50},{90,70}})));
-  Modelica.Blocks.Continuous.Integrator int(
-    k=1)
-    "Integration"
-    annotation (Placement(transformation(extent={{60,120},{80,100}})));
-  Buildings.Fluid.Sensors.MassFlowRate senMasFlo(
+    min=0)=0.1
+    "Derivative time constant of the tower PID controller"
+    annotation (Dialog(enable=(controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID),group="Control Settings"));
+  Medium.ThermodynamicState sta_a=Medium.setState_phX(
+    port_a.p,
+    noEvent(
+      actualStream(
+        port_a.h_outflow)),
+    noEvent(
+      actualStream(
+        port_a.Xi_outflow))) if show_T
+    "Medium properties in port_a";
+  Medium.ThermodynamicState sta_b=Medium.setState_phX(
+    port_b.p,
+    noEvent(
+      actualStream(
+        port_b.h_outflow)),
+    noEvent(
+      actualStream(
+        port_b.Xi_outflow))) if show_T
+    "Medium properties in port_b";
+  Modelica.Fluid.Interfaces.FluidPort_a port_a(
+    redeclare package Medium=Medium)
+    "Fluid connector a (positive design flow direction is from port_a to port_b)"
+    annotation (Placement(transformation(extent={{-110,-10},{-90,10}})));
+  Modelica.Fluid.Interfaces.FluidPort_b port_b(
     redeclare package Medium=Medium)
+    "Fluid connector b (positive design flow direction is from port_a to port_b)"
+    annotation (Placement(transformation(extent={{90,-10},{110,10}})));
+  Modelica.Blocks.Interfaces.RealInput on[num](
+    each min=0,
+    each max=1,
+    each unit="1")
+    "On signal for cooling towers"
+    annotation (Placement(transformation(extent={{-140,20},{-100,60}})));
+  Modelica.Blocks.Interfaces.RealInput TWetBul(
+    final unit="K",
+    displayUnit="degC")
+    "Entering air wetbulb temperature"
+    annotation (Placement(transformation(extent={{-140,-40},{-100,0}})));
+  Modelica.Blocks.Interfaces.RealOutput PFan[num](
+    each final quantity="Power",
+    each final unit="W")
+    "Electric power consumed by fan"
+    annotation (Placement(transformation(extent={{100,50},{120,70}})));
+  Modelica.Blocks.Interfaces.RealOutput TLvg[num](
+    each final unit="K",
+    each displayUnit="degC")
+    "Leaving water temperature"
+    annotation (Placement(transformation(extent={{100,20},{120,40}})));
+  CoolingTowerParallel cooTowSys(
+    use_inputFilter=true,
+    redeclare package Medium=Medium,
+    num=num,
+    show_T=show_T,
+    m_flow_nominal=m_flow_nominal/num,
+    dp_nominal=dp_nominal,
+    ratWatAir_nominal=ratWatAir_nominal,
+    TAirInWB_nominal=TAirInWB_nominal,
+    TWatIn_nominal=TWatIn_nominal,
+    dT_nominal=dT_nominal,
+    PFan_nominal=PFan_nominal)
+    "Cooling tower system"
+    annotation (Placement(transformation(extent={{-10,-10},{10,10}})));
+  Buildings.Fluid.Actuators.Valves.TwoWayEqualPercentage valByp(
+    redeclare package Medium=Medium,
+    m_flow_nominal=m_flow_nominal*0.0001,
+    dpValve_nominal=dp_nominal,
+    use_inputFilter=false)
+    "Condenser water bypass valve"
+    annotation (Placement(transformation(extent={{-10,-10},{10,10}},origin={0,-40})));
+  Buildings.Fluid.Sensors.TemperatureTwoPort senTCWSup(
+    redeclare package Medium=Medium,
+    m_flow_nominal=m_flow_nominal,
+    T_start=Medium.T_default)
+    annotation (Placement(transformation(extent={{60,10},{80,-10}})));
+  Modelica.Blocks.Sources.RealExpression TSetCWSup(
+    y=max(
+      TWetBul+dTApp,
+      TMin))
+    "Condenser water supply temperature setpoint"
     annotation (Placement(transformation(extent={{-60,50},{-40,70}})));
-  Buildings.Fluid.Sensors.TemperatureTwoPort senTBuiSup(
-    redeclare final package Medium=Medium,
-    final m_flow_nominal=mBui_flow_nominal)
-    "Building-side (secondary) supply temperature"
-    annotation (Placement(transformation(extent={{-70,-70},{-90,-50}})));
-  Buildings.Fluid.Actuators.Valves.TwoWayEqualPercentage val(
-    redeclare final package Medium=Medium,
-    final m_flow_nominal=mDis_flow_nominal,
-    final dpValve_nominal=dpValve_nominal,
-    riseTime(
-      displayUnit="s")=60,
-    y_start=0)
-    "District-side (primary) control valve"
-    annotation (Placement(transformation(extent={{-30,70},{-10,50}})));
-  Modelica.Blocks.Math.Gain cp(
-    final k=cp_default)
-    "Specifc heat multiplier to calculate heat flow rate"
-    annotation (Placement(transformation(extent={{20,100},{40,120}})));
-  Modelica.Blocks.Math.Product pro
-    "Product"
-    annotation (Placement(transformation(extent={{-20,100},{0,120}})));
-  Modelica.Blocks.Math.Add dTDis(
-    k1=-1,
-    k2=+1)
-    "Temperatur difference on the district side"
-    annotation (Placement(transformation(extent={{-60,106},{-40,126}})));
-protected
-  final parameter Medium.ThermodynamicState sta_default=Medium.setState_pTX(
-    T=Medium.T_default,
-    p=Medium.p_default,
-    X=Medium.X_default)
-    "Medium state at default properties";
-  final parameter Modelica.Units.SI.SpecificHeatCapacity cp_default=Medium.specificHeatCapacityCp(
-    sta_default)
-    "Specific heat capacity of the fluid";
-{% endraw %}equation
-  {% raw %} connect(hex.port_a2,port_a2)
-    annotation (Line(points={{40,-6},{60,-6},{60,-60},{100,-60}},color={0,127,255}));
-  connect(hex.port_b1,senTDisRet.port_a)
-    annotation (Line(points={{40,6},{60,6},{60,60},{70,60}},color={0,127,255}));
-  connect(val.port_b,hex.port_a1)
-    annotation (Line(points={{-10,60},{0,60},{0,6},{20,6}},color={0,127,255}));
-  connect(senMasFlo.port_b,val.port_a)
-    annotation (Line(points={{-40,60},{-30,60}},color={0,127,255}));
-  connect(port_a1,senTDisSup.port_a)
-    annotation (Line(points={{-100,60},{-90,60}},color={0,127,255}));
-  connect(senTDisSup.port_b,senMasFlo.port_a)
-    annotation (Line(points={{-70,60},{-60,60}},color={0,127,255}));
-  connect(senTDisRet.port_b,port_b1)
-    annotation (Line(points={{90,60},{100,60}},color={0,127,255}));
-  connect(con.y,val.y)
-    annotation (Line(points={{-69,0},{-20,0},{-20,48}},color={0,0,127}));
-  connect(pro.y,cp.u)
-    annotation (Line(points={{1,110},{18,110}},color={0,0,127}));
-  connect(senMasFlo.m_flow,pro.u2)
-    annotation (Line(points={{-50,71},{-50,104},{-22,104}},color={0,0,127}));
-  connect(senTDisSup.T,dTDis.u1)
-    annotation (Line(points={{-80,71},{-80,122},{-62,122}},color={0,0,127}));
-  connect(senTDisRet.T,dTDis.u2)
-    annotation (Line(points={{80,71},{80,80},{-70,80},{-70,110},{-62,110}},color={0,0,127}));
-  connect(dTDis.y,pro.u1)
-    annotation (Line(points={{-39,116},{-22,116}},color={0,0,127}));
-  connect(cp.y,int.u)
-    annotation (Line(points={{41,110},{58,110}},color={0,0,127}));
-  connect(int.y,Q)
-    annotation (Line(points={{81,110},{110,110}},color={0,0,127}));
-  connect(Q_flow,cp.y)
-    annotation (Line(points={{110,150},{50,150},{50,110},{41,110}},color={0,0,127}));
-  connect(TSetBuiSup,con.u_s)
-    annotation (Line(points={{-120,0},{-92,0}},color={0,0,127}));
-  connect(senTBuiSup.port_a,hex.port_b2)
-    annotation (Line(points={{-70,-60},{0,-60},{0,-6},{20,-6}},color={0,127,255}));
-  connect(senTBuiSup.T,con.u_m)
-    annotation (Line(points={{-80,-49},{-80,-12}},color={0,0,127}));
-  connect(port_b2,senTBuiSup.port_b)
-    annotation (Line(points={{-100,-60},{-90,-60}},color={0,127,255}));
+  Modelica.Blocks.Sources.Constant TSetByPas(
+    k=TMin)
+    "Bypass loop temperature setpoint"
+    annotation (Placement(transformation(extent={{-90,-60},{-70,-40}})));
+  Buildings.Controls.Continuous.LimPID bypValCon(
+    u_s(
+      unit="K",
+      displayUnit="degC"),
+    u_m(
+      unit="K",
+      displayUnit="degC"),
+    controllerType=Modelica.Blocks.Types.SimpleController.PI,
+    k=1,
+    Ti=60,
+    final reverseActing=true,
+    reset=Buildings.Types.Reset.Parameter,
+    y_reset=0)
+    "Bypass valve controller"
+    annotation (Placement(transformation(extent={{-60,-60},{-40,-40}})));
+  Buildings.Controls.Continuous.LimPID cooTowSpeCon(
+    u_s(
+      unit="K",
+      displayUnit="degC"),
+    u_m(
+      unit="K",
+      displayUnit="degC"),
+    final reverseActing=false,
+    controllerType=controllerType,
+    k=k,
+    Ti=Ti)
+    "Cooling tower fan speed controller"
+    annotation (Placement(transformation(extent={{-12,50},{8,70}})));
+  Modelica.Blocks.Sources.RealExpression TLvgCooTow(
+    y=senTCWSup.T)
+    "Condenser water temperature leaving the towers"
+    annotation (Placement(transformation(extent={{-30,30},{-10,50}})));
+  Modelica.Blocks.Math.RealToBoolean reaToBoo
+    "Real to boolean signal"
+    annotation (Placement(transformation(extent={{-90,-90},{-70,-70}})));
+equation
+  connect(cooTowSys.TWetBul,TWetBul)
+    annotation (Line(points={{-12,-6},{-40,-6},{-40,-20},{-120,-20}},color={0,0,127}));
+  connect(on,cooTowSys.on)
+    annotation (Line(points={{-120,40},{-40,40},{-40,6},{-12,6}},color={0,0,127}));
+  connect(port_a,cooTowSys.port_a)
+    annotation (Line(points={{-100,0},{-10,0}},color={0,127,255}));
+  connect(cooTowSys.port_b,senTCWSup.port_a)
+    annotation (Line(points={{10,0},{60,0}},color={0,127,255}));
+  connect(senTCWSup.port_b,port_b)
+    annotation (Line(points={{80,0},{100,0}},color={0,127,255}));
+  connect(TSetByPas.y,bypValCon.u_s)
+    annotation (Line(points={{-69,-50},{-62,-50}},color={0,0,127}));
+  connect(senTCWSup.T,bypValCon.u_m)
+    annotation (Line(points={{70,-11},{70,-80},{-50,-80},{-50,-62}},color={0,0,127}));
+  connect(valByp.port_a,cooTowSys.port_a)
+    annotation (Line(points={{-10,-40},{-30,-40},{-30,0},{-10,0}},color={0,127,255}));
+  connect(valByp.port_b,senTCWSup.port_a)
+    annotation (Line(points={{10,-40},{30,-40},{30,0},{60,0}},color={0,127,255}));
+  connect(TSetCWSup.y,cooTowSpeCon.u_s)
+    annotation (Line(points={{-39,60},{-14,60}},color={0,0,127}));
+  connect(cooTowSpeCon.y,cooTowSys.speFan)
+    annotation (Line(points={{9,60},{20,60},{20,20},{-20,20},{-20,2},{-12,2}},color={0,0,127}));
+  connect(cooTowSys.PFan,PFan)
+    annotation (Line(points={{11,6},{40,6},{40,60},{110,60}},color={0,0,127}));
+  connect(cooTowSys.TLvg,TLvg)
+    annotation (Line(points={{11,3},{44,3},{44,30},{110,30}},color={0,0,127}));
+  connect(bypValCon.y,valByp.y)
+    annotation (Line(points={{-39,-50},{-20,-50},{-20,-20},{0,-20},{0,-28}},color={0,0,127}));
+  connect(TLvgCooTow.y,cooTowSpeCon.u_m)
+    annotation (Line(points={{-9,40},{-2,40},{-2,48}},color={0,0,127}));
+  connect(reaToBoo.y,bypValCon.trigger)
+    annotation (Line(points={{-69,-80},{-58,-80},{-58,-62}},color={255,0,255}));
+  connect(on[1],reaToBoo.u)
+    annotation (Line(points={{-120,30},{-96,30},{-96,-80},{-92,-80}},color={0,0,127}));
   annotation (
-    defaultComponentName="heaEts",
+    Diagram(
+      coordinateSystem(
+        preserveAspectRatio=false,
+        extent={{-100,-100},{100,100}})),
     Icon(
       coordinateSystem(
-        preserveAspectRatio=false),
+        preserveAspectRatio=false,
+        extent={{-100,-100},{100,100}}),
       graphics={
+        Polygon(
+          points={{0,-80},{-10,-72},{-10,-88},{0,-80}},
+          lineColor={0,0,0},
+          fillColor={255,255,255},
+          fillPattern=FillPattern.Solid),
+        Polygon(
+          points={{0,-80},{10,-72},{10,-88},{0,-80}},
+          lineColor={0,0,0},
+          fillColor={255,255,255},
+          fillPattern=FillPattern.Solid),
+        Text(
+          extent={{-149,-114},{151,-154}},
+          lineColor={0,0,255},
+          textString="%name"),
         Rectangle(
-          extent={{-100,-56},{100,-64}},
-          fillColor={0,0,0},
-          fillPattern=FillPattern.Solid,
-          pattern=LinePattern.None),
-        Rectangle(
-          extent={{-100,64},{100,56}},
-          fillColor={0,0,0},
-          fillPattern=FillPattern.Solid,
-          pattern=LinePattern.None),
-        Rectangle(
-          extent={{-80,80},{80,-80}},
-          lineColor={175,175,175},
-          fillColor={238,46,47},
+          extent={{-30,94},{30,20}},
+          lineColor={95,95,95},
+          fillColor={95,95,95},
+          fillPattern=FillPattern.Solid),
+        Ellipse(
+          extent={{-22,88},{0,80}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
+          fillPattern=FillPattern.Solid),
+        Ellipse(
+          extent={{0,88},{22,80}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
+          fillPattern=FillPattern.Solid),
+        Line(
+          points={{16,70},{22,58}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{0,70},{6,58}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{0,70},{-6,58}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{16,70},{10,58}},
+          color={255,0,0},
+          thickness=0.5),
+        Rectangle(
+          extent={{-30,8},{30,-66}},
+          lineColor={95,95,95},
+          fillColor={95,95,95},
+          fillPattern=FillPattern.Solid),
+        Ellipse(
+          extent={{-22,2},{0,-6}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
+          fillPattern=FillPattern.Solid),
+        Ellipse(
+          extent={{0,2},{22,-6}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
+        Line(
+          points={{-16,-16},{-22,-28}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{-16,-16},{-10,-28}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{0,-16},{-6,-28}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{0,-16},{6,-28}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{16,-16},{10,-28}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{16,-16},{22,-28}},
+          color={255,0,0},
+          thickness=0.5),
         Rectangle(
-          extent={{-62,80},{-58,-80}},
+          extent={{30,24},{60,20}},
           lineColor={0,0,255},
           pattern=LinePattern.None,
-          fillColor={0,0,0},
+          fillColor={0,0,127},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-22,80},{-18,-80}},
+          extent={{30,-62},{60,-66}},
           lineColor={0,0,255},
           pattern=LinePattern.None,
-          fillColor={0,0,0},
+          fillColor={0,0,127},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{18,80},{22,-80}},
+          extent={{62,2},{92,-2}},
           lineColor={0,0,255},
           pattern=LinePattern.None,
-          fillColor={0,0,0},
+          fillColor={0,0,127},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{58,80},{62,-80}},
+          extent={{58,-80},{62,24}},
           lineColor={0,0,255},
           pattern=LinePattern.None,
-          fillColor={0,0,0},
+          fillColor={0,0,127},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-80,65},{-4,56}},
-          lineColor={0,0,255},
+          extent={{-90,2},{-60,-2}},
+          lineColor={238,46,47},
           pattern=LinePattern.None,
-          fillColor={255,0,0},
+          fillColor={238,46,47},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-4,66},{80,56}},
-          lineColor={0,0,255},
+          extent={{-64,-82},{-60,74}},
+          lineColor={238,46,47},
           pattern=LinePattern.None,
-          fillColor={0,0,255},
+          fillColor={238,46,47},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-80,-55},{-4,-64}},
-          lineColor={0,0,255},
+          extent={{-60,-12},{16,-16}},
+          lineColor={238,46,47},
           pattern=LinePattern.None,
-          fillColor={255,0,0},
+          fillColor={238,46,47},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-4,-54},{80,-64}},
-          lineColor={0,0,255},
+          extent={{-60,74},{16,70}},
+          lineColor={238,46,47},
+          pattern=LinePattern.None,
+          fillColor={238,46,47},
+          fillPattern=FillPattern.Solid),
+        Line(
+          points={{-16,70},{-22,58}},
+          color={255,0,0},
+          thickness=0.5),
+        Line(
+          points={{-16,70},{-10,58}},
+          color={255,0,0},
+          thickness=0.5),
+        Rectangle(
+          extent={{-60,-78},{-10,-82}},
+          lineColor={238,46,47},
           pattern=LinePattern.None,
-          fillColor={0,0,255},
+          fillColor={238,46,47},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-80,-56},{-4,-64}},
+          extent={{10,-78},{62,-82}},
           lineColor={0,0,255},
-          pattern=LinePattern.None)}),
-    Diagram(
-      coordinateSystem(
-        preserveAspectRatio=false,
-        extent={{-100,-100},{100,160}})),
+          pattern=LinePattern.None,
+          fillColor={0,0,127},
+          fillPattern=FillPattern.Solid)}),
     Documentation(
-      info="<html>
-      </html>",
       revisions="<html>
-  <li>
-  August 1, 2020, by Hagar Elarga:<br/>
-  First implementation.
-  </li>
-  </ul>
-  </html>"));
-{% endraw %}end {{ model_filename }};
+<ul>
+<li>
+March 30, 2014 by Sen Huang:<br/>
+First implementation.
+</li>
+</ul>
+</html>"));
+end CoolingTowerWithBypass;
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect_Instance.mopt`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-  // heating indirect instance
+  // cooling indirect instance
   {{ model.modelica_type }} {{ model.id }}(
-    allowFlowReversal1=false,
-    allowFlowReversal2=false,
-    show_T=true,
     redeclare package Medium={{ globals.medium_w }},
+    allowFlowReversal1=true,
+    allowFlowReversal2=true,
     mDis_flow_nominal=mDis_flow_nominal_{{ couplings.load_couplings[0].id }},
     mBui_flow_nominal=mBui_flow_nominal_{{ couplings.load_couplings[0].id }},
-    dpValve_nominal=6000,
     dp1_nominal=500,
     dp2_nominal=500,
+    dpValve_nominal=7000,
     use_Q_flow_nominal=true,
     Q_flow_nominal=Q_flow_nominal_{{ couplings.load_couplings[0].id }},
-    T_a1_nominal=55+273.15,
-    T_a2_nominal=35+273.15,
-    k=0.1,
-    Ti=60,
-    reverseActing=true)
-    annotation (Placement({{ diagram.transformation.hea_ets.ets }}));
+    // TODO: dehardcode the nominal temperatures?
+    T_a1_nominal=273.15+5,
+    T_a2_nominal=273.15+13)
+    "Indirect cooling energy transfer station ETS."
+    annotation (Placement({{ diagram.transformation.coo_ets.ets }}));
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/load_base.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/load_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,10 @@
-"""
-****************************************************************************************************
-:copyright (c) 2019-2022, Alliance for Sustainable Energy, LLC, and other contributors.
+# :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
+# See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met:
-
-Redistributions of source code must retain the above copyright notice, this list of conditions
-and the following disclaimer.
-
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials provided with the
-distribution.
-
-Neither the name of the copyright holder nor the names of its contributors may be used to endorse
-or promote products derived from this software without specific prior written permission.
-
-Redistribution of this software, without modification, must refer to the software by the same
-designation. Redistribution of a modified version of this software (i) may not refer to the
-modified version by the same designation, or by any confusingly similar designation, and
-(ii) must refer to the underlying software originally provided by Alliance as “URBANopt”. Except
-to comply with the foregoing, the term “URBANopt”, or any confusingly similar designation may
-not be used to refer to any modified version of this software or any modified version of the
-underlying software originally provided by Alliance without the prior written consent of Alliance.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
-IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
-IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-****************************************************************************************************
-"""
 from pathlib import Path
 
 from geojson_modelica_translator.model_connectors.model_base import ModelBase
 from geojson_modelica_translator.utils import convert_c_to_k
 
 
 class LoadBase(ModelBase):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/spawn.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/spawn.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/teaser.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/teaser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,9 @@
-"""
-****************************************************************************************************
-:copyright (c) 2019-2022, Alliance for Sustainable Energy, LLC, and other contributors.
-
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met:
-
-Redistributions of source code must retain the above copyright notice, this list of conditions
-and the following disclaimer.
-
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials provided with the
-distribution.
-
-Neither the name of the copyright holder nor the names of its contributors may be used to endorse
-or promote products derived from this software without specific prior written permission.
-
-Redistribution of this software, without modification, must refer to the software by the same
-designation. Redistribution of a modified version of this software (i) may not refer to the
-modified version by the same designation, or by any confusingly similar designation, and
-(ii) must refer to the underlying software originally provided by Alliance as “URBANopt”. Except
-to comply with the foregoing, the term “URBANopt”, or any confusingly similar designation may
-not be used to refer to any modified version of this software or any modified version of the
-underlying software originally provided by Alliance without the prior written consent of Alliance.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
-IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
-IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-****************************************************************************************************
-"""
+# :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
+# See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import glob
 import os
 import shutil
 from os import fdopen, remove
 from shutil import copymode, move
 from tempfile import mkstemp
@@ -395,15 +360,15 @@
                 mofile.insert_component(
                     'Buildings.Controls.OBC.CDL.Interfaces.RealOutput', 'TAir',
                     modifications={
                         'quantity': '"ThermodynamicTemperature"',
                         'unit': '"K"',
                         'displayUnit': '"degC"',
                     },
-                    conditional=f'if {thermal_zone_name}.ATot > 0 or {thermal_zone_name}.VAir > 0',
+                    conditional=f'if {thermal_zone_name}.VAir > 0',
                     string_comment='Room air temperature',
                     annotations=['Placement(transformation(extent={{100,38},{120,58}}))']
                 )
 
                 # In TEASER 0.7.5 the hConvWinOut, hConvExt, hConvWin, hConvInt, hConvFloor, hConvRoof in various of
                 # the ReducedOrder models should be hCon* not hConv*. This has been fixed on the development branch
                 # of TEASER, but the team doesn't appear to be releasing nor merging the development branch (yet).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/RunSpawnCouplingBuilding.most` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/RunSpawnCouplingBuilding.most`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/RunTeaserCouplingBuilding.most` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/RunTeaserCouplingBuilding.most`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnBuilding.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnBuilding.mot`

 * *Files 2% similar despite different names*

```diff
@@ -110,24 +110,26 @@
     each T_aHeaWat_nominal=T_aHeaWat_nominal,
     final mLoaHea_flow_nominal=mLoaHea_flow_nominal,
     final mLoaCoo_flow_nominal=mLoaCoo_flow_nominal)
     "Terminal unit"
     annotation (Placement(transformation(extent={{-140,-2},{-120,20}})));
   Buildings.Experimental.DHC.Loads.BaseClasses.FlowDistribution disFloHea(
     redeclare package Medium=MediumW,
+    allowFlowReversal=true,
     m_flow_nominal=sum(
       terUni.mHeaWat_flow_nominal .* terUni.facMulZon),
     have_pum=have_pum,
     dp_nominal=100000,
     nPorts_a1=nZon,
     nPorts_b1=nZon)
     "Heating water distribution system"
     annotation (Placement(transformation(extent={{-236,-188},{-216,-168}})));
   Buildings.Experimental.DHC.Loads.BaseClasses.FlowDistribution disFloCoo(
     redeclare package Medium=MediumW,
+    allowFlowReversal=true,
     m_flow_nominal=sum(
       terUni.mChiWat_flow_nominal .* terUni.facMulZon),
     typDis=Buildings.Experimental.DHC.Loads.BaseClasses.Types.DistributionType.ChilledWater,
     dp_nominal=100000,
     have_pum=have_pum,
     nPorts_a1=nZon,
     nPorts_b1=nZon)
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnCouplingBuilding.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnCouplingBuilding.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/Spawn_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/Spawn_Instance.mopt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
   parameter Modelica.Units.SI.MassFlowRate mLoaCoo_flow_nominal_{{ model.id }}[{{ model.id }}.nZon]={(-1*{{ model.id }}.QCoo_flow_nominal[i]*(0.06)/1000) for i in 1:{{ model.id }}.nZon};
   parameter Modelica.Units.SI.MassFlowRate mLoaHea_flow_nominal_{{ model.id }}[{{ model.id }}.nZon]={({{ model.id }}.QHea_flow_nominal[i]*(0.05)/1000) for i in 1:{{ model.id }}.nZon};
   {{ model.modelica_type }} {{ model.id }}(
     mLoaCoo_flow_nominal=mLoaCoo_flow_nominal_{{ model.id }},
     mLoaHea_flow_nominal=mLoaHea_flow_nominal_{{ model.id }},
+    allowFlowReversal = true,
     nPorts_aHeaWat=1,
     nPorts_bHeaWat=1,
     nPorts_aChiWat=1,
     nPorts_bChiWat=1,
     have_pum=true)
     "Building spawn model"
     annotation (Placement({{ diagram.transformation.spawn_load.load }}));
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserBuilding.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserBuilding.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserCouplingBuilding.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserCouplingBuilding.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuilding.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuilding.mot`

 * *Files 1% similar despite different names*

```diff
@@ -175,21 +175,21 @@
     "Cooling terminal unit"
     annotation (Placement(transformation(extent={{70,26},{90,46}})));
   Buildings.Controls.OBC.CDL.Interfaces.RealOutput QReqHotWat_flow(
     unit="W") if have_hotWat
     "SHW load"
     annotation (Placement(transformation(extent={{300,-140},{340,-100}}),iconTransformation(extent={{-40,-40},{40,40}},rotation=-90,origin={280,-340})));
   Modelica.Blocks.Interfaces.RealOutput QReqHea_flow(
-    quantity="HeatFlowRate",
-    unit="W") if have_heaLoa
+    each quantity="HeatFlowRate",
+    each unit="W") if have_heaLoa
     "Heating load"
     annotation (Placement(transformation(extent={{300,20},{340,60}}),iconTransformation(extent={{-20,-20},{20,20}},rotation=-90,origin={200,-320})));
   Modelica.Blocks.Interfaces.RealOutput QReqCoo_flow(
-    quantity="HeatFlowRate",
-    unit="W") if have_cooLoa
+    each quantity="HeatFlowRate",
+    each unit="W") if have_cooLoa
     "Cooling load"
     annotation (Placement(transformation(extent={{300,-20},{340,20}}),iconTransformation(extent={{-20,-20},{20,20}},rotation=-90,origin={260,-320})));
   Buildings.Controls.OBC.CDL.Continuous.Sources.Constant noHea(
     k=0) if not have_heaWat
     "No heating system"
     annotation (Placement(transformation(extent={{80,120},{100,140}})));
   Buildings.Controls.OBC.CDL.Continuous.Sources.Constant noCoo(
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuildingWithETS.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuildingWithETS.mot`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 within {{ project_name }}.Loads.{{ model_name }};
 {% raw %}model building
   "Model of a building with an internal ETS. Building loads provided as time series"
   extends Buildings.Experimental.DHC.Loads.Combined.BaseClasses.PartialBuildingWithETS(
+    final allowFlowReversalSer=true,
     // redeclare Buildings.Experimental.DHC.Loads.BaseClasses.Examples.BaseClasses.BuildingTimeSeries bui(
-    {% endraw %}redeclare {{ project_name }}.Loads.{{ model_name }}.BuildingTimeSeries bui(
+    {% endraw %}redeclare {{ project_name }}.Loads.{{ model_name }}.TimeSeriesBuilding bui(
       {% raw %}have_hotWat=false,
       T_aHeaWat_nominal=ets.THeaWatSup_nominal,
       T_bHeaWat_nominal=ets.THeaWatRet_nominal,
       T_aChiWat_nominal=ets.TChiWatSup_nominal,
       T_bChiWat_nominal=ets.TChiWatRet_nominal,
       facMulHea=10*QHea_flow_nominal/(1.7E5),
       facMulCoo=40*QCoo_flow_nominal/(-1.5E5)),
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMassFlowTemperatures.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMassFlowTemperatures.mot`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-within {{project_name}}.Loads.{{ model_name }};
+within {{ project_name }}.Loads.{{ model_name }};
 model building
   "Time series water mass flow rates and temperatures for a building thermal
   loads generated from Energy PLus."
   extends Modelica.Icons.Example;
   {% raw %}package MediumW=Buildings.Media.Water;
   {% endraw %}parameter String filNam="modelica://{{project_name}}/Loads/{{data['load_resources_path']}}/{{data['time_series']['filename']}}";
   {% raw %}parameter Modelica.Units.SI.MassFlowRate mChW_flow_nominal=getPeakMassFlowRate(
@@ -57,27 +57,39 @@
     annotation (Placement(transformation(extent={{80,-60},{60,-40}})));
   Modelica.Blocks.Sources.RealExpression mBuiHW(
     y=buiMasTem.y[5])
     annotation (Placement(transformation(extent={{80,-20},{60,0}})));
   Modelica.Blocks.Sources.RealExpression mBuiChW(
     y=buiMasTem.y[6])
     annotation (Placement(transformation(extent={{82,50},{62,70}})));
-  Modelica.Fluid.Interfaces.FluidPorts_a ports_aHeaWat[1]
+  Modelica.Fluid.Interfaces.FluidPorts_a ports_aHeaWat[1](
+    redeclare package Medium=MediumW)
     "Heating water inlet port"
     annotation (Placement(transformation(extent={{-310,-100},{-290,-20}}),iconTransformation(extent={{-310,-100},{-290,-20}})));
-  Modelica.Fluid.Interfaces.FluidPorts_a ports_aChiWat[1]
+  Modelica.Fluid.Interfaces.FluidPorts_a ports_aChiWat[1](
+    redeclare package Medium=MediumW)
     "Chilled water inlet port"
     annotation (Placement(transformation(extent={{-310,-300},{-290,-220}}),iconTransformation(extent={{-310,-220},{-290,-140}})));
-  Modelica.Fluid.Interfaces.FluidPorts_b ports_bHeaWat[1]
+  Modelica.Fluid.Interfaces.FluidPorts_b ports_bHeaWat[1](
+    redeclare package Medium=MediumW)
     "Heating water outlet port"
     annotation (Placement(transformation(extent={{290,-100},{310,-20}}),iconTransformation(extent={{290,-100},{310,-20}})));
-  Modelica.Fluid.Interfaces.FluidPorts_b ports_bChiWat[1]
+  Modelica.Fluid.Interfaces.FluidPorts_b ports_bChiWat[1](
+    redeclare package Medium=MediumW)
     "Chilled water outlet port"
     annotation (Placement(transformation(extent={{290,-300},{310,-220}}),iconTransformation(extent={{290,-220},{310,-140}})));
+  Modelica.Blocks.Interfaces.RealOutput y
+    annotation (Placement(visible=true,transformation(origin={308,146},extent={{-10,-10},{10,10}},rotation=0),iconTransformation(origin={416,152},extent={{-10,-10},{10,10}},rotation=0)));
+  Modelica.Blocks.Interfaces.RealOutput realOutput
+    annotation (Placement(visible=true,transformation(origin={312,110},extent={{-10,-10},{10,10}},rotation=0),iconTransformation(origin={416,152},extent={{-10,-10},{10,10}},rotation=0)));
 equation
+  connect(buiMasTem.y[2],y)
+    annotation (Line(points={{100,-10},{96,-10},{96,146},{308,146}},color={0,0,127}));
+  connect(buiMasTem.y[4],realOutput)
+    annotation (Line(points={{100,-10},{192,-10},{192,110},{312,110}},color={0,0,127}));
   connect(buiCooSin.ports[1],ports_aChiWat[1])
     annotation (Line(points={{-60,10},{-60,-46},{-118,-46},{-118,-290},{-300,-290}},color={0,0,127}));
   connect(buiHeaSin.ports[1],ports_aHeaWat[1])
     annotation (Line(points={{-60,-70},{-180,-70},{-180,-90},{-300,-90}},color={0,0,127}));
   connect(supChiWat.ports[1],ports_bChiWat[1])
     annotation (Line(points={{20,10},{160,10},{160,-290},{300,-290}},color={0,0,127}));
   connect(supHeaWat.ports[1],ports_bHeaWat[1])
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeries_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeries_Instance.mopt`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,28 @@
   // time series load
   {{ model.modelica_type }} {{ model.id }}(
     {% if model.is_5g_district == 'bui' %}
+    allowFlowReversalBui = true,
+    allowFlowReversalSer = true,
     {{ model.is_5g_district }}(T_aHeaWat_nominal(displayUnit="K")=318.15,
     T_aChiWat_nominal(displayUnit="K")=291.15,
     delTAirCoo(displayUnit="degC")=10,
     delTAirHea(displayUnit="degC")=20,
     k=0.1,
     Ti=120
     ), ets(have_hotWat = false)
     {% else %}
+    allowFlowReversal = true,
     T_aHeaWat_nominal(displayUnit="K")=318.15,
     T_aChiWat_nominal(displayUnit="K")=280.15,
     delTAirCoo(displayUnit="degC")=10,
     delTAirHea(displayUnit="degC")=20,
     k=0.1,
-    Ti=120
+    Ti=120,
+    nPorts_aHeaWat=1,
+    nPorts_bHeaWat=1,
+    nPorts_aChiWat=1,
+    nPorts_bChiWat=1
     {% endif %}
     )
     "Building model integrating multiple time series thermal zones."
     annotation (Placement({{ diagram.transformation.ts_load.load }}));
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/templates/getPeakMassFlowRate.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/templates/getPeakMassFlowRate.mot`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+within {{ project_name }}.Loads.{{ model_name }};
 function getPeakMassFlowRate
   "Function that reads the peak mass flow Rate from the load profile"
   input String string
     "String that is written before the '=' sign";
   input String filNam
     "Name of data file with heating and cooling  water mass flow rate"
     annotation (Dialog(loadSelector(filter="Load file (*.mos)",caption="Select load file")));
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-function getPeakMassFlowRate "Function that reads the peak mass flow Rate from
-the load profile" input String string "String that is written before the '='
-sign"; input String filNam "Name of data file with heating and cooling water
-mass flow rate" annotation (Dialog(loadSelector(filter="Load file
-(*.mos)",caption="Select load file"))); output Real number "Number that is read
-from the file"; protected String lin "Line that is used in parser"; Integer
-iLin "Line number"; Integer index=0 "Index of string 'string'"; Integer staInd
-"Start index used when parsing a real number"; Integer nexInd "Next index used
-when parsing a real number"; Boolean found "Flag, true if 'string' has been
-found"; Boolean EOF "Flag, true if EOF has been reached"; String del "Found
-delimiter"; algorithm // Get line that contains 'string' iLin := 0; EOF :
-= false; while(not EOF) and(index == 0) loop iLin := iLin+1; (lin,EOF) :
-= Modelica.Utilities.Streams.readLine( fileName=filNam, lineNumber=iLin); index
-:= Modelica.Utilities.Strings.find( string=lin, searchString=string,
-startIndex=1, caseSensitive=true); end while; assert( not EOF, "Error: Did not
-find '"+string+"' when scanning '"+filNam+"'."+"\n Check for correct file
-syntax."); // Search for the equality sign (del,nexInd) :
-= Modelica.Utilities.Strings.scanDelimiter( string=lin,
+within {{ project_name }}.Loads.{{ model_name }}; function getPeakMassFlowRate
+"Function that reads the peak mass flow Rate from the load profile" input
+String string "String that is written before the '=' sign"; input String filNam
+"Name of data file with heating and cooling water mass flow rate" annotation
+(Dialog(loadSelector(filter="Load file (*.mos)",caption="Select load file")));
+output Real number "Number that is read from the file"; protected String lin
+"Line that is used in parser"; Integer iLin "Line number"; Integer index=0
+"Index of string 'string'"; Integer staInd "Start index used when parsing a
+real number"; Integer nexInd "Next index used when parsing a real number";
+Boolean found "Flag, true if 'string' has been found"; Boolean EOF "Flag, true
+if EOF has been reached"; String del "Found delimiter"; algorithm // Get line
+that contains 'string' iLin := 0; EOF := false; while(not EOF) and(index == 0)
+loop iLin := iLin+1; (lin,EOF) := Modelica.Utilities.Streams.readLine
+( fileName=filNam, lineNumber=iLin); index := Modelica.Utilities.Strings.find
+( string=lin, searchString=string, startIndex=1, caseSensitive=true); end
+while; assert( not EOF, "Error: Did not find '"+string+"' when scanning
+'"+filNam+"'."+"\n Check for correct file syntax."); // Search for the equality
+sign (del,nexInd) := Modelica.Utilities.Strings.scanDelimiter( string=lin,
 startIndex=Modelica.Utilities.Strings.length(string)+1, requiredDelimiters=
 {"="}, message="Failed to find '=' when reading water mass flow rate in
 '"+filNam+"'."); // Read the value behind it. number :
 = Modelica.Utilities.Strings.scanReal( string=lin, startIndex=nexInd,
 message="Failed to read double value when reading water mass flow rate in
 '"+filNam+"'."); annotation ( Documentation( info="
 This Function that reads a double value from a text file.
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/time_series.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/time_series.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,9 @@
-"""
-****************************************************************************************************
-:copyright (c) 2019-2022, Alliance for Sustainable Energy, LLC, and other contributors.
-
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met:
-
-Redistributions of source code must retain the above copyright notice, this list of conditions
-and the following disclaimer.
-
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials provided with the
-distribution.
-
-Neither the name of the copyright holder nor the names of its contributors may be used to endorse
-or promote products derived from this software without specific prior written permission.
-
-Redistribution of this software, without modification, must refer to the software by the same
-designation. Redistribution of a modified version of this software (i) may not refer to the
-modified version by the same designation, or by any confusingly similar designation, and
-(ii) must refer to the underlying software originally provided by Alliance as “URBANopt”. Except
-to comply with the foregoing, the term “URBANopt”, or any confusingly similar designation may
-not be used to refer to any modified version of this software or any modified version of the
-underlying software originally provided by Alliance without the prior written consent of Alliance.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
-IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
-IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-****************************************************************************************************
-"""
+# :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
+# See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import os
 import shutil
 
 from geojson_modelica_translator.model_connectors.load_connectors.load_base import (
     LoadBase
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/load_connectors/time_series_mft_ets_coupling.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/load_connectors/time_series_mft_ets_coupling.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 
     def __init__(self, system_parameters, geojson_load):
         super().__init__(system_parameters, geojson_load)
         self.id = 'TimeSerMFTLoa_' + simple_uuid()
 
         # Note that the order of the required MO files is important as it will be the order that
         # the "package.order" will be in.
-        self.required_mo_files.append(os.path.join(self.template_dir, 'getPeakMassFlowRate.mo'))
+        # self.required_mo_files.append(os.path.join(self.template_dir, 'getPeakMassFlowRate.mo'))
 
     def to_modelica(self, scaffold):
         """
         Create TimeSeries models based on the data in the building and geojson
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
 
         # MassFlowrate Temperature models
         time_series_mft_template = self.template_env.get_template("TimeSeriesMassFlowTemperatures.mot")
+        peak_mfr_template = self.template_env.get_template("getPeakMassFlowRate.mot")
+        templates = {"building.mo": time_series_mft_template, "getPeakMassFlowRate.mo": peak_mfr_template}
 
         b_modelica_path = ModelicaPath(
             self.building_name, scaffold.loads_path.files_dir, True
         )
 
         # grab the data from the system_parameter file for this building id
         # TODO: create method in system_parameter class to make this easier and respect the defaults
@@ -86,22 +88,24 @@
             ets_data = self.system_parameters.get_param_by_building_id(
                 self.building_id,
                 "ets_indirect_parameters"
             )
         else:
             raise Exception("Only ETS Model of type 'Indirect Heating and Cooling' type enabled currently")
 
-        self.run_template(
-            template=time_series_mft_template,
-            save_file_name=Path(b_modelica_path.files_dir) / "building.mo",
-            project_name=scaffold.project_name,
-            model_name=self.building_name,
-            data=template_data,
-            ets_data=ets_data,
-        )
+        # Run building templates to write actual Modelica models
+        for template_filename, template in templates.items():
+            self.run_template(
+                template=template,
+                save_file_name=Path(b_modelica_path.files_dir) / template_filename,
+                project_name=scaffold.project_name,
+                model_name=self.building_name,
+                data=template_data,
+                ets_data=ets_data,
+            )
 
         self.copy_required_mo_files(b_modelica_path.files_dir, within=f'{scaffold.project_name}.Loads')
 
         # Run post process to create the remaining project files for this building
         self.post_process(scaffold)
 
     def post_process(self, scaffold):
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/model_base.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/model_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import logging
 import shutil
 from pathlib import Path
+from typing import Union
 
 from jinja2 import Environment, FileSystemLoader, StrictUndefined, exceptions
 from modelica_builder.model import Model
 
 from geojson_modelica_translator.jinja_filters import ALL_CUSTOM_FILTERS
 
 logger = logging.getLogger(__name__)
@@ -15,20 +16,19 @@
     level=logging.INFO,
     format='%(asctime)s - %(levelname)s: %(message)s',
     datefmt='%d-%b-%y %H:%M:%S',
 )
 
 
 class ModelBase(object):
-    """
-    Base class of the model connectors. The connectors can utilize various methods to create a building (or other
+    """Base class of the model connectors. The connectors can utilize various methods to create a building (or other
     feature) to a detailed Modelica connection. For example, a simple RC model (using TEASER), a ROM, CSV file, etc.
     """
     # model_name must be overridden in subclass
-    model_name = None
+    model_name: Union[str, None] = None
 
     def __init__(self, system_parameters, template_dir):
         """
         Base initializer
 
         :param system_parameters: SystemParameters object
         """
@@ -54,16 +54,16 @@
 
         # Read district-level system params. Used when templating ets mofiles, for instance in heating_indirect.py
         if system_parameters is not None:
             # TODO: DRY up this handling of different generations
             district_params = self.system_parameters.get_param("district_system")
             if 'fifth_generation' in district_params:
                 self.district_template_data = {
-                    "temp_setpoint_hhw": district_params['fifth_generation']['central_heating_plant_parameters']['temp_setpoint_hhw'],
-                    "temp_setpoint_chw": district_params['fifth_generation']['central_cooling_plant_parameters']['temp_setpoint_chw'],
+                    # "temp_setpoint_hhw": district_params['fifth_generation']['central_heating_plant_parameters']['temp_setpoint_hhw'],
+                    # "temp_setpoint_chw": district_params['fifth_generation']['central_cooling_plant_parameters']['temp_setpoint_chw'],
                 }
             elif 'fourth_generation' in district_params:
                 self.district_template_data = {
                     "temp_setpoint_hhw": district_params['fourth_generation']['central_heating_plant_parameters']['temp_setpoint_hhw'],
                     "temp_setpoint_chw": district_params['fourth_generation']['central_cooling_plant_parameters']['temp_setpoint_chw'],
                 }
 
@@ -110,15 +110,17 @@
         :param do_not_add_to_list: boolean, set to true if you do not want the file to be added to the package.order
         :param kwargs: These are the arguments that need to be passed to the template.
 
         :return: None
         """
         file_data = template.render(**kwargs)
 
-        Path(save_file_name).parent.mkdir(parents=True, exist_ok=True)
+        if not isinstance(save_file_name, Path):
+            save_file_name = Path(save_file_name)
+        save_file_name.parent.mkdir(parents=True, exist_ok=True)
         with open(save_file_name, "w") as f:
             f.write(file_data)
 
         # add to the list of files to include in the package
         if not do_not_add_to_list:
             self.template_files_to_include.append(Path(save_file_name).stem)
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_2_pipe.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_2_pipe.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_ambient_water_stub.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_ambient_water_stub.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_base.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_base.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_chilled_water_stub.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_chilled_water_stub.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/network_heated_water_stub.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/network_heated_water_stub.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/templates/Network2Pipe_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/templates/Network2Pipe_Instance.mopt`

 * *Files 0% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 
   {{ model.modelica_type }} {{ model.id }}(
     redeclare final package Medium={{ globals.medium_w }},
     final nCon=nBui_{{ model.id }},
     iConDpSen=nBui_{{ model.id }},
     final mDis_flow_nominal=mDis_flow_nominal_{{ model.id }},
     final mCon_flow_nominal=mCon_flow_nominal_{{ model.id }},
-    final allowFlowReversal=false,
+    final allowFlowReversal=true,
     dpDis_nominal=dpDis_nominal_{{ model.id }})
     "Distribution network."
     annotation (Placement({{ diagram.transformation.two_pipe.network }}));
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/templates/NetworkAmbientWaterStub_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkHeatedWaterStub_Instance.mopt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
   // heated water stub
   // TODO: move these components into a single component
   Buildings.Fluid.Sources.MassFlowSource_T supHeaWat(
     redeclare package Medium={{ globals.medium_w }},
     use_m_flow_in=true,
     use_T_in=false,
-    T={{ sys_params.district_system.fifth_generation.central_heating_plant_parameters.temp_setpoint_hhw }}+273.15,
+    T={{ sys_params.district_system.fourth_generation.central_heating_plant_parameters.temp_setpoint_hhw }}+273.15,
     nPorts=1)
     "Heating water supply temperature (district side)."
     annotation (Placement({{ diagram.transformation.sup_hea_wat.boundary_pt }}));
   Buildings.Fluid.Sources.Boundary_pT sinHeaWat(
     redeclare package Medium={{ globals.medium_w }},
     nPorts=1)
     "Heating water sink (district side)"
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/templates/NetworkChilledWaterStub_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkChilledWaterStub_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/networks/templates/NetworkHeatedWaterStub_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkAmbientWaterStub_Instance.mopt`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
   // heated water stub
   // TODO: move these components into a single component
-  Buildings.Fluid.Sources.MassFlowSource_T supHeaWat(
+  {% for building in range( sys_params.num_buildings ) %}
+  Buildings.Fluid.Sources.MassFlowSource_T supHeaWat_{{ building + 1 }}(
     redeclare package Medium={{ globals.medium_w }},
     use_m_flow_in=true,
     use_T_in=false,
-    T={{ sys_params.district_system.fourth_generation.central_heating_plant_parameters.temp_setpoint_hhw }}+273.15,
+    {% if 'ghe_parameters' in sys_params.district_system['fifth_generation'] %}
+    T={{ sys_params.district_system.fifth_generation.ghe_parameters.soil.undisturbed_temp}}+273.15,
+    {% else %}
+    T={{ sys_params.district_system.fifth_generation.central_heating_plant_parameters.temp_setpoint_hhw }}+273.15,
+    {% endif %}
     nPorts=1)
     "Heating water supply temperature (district side)."
     annotation (Placement({{ diagram.transformation.sup_hea_wat.boundary_pt }}));
-  Buildings.Fluid.Sources.Boundary_pT sinHeaWat(
+  {% endfor %}Buildings.Fluid.Sources.Boundary_pT sinHeaWat(
     redeclare package Medium={{ globals.medium_w }},
-    nPorts=1)
+    nPorts={{ sys_params.num_buildings }})
     "Heating water sink (district side)"
     annotation (Placement({{ diagram.transformation.sin_hea_wat.boundary_pt }}));
 
   // NOTE: this differential pressure setpoint is currently utilized by plants elsewhere
   parameter Modelica.Units.SI.Pressure dpSetPoi_{{ model.id }}=50000
     "Differential pressure setpoint";
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/chp.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/chp.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters)
         self.id = 'chpPla_' + simple_uuid()
         self.chp_installed = self.system_parameters.get_param(
             "$.district_system.fourth_generation.central_heating_plant_parameters.chp_installed"
         )
-        if not self.chp_installed:
+        if self.chp_installed is not True:
             self.required_mo_files.append(Path(self.template_dir) / 'CentralHeatingPlant.mo')
             self.id = 'heaPla' + simple_uuid()
 
         self.required_mo_files.append(Path(self.template_dir) / 'Boiler_TParallel.mo')
         self.required_mo_files.append(Path(self.template_dir) / 'BoilerStage.mo')
         self.required_mo_files.append(Path(self.template_dir) / 'HeatingWaterPumpSpeed.mo')
         self.required_mo_files.append(Path(self.template_dir) / 'PartialPlantParallel.mo')
@@ -80,15 +80,18 @@
             within=f'{scaffold.project_name}.Plants')
 
         package = PackageParser(scaffold.project_path)
         if 'Plants' not in package.order:
             package.add_model('Plants')
             package.save()
 
-        package_models = ['CentralHeatingPlant'] + [Path(mo).stem for mo in self.required_mo_files]
+        if self.chp_installed:
+            package_models = ['CentralHeatingPlant'] + [Path(mo).stem for mo in self.required_mo_files]
+        else:
+            package_models = [Path(mo).stem for mo in self.required_mo_files]
         plants_package = PackageParser(scaffold.plants_path.files_dir)
         if plants_package.order_data is None:
             plants_package = PackageParser.new_from_template(
                 path=scaffold.plants_path.files_dir,
                 name="Plants",
                 order=package_models,
                 within=scaffold.project_name)
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/cooling_plant.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/cooling_plant.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/plant_base.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/plant_base.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/BoilerStage.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/BoilerStage.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel.mo`

 * *Files 1% similar despite different names*

```diff
@@ -42,260 +42,260 @@
 00000290: 6561 7446 6c6f 7752 6174 6520 515f 666c  eatFlowRate Q_fl
 000002a0: 6f77 5f6e 6f6d 696e 616c 3b0a 2020 7061  ow_nominal;.  pa
 000002b0: 7261 6d65 7465 7220 496e 7465 6765 7220  rameter Integer 
 000002c0: 6e75 6d42 6f69 3b0a 2020 4d6f 6465 6c69  numBoi;.  Modeli
 000002d0: 6361 2e42 6c6f 636b 732e 496e 7465 7266  ca.Blocks.Interf
 000002e0: 6163 6573 2e52 6561 6c4f 7574 7075 7420  aces.RealOutput 
 000002f0: 5442 6f69 4c76 675b 6e75 6d5d 280a 2020  TBoiLvg[num](.  
-00000300: 2020 756e 6974 3d22 4b22 2c0a 2020 2020    unit="K",.    
-00000310: 6469 7370 6c61 7955 6e69 743d 2264 6567  displayUnit="deg
-00000320: 4322 290a 2020 2020 2242 6f69 6c65 7220  C").    "Boiler 
-00000330: 6c65 6176 696e 6720 7761 7465 7220 7465  leaving water te
-00000340: 6d70 6572 6174 7572 652e 220a 2020 2020  mperature.".    
-00000350: 616e 6e6f 7461 7469 6f6e 2028 506c 6163  annotation (Plac
-00000360: 656d 656e 7428 7472 616e 7366 6f72 6d61  ement(transforma
-00000370: 7469 6f6e 2865 7874 656e 743d 7b7b 3130  tion(extent={{10
-00000380: 302c 3330 7d2c 7b31 3230 2c35 307d 7d29  0,30},{120,50}})
-00000390: 2c69 636f 6e54 7261 6e73 666f 726d 6174  ,iconTransformat
-000003a0: 696f 6e28 6578 7465 6e74 3d7b 7b31 3030  ion(extent={{100
-000003b0: 2c33 307d 2c7b 3132 302c 3530 7d7d 2929  ,30},{120,50}}))
-000003c0: 293b 0a20 204d 6f64 656c 6963 612e 426c  );.  Modelica.Bl
-000003d0: 6f63 6b73 2e4d 6174 682e 426f 6f6c 6561  ocks.Math.Boolea
-000003e0: 6e54 6f52 6561 6c20 626f 6f54 6f52 6561  nToReal booToRea
-000003f0: 5b6e 756d 5d28 0a20 2020 2065 6163 6820  [num](.    each 
-00000400: 6669 6e61 6c20 7265 616c 5472 7565 3d31  final realTrue=1
-00000410: 2c0a 2020 2020 6561 6368 2066 696e 616c  ,.    each final
-00000420: 2072 6561 6c46 616c 7365 3d30 290a 2020   realFalse=0).  
-00000430: 2020 2242 6f6f 6c65 616e 2074 6f20 7265    "Boolean to re
-00000440: 616c 2028 6966 2074 7275 6520 7468 656e  al (if true then
-00000450: 2031 2065 6c73 6520 3029 220a 2020 2020   1 else 0)".    
-00000460: 616e 6e6f 7461 7469 6f6e 2028 506c 6163  annotation (Plac
-00000470: 656d 656e 7428 7472 616e 7366 6f72 6d61  ement(transforma
-00000480: 7469 6f6e 2865 7874 656e 743d 7b7b 2d39  tion(extent={{-9
-00000490: 322c 3430 7d2c 7b2d 3732 2c36 307d 7d29  2,40},{-72,60}})
-000004a0: 2929 3b0a 2020 4d6f 6465 6c69 6361 2e42  ));.  Modelica.B
-000004b0: 6c6f 636b 732e 496e 7465 7266 6163 6573  locks.Interfaces
-000004c0: 2e42 6f6f 6c65 616e 496e 7075 7420 6f6e  .BooleanInput on
-000004d0: 5b6e 756d 5d0a 2020 2020 224f 6e20 7369  [num].    "On si
-000004e0: 676e 616c 206f 6620 7468 6520 706c 616e  gnal of the plan
-000004f0: 7422 0a20 2020 2061 6e6e 6f74 6174 696f  t".    annotatio
-00000500: 6e20 2850 6c61 6365 6d65 6e74 2874 7261  n (Placement(tra
-00000510: 6e73 666f 726d 6174 696f 6e28 6578 7465  nsformation(exte
-00000520: 6e74 3d7b 7b2d 3132 302c 3430 7d2c 7b2d  nt={{-120,40},{-
-00000530: 3130 302c 3630 7d7d 292c 6963 6f6e 5472  100,60}}),iconTr
-00000540: 616e 7366 6f72 6d61 7469 6f6e 2865 7874  ansformation(ext
-00000550: 656e 743d 7b7b 2d31 3230 2c38 307d 2c7b  ent={{-120,80},{
-00000560: 2d31 3030 2c31 3030 7d7d 2929 293b 0a20  -100,100}})));. 
-00000570: 2042 7569 6c64 696e 6773 2e43 6f6e 7472   Buildings.Contr
-00000580: 6f6c 732e 436f 6e74 696e 756f 7573 2e4c  ols.Continuous.L
-00000590: 696d 5049 4420 5049 5f54 426f 694c 7667  imPID PI_TBoiLvg
-000005a0: 280a 2020 2020 755f 7328 0a20 2020 2020  (.    u_s(.     
-000005b0: 2075 6e69 743d 224b 222c 0a20 2020 2020   unit="K",.     
-000005c0: 2064 6973 706c 6179 556e 6974 3d22 6465   displayUnit="de
-000005d0: 6743 2229 2c0a 2020 2020 755f 6d28 0a20  gC"),.    u_m(. 
-000005e0: 2020 2020 2075 6e69 743d 224b 222c 0a20       unit="K",. 
-000005f0: 2020 2020 2064 6973 706c 6179 556e 6974       displayUnit
-00000600: 3d22 6465 6743 2229 2c0a 2020 2020 636f  ="degC"),.    co
-00000610: 6e74 726f 6c6c 6572 5479 7065 3d4d 6f64  ntrollerType=Mod
-00000620: 656c 6963 612e 426c 6f63 6b73 2e54 7970  elica.Blocks.Typ
-00000630: 6573 2e53 696d 706c 6543 6f6e 7472 6f6c  es.SimpleControl
-00000640: 6c65 722e 5049 2c0a 2020 2020 6b3d 312c  ler.PI,.    k=1,
-00000650: 0a20 2020 2054 693d 3630 2c0a 2020 2020  .    Ti=60,.    
-00000660: 7265 7665 7273 6541 6374 696e 673d 7472  reverseActing=tr
-00000670: 7565 2c0a 2020 2020 7265 7365 743d 4275  ue,.    reset=Bu
-00000680: 696c 6469 6e67 732e 5479 7065 732e 5265  ildings.Types.Re
-00000690: 7365 742e 4469 7361 626c 6564 2c0a 2020  set.Disabled,.  
-000006a0: 2020 795f 7265 7365 743d 3029 0a20 2020    y_reset=0).   
-000006b0: 2022 426f 696c 6572 206c 6561 7669 6e67   "Boiler leaving
-000006c0: 2077 6174 6572 2074 656d 7065 7261 7475   water temperatu
-000006d0: 7265 2063 6f6e 7472 6f6c 6c65 7222 0a20  re controller". 
-000006e0: 2020 2061 6e6e 6f74 6174 696f 6e20 2850     annotation (P
-000006f0: 6c61 6365 6d65 6e74 2874 7261 6e73 666f  lacement(transfo
-00000700: 726d 6174 696f 6e28 6578 7465 6e74 3d7b  rmation(extent={
-00000710: 7b2d 3732 2c2d 3430 7d2c 7b2d 3532 2c2d  {-72,-40},{-52,-
-00000720: 3230 7d7d 2929 293b 0a20 204d 6f64 656c  20}})));.  Model
-00000730: 6963 612e 426c 6f63 6b73 2e4d 6174 682e  ica.Blocks.Math.
-00000740: 5072 6f64 7563 7420 7072 6f5b 6e75 6d42  Product pro[numB
-00000750: 6f69 5d0a 2020 2020 2250 726f 6475 6374  oi].    "Product
-00000760: 206f 6620 504c 5220 616e 6420 4f6e 2062   of PLR and On b
-00000770: 6f69 6c65 7220 7369 676e 616c 220a 2020  oiler signal".  
-00000780: 2020 616e 6e6f 7461 7469 6f6e 2028 506c    annotation (Pl
-00000790: 6163 656d 656e 7428 7472 616e 7366 6f72  acement(transfor
-000007a0: 6d61 7469 6f6e 2865 7874 656e 743d 7b7b  mation(extent={{
-000007b0: 2d33 362c 3138 7d2c 7b2d 3136 2c33 387d  -36,18},{-16,38}
-000007c0: 7d29 2929 3b0a 2020 4275 696c 6469 6e67  })));.  Building
-000007d0: 732e 466c 7569 642e 5365 6e73 6f72 732e  s.Fluid.Sensors.
-000007e0: 5465 6d70 6572 6174 7572 6554 776f 506f  TemperatureTwoPo
-000007f0: 7274 2073 656e 5444 6973 5375 7028 0a20  rt senTDisSup(. 
-00000800: 2020 2072 6564 6563 6c61 7265 2066 696e     redeclare fin
-00000810: 616c 2070 6163 6b61 6765 204d 6564 6975  al package Mediu
-00000820: 6d3d 4d65 6469 756d 2c0a 2020 2020 6669  m=Medium,.    fi
-00000830: 6e61 6c20 6d5f 666c 6f77 5f6e 6f6d 696e  nal m_flow_nomin
-00000840: 616c 3d6d 5f66 6c6f 775f 6e6f 6d69 6e61  al=m_flow_nomina
-00000850: 6c29 0a20 2020 2022 4469 7374 7269 6374  l).    "District
-00000860: 2d73 6964 6520 2870 7269 6d61 7279 2920  -side (primary) 
-00000870: 7375 7070 6c79 2074 656d 7065 7261 7475  supply temperatu
-00000880: 7265 2073 656e 736f 7222 0a20 2020 2061  re sensor".    a
-00000890: 6e6e 6f74 6174 696f 6e20 2850 6c61 6365  nnotation (Place
-000008a0: 6d65 6e74 2874 7261 6e73 666f 726d 6174  ment(transformat
-000008b0: 696f 6e28 6578 7465 6e74 3d7b 7b2d 3130  ion(extent={{-10
-000008c0: 2c2d 3130 7d2c 7b31 302c 3130 7d7d 2c72  ,-10},{10,10}},r
-000008d0: 6f74 6174 696f 6e3d 302c 6f72 6967 696e  otation=0,origin
-000008e0: 3d7b 3736 2c30 7d29 2929 3b0a 2020 4d6f  ={76,0})));.  Mo
-000008f0: 6465 6c69 6361 2e42 6c6f 636b 732e 496e  delica.Blocks.In
-00000900: 7465 7266 6163 6573 2e52 6561 6c49 6e70  terfaces.RealInp
-00000910: 7574 2054 4865 6157 6174 5365 740a 2020  ut THeaWatSet.  
-00000920: 2020 2248 6561 7469 6e67 2077 6174 6572    "Heating water
-00000930: 2073 6574 2070 6f69 6e74 2e22 0a20 2020   set point.".   
-00000940: 2061 6e6e 6f74 6174 696f 6e20 2850 6c61   annotation (Pla
-00000950: 6365 6d65 6e74 2874 7261 6e73 666f 726d  cement(transform
-00000960: 6174 696f 6e28 6578 7465 6e74 3d7b 7b2d  ation(extent={{-
-00000970: 3130 2c2d 3130 7d2c 7b31 302c 3130 7d7d  10,-10},{10,10}}
-00000980: 2c72 6f74 6174 696f 6e3d 302c 6f72 6967  ,rotation=0,orig
-00000990: 696e 3d7b 2d31 3130 2c2d 3630 7d29 2c69  in={-110,-60}),i
-000009a0: 636f 6e54 7261 6e73 666f 726d 6174 696f  conTransformatio
-000009b0: 6e28 6578 7465 6e74 3d7b 7b2d 3130 2c2d  n(extent={{-10,-
-000009c0: 3130 7d2c 7b31 302c 3130 7d7d 2c72 6f74  10},{10,10}},rot
-000009d0: 6174 696f 6e3d 302c 6f72 6967 696e 3d7b  ation=0,origin={
-000009e0: 2d31 3130 2c2d 3630 7d29 2929 3b0a 6571  -110,-60})));.eq
-000009f0: 7561 7469 6f6e 0a20 2066 6f72 2069 2069  uation.  for i i
-00000a00: 6e20 313a 6e75 6d42 6f69 206c 6f6f 700a  n 1:numBoi loop.
-00000a10: 2020 2020 636f 6e6e 6563 7428 706f 7274      connect(port
-00000a20: 5f61 2c62 6f69 5b69 5d2e 706f 7274 5f61  _a,boi[i].port_a
-00000a30: 290a 2020 2020 2020 616e 6e6f 7461 7469  ).      annotati
-00000a40: 6f6e 2028 4c69 6e65 2870 6f69 6e74 733d  on (Line(points=
-00000a50: 7b7b 2d31 3030 2c30 7d2c 7b2d 322c 307d  {{-100,0},{-2,0}
-00000a60: 7d2c 636f 6c6f 723d 7b30 2c31 3237 2c32  },color={0,127,2
-00000a70: 3535 7d29 293b 0a20 2020 2063 6f6e 6e65  55}));.    conne
-00000a80: 6374 2876 616c 5b69 5d2e 706f 7274 5f62  ct(val[i].port_b
-00000a90: 2c73 656e 5444 6973 5375 702e 706f 7274  ,senTDisSup.port
-00000aa0: 5f61 290a 2020 2020 2020 616e 6e6f 7461  _a).      annota
-00000ab0: 7469 6f6e 2028 4c69 6e65 2870 6f69 6e74  tion (Line(point
-00000ac0: 733d 7b7b 3536 2c30 7d2c 7b36 362c 307d  s={{56,0},{66,0}
-00000ad0: 7d2c 636f 6c6f 723d 7b30 2c31 3237 2c32  },color={0,127,2
-00000ae0: 3535 7d29 293b 0a20 2065 6e64 2066 6f72  55}));.  end for
-00000af0: 3b0a 2020 636f 6e6e 6563 7428 6f6e 2c62  ;.  connect(on,b
-00000b00: 6f6f 546f 5265 612e 7529 0a20 2020 2061  ooToRea.u).    a
-00000b10: 6e6e 6f74 6174 696f 6e20 284c 696e 6528  nnotation (Line(
-00000b20: 706f 696e 7473 3d7b 7b2d 3131 302c 3530  points={{-110,50
-00000b30: 7d2c 7b2d 3934 2c35 307d 7d2c 636f 6c6f  },{-94,50}},colo
-00000b40: 723d 7b32 3535 2c30 2c32 3535 7d29 293b  r={255,0,255}));
-00000b50: 0a20 2063 6f6e 6e65 6374 2862 6f69 2e70  .  connect(boi.p
-00000b60: 6f72 745f 622c 7661 6c2e 706f 7274 5f61  ort_b,val.port_a
-00000b70: 290a 2020 2020 616e 6e6f 7461 7469 6f6e  ).    annotation
-00000b80: 2028 4c69 6e65 2870 6f69 6e74 733d 7b7b   (Line(points={{
-00000b90: 3138 2c30 7d2c 7b33 362c 307d 7d2c 636f  18,0},{36,0}},co
-00000ba0: 6c6f 723d 7b30 2c31 3237 2c32 3535 7d29  lor={0,127,255})
-00000bb0: 293b 0a20 2063 6f6e 6e65 6374 2862 6f69  );.  connect(boi
-00000bc0: 2e54 2c54 426f 694c 7667 290a 2020 2020  .T,TBoiLvg).    
-00000bd0: 616e 6e6f 7461 7469 6f6e 2028 4c69 6e65  annotation (Line
-00000be0: 2870 6f69 6e74 733d 7b7b 3139 2c38 7d2c  (points={{19,8},
-00000bf0: 7b32 302c 387d 2c7b 3230 2c34 307d 2c7b  {20,8},{20,40},{
-00000c00: 3131 302c 3430 7d7d 2c63 6f6c 6f72 3d7b  110,40}},color={
-00000c10: 302c 302c 3132 377d 2929 3b0a 2020 636f  0,0,127}));.  co
-00000c20: 6e6e 6563 7428 626f 6f54 6f52 6561 2e79  nnect(booToRea.y
-00000c30: 2c66 696c 7465 722e 7529 0a20 2020 2061  ,filter.u).    a
-00000c40: 6e6e 6f74 6174 696f 6e20 284c 696e 6528  nnotation (Line(
-00000c50: 706f 696e 7473 3d7b 7b2d 3731 2c35 307d  points={{-71,50}
-00000c60: 2c7b 2d36 302c 3530 7d2c 7b2d 3630 2c38  ,{-60,50},{-60,8
-00000c70: 347d 2c7b 2d35 352e 322c 3834 7d7d 2c63  4},{-55.2,84}},c
-00000c80: 6f6c 6f72 3d7b 302c 302c 3132 377d 2929  olor={0,0,127}))
-00000c90: 3b0a 2020 636f 6e6e 6563 7428 626f 6f54  ;.  connect(booT
-00000ca0: 6f52 6561 2e79 2c70 726f 2e75 3129 0a20  oRea.y,pro.u1). 
-00000cb0: 2020 2061 6e6e 6f74 6174 696f 6e20 284c     annotation (L
-00000cc0: 696e 6528 706f 696e 7473 3d7b 7b2d 3731  ine(points={{-71
-00000cd0: 2c35 307d 2c7b 2d36 302c 3530 7d2c 7b2d  ,50},{-60,50},{-
-00000ce0: 3630 2c33 347d 2c7b 2d33 382c 3334 7d7d  60,34},{-38,34}}
-00000cf0: 2c63 6f6c 6f72 3d7b 302c 302c 3132 377d  ,color={0,0,127}
-00000d00: 2929 3b0a 2020 636f 6e6e 6563 7428 7072  ));.  connect(pr
-00000d10: 6f2e 792c 626f 692e 7929 0a20 2020 2061  o.y,boi.y).    a
-00000d20: 6e6e 6f74 6174 696f 6e20 284c 696e 6528  nnotation (Line(
-00000d30: 706f 696e 7473 3d7b 7b2d 3135 2c32 387d  points={{-15,28}
-00000d40: 2c7b 2d31 322c 3238 7d2c 7b2d 3132 2c38  ,{-12,28},{-12,8
-00000d50: 7d2c 7b2d 342c 387d 7d2c 636f 6c6f 723d  },{-4,8}},color=
-00000d60: 7b30 2c30 2c31 3237 7d29 293b 0a20 2063  {0,0,127}));.  c
-00000d70: 6f6e 6e65 6374 2850 495f 5442 6f69 4c76  onnect(PI_TBoiLv
-00000d80: 672e 792c 7072 6f5b 315d 2e75 3229 0a20  g.y,pro[1].u2). 
-00000d90: 2020 2061 6e6e 6f74 6174 696f 6e20 284c     annotation (L
-00000da0: 696e 6528 706f 696e 7473 3d7b 7b2d 3531  ine(points={{-51
-00000db0: 2c2d 3330 7d2c 7b2d 3434 2c2d 3330 7d2c  ,-30},{-44,-30},
-00000dc0: 7b2d 3434 2c32 327d 2c7b 2d33 382c 3232  {-44,22},{-38,22
-00000dd0: 7d7d 2c63 6f6c 6f72 3d7b 302c 302c 3132  }},color={0,0,12
-00000de0: 377d 2929 3b0a 2020 636f 6e6e 6563 7428  7}));.  connect(
-00000df0: 5049 5f54 426f 694c 7667 2e79 2c70 726f  PI_TBoiLvg.y,pro
-00000e00: 5b32 5d2e 7532 290a 2020 2020 616e 6e6f  [2].u2).    anno
-00000e10: 7461 7469 6f6e 2028 4c69 6e65 2870 6f69  tation (Line(poi
-00000e20: 6e74 733d 7b7b 2d35 312c 2d33 307d 2c7b  nts={{-51,-30},{
-00000e30: 2d34 342c 2d33 307d 2c7b 2d34 342c 3232  -44,-30},{-44,22
-00000e40: 7d2c 7b2d 3338 2c32 327d 7d2c 636f 6c6f  },{-38,22}},colo
-00000e50: 723d 7b30 2c30 2c31 3237 7d29 293b 0a20  r={0,0,127}));. 
-00000e60: 2063 6f6e 6e65 6374 2870 6f72 745f 622c   connect(port_b,
-00000e70: 7365 6e54 4469 7353 7570 2e70 6f72 745f  senTDisSup.port_
-00000e80: 6229 0a20 2020 2061 6e6e 6f74 6174 696f  b).    annotatio
-00000e90: 6e20 284c 696e 6528 706f 696e 7473 3d7b  n (Line(points={
-00000ea0: 7b31 3030 2c30 7d2c 7b38 362c 307d 7d2c  {100,0},{86,0}},
-00000eb0: 636f 6c6f 723d 7b30 2c31 3237 2c32 3535  color={0,127,255
-00000ec0: 7d29 293b 0a20 2063 6f6e 6e65 6374 2873  }));.  connect(s
-00000ed0: 656e 5444 6973 5375 702e 542c 5049 5f54  enTDisSup.T,PI_T
-00000ee0: 426f 694c 7667 2e75 5f6d 290a 2020 2020  BoiLvg.u_m).    
-00000ef0: 616e 6e6f 7461 7469 6f6e 2028 4c69 6e65  annotation (Line
-00000f00: 2870 6f69 6e74 733d 7b7b 3736 2c31 317d  (points={{76,11}
-00000f10: 2c7b 3736 2c31 387d 2c7b 3632 2c31 387d  ,{76,18},{62,18}
-00000f20: 2c7b 3632 2c2d 3734 7d2c 7b2d 3632 2c2d  ,{62,-74},{-62,-
-00000f30: 3734 7d2c 7b2d 3632 2c2d 3432 7d7d 2c63  74},{-62,-42}},c
-00000f40: 6f6c 6f72 3d7b 302c 302c 3132 377d 2929  olor={0,0,127}))
-00000f50: 3b0a 2020 636f 6e6e 6563 7428 5448 6561  ;.  connect(THea
-00000f60: 5761 7453 6574 2c50 495f 5442 6f69 4c76  WatSet,PI_TBoiLv
-00000f70: 672e 755f 7329 0a20 2020 2061 6e6e 6f74  g.u_s).    annot
-00000f80: 6174 696f 6e20 284c 696e 6528 706f 696e  ation (Line(poin
-00000f90: 7473 3d7b 7b2d 3131 302c 2d36 307d 2c7b  ts={{-110,-60},{
-00000fa0: 2d39 322c 2d36 307d 2c7b 2d39 322c 2d33  -92,-60},{-92,-3
-00000fb0: 307d 2c7b 2d37 342c 2d33 307d 7d2c 636f  0},{-74,-30}},co
-00000fc0: 6c6f 723d 7b30 2c30 2c31 3237 7d29 293b  lor={0,0,127}));
-00000fd0: 0a20 2061 6e6e 6f74 6174 696f 6e20 280a  .  annotation (.
-00000fe0: 2020 2020 446f 6375 6d65 6e74 6174 696f      Documentatio
-00000ff0: 6e28 0a20 2020 2020 2069 6e66 6f3d 223c  n(.      info="<
-00001000: 6874 6d6c 3e0a 2020 3c70 3e0a 2020 5468  html>.  <p>.  Th
-00001010: 6973 206d 6f64 656c 2069 6d70 6c65 6d65  is model impleme
-00001020: 6e74 7320 6120 6865 6174 696e 6720 7761  nts a heating wa
-00001030: 7465 7220 7061 7261 6c6c 656c 2062 6f69  ter parallel boi
-00001040: 6c65 7273 2e20 466f 7220 7468 6520 626f  lers. For the bo
-00001050: 696c 6572 206d 6f64 656c 2070 6c65 6173  iler model pleas
-00001060: 6520 7365 650a 2020 3c61 2068 7265 663d  e see.  <a href=
-00001070: 5c22 6d6f 6465 6c69 6361 3a2f 2f42 7569  \"modelica://Bui
-00001080: 6c64 696e 6773 2e46 6c75 6964 2e42 6f69  ldings.Fluid.Boi
-00001090: 6c65 7273 2e42 6f69 6c65 7250 6f6c 796e  lers.BoilerPolyn
-000010a0: 6f6d 6961 6c5c 223e 4275 696c 6469 6e67  omial\">Building
-000010b0: 732e 466c 7569 642e 426f 696c 6572 732e  s.Fluid.Boilers.
-000010c0: 426f 696c 6572 506f 6c79 6e6f 6d69 616c  BoilerPolynomial
-000010d0: 3c2f 613e 2e0a 2020 3c2f 703e 0a20 203c  </a>..  </p>.  <
-000010e0: 2f68 746d 6c3e 222c 0a20 2020 2020 2072  /html>",.      r
-000010f0: 6576 6973 696f 6e73 3d22 3c68 746d 6c3e  evisions="<html>
-00001100: 0a20 203c 756c 3e0a 2020 3c6c 693e 0a20  .  <ul>.  <li>. 
-00001110: 204a 756e 6520 3330 2c20 3230 3230 2c20   June 30, 2020, 
-00001120: 6279 2048 6167 6172 2045 6c61 7267 613a  by Hagar Elarga:
-00001130: 3c62 722f 3e0a 2020 4669 7273 7420 696d  <br/>.  First im
-00001140: 706c 656d 656e 7461 7469 6f6e 2e0a 2020  plementation..  
-00001150: 3c2f 6c69 3e0a 2020 3c2f 756c 3e0a 2020  </li>.  </ul>.  
-00001160: 3c2f 6874 6d6c 3e22 292c 0a20 2020 2049  </html>"),.    I
-00001170: 636f 6e28 0a20 2020 2020 2067 7261 7068  con(.      graph
-00001180: 6963 733d 7b0a 2020 2020 2020 2020 4c69  ics={.        Li
-00001190: 6e65 280a 2020 2020 2020 2020 2020 706f  ne(.          po
-000011a0: 696e 7473 3d7b 7b2d 3932 2c30 7d2c 7b30  ints={{-92,0},{0
-000011b0: 2c30 7d7d 2c0a 2020 2020 2020 2020 2020  ,0}},.          
-000011c0: 636f 6c6f 723d 7b32 382c 3130 382c 3230  color={28,108,20
-000011d0: 307d 2c0a 2020 2020 2020 2020 2020 7468  0},.          th
-000011e0: 6963 6b6e 6573 733d 3129 2c0a 2020 2020  ickness=1),.    
-000011f0: 2020 2020 4c69 6e65 280a 2020 2020 2020      Line(.      
-00001200: 2020 2020 706f 696e 7473 3d7b 7b30 2c30      points={{0,0
-00001210: 7d2c 7b39 322c 307d 7d2c 0a20 2020 2020  },{92,0}},.     
-00001220: 2020 2020 2063 6f6c 6f72 3d7b 3233 382c       color={238,
-00001230: 3436 2c34 377d 2c0a 2020 2020 2020 2020  46,47},.        
-00001240: 2020 7468 6963 6b6e 6573 733d 3129 2c0a    thickness=1),.
-00001250: 2020 2020 2020 2020 5265 6374 616e 676c          Rectangl
-00001260: 6528 0a20 2020 2020 2020 2020 2065 7874  e(.          ext
-00001270: 656e 743d 7b7b 2d35 342c 3534 7d2c 7b35  ent={{-54,54},{5
-00001280: 342c 2d35 347d 7d2c 0a20 2020 2020 2020  4,-54}},.       
-00001290: 2020 206c 696e 6543 6f6c 6f72 3d7b 3130     lineColor={10
-000012a0: 322c 3434 2c31 3435 7d29 7d29 293b 0a65  2,44,145})}));.e
-000012b0: 6e64 2042 6f69 6c65 725f 5450 6172 616c  nd Boiler_TParal
-000012c0: 6c65 6c3b 0a                             lel;.
+00000300: 2020 6561 6368 2075 6e69 743d 224b 222c    each unit="K",
+00000310: 0a20 2020 2065 6163 6820 6469 7370 6c61  .    each displa
+00000320: 7955 6e69 743d 2264 6567 4322 290a 2020  yUnit="degC").  
+00000330: 2020 2242 6f69 6c65 7220 6c65 6176 696e    "Boiler leavin
+00000340: 6720 7761 7465 7220 7465 6d70 6572 6174  g water temperat
+00000350: 7572 652e 220a 2020 2020 616e 6e6f 7461  ure.".    annota
+00000360: 7469 6f6e 2028 506c 6163 656d 656e 7428  tion (Placement(
+00000370: 7472 616e 7366 6f72 6d61 7469 6f6e 2865  transformation(e
+00000380: 7874 656e 743d 7b7b 3130 302c 3330 7d2c  xtent={{100,30},
+00000390: 7b31 3230 2c35 307d 7d29 2c69 636f 6e54  {120,50}}),iconT
+000003a0: 7261 6e73 666f 726d 6174 696f 6e28 6578  ransformation(ex
+000003b0: 7465 6e74 3d7b 7b31 3030 2c33 307d 2c7b  tent={{100,30},{
+000003c0: 3132 302c 3530 7d7d 2929 293b 0a20 204d  120,50}})));.  M
+000003d0: 6f64 656c 6963 612e 426c 6f63 6b73 2e4d  odelica.Blocks.M
+000003e0: 6174 682e 426f 6f6c 6561 6e54 6f52 6561  ath.BooleanToRea
+000003f0: 6c20 626f 6f54 6f52 6561 5b6e 756d 5d28  l booToRea[num](
+00000400: 0a20 2020 2065 6163 6820 6669 6e61 6c20  .    each final 
+00000410: 7265 616c 5472 7565 3d31 2c0a 2020 2020  realTrue=1,.    
+00000420: 6561 6368 2066 696e 616c 2072 6561 6c46  each final realF
+00000430: 616c 7365 3d30 290a 2020 2020 2242 6f6f  alse=0).    "Boo
+00000440: 6c65 616e 2074 6f20 7265 616c 2028 6966  lean to real (if
+00000450: 2074 7275 6520 7468 656e 2031 2065 6c73   true then 1 els
+00000460: 6520 3029 220a 2020 2020 616e 6e6f 7461  e 0)".    annota
+00000470: 7469 6f6e 2028 506c 6163 656d 656e 7428  tion (Placement(
+00000480: 7472 616e 7366 6f72 6d61 7469 6f6e 2865  transformation(e
+00000490: 7874 656e 743d 7b7b 2d39 322c 3430 7d2c  xtent={{-92,40},
+000004a0: 7b2d 3732 2c36 307d 7d29 2929 3b0a 2020  {-72,60}})));.  
+000004b0: 4d6f 6465 6c69 6361 2e42 6c6f 636b 732e  Modelica.Blocks.
+000004c0: 496e 7465 7266 6163 6573 2e42 6f6f 6c65  Interfaces.Boole
+000004d0: 616e 496e 7075 7420 6f6e 5b6e 756d 5d0a  anInput on[num].
+000004e0: 2020 2020 224f 6e20 7369 676e 616c 206f      "On signal o
+000004f0: 6620 7468 6520 706c 616e 7422 0a20 2020  f the plant".   
+00000500: 2061 6e6e 6f74 6174 696f 6e20 2850 6c61   annotation (Pla
+00000510: 6365 6d65 6e74 2874 7261 6e73 666f 726d  cement(transform
+00000520: 6174 696f 6e28 6578 7465 6e74 3d7b 7b2d  ation(extent={{-
+00000530: 3132 302c 3430 7d2c 7b2d 3130 302c 3630  120,40},{-100,60
+00000540: 7d7d 292c 6963 6f6e 5472 616e 7366 6f72  }}),iconTransfor
+00000550: 6d61 7469 6f6e 2865 7874 656e 743d 7b7b  mation(extent={{
+00000560: 2d31 3230 2c38 307d 2c7b 2d31 3030 2c31  -120,80},{-100,1
+00000570: 3030 7d7d 2929 293b 0a20 2042 7569 6c64  00}})));.  Build
+00000580: 696e 6773 2e43 6f6e 7472 6f6c 732e 436f  ings.Controls.Co
+00000590: 6e74 696e 756f 7573 2e4c 696d 5049 4420  ntinuous.LimPID 
+000005a0: 5049 5f54 426f 694c 7667 280a 2020 2020  PI_TBoiLvg(.    
+000005b0: 755f 7328 0a20 2020 2020 2075 6e69 743d  u_s(.      unit=
+000005c0: 224b 222c 0a20 2020 2020 2064 6973 706c  "K",.      displ
+000005d0: 6179 556e 6974 3d22 6465 6743 2229 2c0a  ayUnit="degC"),.
+000005e0: 2020 2020 755f 6d28 0a20 2020 2020 2075      u_m(.      u
+000005f0: 6e69 743d 224b 222c 0a20 2020 2020 2064  nit="K",.      d
+00000600: 6973 706c 6179 556e 6974 3d22 6465 6743  isplayUnit="degC
+00000610: 2229 2c0a 2020 2020 636f 6e74 726f 6c6c  "),.    controll
+00000620: 6572 5479 7065 3d4d 6f64 656c 6963 612e  erType=Modelica.
+00000630: 426c 6f63 6b73 2e54 7970 6573 2e53 696d  Blocks.Types.Sim
+00000640: 706c 6543 6f6e 7472 6f6c 6c65 722e 5049  pleController.PI
+00000650: 2c0a 2020 2020 6b3d 312c 0a20 2020 2054  ,.    k=1,.    T
+00000660: 693d 3630 2c0a 2020 2020 7265 7665 7273  i=60,.    revers
+00000670: 6541 6374 696e 673d 7472 7565 2c0a 2020  eActing=true,.  
+00000680: 2020 7265 7365 743d 4275 696c 6469 6e67    reset=Building
+00000690: 732e 5479 7065 732e 5265 7365 742e 4469  s.Types.Reset.Di
+000006a0: 7361 626c 6564 2c0a 2020 2020 795f 7265  sabled,.    y_re
+000006b0: 7365 743d 3029 0a20 2020 2022 426f 696c  set=0).    "Boil
+000006c0: 6572 206c 6561 7669 6e67 2077 6174 6572  er leaving water
+000006d0: 2074 656d 7065 7261 7475 7265 2063 6f6e   temperature con
+000006e0: 7472 6f6c 6c65 7222 0a20 2020 2061 6e6e  troller".    ann
+000006f0: 6f74 6174 696f 6e20 2850 6c61 6365 6d65  otation (Placeme
+00000700: 6e74 2874 7261 6e73 666f 726d 6174 696f  nt(transformatio
+00000710: 6e28 6578 7465 6e74 3d7b 7b2d 3732 2c2d  n(extent={{-72,-
+00000720: 3430 7d2c 7b2d 3532 2c2d 3230 7d7d 2929  40},{-52,-20}}))
+00000730: 293b 0a20 204d 6f64 656c 6963 612e 426c  );.  Modelica.Bl
+00000740: 6f63 6b73 2e4d 6174 682e 5072 6f64 7563  ocks.Math.Produc
+00000750: 7420 7072 6f5b 6e75 6d42 6f69 5d0a 2020  t pro[numBoi].  
+00000760: 2020 2250 726f 6475 6374 206f 6620 504c    "Product of PL
+00000770: 5220 616e 6420 4f6e 2062 6f69 6c65 7220  R and On boiler 
+00000780: 7369 676e 616c 220a 2020 2020 616e 6e6f  signal".    anno
+00000790: 7461 7469 6f6e 2028 506c 6163 656d 656e  tation (Placemen
+000007a0: 7428 7472 616e 7366 6f72 6d61 7469 6f6e  t(transformation
+000007b0: 2865 7874 656e 743d 7b7b 2d33 362c 3138  (extent={{-36,18
+000007c0: 7d2c 7b2d 3136 2c33 387d 7d29 2929 3b0a  },{-16,38}})));.
+000007d0: 2020 4275 696c 6469 6e67 732e 466c 7569    Buildings.Flui
+000007e0: 642e 5365 6e73 6f72 732e 5465 6d70 6572  d.Sensors.Temper
+000007f0: 6174 7572 6554 776f 506f 7274 2073 656e  atureTwoPort sen
+00000800: 5444 6973 5375 7028 0a20 2020 2072 6564  TDisSup(.    red
+00000810: 6563 6c61 7265 2066 696e 616c 2070 6163  eclare final pac
+00000820: 6b61 6765 204d 6564 6975 6d3d 4d65 6469  kage Medium=Medi
+00000830: 756d 2c0a 2020 2020 6669 6e61 6c20 6d5f  um,.    final m_
+00000840: 666c 6f77 5f6e 6f6d 696e 616c 3d6d 5f66  flow_nominal=m_f
+00000850: 6c6f 775f 6e6f 6d69 6e61 6c29 0a20 2020  low_nominal).   
+00000860: 2022 4469 7374 7269 6374 2d73 6964 6520   "District-side 
+00000870: 2870 7269 6d61 7279 2920 7375 7070 6c79  (primary) supply
+00000880: 2074 656d 7065 7261 7475 7265 2073 656e   temperature sen
+00000890: 736f 7222 0a20 2020 2061 6e6e 6f74 6174  sor".    annotat
+000008a0: 696f 6e20 2850 6c61 6365 6d65 6e74 2874  ion (Placement(t
+000008b0: 7261 6e73 666f 726d 6174 696f 6e28 6578  ransformation(ex
+000008c0: 7465 6e74 3d7b 7b2d 3130 2c2d 3130 7d2c  tent={{-10,-10},
+000008d0: 7b31 302c 3130 7d7d 2c72 6f74 6174 696f  {10,10}},rotatio
+000008e0: 6e3d 302c 6f72 6967 696e 3d7b 3736 2c30  n=0,origin={76,0
+000008f0: 7d29 2929 3b0a 2020 4d6f 6465 6c69 6361  })));.  Modelica
+00000900: 2e42 6c6f 636b 732e 496e 7465 7266 6163  .Blocks.Interfac
+00000910: 6573 2e52 6561 6c49 6e70 7574 2054 4865  es.RealInput THe
+00000920: 6157 6174 5365 740a 2020 2020 2248 6561  aWatSet.    "Hea
+00000930: 7469 6e67 2077 6174 6572 2073 6574 2070  ting water set p
+00000940: 6f69 6e74 2e22 0a20 2020 2061 6e6e 6f74  oint.".    annot
+00000950: 6174 696f 6e20 2850 6c61 6365 6d65 6e74  ation (Placement
+00000960: 2874 7261 6e73 666f 726d 6174 696f 6e28  (transformation(
+00000970: 6578 7465 6e74 3d7b 7b2d 3130 2c2d 3130  extent={{-10,-10
+00000980: 7d2c 7b31 302c 3130 7d7d 2c72 6f74 6174  },{10,10}},rotat
+00000990: 696f 6e3d 302c 6f72 6967 696e 3d7b 2d31  ion=0,origin={-1
+000009a0: 3130 2c2d 3630 7d29 2c69 636f 6e54 7261  10,-60}),iconTra
+000009b0: 6e73 666f 726d 6174 696f 6e28 6578 7465  nsformation(exte
+000009c0: 6e74 3d7b 7b2d 3130 2c2d 3130 7d2c 7b31  nt={{-10,-10},{1
+000009d0: 302c 3130 7d7d 2c72 6f74 6174 696f 6e3d  0,10}},rotation=
+000009e0: 302c 6f72 6967 696e 3d7b 2d31 3130 2c2d  0,origin={-110,-
+000009f0: 3630 7d29 2929 3b0a 6571 7561 7469 6f6e  60})));.equation
+00000a00: 0a20 2066 6f72 2069 2069 6e20 313a 6e75  .  for i in 1:nu
+00000a10: 6d42 6f69 206c 6f6f 700a 2020 2020 636f  mBoi loop.    co
+00000a20: 6e6e 6563 7428 706f 7274 5f61 2c62 6f69  nnect(port_a,boi
+00000a30: 5b69 5d2e 706f 7274 5f61 290a 2020 2020  [i].port_a).    
+00000a40: 2020 616e 6e6f 7461 7469 6f6e 2028 4c69    annotation (Li
+00000a50: 6e65 2870 6f69 6e74 733d 7b7b 2d31 3030  ne(points={{-100
+00000a60: 2c30 7d2c 7b2d 322c 307d 7d2c 636f 6c6f  ,0},{-2,0}},colo
+00000a70: 723d 7b30 2c31 3237 2c32 3535 7d29 293b  r={0,127,255}));
+00000a80: 0a20 2020 2063 6f6e 6e65 6374 2876 616c  .    connect(val
+00000a90: 5b69 5d2e 706f 7274 5f62 2c73 656e 5444  [i].port_b,senTD
+00000aa0: 6973 5375 702e 706f 7274 5f61 290a 2020  isSup.port_a).  
+00000ab0: 2020 2020 616e 6e6f 7461 7469 6f6e 2028      annotation (
+00000ac0: 4c69 6e65 2870 6f69 6e74 733d 7b7b 3536  Line(points={{56
+00000ad0: 2c30 7d2c 7b36 362c 307d 7d2c 636f 6c6f  ,0},{66,0}},colo
+00000ae0: 723d 7b30 2c31 3237 2c32 3535 7d29 293b  r={0,127,255}));
+00000af0: 0a20 2065 6e64 2066 6f72 3b0a 2020 636f  .  end for;.  co
+00000b00: 6e6e 6563 7428 6f6e 2c62 6f6f 546f 5265  nnect(on,booToRe
+00000b10: 612e 7529 0a20 2020 2061 6e6e 6f74 6174  a.u).    annotat
+00000b20: 696f 6e20 284c 696e 6528 706f 696e 7473  ion (Line(points
+00000b30: 3d7b 7b2d 3131 302c 3530 7d2c 7b2d 3934  ={{-110,50},{-94
+00000b40: 2c35 307d 7d2c 636f 6c6f 723d 7b32 3535  ,50}},color={255
+00000b50: 2c30 2c32 3535 7d29 293b 0a20 2063 6f6e  ,0,255}));.  con
+00000b60: 6e65 6374 2862 6f69 2e70 6f72 745f 622c  nect(boi.port_b,
+00000b70: 7661 6c2e 706f 7274 5f61 290a 2020 2020  val.port_a).    
+00000b80: 616e 6e6f 7461 7469 6f6e 2028 4c69 6e65  annotation (Line
+00000b90: 2870 6f69 6e74 733d 7b7b 3138 2c30 7d2c  (points={{18,0},
+00000ba0: 7b33 362c 307d 7d2c 636f 6c6f 723d 7b30  {36,0}},color={0
+00000bb0: 2c31 3237 2c32 3535 7d29 293b 0a20 2063  ,127,255}));.  c
+00000bc0: 6f6e 6e65 6374 2862 6f69 2e54 2c54 426f  onnect(boi.T,TBo
+00000bd0: 694c 7667 290a 2020 2020 616e 6e6f 7461  iLvg).    annota
+00000be0: 7469 6f6e 2028 4c69 6e65 2870 6f69 6e74  tion (Line(point
+00000bf0: 733d 7b7b 3139 2c38 7d2c 7b32 302c 387d  s={{19,8},{20,8}
+00000c00: 2c7b 3230 2c34 307d 2c7b 3131 302c 3430  ,{20,40},{110,40
+00000c10: 7d7d 2c63 6f6c 6f72 3d7b 302c 302c 3132  }},color={0,0,12
+00000c20: 377d 2929 3b0a 2020 636f 6e6e 6563 7428  7}));.  connect(
+00000c30: 626f 6f54 6f52 6561 2e79 2c66 696c 7465  booToRea.y,filte
+00000c40: 722e 7529 0a20 2020 2061 6e6e 6f74 6174  r.u).    annotat
+00000c50: 696f 6e20 284c 696e 6528 706f 696e 7473  ion (Line(points
+00000c60: 3d7b 7b2d 3731 2c35 307d 2c7b 2d36 302c  ={{-71,50},{-60,
+00000c70: 3530 7d2c 7b2d 3630 2c38 347d 2c7b 2d35  50},{-60,84},{-5
+00000c80: 352e 322c 3834 7d7d 2c63 6f6c 6f72 3d7b  5.2,84}},color={
+00000c90: 302c 302c 3132 377d 2929 3b0a 2020 636f  0,0,127}));.  co
+00000ca0: 6e6e 6563 7428 626f 6f54 6f52 6561 2e79  nnect(booToRea.y
+00000cb0: 2c70 726f 2e75 3129 0a20 2020 2061 6e6e  ,pro.u1).    ann
+00000cc0: 6f74 6174 696f 6e20 284c 696e 6528 706f  otation (Line(po
+00000cd0: 696e 7473 3d7b 7b2d 3731 2c35 307d 2c7b  ints={{-71,50},{
+00000ce0: 2d36 302c 3530 7d2c 7b2d 3630 2c33 347d  -60,50},{-60,34}
+00000cf0: 2c7b 2d33 382c 3334 7d7d 2c63 6f6c 6f72  ,{-38,34}},color
+00000d00: 3d7b 302c 302c 3132 377d 2929 3b0a 2020  ={0,0,127}));.  
+00000d10: 636f 6e6e 6563 7428 7072 6f2e 792c 626f  connect(pro.y,bo
+00000d20: 692e 7929 0a20 2020 2061 6e6e 6f74 6174  i.y).    annotat
+00000d30: 696f 6e20 284c 696e 6528 706f 696e 7473  ion (Line(points
+00000d40: 3d7b 7b2d 3135 2c32 387d 2c7b 2d31 322c  ={{-15,28},{-12,
+00000d50: 3238 7d2c 7b2d 3132 2c38 7d2c 7b2d 342c  28},{-12,8},{-4,
+00000d60: 387d 7d2c 636f 6c6f 723d 7b30 2c30 2c31  8}},color={0,0,1
+00000d70: 3237 7d29 293b 0a20 2063 6f6e 6e65 6374  27}));.  connect
+00000d80: 2850 495f 5442 6f69 4c76 672e 792c 7072  (PI_TBoiLvg.y,pr
+00000d90: 6f5b 315d 2e75 3229 0a20 2020 2061 6e6e  o[1].u2).    ann
+00000da0: 6f74 6174 696f 6e20 284c 696e 6528 706f  otation (Line(po
+00000db0: 696e 7473 3d7b 7b2d 3531 2c2d 3330 7d2c  ints={{-51,-30},
+00000dc0: 7b2d 3434 2c2d 3330 7d2c 7b2d 3434 2c32  {-44,-30},{-44,2
+00000dd0: 327d 2c7b 2d33 382c 3232 7d7d 2c63 6f6c  2},{-38,22}},col
+00000de0: 6f72 3d7b 302c 302c 3132 377d 2929 3b0a  or={0,0,127}));.
+00000df0: 2020 636f 6e6e 6563 7428 5049 5f54 426f    connect(PI_TBo
+00000e00: 694c 7667 2e79 2c70 726f 5b32 5d2e 7532  iLvg.y,pro[2].u2
+00000e10: 290a 2020 2020 616e 6e6f 7461 7469 6f6e  ).    annotation
+00000e20: 2028 4c69 6e65 2870 6f69 6e74 733d 7b7b   (Line(points={{
+00000e30: 2d35 312c 2d33 307d 2c7b 2d34 342c 2d33  -51,-30},{-44,-3
+00000e40: 307d 2c7b 2d34 342c 3232 7d2c 7b2d 3338  0},{-44,22},{-38
+00000e50: 2c32 327d 7d2c 636f 6c6f 723d 7b30 2c30  ,22}},color={0,0
+00000e60: 2c31 3237 7d29 293b 0a20 2063 6f6e 6e65  ,127}));.  conne
+00000e70: 6374 2870 6f72 745f 622c 7365 6e54 4469  ct(port_b,senTDi
+00000e80: 7353 7570 2e70 6f72 745f 6229 0a20 2020  sSup.port_b).   
+00000e90: 2061 6e6e 6f74 6174 696f 6e20 284c 696e   annotation (Lin
+00000ea0: 6528 706f 696e 7473 3d7b 7b31 3030 2c30  e(points={{100,0
+00000eb0: 7d2c 7b38 362c 307d 7d2c 636f 6c6f 723d  },{86,0}},color=
+00000ec0: 7b30 2c31 3237 2c32 3535 7d29 293b 0a20  {0,127,255}));. 
+00000ed0: 2063 6f6e 6e65 6374 2873 656e 5444 6973   connect(senTDis
+00000ee0: 5375 702e 542c 5049 5f54 426f 694c 7667  Sup.T,PI_TBoiLvg
+00000ef0: 2e75 5f6d 290a 2020 2020 616e 6e6f 7461  .u_m).    annota
+00000f00: 7469 6f6e 2028 4c69 6e65 2870 6f69 6e74  tion (Line(point
+00000f10: 733d 7b7b 3736 2c31 317d 2c7b 3736 2c31  s={{76,11},{76,1
+00000f20: 387d 2c7b 3632 2c31 387d 2c7b 3632 2c2d  8},{62,18},{62,-
+00000f30: 3734 7d2c 7b2d 3632 2c2d 3734 7d2c 7b2d  74},{-62,-74},{-
+00000f40: 3632 2c2d 3432 7d7d 2c63 6f6c 6f72 3d7b  62,-42}},color={
+00000f50: 302c 302c 3132 377d 2929 3b0a 2020 636f  0,0,127}));.  co
+00000f60: 6e6e 6563 7428 5448 6561 5761 7453 6574  nnect(THeaWatSet
+00000f70: 2c50 495f 5442 6f69 4c76 672e 755f 7329  ,PI_TBoiLvg.u_s)
+00000f80: 0a20 2020 2061 6e6e 6f74 6174 696f 6e20  .    annotation 
+00000f90: 284c 696e 6528 706f 696e 7473 3d7b 7b2d  (Line(points={{-
+00000fa0: 3131 302c 2d36 307d 2c7b 2d39 322c 2d36  110,-60},{-92,-6
+00000fb0: 307d 2c7b 2d39 322c 2d33 307d 2c7b 2d37  0},{-92,-30},{-7
+00000fc0: 342c 2d33 307d 7d2c 636f 6c6f 723d 7b30  4,-30}},color={0
+00000fd0: 2c30 2c31 3237 7d29 293b 0a20 2061 6e6e  ,0,127}));.  ann
+00000fe0: 6f74 6174 696f 6e20 280a 2020 2020 446f  otation (.    Do
+00000ff0: 6375 6d65 6e74 6174 696f 6e28 0a20 2020  cumentation(.   
+00001000: 2020 2069 6e66 6f3d 223c 6874 6d6c 3e0a     info="<html>.
+00001010: 2020 3c70 3e0a 2020 5468 6973 206d 6f64    <p>.  This mod
+00001020: 656c 2069 6d70 6c65 6d65 6e74 7320 6120  el implements a 
+00001030: 6865 6174 696e 6720 7761 7465 7220 7061  heating water pa
+00001040: 7261 6c6c 656c 2062 6f69 6c65 7273 2e20  rallel boilers. 
+00001050: 466f 7220 7468 6520 626f 696c 6572 206d  For the boiler m
+00001060: 6f64 656c 2070 6c65 6173 6520 7365 650a  odel please see.
+00001070: 2020 3c61 2068 7265 663d 5c22 6d6f 6465    <a href=\"mode
+00001080: 6c69 6361 3a2f 2f42 7569 6c64 696e 6773  lica://Buildings
+00001090: 2e46 6c75 6964 2e42 6f69 6c65 7273 2e42  .Fluid.Boilers.B
+000010a0: 6f69 6c65 7250 6f6c 796e 6f6d 6961 6c5c  oilerPolynomial\
+000010b0: 223e 4275 696c 6469 6e67 732e 466c 7569  ">Buildings.Flui
+000010c0: 642e 426f 696c 6572 732e 426f 696c 6572  d.Boilers.Boiler
+000010d0: 506f 6c79 6e6f 6d69 616c 3c2f 613e 2e0a  Polynomial</a>..
+000010e0: 2020 3c2f 703e 0a20 203c 2f68 746d 6c3e    </p>.  </html>
+000010f0: 222c 0a20 2020 2020 2072 6576 6973 696f  ",.      revisio
+00001100: 6e73 3d22 3c68 746d 6c3e 0a20 203c 756c  ns="<html>.  <ul
+00001110: 3e0a 2020 3c6c 693e 0a20 204a 756e 6520  >.  <li>.  June 
+00001120: 3330 2c20 3230 3230 2c20 6279 2048 6167  30, 2020, by Hag
+00001130: 6172 2045 6c61 7267 613a 3c62 722f 3e0a  ar Elarga:<br/>.
+00001140: 2020 4669 7273 7420 696d 706c 656d 656e    First implemen
+00001150: 7461 7469 6f6e 2e0a 2020 3c2f 6c69 3e0a  tation..  </li>.
+00001160: 2020 3c2f 756c 3e0a 2020 3c2f 6874 6d6c    </ul>.  </html
+00001170: 3e22 292c 0a20 2020 2049 636f 6e28 0a20  >"),.    Icon(. 
+00001180: 2020 2020 2067 7261 7068 6963 733d 7b0a       graphics={.
+00001190: 2020 2020 2020 2020 4c69 6e65 280a 2020          Line(.  
+000011a0: 2020 2020 2020 2020 706f 696e 7473 3d7b          points={
+000011b0: 7b2d 3932 2c30 7d2c 7b30 2c30 7d7d 2c0a  {-92,0},{0,0}},.
+000011c0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+000011d0: 7b32 382c 3130 382c 3230 307d 2c0a 2020  {28,108,200},.  
+000011e0: 2020 2020 2020 2020 7468 6963 6b6e 6573          thicknes
+000011f0: 733d 3129 2c0a 2020 2020 2020 2020 4c69  s=1),.        Li
+00001200: 6e65 280a 2020 2020 2020 2020 2020 706f  ne(.          po
+00001210: 696e 7473 3d7b 7b30 2c30 7d2c 7b39 322c  ints={{0,0},{92,
+00001220: 307d 7d2c 0a20 2020 2020 2020 2020 2063  0}},.          c
+00001230: 6f6c 6f72 3d7b 3233 382c 3436 2c34 377d  olor={238,46,47}
+00001240: 2c0a 2020 2020 2020 2020 2020 7468 6963  ,.          thic
+00001250: 6b6e 6573 733d 3129 2c0a 2020 2020 2020  kness=1),.      
+00001260: 2020 5265 6374 616e 676c 6528 0a20 2020    Rectangle(.   
+00001270: 2020 2020 2020 2065 7874 656e 743d 7b7b         extent={{
+00001280: 2d35 342c 3534 7d2c 7b35 342c 2d35 347d  -54,54},{54,-54}
+00001290: 7d2c 0a20 2020 2020 2020 2020 206c 696e  },.          lin
+000012a0: 6543 6f6c 6f72 3d7b 3130 322c 3434 2c31  eColor={102,44,1
+000012b0: 3435 7d29 7d29 293b 0a65 6e64 2042 6f69  45})}));.end Boi
+000012c0: 6c65 725f 5450 6172 616c 6c65 6c3b 0a    ler_TParallel;.
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CentralCoolingPlant.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CentralCoolingPlant.mot`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,16 @@
     redeclare package Medium=Medium)
     "Fluid connector b (positive design flow direction is from port_a to port_b)"
     annotation (Placement(transformation(extent={{150,-60},{170,-40}}),iconTransformation(extent={{90,-60},{110,-40}})));
   Modelica.Blocks.Interfaces.BooleanInput on
     "On signal of the plant"
     annotation (Placement(transformation(extent={{-180,40},{-140,80}}),iconTransformation(extent={{-140,60},{-100,100}})));
   Modelica.Blocks.Interfaces.RealInput TCHWSupSet(
-    final unit="K",
-    displayUnit="degC")
+    each final unit="K",
+    each displayUnit="degC")
     "Set point for chilled water supply temperature"
     annotation (Placement(transformation(extent={{-180,0},{-140,40}}),iconTransformation(extent={{-140,10},{-100,50}})));
   Modelica.Blocks.Interfaces.RealInput dpMea(
     final unit="Pa")
     "Measured pressure difference"
     annotation (Placement(transformation(extent={{-180,-40},{-140,0}}),iconTransformation(extent={{-140,-50},{-100,-10}})));
   Buildings.Applications.BaseClasses.Equipment.ElectricChillerParallel mulChiSys(
@@ -160,15 +160,15 @@
     m_flow_nominal=mCW_flow_nominal,
     dpValve_nominal=dpCWPum_nominal,
     num=numChi)
     "Condenser water pumps"
     annotation (Placement(transformation(extent={{-10,-60},{10,-40}})));
   Buildings.Fluid.Actuators.Valves.TwoWayEqualPercentage valByp(
     redeclare package Medium=Medium,
-    allowFlowReversal=false,
+    allowFlowReversal=true,
     m_flow_nominal=mCHW_flow_nominal*0.05,
     dpValve_nominal=dpCHW_nominal)
     "Chilled water bypass valve"
     annotation (Placement(transformation(extent={{-10,10},{10,-10}},rotation=90,origin={80,0})));
   Buildings.Fluid.Sensors.MassFlowRate senMasFloByp(
     redeclare package Medium=Medium)
     "Chilled water bypass valve mass flow meter"
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CentralHeatingPlant.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CentralHeatingPlant.mo`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     dpValve_nominal=7000,
     num=numBoi,
     l=0.001)
     "Parallel heating water pumps."
     annotation (Placement(transformation(extent={{0,40},{-20,60}})));
   Buildings.Fluid.Actuators.Valves.TwoWayEqualPercentage valByp(
     redeclare package Medium=Medium,
-    allowFlowReversal=false,
+    allowFlowReversal=true,
     m_flow_nominal=mHW_flow_nominal*0.05,
     dpValve_nominal=7000,
     l=0.001)
     "Heating water bypass valve"
     annotation (Placement(transformation(extent={{-10,10},{10,-10}},rotation=90,origin={54,0})));
   Buildings.Fluid.Sensors.MassFlowRate senMasFlo(
     redeclare package Medium=Medium)
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/ChilledWaterPumpSpeed.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/ChilledWaterPumpSpeed.mo`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     "Total mass flowrate of chilled water pumps"
     annotation (Placement(transformation(extent={{-140,20},{-100,60}})));
   Modelica.Blocks.Interfaces.RealInput dpMea(
     final unit="Pa")
     "Measured pressure difference"
     annotation (Placement(transformation(extent={{-140,-60},{-100,-20}})));
   Modelica.Blocks.Interfaces.RealOutput y[numPum](
-    unit="1",
-    min=0,
-    max=1)
+    each unit="1",
+    each min=0,
+    each max=1)
     "Pump speed signal"
     annotation (Placement(transformation(extent={{100,-10},{120,10}})));
   Modelica.Blocks.Math.Product pumSpe[numPum]
     "Output pump speed"
     annotation (Placement(transformation(extent={{40,-10},{60,10}})));
   Buildings.Applications.BaseClasses.Controls.VariableSpeedPumpStage pumStaCon(
     tWai=tWai,
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/ChillerStage.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/ChillerStage.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CoolingPlant_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingPlant_Instance.mopt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Differential pressure setpoint";
   parameter Modelica.Units.SI.Pressure pumDP_{{ model.id }}=dpCHW_nominal_{{ model.id }}+dpSetPoi_{{ model.id }}+200000;
   parameter Modelica.Units.SI.Time tWai_{{ model.id }}=30
     "Waiting time";
   // pumps
   parameter Buildings.Fluid.Movers.Data.Generic perCHWPum_{{ model.id }}(
     pressure=Buildings.Fluid.Movers.BaseClasses.Characteristics.flowParameters(
-      V_flow=((mCHW_flow_nominal_{{ model.id }}/{{ model.id }}.numChi)/1000)*{0.1,1,1.2},
+      V_flow=((mCHW_flow_nominal_{{ model.id }}/numberofchillers)/1000)*{0.1,1,1.2},
       dp=pumDP_{{ model.id }}*{1.2,1,0.1}))
     "Performance data for chilled water pumps";
   parameter Buildings.Fluid.Movers.Data.Generic perCWPum_{{ model.id }}(
     pressure=Buildings.Fluid.Movers.BaseClasses.Characteristics.flowParameters(
       V_flow=mCW_flow_nominal_{{ model.id }}/1000*{0.2,0.6,1.0,1.2},
       dp=(dpCW_nominal_{{ model.id }}+60000+6000)*{1.2,1.1,1.0,0.6}))
     "Performance data for condenser water pumps";
@@ -34,14 +34,15 @@
     "Chilled water supply temperature set point on district level."
     annotation (Placement({{ diagram.transformation.t_set_chi_wat_dis.real_expression }}));
   Modelica.Blocks.Sources.BooleanConstant on_{{ model.id }}
     "On signal of the plant"
     annotation (Placement({{ diagram.transformation.on.boolean_constant }}));
 
   {{ model.modelica_type }} {{ model.id }}(
+    numChi = numberofchillers,
     redeclare Buildings.Fluid.Chillers.Data.ElectricEIR.ElectricEIRChiller_Carrier_19EX_5208kW_6_88COP_Vanes perChi,
     perCHWPum=perCHWPum_{{ model.id }},
     perCWPum=perCWPum_{{ model.id }},
     mCHW_flow_nominal=mCHW_flow_nominal_{{ model.id }},
     dpCHW_nominal=dpCHW_nominal_{{ model.id }},
     QEva_nominal=QEva_nominal_{{ model.id }},
     mMin_flow=mMin_flow_{{ model.id }},
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerParallel.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerParallel.mo`

 * *Files 1% similar despite different names*

```diff
@@ -59,36 +59,36 @@
     "Fluid connector a (positive design flow direction is from port_a to port_b)"
     annotation (Placement(transformation(extent={{-110,-10},{-90,10}})));
   Modelica.Fluid.Interfaces.FluidPort_b port_b(
     redeclare package Medium=Medium)
     "Fluid connector b (positive design flow direction is from port_a to port_b)"
     annotation (Placement(transformation(extent={{90,-10},{110,10}})));
   Modelica.Blocks.Interfaces.RealInput on[num](
-    min=0,
-    max=1,
-    unit="1")
+    each min=0,
+    each max=1,
+    each unit="1")
     "On signal for cooling towers"
     annotation (Placement(transformation(extent={{-140,40},{-100,80}})));
   Modelica.Blocks.Interfaces.RealInput speFan(
     unit="1")
     "Fan speed control signal"
     annotation (Placement(transformation(extent={{-140,0},{-100,40}})));
   Modelica.Blocks.Interfaces.RealInput TWetBul(
     final unit="K",
     displayUnit="degC")
     "Entering air wetbulb temperature"
     annotation (Placement(transformation(extent={{-140,-80},{-100,-40}})));
   Modelica.Blocks.Interfaces.RealOutput PFan[num](
-    final quantity="Power",
-    final unit="W")
+    each final quantity="Power",
+    each final unit="W")
     "Electric power consumed by fan"
     annotation (Placement(transformation(extent={{100,50},{120,70}})));
   Modelica.Blocks.Interfaces.RealOutput TLvg[num](
-    final unit="K",
-    displayUnit="degC")
+    each final unit="K",
+    each displayUnit="degC")
     "Leaving water temperature"
     annotation (Placement(transformation(extent={{100,20},{120,40}})));
   replaceable Buildings.Fluid.HeatExchangers.CoolingTowers.Merkel cooTow[num](
     each final ratWatAir_nominal=ratWatAir_nominal,
     each final TAirInWB_nominal=TAirInWB_nominal,
     each final TWatIn_nominal=TWatIn_nominal,
     each final TWatOut_nominal=TWatIn_nominal-dT_nominal,
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerWithBypass.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlantWithCHP.mot`

 * *Files 20% similar despite different names*

```diff
@@ -1,381 +1,358 @@
-within geojson_modelica_translator.model_connectors.templates;
-model CoolingTowerWithBypass
-  "Cooling tower system with bypass valve"
-  replaceable package Medium=Buildings.Media.Water
-    "Condenser water medium";
-  parameter Integer num(
-    min=1)=2
-    "Number of cooling towers";
+within {{ project_name }}.Plants;
+{% raw %}model CentralHeatingPlant
+  "Central heating plant."
+  package Medium=Buildings.Media.Water
+    "MediumW model";
+  parameter Integer numBoi=2
+    "Number of boilers, maximum is 2";
   parameter Boolean show_T=true
     "= true, if actual temperature at port is computed"
     annotation (Dialog(tab="Advanced",group="Diagnostics"));
-  parameter Modelica.Units.SI.MassFlowRate m_flow_nominal
-    "Total nominal mass flow rate of condenser water"
-    annotation (Dialog(group="Nominal condition"));
-  parameter Modelica.Units.SI.Pressure dp_nominal
-    "Nominal pressure difference of the tower"
-    annotation (Dialog(group="Nominal condition"));
-  parameter Real ratWatAir_nominal(
-    min=0,
-    unit="1")=0.625
-    "Design water-to-air ratio"
-    annotation (Dialog(group="Nominal condition"));
-  parameter Modelica.Units.SI.Temperature TAirInWB_nominal
-    "Nominal outdoor (air inlet) wetbulb temperature"
-    annotation (Dialog(group="Heat transfer"));
-  parameter Modelica.Units.SI.Temperature TWatIn_nominal
-    "Nominal water inlet temperature"
-    annotation (Dialog(group="Heat transfer"));
-  parameter Modelica.Units.SI.TemperatureDifference dT_nominal
-    "Temperature difference between inlet and outlet of the tower"
-    annotation (Dialog(group="Heat transfer"));
-  parameter Modelica.Units.SI.Power PFan_nominal
-    "Fan power"
-    annotation (Dialog(group="Fan"));
-  parameter Modelica.Units.SI.TemperatureDifference dTApp=3
-    "Approach temperature"
+  // boiler parameters
+  parameter Modelica.Units.SI.MassFlowRate mHW_flow_nominal
+    "Nominal heating water mass flow rate"
+    annotation (Dialog(group="Boiler"));
+  parameter Modelica.Units.SI.Power QBoi_flow_nominal
+    "Nominal heating capacity of single boiler"
+    annotation (Dialog(group="Boiler"));
+  parameter Modelica.Units.SI.MassFlowRate mMin_flow
+    "Minimum mass flow rate of single boiler"
+    annotation (Dialog(group="Boiler"));
+  parameter Modelica.Units.SI.MassFlowRate mBoi_flow_nominal
+    "Nominal mass flow rate of single boiler"
+    annotation (Dialog(group="Boiler"));
+  parameter Modelica.Units.SI.Pressure dpBoi_nominal
+    "Pressure difference at the boiler water side"
+    annotation (Dialog(group="Boiler"));
+  parameter Modelica.Units.SI.TemperatureDifference delT_nominal
+    "Design heating water temperature Difference";
+  // pump parameters
+  replaceable parameter Buildings.Fluid.Movers.Data.Generic perHWPum
+    constrainedby Buildings.Fluid.Movers.Data.Generic
+    "Performance data of heating water pump"
+    annotation (Dialog(group="Pump"),choicesAllMatching=true,Placement(transformation(extent={{138,82},{152,96}})));
+  // control settings
+  parameter Modelica.Units.SI.Time tWai
+    "Waiting time"
     annotation (Dialog(group="Control Settings"));
-  parameter Modelica.Units.SI.Temperature TMin
-    "Minimum allowed water temperature entering chiller"
+  parameter Modelica.Units.SI.PressureDifference dpSetPoi(
+    displayUnit="Pa")
+    "Demand side pressure difference setpoint"
     annotation (Dialog(group="Control Settings"));
-  parameter Modelica.Blocks.Types.SimpleController controllerType=Modelica.Blocks.Types.SimpleController.PI
-    "Type of fan speed controller"
-    annotation (Dialog(group="Control Settings"));
-  parameter Real k(
-    unit="1",
-    min=0)=1
-    "Gain of the tower PID controller"
-    annotation (Dialog(group="Control Settings"));
-  parameter Modelica.Units.SI.Time Ti(
-    min=Modelica.Constants.small)=60
-    "Integrator time constant of the tower PID controller"
-    annotation (Dialog(enable=(controllerType == Modelica.Blocks.Types.SimpleController.PI or controllerType == Modelica.Blocks.Types.SimpleController.PID),group="Control Settings"));
-  parameter Modelica.Units.SI.Time Td(
-    min=0)=0.1
-    "Derivative time constant of the tower PID controller"
-    annotation (Dialog(enable=(controllerType == Modelica.Blocks.Types.SimpleController.PD or controllerType == Modelica.Blocks.Types.SimpleController.PID),group="Control Settings"));
+  // diagnostics
   Medium.ThermodynamicState sta_a=Medium.setState_phX(
     port_a.p,
     noEvent(
       actualStream(
         port_a.h_outflow)),
     noEvent(
       actualStream(
         port_a.Xi_outflow))) if show_T
-    "Medium properties in port_a";
+    "MediumW properties in port_a";
   Medium.ThermodynamicState sta_b=Medium.setState_phX(
     port_b.p,
     noEvent(
       actualStream(
         port_b.h_outflow)),
     noEvent(
       actualStream(
         port_b.Xi_outflow))) if show_T
-    "Medium properties in port_b";
+    "MediumW properties in port_b";
   Modelica.Fluid.Interfaces.FluidPort_a port_a(
     redeclare package Medium=Medium)
     "Fluid connector a (positive design flow direction is from port_a to port_b)"
-    annotation (Placement(transformation(extent={{-110,-10},{-90,10}})));
+    annotation (Placement(transformation(extent={{150,40},{170,60}}),iconTransformation(extent={{90,40},{110,60}})));
   Modelica.Fluid.Interfaces.FluidPort_b port_b(
     redeclare package Medium=Medium)
     "Fluid connector b (positive design flow direction is from port_a to port_b)"
-    annotation (Placement(transformation(extent={{90,-10},{110,10}})));
-  Modelica.Blocks.Interfaces.RealInput on[num](
-    min=0,
-    max=1,
-    unit="1")
-    "On signal for cooling towers"
-    annotation (Placement(transformation(extent={{-140,20},{-100,60}})));
-  Modelica.Blocks.Interfaces.RealInput TWetBul(
-    final unit="K",
-    displayUnit="degC")
-    "Entering air wetbulb temperature"
-    annotation (Placement(transformation(extent={{-140,-40},{-100,0}})));
-  Modelica.Blocks.Interfaces.RealOutput PFan[num](
-    final quantity="Power",
-    final unit="W")
-    "Electric power consumed by fan"
-    annotation (Placement(transformation(extent={{100,50},{120,70}})));
-  Modelica.Blocks.Interfaces.RealOutput TLvg[num](
-    final unit="K",
-    displayUnit="degC")
-    "Leaving water temperature"
-    annotation (Placement(transformation(extent={{100,20},{120,40}})));
-  CoolingTowerParallel cooTowSys(
-    use_inputFilter=true,
+    annotation (Placement(transformation(extent={{150,-60},{170,-40}}),iconTransformation(extent={{90,-60},{110,-40}})));
+  Modelica.Blocks.Interfaces.BooleanInput on
+    "On signal of the plant"
+    annotation (Placement(transformation(extent={{-160,58},{-140,78}}),iconTransformation(extent={{-140,60},{-100,100}})));
+  Modelica.Blocks.Interfaces.RealInput dpMea(
+    final unit="Pa")
+    "Measured pressure difference"
+    annotation (Placement(transformation(extent={{-160,-40},{-140,-20}}),iconTransformation(extent={{-140,-50},{-100,-10}})));
+  Boiler_TParallel boiHotWat(
+    redeclare package Medium=Medium,
+    m_flow_nominal=mBoi_flow_nominal,
+    Q_flow_nominal=QBoi_flow_nominal,
+    dp_nominal=dpBoi_nominal,
+    numBoi=numBoi)
+    "Parallel boilers."
+    annotation (Placement(transformation(extent={{10,-60},{30,-40}})));
+  Buildings.Fluid.Sensors.TemperatureTwoPort THWSup(
+    redeclare package Medium=Medium,
+    m_flow_nominal=mHW_flow_nominal)
+    "Heating water supply temperature"
+    annotation (Placement(transformation(extent={{-10,-10},{10,10}},rotation=0,origin={132,-50})));
+  HeatingWaterPumpSpeed heaWatPumCon(
+    tWai=0,
+    m_flow_nominal=mBoi_flow_nominal,
+    dpSetPoi=dpSetPoi,
+    controllerType=Modelica.Blocks.Types.SimpleController.PI,
+    Ti=30,
+    k=0.1)
+    "Heating water pump controller."
+    annotation (Placement(transformation(extent={{-120,-40},{-100,-20}})));
+  BoilerStage boiStaCon(
+    tWai=tWai,
+    QBoi_nominal=QBoi_flow_nominal,
+    criPoiLoa=0.55*QBoi_flow_nominal,
+    dQ=0.25*QBoi_flow_nominal,
+    numBoi=numBoi)
+    "Boiler staging controller."
+    annotation (Placement(transformation(extent={{-120,58},{-100,78}})));
+  Modelica.Blocks.Sources.RealExpression mPum_flow(
+    y=pumHW.port_a.m_flow)
+    "Total heating water pump mass flow rate"
+    annotation (Placement(transformation(extent={{-100,30},{-120,50}})));
+  Buildings.Fluid.Sensors.TemperatureTwoPort THWRet(
+    redeclare package Medium=Medium,
+    m_flow_nominal=mHW_flow_nominal)
+    "Heating water return temperature"
+    annotation (Placement(transformation(extent={{10,-10},{-10,10}},rotation=0,origin={104,50})));
+  Buildings.Applications.BaseClasses.Equipment.FlowMachine_y pumHW(
+    per=fill(
+      perHWPum,
+      numBoi),
     redeclare package Medium=Medium,
-    num=num,
-    show_T=show_T,
-    m_flow_nominal=m_flow_nominal/num,
-    dp_nominal=dp_nominal,
-    ratWatAir_nominal=ratWatAir_nominal,
-    TAirInWB_nominal=TAirInWB_nominal,
-    TWatIn_nominal=TWatIn_nominal,
-    dT_nominal=dT_nominal,
-    PFan_nominal=PFan_nominal)
-    "Cooling tower system"
-    annotation (Placement(transformation(extent={{-10,-10},{10,10}})));
+    m_flow_nominal=mBoi_flow_nominal,
+    {% endraw %}dpValve_nominal={{ data["nominal_values"]["pressure_drop_hhw_valve_nominal"] }} {% raw %},
+    num=numBoi,
+    l=0.001)
+    "Parallel heating water pumps."
+    annotation (Placement(transformation(extent={{0,40},{-20,60}})));
   Buildings.Fluid.Actuators.Valves.TwoWayEqualPercentage valByp(
     redeclare package Medium=Medium,
-    m_flow_nominal=m_flow_nominal*0.0001,
-    dpValve_nominal=dp_nominal,
-    use_inputFilter=false)
-    "Condenser water bypass valve"
-    annotation (Placement(transformation(extent={{-10,-10},{10,10}},origin={0,-40})));
-  Buildings.Fluid.Sensors.TemperatureTwoPort senTCWSup(
+    allowFlowReversal=true,
+    m_flow_nominal=mHW_flow_nominal*0.05,
+    {% endraw %}dpValve_nominal={{ data["nominal_values"]["pressure_drop_hhw_valve_nominal"] }} {% raw %},
+    l=0.001)
+    "Heating water bypass valve"
+    annotation (Placement(transformation(extent={{-10,10},{10,-10}},rotation=90,origin={54,0})));
+  Buildings.Fluid.Sensors.MassFlowRate senMasFlo(
+    redeclare package Medium=Medium)
+    "Heating water return mass flow"
+    annotation (Placement(transformation(extent={{42,40},{22,60}})));
+  Buildings.Fluid.Sensors.MassFlowRate senMasFloByp(
+    redeclare package Medium=Medium)
+    "Heating water bypass valve mass flow meter"
+    annotation (Placement(transformation(extent={{10,10},{-10,-10}},rotation=-90,origin={54,-30})));
+  final parameter Medium.ThermodynamicState sta_default=Medium.setState_pTX(
+    T=Medium.T_default,
+    p=Medium.p_default,
+    X=Medium.X_default)
+    "Medium state at default properties";
+  final parameter Modelica.Units.SI.SpecificHeatCapacity cp_default=Medium.specificHeatCapacityCp(
+    sta_default)
+    "Specific heat capacity of the fluid";
+  Buildings.Fluid.Sources.Boundary_pT expTanHW(
+    redeclare package Medium=Medium,
+    nPorts=1)
+    "Heating water expansion tank"
+    annotation (Placement(transformation(extent={{-8,6},{12,26}})));
+  Modelica.Blocks.Interfaces.RealInput THeaSet(
+    each final unit="K",
+    each displayUnit="degC")
+    "Heating water setpoint."
+    annotation (Placement(transformation(extent={{-160,-60},{-140,-40}}),iconTransformation(extent={{-140,-104},{-100,-64}})));
+  Modelica.Blocks.Math.Product pumOn[numBoi]
+    "Output pump speed"
+    annotation (Placement(transformation(extent={{-80,0},{-60,20}})));
+  Buildings.Fluid.CHPs.ThermalElectricalFollowing eleFol(
     redeclare package Medium=Medium,
-    m_flow_nominal=m_flow_nominal,
-    T_start=Medium.T_default)
-    annotation (Placement(transformation(extent={{60,10},{80,-10}})));
-  Modelica.Blocks.Sources.RealExpression TSetCWSup(
-    y=max(
-      TWetBul+dTApp,
-      TMin))
-    "Condenser water supply temperature setpoint"
-    annotation (Placement(transformation(extent={{-60,50},{-40,70}})));
-  Modelica.Blocks.Sources.Constant TSetByPas(
-    k=TMin)
-    "Bypass loop temperature setpoint"
-    annotation (Placement(transformation(extent={{-90,-60},{-70,-40}})));
-  Buildings.Controls.Continuous.LimPID bypValCon(
-    u_s(
-      unit="K",
-      displayUnit="degC"),
-    u_m(
-      unit="K",
-      displayUnit="degC"),
-    controllerType=Modelica.Blocks.Types.SimpleController.PI,
-    k=1,
-    Ti=60,
-    final reverseActing=true,
-    reset=Buildings.Types.Reset.Parameter,
-    y_reset=0)
-    "Bypass valve controller"
-    annotation (Placement(transformation(extent={{-60,-60},{-40,-40}})));
-  Buildings.Controls.Continuous.LimPID cooTowSpeCon(
-    u_s(
-      unit="K",
-      displayUnit="degC"),
-    u_m(
-      unit="K",
-      displayUnit="degC"),
-    final reverseActing=false,
-    controllerType=controllerType,
-    k=k,
-    Ti=Ti)
-    "Cooling tower fan speed controller"
-    annotation (Placement(transformation(extent={{-12,50},{8,70}})));
-  Modelica.Blocks.Sources.RealExpression TLvgCooTow(
-    y=senTCWSup.T)
-    "Condenser water temperature leaving the towers"
-    annotation (Placement(transformation(extent={{-30,30},{-10,50}})));
-  Modelica.Blocks.Math.RealToBoolean reaToBoo
-    "Real to boolean signal"
-    annotation (Placement(transformation(extent={{-90,-90},{-70,-70}})));
+    m_flow_nominal=0.4,
+    redeclare Buildings.Fluid.CHPs.Data.Senertech5_5kW per,
+    TEngIni=273.15+69.55,
+    waitTime=0)
+    annotation (Placement(transformation(extent={{-80,28},{-60,48}})));
+  Modelica.Blocks.Sources.Constant ElePowDem(
+    k=5500)
+    annotation (Placement(transformation(extent={{-120,82},{-100,102}})));
+  Modelica.Blocks.Sources.Constant TWatOutSet(
+    k=273.15+60)
+    annotation (Placement(transformation(extent={{-120,52},{-100,72}})));
+  Buildings.Fluid.Movers.FlowControlled_m_flow fan(
+    redeclare package Medium=Medium,
+    m_flow_nominal=0.4,
+    nominalValuesDefineDefaultPressureCurve=true)
+    annotation (Placement(transformation(extent={{-172,-132},{-152,-110}})));
+  Buildings.HeatTransfer.Sources.FixedTemperature preTem(
+    T(
+      displayUnit="K")=273.15+25)
+    annotation (Placement(transformation(extent={{-160,-180},{-140,-160}})));
+protected
+  {% endraw %} Modelica.Blocks.Sources.BooleanExpression theFolSig(
+    final y={{ data["signals"]["thermal_following"] }})
+    {% raw %} "Signal for thermal following, set to false if electrical following"
+    annotation (Placement(transformation(extent={{-160,50},{-140,66}})));
 equation
-  connect(cooTowSys.TWetBul,TWetBul)
-    annotation (Line(points={{-12,-6},{-40,-6},{-40,-20},{-120,-20}},color={0,0,127}));
-  connect(on,cooTowSys.on)
-    annotation (Line(points={{-120,40},{-40,40},{-40,6},{-12,6}},color={0,0,127}));
-  connect(port_a,cooTowSys.port_a)
-    annotation (Line(points={{-100,0},{-10,0}},color={0,127,255}));
-  connect(cooTowSys.port_b,senTCWSup.port_a)
-    annotation (Line(points={{10,0},{60,0}},color={0,127,255}));
-  connect(senTCWSup.port_b,port_b)
-    annotation (Line(points={{80,0},{100,0}},color={0,127,255}));
-  connect(TSetByPas.y,bypValCon.u_s)
-    annotation (Line(points={{-69,-50},{-62,-50}},color={0,0,127}));
-  connect(senTCWSup.T,bypValCon.u_m)
-    annotation (Line(points={{70,-11},{70,-80},{-50,-80},{-50,-62}},color={0,0,127}));
-  connect(valByp.port_a,cooTowSys.port_a)
-    annotation (Line(points={{-10,-40},{-30,-40},{-30,0},{-10,0}},color={0,127,255}));
-  connect(valByp.port_b,senTCWSup.port_a)
-    annotation (Line(points={{10,-40},{30,-40},{30,0},{60,0}},color={0,127,255}));
-  connect(TSetCWSup.y,cooTowSpeCon.u_s)
-    annotation (Line(points={{-39,60},{-14,60}},color={0,0,127}));
-  connect(cooTowSpeCon.y,cooTowSys.speFan)
-    annotation (Line(points={{9,60},{20,60},{20,20},{-20,20},{-20,2},{-12,2}},color={0,0,127}));
-  connect(cooTowSys.PFan,PFan)
-    annotation (Line(points={{11,6},{40,6},{40,60},{110,60}},color={0,0,127}));
-  connect(cooTowSys.TLvg,TLvg)
-    annotation (Line(points={{11,3},{44,3},{44,30},{110,30}},color={0,0,127}));
-  connect(bypValCon.y,valByp.y)
-    annotation (Line(points={{-39,-50},{-20,-50},{-20,-20},{0,-20},{0,-28}},color={0,0,127}));
-  connect(TLvgCooTow.y,cooTowSpeCon.u_m)
-    annotation (Line(points={{-9,40},{-2,40},{-2,48}},color={0,0,127}));
-  connect(reaToBoo.y,bypValCon.trigger)
-    annotation (Line(points={{-69,-80},{-58,-80},{-58,-62}},color={255,0,255}));
-  connect(on[1],reaToBoo.u)
-    annotation (Line(points={{-120,30},{-96,30},{-96,-80},{-92,-80}},color={0,0,127}));
+  connect(theFolSig.y,eleFol.theFol)
+    annotation (Line(points={{-139,58},{-136,58},{-136,45},{-82,45}},color={255,0,255}));
+  connect(TWatOutSet.y,eleFol.TWatOutSet)
+    annotation (Line(points={{-99,62},{-92,62},{-92,43},{-82,43}},color={0,0,127}));
+  connect(ElePowDem.y,eleFol.PEleDem)
+    annotation (Line(points={{-99,92},{-92,92},{-92,41},{-82,41}},color={0,0,127}));
+  connect(eleFol.port_b,port_b)
+    annotation (Line(points={{-106,-136},{-102,-136},{-102,-50},{160,-50}},color={0,0,127}));
+  connect(THeaSet,boiHotWat.THeaWatSet)
+    annotation (Line(points={{-150,-50},{-72,-50},{-72,-56},{9,-56}},color={0,0,127}));
+  connect(on,boiStaCon.on)
+    annotation (Line(points={{-150,68},{-121,68}},color={255,0,255}));
+  connect(dpMea,heaWatPumCon.dpMea)
+    annotation (Line(points={{-150,-30},{-138,-30},{-138,-35},{-121,-35}},color={0,0,127}));
+  connect(valByp.port_a,senMasFloByp.port_b)
+    annotation (Line(points={{54,-10},{54,-20}},color={0,127,255}));
+  connect(senMasFloByp.m_flow,heaWatPumCon.meaFloByPas)
+    annotation (Line(points={{43,-30},{40,-30},{40,-74},{-130,-74},{-130,-38.8},{-121,-38.8}},color={0,0,127}));
+  connect(port_a,THWRet.port_a)
+    annotation (Line(points={{160,50},{114,50}},color={0,127,255}));
+  connect(pumHW.port_b,boiHotWat.port_a)
+    annotation (Line(points={{-20,50},{-36,50},{-36,-50},{10,-50}},color={0,127,255}));
+  connect(boiHotWat.port_b,THWSup.port_a)
+    annotation (Line(points={{30,-50},{122,-50}},color={0,127,255}));
+  connect(THWSup.port_b,port_b)
+    annotation (Line(points={{142,-50},{160,-50}},color={0,127,255}));
+  connect(pumHW.port_a,senMasFlo.port_b)
+    annotation (Line(points={{0,50},{22,50}},color={0,127,255}));
+  connect(senMasFlo.port_a,THWRet.port_b)
+    annotation (Line(points={{42,50},{94,50}},color={0,127,255}));
+  connect(heaWatPumCon.deCouVal,valByp.y)
+    annotation (Line(points={{-99,-35},{-94,-35},{-94,-70},{80,-70},{80,0},{74,0},{74,-6},{66,-6}},color={0,0,127}));
+  connect(valByp.port_b,senMasFlo.port_a)
+    annotation (Line(points={{54,10},{54,50},{42,50}},color={0,127,255}));
+  connect(boiHotWat.port_b,senMasFloByp.port_a)
+    annotation (Line(points={{30,-50},{54,-50},{54,-40}},color={0,127,255}));
+  connect(expTanHW.ports[1],senMasFlo.port_a)
+    annotation (Line(points={{12,16},{42,16},{42,50}},color={0,127,255}));
+  connect(boiStaCon.y_On,boiHotWat.on)
+    annotation (Line(points={{-99,70.6},{-72,70.6},{-72,-45},{9,-45}},color={255,0,255}));
+  connect(THWSup.T,boiStaCon.TDisSup)
+    annotation (Line(points={{132,-39},{132,96},{-134,96},{-134,70.6},{-121,70.6}},color={0,0,127}));
+  connect(THWRet.T,boiStaCon.TDisRet)
+    annotation (Line(points={{104,61},{104,88},{-130,88},{-130,73.4},{-121,73.4}},color={0,0,127}));
+  connect(senMasFlo.m_flow,boiStaCon.mHeaDis)
+    annotation (Line(points={{32,61},{32,86},{-126,86},{-126,76.6},{-121,76.6}},color={0,0,127}));
+  connect(boiStaCon.y,pumOn.u1)
+    annotation (Line(points={{-99,66},{-92,66},{-92,16},{-82,16}},color={0,0,127}));
+  connect(heaWatPumCon.y,pumOn.u2)
+    annotation (Line(points={{-99,-30},{-94,-30},{-94,4},{-82,4}},color={0,0,127}));
+  connect(pumOn.y,pumHW.u)
+    annotation (Line(points={{-59,10},{-46,10},{-46,72},{12,72},{12,54},{2,54}},color={0,0,127}));
+  connect(boiStaCon.y_On,heaWatPumCon.ON)
+    annotation (Line(points={{-99,70.6},{-88,70.6},{-88,24},{-128,24},{-128,-23.4},{-121,-23.4}},color={255,0,255}));
+  connect(mPum_flow.y,heaWatPumCon.masFloPum)
+    annotation (Line(points={{-121,40},{-134,40},{-134,-25.6},{-121,-25.6}},color={0,0,127}));
+  connect(theFolSig.y,eleFol.avaSig)
+    annotation (Line(points={{-139,58},{-128,58},{-128,-139},{-120,-139}},color={255,0,255}));
+  connect(port_a,fan.port_a)
+    annotation (Line(points={{160,50},{-190,50},{-190,-121},{-172,-121}},color={0,127,255}));
+  connect(fan.port_b,eleFol.port_a)
+    annotation (Line(points={{-152,-121},{-146,-121},{-146,-148},{-118,-148}},color={0,127,255}));
+  connect(eleFol.mWatSet_flow,fan.m_flow_in)
+    annotation (Line(points={{-96,-139},{-82,-139},{-82,-94},{-162,-94},{-162,-107.8}},color={0,0,127}));
+  connect(preTem.port,eleFol.TRoo)
+    annotation (Line(points={{-140,-170},{-134,-170},{-134,-155},{-118,-155}},color={191,0,0}));
   annotation (
     Diagram(
       coordinateSystem(
         preserveAspectRatio=false,
-        extent={{-100,-100},{100,100}})),
+        extent={{-140,-80},{120,100}})),
     Icon(
-      coordinateSystem(
-        preserveAspectRatio=false,
-        extent={{-100,-100},{100,100}}),
       graphics={
-        Polygon(
-          points={{0,-80},{-10,-72},{-10,-88},{0,-80}},
-          lineColor={0,0,0},
+        Rectangle(
+          extent={{-100,-100},{100,100}},
+          lineColor={0,0,127},
           fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
         Polygon(
-          points={{0,-80},{10,-72},{10,-88},{0,-80}},
-          lineColor={0,0,0},
+          points={{-62,-14},{-62,-14}},
+          lineColor={238,46,47},
           fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
-        Text(
-          extent={{-149,-114},{151,-154}},
-          lineColor={0,0,255},
-          textString="%name"),
-        Rectangle(
-          extent={{-30,94},{30,20}},
+        Polygon(
+          points={{80,-60},{-80,-60},{-80,60},{-60,60},{-60,0},{-40,0},{-40,20},{0,0},{0,20},{40,0},{40,20},{80,0},{80,-60}},
           lineColor={95,95,95},
-          fillColor={95,95,95},
+          fillColor={238,46,47},
           fillPattern=FillPattern.Solid),
-        Ellipse(
-          extent={{-22,88},{0,80}},
+        Rectangle(
+          extent={{46,-38},{58,-26}},
           lineColor={255,255,255},
           fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
-        Ellipse(
-          extent={{0,88},{22,80}},
+        Rectangle(
+          extent={{62,-38},{74,-26}},
           lineColor={255,255,255},
           fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
-        Line(
-          points={{16,70},{22,58}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{0,70},{6,58}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{0,70},{-6,58}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{16,70},{10,58}},
-          color={255,0,0},
-          thickness=0.5),
         Rectangle(
-          extent={{-30,8},{30,-66}},
-          lineColor={95,95,95},
-          fillColor={95,95,95},
-          fillPattern=FillPattern.Solid),
-        Ellipse(
-          extent={{-22,2},{0,-6}},
+          extent={{62,-54},{74,-42}},
           lineColor={255,255,255},
           fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
-        Ellipse(
-          extent={{0,2},{22,-6}},
+        Rectangle(
+          extent={{46,-54},{58,-42}},
           lineColor={255,255,255},
           fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
-        Line(
-          points={{-16,-16},{-22,-28}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{-16,-16},{-10,-28}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{0,-16},{-6,-28}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{0,-16},{6,-28}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{16,-16},{10,-28}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{16,-16},{22,-28}},
-          color={255,0,0},
-          thickness=0.5),
         Rectangle(
-          extent={{30,24},{60,20}},
-          lineColor={0,0,255},
-          pattern=LinePattern.None,
-          fillColor={0,0,127},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{30,-62},{60,-66}},
-          lineColor={0,0,255},
-          pattern=LinePattern.None,
-          fillColor={0,0,127},
+          extent={{22,-54},{34,-42}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{62,2},{92,-2}},
-          lineColor={0,0,255},
-          pattern=LinePattern.None,
-          fillColor={0,0,127},
+          extent={{6,-54},{18,-42}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{58,-80},{62,24}},
-          lineColor={0,0,255},
-          pattern=LinePattern.None,
-          fillColor={0,0,127},
+          extent={{6,-38},{18,-26}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-90,2},{-60,-2}},
-          lineColor={238,46,47},
-          pattern=LinePattern.None,
-          fillColor={238,46,47},
+          extent={{22,-38},{34,-26}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-64,-82},{-60,74}},
-          lineColor={238,46,47},
-          pattern=LinePattern.None,
-          fillColor={238,46,47},
+          extent={{-18,-54},{-6,-42}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-60,-12},{16,-16}},
-          lineColor={238,46,47},
-          pattern=LinePattern.None,
-          fillColor={238,46,47},
+          extent={{-34,-54},{-22,-42}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
         Rectangle(
-          extent={{-60,74},{16,70}},
-          lineColor={238,46,47},
-          pattern=LinePattern.None,
-          fillColor={238,46,47},
+          extent={{-34,-38},{-22,-26}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
-        Line(
-          points={{-16,70},{-22,58}},
-          color={255,0,0},
-          thickness=0.5),
-        Line(
-          points={{-16,70},{-10,58}},
-          color={255,0,0},
-          thickness=0.5),
         Rectangle(
-          extent={{-60,-78},{-10,-82}},
-          lineColor={238,46,47},
-          pattern=LinePattern.None,
-          fillColor={238,46,47},
+          extent={{-18,-38},{-6,-26}},
+          lineColor={255,255,255},
+          fillColor={255,255,255},
           fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{10,-78},{62,-82}},
+        Text(
+          extent={{-149,-114},{151,-154}},
           lineColor={0,0,255},
-          pattern=LinePattern.None,
-          fillColor={0,0,127},
-          fillPattern=FillPattern.Solid)}),
+          textString="%name")}),
     Documentation(
+      info="<html>
+   <p>
+   This model presents a heating water central plant for the distrcit systems application.
+   </p>
+   </html>",
       revisions="<html>
-<ul>
-<li>
-March 30, 2014 by Sen Huang:<br/>
-First implementation.
-</li>
-</ul>
-</html>"));
-end CoolingTowerWithBypass;
+   <ul>
+   <li>
+   June 30, 2020, by Hagar Elarga:<br/>
+   First implementation.
+   </li>
+   </ul>
+   </html>"));
+end CentralHeatingPlant;
+{% endraw %}
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlantWithCHP.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/BorefieldOneUTube.mot`

 * *Files 24% similar despite different names*

```diff
@@ -1,358 +1,361 @@
-within {{ project_name }}.Plants;
-{% raw %}model CentralHeatingPlant
-  "Central heating plant."
-  package Medium=Buildings.Media.Water
-    "MediumW model";
-  parameter Integer numBoi=2
-    "Number of boilers, maximum is 2";
-  parameter Boolean show_T=true
-    "= true, if actual temperature at port is computed"
-    annotation (Dialog(tab="Advanced",group="Diagnostics"));
-  // boiler parameters
-  parameter Modelica.Units.SI.MassFlowRate mHW_flow_nominal
-    "Nominal heating water mass flow rate"
-    annotation (Dialog(group="Boiler"));
-  parameter Modelica.Units.SI.Power QBoi_flow_nominal
-    "Nominal heating capacity of single boiler"
-    annotation (Dialog(group="Boiler"));
-  parameter Modelica.Units.SI.MassFlowRate mMin_flow
-    "Minimum mass flow rate of single boiler"
-    annotation (Dialog(group="Boiler"));
-  parameter Modelica.Units.SI.MassFlowRate mBoi_flow_nominal
-    "Nominal mass flow rate of single boiler"
-    annotation (Dialog(group="Boiler"));
-  parameter Modelica.Units.SI.Pressure dpBoi_nominal
-    "Pressure difference at the boiler water side"
-    annotation (Dialog(group="Boiler"));
-  parameter Modelica.Units.SI.TemperatureDifference delT_nominal
-    "Design heating water temperature Difference";
-  // pump parameters
-  replaceable parameter Buildings.Fluid.Movers.Data.Generic perHWPum
-    constrainedby Buildings.Fluid.Movers.Data.Generic
-    "Performance data of heating water pump"
-    annotation (Dialog(group="Pump"),choicesAllMatching=true,Placement(transformation(extent={{138,82},{152,96}})));
-  // control settings
-  parameter Modelica.Units.SI.Time tWai
-    "Waiting time"
-    annotation (Dialog(group="Control Settings"));
-  parameter Modelica.Units.SI.PressureDifference dpSetPoi(
-    displayUnit="Pa")
-    "Demand side pressure difference setpoint"
-    annotation (Dialog(group="Control Settings"));
-  // diagnostics
-  Medium.ThermodynamicState sta_a=Medium.setState_phX(
-    port_a.p,
-    noEvent(
-      actualStream(
-        port_a.h_outflow)),
-    noEvent(
-      actualStream(
-        port_a.Xi_outflow))) if show_T
-    "MediumW properties in port_a";
-  Medium.ThermodynamicState sta_b=Medium.setState_phX(
-    port_b.p,
-    noEvent(
-      actualStream(
-        port_b.h_outflow)),
-    noEvent(
-      actualStream(
-        port_b.Xi_outflow))) if show_T
-    "MediumW properties in port_b";
-  Modelica.Fluid.Interfaces.FluidPort_a port_a(
-    redeclare package Medium=Medium)
-    "Fluid connector a (positive design flow direction is from port_a to port_b)"
-    annotation (Placement(transformation(extent={{150,40},{170,60}}),iconTransformation(extent={{90,40},{110,60}})));
-  Modelica.Fluid.Interfaces.FluidPort_b port_b(
-    redeclare package Medium=Medium)
-    "Fluid connector b (positive design flow direction is from port_a to port_b)"
-    annotation (Placement(transformation(extent={{150,-60},{170,-40}}),iconTransformation(extent={{90,-60},{110,-40}})));
-  Modelica.Blocks.Interfaces.BooleanInput on
-    "On signal of the plant"
-    annotation (Placement(transformation(extent={{-160,58},{-140,78}}),iconTransformation(extent={{-140,60},{-100,100}})));
-  Modelica.Blocks.Interfaces.RealInput dpMea(
-    final unit="Pa")
-    "Measured pressure difference"
-    annotation (Placement(transformation(extent={{-160,-40},{-140,-20}}),iconTransformation(extent={{-140,-50},{-100,-10}})));
-  Boiler_TParallel boiHotWat(
+within {{ project_name }}.Plants.{{ model_name }};
+{% raw %}model Borefield
+  "Borefield model using single U-tube borehole heat exchanger configuration.Calculates the average fluid temperature T_fts of the borefield for a given (time dependent) load Q_flow"
+  extends Buildings.Fluid.Interfaces.PartialTwoPortInterface(
     redeclare package Medium=Medium,
-    m_flow_nominal=mBoi_flow_nominal,
-    Q_flow_nominal=QBoi_flow_nominal,
-    dp_nominal=dpBoi_nominal,
-    numBoi=numBoi)
-    "Parallel boilers."
-    annotation (Placement(transformation(extent={{10,-60},{30,-40}})));
-  Buildings.Fluid.Sensors.TemperatureTwoPort THWSup(
-    redeclare package Medium=Medium,
-    m_flow_nominal=mHW_flow_nominal)
-    "Heating water supply temperature"
-    annotation (Placement(transformation(extent={{-10,-10},{10,10}},rotation=0,origin={132,-50})));
-  HeatingWaterPumpSpeed heaWatPumCon(
-    tWai=0,
-    m_flow_nominal=mBoi_flow_nominal,
-    dpSetPoi=dpSetPoi,
-    controllerType=Modelica.Blocks.Types.SimpleController.PI,
-    Ti=30,
-    k=0.1)
-    "Heating water pump controller."
-    annotation (Placement(transformation(extent={{-120,-40},{-100,-20}})));
-  BoilerStage boiStaCon(
-    tWai=tWai,
-    QBoi_nominal=QBoi_flow_nominal,
-    criPoiLoa=0.55*QBoi_flow_nominal,
-    dQ=0.25*QBoi_flow_nominal,
-    numBoi=numBoi)
-    "Boiler staging controller."
-    annotation (Placement(transformation(extent={{-120,58},{-100,78}})));
-  Modelica.Blocks.Sources.RealExpression mPum_flow(
-    y=pumHW.port_a.m_flow)
-    "Total heating water pump mass flow rate"
-    annotation (Placement(transformation(extent={{-100,30},{-120,50}})));
-  Buildings.Fluid.Sensors.TemperatureTwoPort THWRet(
-    redeclare package Medium=Medium,
-    m_flow_nominal=mHW_flow_nominal)
-    "Heating water return temperature"
-    annotation (Placement(transformation(extent={{10,-10},{-10,10}},rotation=0,origin={104,50})));
-  Buildings.Applications.BaseClasses.Equipment.FlowMachine_y pumHW(
-    per=fill(
-      perHWPum,
-      numBoi),
-    redeclare package Medium=Medium,
-    m_flow_nominal=mBoi_flow_nominal,
-    {% endraw %}dpValve_nominal={{ data["nominal_values"]["pressure_drop_hhw_valve_nominal"] }} {% raw %},
-    num=numBoi,
-    l=0.001)
-    "Parallel heating water pumps."
-    annotation (Placement(transformation(extent={{0,40},{-20,60}})));
-  Buildings.Fluid.Actuators.Valves.TwoWayEqualPercentage valByp(
-    redeclare package Medium=Medium,
-    allowFlowReversal=false,
-    m_flow_nominal=mHW_flow_nominal*0.05,
-    {% endraw %}dpValve_nominal={{ data["nominal_values"]["pressure_drop_hhw_valve_nominal"] }} {% raw %},
-    l=0.001)
-    "Heating water bypass valve"
-    annotation (Placement(transformation(extent={{-10,10},{10,-10}},rotation=90,origin={54,0})));
-  Buildings.Fluid.Sensors.MassFlowRate senMasFlo(
-    redeclare package Medium=Medium)
-    "Heating water return mass flow"
-    annotation (Placement(transformation(extent={{42,40},{22,60}})));
-  Buildings.Fluid.Sensors.MassFlowRate senMasFloByp(
-    redeclare package Medium=Medium)
-    "Heating water bypass valve mass flow meter"
-    annotation (Placement(transformation(extent={{10,10},{-10,-10}},rotation=-90,origin={54,-30})));
-  final parameter Medium.ThermodynamicState sta_default=Medium.setState_pTX(
-    T=Medium.T_default,
-    p=Medium.p_default,
-    X=Medium.X_default)
-    "Medium state at default properties";
-  final parameter Modelica.Units.SI.SpecificHeatCapacity cp_default=Medium.specificHeatCapacityCp(
-    sta_default)
-    "Specific heat capacity of the fluid";
-  Buildings.Fluid.Sources.Boundary_pT expTanHW(
-    redeclare package Medium=Medium,
-    nPorts=1)
-    "Heating water expansion tank"
-    annotation (Placement(transformation(extent={{-8,6},{12,26}})));
-  Modelica.Blocks.Interfaces.RealInput THeaSet(
+    // need to be able to change the medium in the future
+    final m_flow_nominal=borFieDat.conDat.mBorFie_flow_nominal);
+  extends Buildings.Fluid.Interfaces.TwoPortFlowResistanceParameters(
+    final dp_nominal=borFieDat.conDat.dp_nominal,
+    final computeFlowResistance=(borFieDat.conDat.dp_nominal > Modelica.Constants.eps));
+  replaceable package Medium=Buildings.Media.Water
+    "Medium in the component"
+    annotation (choices(choice(redeclare package Medium=Buildings.Media.Water "Water"),choice(redeclare package Medium=Buildings.Media.Antifreeze.PropyleneGlycolWater(property_T=293.15,X_a=0.40) "Propylene glycol water, 40% mass fraction")));
+  constant Real mSenFac(
+    min=1)=1
+    "Factor for scaling the sensible thermal mass of the volume";
+  // Assumptions
+  parameter Modelica.Fluid.Types.Dynamics energyDynamics=Modelica.Fluid.Types.Dynamics.FixedInitial
+    "Type of energy balance: dynamic (3 initialization options) or steady state"
+    annotation (Evaluate=true,Dialog(tab="Dynamics",group="Conservation equations"));
+  // Initialization
+  parameter Medium.AbsolutePressure p_start=Medium.p_default
+    "Start value of pressure"
+    annotation (Dialog(tab="Initialization"));
+  // Simulation parameters
+  parameter Modelica.Units.SI.Time tLoaAgg=300
+    "Time resolution of load aggregation";
+  parameter Integer nCel(
+    min=1)=5
+    "Number of cells per aggregation level";
+  parameter Integer nSeg(
+    min=1)=10
+    "Number of segments to use in vertical discretization of the boreholes";
+  parameter Boolean forceGFunCalc=false
+    "Set to true to force the thermal response to be calculated at the start instead of checking whether this has been pre-computed"
+    annotation (Dialog(tab="Advanced"));
+  {% endraw %}parameter String gFunFilNam=Modelica.Utilities.Files.loadResource(
+    "{{ghe_data["gfunction"]["gfunction_file_path"]}}")
+    {% raw %} "File name of g-function data file in MAT format";
+  {% endraw %}parameter Integer nTimTot={{ghe_data["gfunction"]["gfunction_file_rows"]}}
+    {% raw %} "Total length of g-function vector";
+  // General parameters of borefield
+  parameter Buildings.Fluid.Geothermal.Borefields.Data.Borefield.Template borFieDat(
+    final filDat=Buildings.Fluid.Geothermal.Borefields.Data.Filling.Bentonite(
+      {% endraw %}kFil={{ghe_data["fill"]["conductivity"]}},
+      cFil={{ghe_data["fill"]["volumetric_heat_capacity"]}}/1450 {% raw %},
+      dFil=1450),
+    final soiDat=Buildings.Fluid.Geothermal.Borefields.Data.Soil.SandStone(
+      {% endraw %}kSoi={{ghe_data["soil"]["conductivity"]}},
+      cSoi={{ghe_data["soil"]["volumetric_heat_capacity"]}}/2600 {% raw %},
+      dSoi=2600),
+    final conDat=Buildings.Fluid.Geothermal.Borefields.Data.Configuration.Example(
+      dp_nominal=35000,
+      {% endraw %}borCon={{ghe_data["configuration"]["borehole_configuration"]}},
+      mBor_flow_nominal={{ghe_data["configuration"]["nominal_mass_flow_per_borehole"]}},
+      hBor={{ghe_data["configuration"]["borehole_height"]}},
+      rBor={{ghe_data["configuration"]["borehole_diameter"]}}/2,
+      dBor={{ghe_data["configuration"]["borehole_buried_depth"]}},
+      nBor={{ghe_data["configuration"]["number_of_boreholes"]}},
+      rTub={{ghe_data["tube"]["outer_diameter"]}}/2,
+      kTub={{ghe_data["tube"]["conductivity"]}},
+      eTub={{ghe_data["tube"]["thickness"]}},
+      xC={{ghe_data["tube"]["shank_spacing"]}} {% raw %}))
+    "Borefield data"
+    annotation (choicesAllMatching=true,Placement(transformation(extent={{-80,-80},{-60,-60}})));
+  // Temperature gradient in undisturbed soil
+  {% endraw %}parameter Modelica.Units.SI.Temperature TExt0_start={{ghe_data["soil"]["initial_ground_temperature"]}}+273.15
+    {% raw %} "Initial far field temperature"
+    annotation (Dialog(tab="Initialization",group="Soil"));
+  parameter Modelica.Units.SI.Temperature TExt_start[nSeg]={
+    if z[i] >= z0 then
+      TExt0_start+(z[i]-z0)*dT_dz
+    else
+      TExt0_start for i in 1:nSeg}
+    "Temperature of the undisturbed ground"
+    annotation (Dialog(tab="Initialization",group="Soil"));
+  parameter Modelica.Units.SI.Temperature TGro_start[nSeg]=TExt_start
+    "Start value of grout temperature"
+    annotation (Dialog(tab="Initialization",group="Filling material"));
+  parameter Modelica.Units.SI.Temperature TFlu_start[nSeg]=TGro_start
+    "Start value of fluid temperature"
+    annotation (Dialog(tab="Initialization"));
+  parameter Modelica.Units.SI.Height z0=10
+    "Depth below which the temperature gradient starts"
+    annotation (Dialog(tab="Initialization",group="Temperature profile"));
+  parameter Real dT_dz(
+    unit="K/m")=0.01
+    "Vertical temperature gradient of the undisturbed soil for h below z0"
+    annotation (Dialog(tab="Initialization",group="Temperature profile"));
+  // Dynamics of filling material
+  parameter Boolean dynFil=false
+    "Set to false to remove the dynamics of the filling material."
+    annotation (Dialog(tab="Dynamics"));
+  Modelica.Blocks.Interfaces.RealOutput TBorAve(
+    final quantity="ThermodynamicTemperature",
     final unit="K",
-    displayUnit="degC")
-    "Heating water setpoint."
-    annotation (Placement(transformation(extent={{-160,-60},{-140,-40}}),iconTransformation(extent={{-140,-104},{-100,-64}})));
-  Modelica.Blocks.Math.Product pumOn[numBoi]
-    "Output pump speed"
-    annotation (Placement(transformation(extent={{-80,0},{-60,20}})));
-  Buildings.Fluid.CHPs.ThermalElectricalFollowing eleFol(
-    redeclare package Medium=Medium,
-    m_flow_nominal=0.4,
-    redeclare Buildings.Fluid.CHPs.Data.Senertech5_5kW per,
-    TEngIni=273.15+69.55,
-    waitTime=0)
-    annotation (Placement(transformation(extent={{-80,28},{-60,48}})));
-  Modelica.Blocks.Sources.Constant ElePowDem(
-    k=5500)
-    annotation (Placement(transformation(extent={{-120,82},{-100,102}})));
-  Modelica.Blocks.Sources.Constant TWatOutSet(
-    k=273.15+60)
-    annotation (Placement(transformation(extent={{-120,52},{-100,72}})));
-  Buildings.Fluid.Movers.FlowControlled_m_flow fan(
-    redeclare package Medium=Medium,
-    m_flow_nominal=0.4,
-    nominalValuesDefineDefaultPressureCurve=true)
-    annotation (Placement(transformation(extent={{-172,-132},{-152,-110}})));
-  Buildings.HeatTransfer.Sources.FixedTemperature preTem(
-    T(
-      displayUnit="K")=273.15+25)
-    annotation (Placement(transformation(extent={{-160,-180},{-140,-160}})));
+    displayUnit="degC",
+    start=TExt0_start)
+    "Average borehole wall temperature in the borefield"
+    annotation (Placement(transformation(extent={{100,34},{120,54}})));
+  {% endraw %}{{ project_name }}.Plants.GroundTemperatureResponse groTemRes(
+    {% raw %}final tLoaAgg=tLoaAgg,
+    final nCel=nCel,
+    final borFieDat=borFieDat,
+    final forceGFunCalc=forceGFunCalc,
+    final gFunFilNam=gFunFilNam,
+    final nTimTot=nTimTot)
+    "Ground temperature response"
+    annotation (Placement(transformation(extent={{20,70},{40,90}})));
+  replaceable Buildings.Fluid.Geothermal.Borefields.BaseClasses.Boreholes.OneUTube borHol
+    constrainedby Buildings.Fluid.Geothermal.Borefields.BaseClasses.Boreholes.BaseClasses.PartialBorehole(
+      redeclare final package Medium=Medium,
+      final borFieDat=borFieDat,
+      final nSeg=nSeg,
+      final m_flow_nominal=m_flow_nominal/borFieDat.conDat.nBor,
+      final dp_nominal=dp_nominal,
+      final allowFlowReversal=allowFlowReversal,
+      final m_flow_small=m_flow_small,
+      final show_T=show_T,
+      final computeFlowResistance=computeFlowResistance,
+      final from_dp=from_dp,
+      final linearizeFlowResistance=linearizeFlowResistance,
+      final deltaM=deltaM,
+      final energyDynamics=energyDynamics,
+      final p_start=p_start,
+      final mSenFac=mSenFac,
+      final dynFil=dynFil,
+      final TFlu_start=TFlu_start,
+      final TGro_start=TGro_start)
+    "Borehole"
+    annotation (Placement(transformation(extent={{-10,-50},{10,-30}})));
 protected
-  {% endraw %} Modelica.Blocks.Sources.BooleanExpression theFolSig(
-    final y={{ data["signals"]["thermal_following"] }})
-    {% raw %} "Signal for thermal following, set to false if electrical following"
-    annotation (Placement(transformation(extent={{-160,50},{-140,66}})));
+  parameter Modelica.Units.SI.Height z[nSeg]={borFieDat.conDat.hBor/nSeg*(i-0.5) for i in 1:nSeg}
+    "Distance from the surface to the considered segment";
+  Buildings.Fluid.BaseClasses.MassFlowRateMultiplier masFloDiv(
+    redeclare final package Medium=Medium,
+    allowFlowReversal=allowFlowReversal,
+    final k=1/borFieDat.conDat.nBor)
+    "Division of flow rate"
+    annotation (Placement(transformation(extent={{-80,-50},{-60,-30}})));
+  Buildings.Fluid.BaseClasses.MassFlowRateMultiplier masFloMul(
+    redeclare final package Medium=Medium,
+    allowFlowReversal=allowFlowReversal,
+    final k=borFieDat.conDat.nBor)
+    "Mass flow multiplier"
+    annotation (Placement(transformation(extent={{60,-50},{80,-30}})));
+  Modelica.Blocks.Math.Gain gaiQ_flow(
+    k=borFieDat.conDat.nBor)
+    "Gain to multiply the heat extracted by one borehole by the number of boreholes"
+    annotation (Placement(transformation(extent={{-20,70},{0,90}})));
+  Buildings.Utilities.Math.Average AveTBor(
+    nin=nSeg)
+    "Average temperature of all the borehole segments"
+    annotation (Placement(transformation(extent={{50,34},{70,54}})));
+  Modelica.Blocks.Sources.Constant TSoiUnd[nSeg](
+    k=TExt_start,
+    each y(
+      unit="K",
+      displayUnit="degC"))
+    "Undisturbed soil temperature"
+    annotation (Placement(transformation(extent={{-40,14},{-20,34}})));
+  Modelica.Thermal.HeatTransfer.Sensors.HeatFlowSensor QBorHol[nSeg]
+    "Heat flow rate of all segments of the borehole"
+    annotation (Placement(transformation(extent={{-10,10},{10,-10}},rotation=90,origin={0,-10})));
+  Buildings.HeatTransfer.Sources.PrescribedTemperature TemBorWal[nSeg]
+    "Borewall temperature"
+    annotation (Placement(transformation(extent={{50,6},{70,26}})));
+  Modelica.Blocks.Math.Add TSoiDis[nSeg](
+    each final k1=1,
+    each final k2=1)
+    "Addition of undisturbed soil temperature and change of soil temperature"
+    annotation (Placement(transformation(extent={{10,20},{30,40}})));
+  Modelica.Blocks.Math.Sum QTotSeg_flow(
+    final nin=nSeg,
+    final k=ones(
+      nSeg))
+    "Total heat flow rate for all segments of this borehole"
+    annotation (Placement(transformation(extent={{-60,70},{-40,90}})));
+  Modelica.Blocks.Routing.Replicator repDelTBor(
+    final nout=nSeg)
+    "Signal replicator for temperature difference of the borehole"
+    annotation (Placement(transformation(extent={{60,70},{80,90}})));
 equation
-  connect(theFolSig.y,eleFol.theFol)
-    annotation (Line(points={{-139,58},{-136,58},{-136,45},{-82,45}},color={255,0,255}));
-  connect(TWatOutSet.y,eleFol.TWatOutSet)
-    annotation (Line(points={{-99,62},{-92,62},{-92,43},{-82,43}},color={0,0,127}));
-  connect(ElePowDem.y,eleFol.PEleDem)
-    annotation (Line(points={{-99,92},{-92,92},{-92,41},{-82,41}},color={0,0,127}));
-  connect(eleFol.port_b,port_b)
-    annotation (Line(points={{-106,-136},{-102,-136},{-102,-50},{160,-50}},color={0,0,127}));
-  connect(THeaSet,boiHotWat.THeaWatSet)
-    annotation (Line(points={{-150,-50},{-72,-50},{-72,-56},{9,-56}},color={0,0,127}));
-  connect(on,boiStaCon.on)
-    annotation (Line(points={{-150,68},{-121,68}},color={255,0,255}));
-  connect(dpMea,heaWatPumCon.dpMea)
-    annotation (Line(points={{-150,-30},{-138,-30},{-138,-35},{-121,-35}},color={0,0,127}));
-  connect(valByp.port_a,senMasFloByp.port_b)
-    annotation (Line(points={{54,-10},{54,-20}},color={0,127,255}));
-  connect(senMasFloByp.m_flow,heaWatPumCon.meaFloByPas)
-    annotation (Line(points={{43,-30},{40,-30},{40,-74},{-130,-74},{-130,-38.8},{-121,-38.8}},color={0,0,127}));
-  connect(port_a,THWRet.port_a)
-    annotation (Line(points={{160,50},{114,50}},color={0,127,255}));
-  connect(pumHW.port_b,boiHotWat.port_a)
-    annotation (Line(points={{-20,50},{-36,50},{-36,-50},{10,-50}},color={0,127,255}));
-  connect(boiHotWat.port_b,THWSup.port_a)
-    annotation (Line(points={{30,-50},{122,-50}},color={0,127,255}));
-  connect(THWSup.port_b,port_b)
-    annotation (Line(points={{142,-50},{160,-50}},color={0,127,255}));
-  connect(pumHW.port_a,senMasFlo.port_b)
-    annotation (Line(points={{0,50},{22,50}},color={0,127,255}));
-  connect(senMasFlo.port_a,THWRet.port_b)
-    annotation (Line(points={{42,50},{94,50}},color={0,127,255}));
-  connect(heaWatPumCon.deCouVal,valByp.y)
-    annotation (Line(points={{-99,-35},{-94,-35},{-94,-70},{80,-70},{80,0},{74,0},{74,-6},{66,-6}},color={0,0,127}));
-  connect(valByp.port_b,senMasFlo.port_a)
-    annotation (Line(points={{54,10},{54,50},{42,50}},color={0,127,255}));
-  connect(boiHotWat.port_b,senMasFloByp.port_a)
-    annotation (Line(points={{30,-50},{54,-50},{54,-40}},color={0,127,255}));
-  connect(expTanHW.ports[1],senMasFlo.port_a)
-    annotation (Line(points={{12,16},{42,16},{42,50}},color={0,127,255}));
-  connect(boiStaCon.y_On,boiHotWat.on)
-    annotation (Line(points={{-99,70.6},{-72,70.6},{-72,-45},{9,-45}},color={255,0,255}));
-  connect(THWSup.T,boiStaCon.TDisSup)
-    annotation (Line(points={{132,-39},{132,96},{-134,96},{-134,70.6},{-121,70.6}},color={0,0,127}));
-  connect(THWRet.T,boiStaCon.TDisRet)
-    annotation (Line(points={{104,61},{104,88},{-130,88},{-130,73.4},{-121,73.4}},color={0,0,127}));
-  connect(senMasFlo.m_flow,boiStaCon.mHeaDis)
-    annotation (Line(points={{32,61},{32,86},{-126,86},{-126,76.6},{-121,76.6}},color={0,0,127}));
-  connect(boiStaCon.y,pumOn.u1)
-    annotation (Line(points={{-99,66},{-92,66},{-92,16},{-82,16}},color={0,0,127}));
-  connect(heaWatPumCon.y,pumOn.u2)
-    annotation (Line(points={{-99,-30},{-94,-30},{-94,4},{-82,4}},color={0,0,127}));
-  connect(pumOn.y,pumHW.u)
-    annotation (Line(points={{-59,10},{-46,10},{-46,72},{12,72},{12,54},{2,54}},color={0,0,127}));
-  connect(boiStaCon.y_On,heaWatPumCon.ON)
-    annotation (Line(points={{-99,70.6},{-88,70.6},{-88,24},{-128,24},{-128,-23.4},{-121,-23.4}},color={255,0,255}));
-  connect(mPum_flow.y,heaWatPumCon.masFloPum)
-    annotation (Line(points={{-121,40},{-134,40},{-134,-25.6},{-121,-25.6}},color={0,0,127}));
-  connect(theFolSig.y,eleFol.avaSig)
-    annotation (Line(points={{-139,58},{-128,58},{-128,-139},{-120,-139}},color={255,0,255}));
-  connect(port_a,fan.port_a)
-    annotation (Line(points={{160,50},{-190,50},{-190,-121},{-172,-121}},color={0,127,255}));
-  connect(fan.port_b,eleFol.port_a)
-    annotation (Line(points={{-152,-121},{-146,-121},{-146,-148},{-118,-148}},color={0,127,255}));
-  connect(eleFol.mWatSet_flow,fan.m_flow_in)
-    annotation (Line(points={{-96,-139},{-82,-139},{-82,-94},{-162,-94},{-162,-107.8}},color={0,0,127}));
-  connect(preTem.port,eleFol.TRoo)
-    annotation (Line(points={{-140,-170},{-134,-170},{-134,-155},{-118,-155}},color={191,0,0}));
+  connect(masFloMul.port_b,port_b)
+    annotation (Line(points={{80,-40},{90,-40},{90,0},{100,0}},color={0,127,255}));
+  connect(masFloDiv.port_a,port_a)
+    annotation (Line(points={{-80,-40},{-90,-40},{-90,0},{-100,0}},color={0,127,255}));
+  connect(masFloDiv.port_b,borHol.port_a)
+    annotation (Line(points={{-60,-40},{-10,-40}},color={0,127,255}));
+  connect(borHol.port_b,masFloMul.port_a)
+    annotation (Line(points={{10,-40},{60,-40}},color={0,127,255}));
+  connect(QBorHol.port_a,borHol.port_wall)
+    annotation (Line(points={{-4.44089e-16,-20},{0,-20},{0,-30}},color={191,0,0}));
+  connect(QBorHol.Q_flow,QTotSeg_flow.u)
+    annotation (Line(points={{-11,-10},{-86,-10},{-86,80},{-62,80}},color={0,0,127}));
+  connect(groTemRes.delTBor,repDelTBor.u)
+    annotation (Line(points={{41,80},{58,80}},color={0,0,127}));
+  connect(TSoiDis.u1,repDelTBor.y)
+    annotation (Line(points={{8,36},{0,36},{0,60},{90,60},{90,80},{81,80}},color={0,0,127}));
+  connect(TSoiDis.u2,TSoiUnd.y)
+    annotation (Line(points={{8,24},{-19,24}},color={0,0,127}));
+  connect(QTotSeg_flow.y,gaiQ_flow.u)
+    annotation (Line(points={{-39,80},{-22,80}},color={0,0,127}));
+  connect(gaiQ_flow.y,groTemRes.QBor_flow)
+    annotation (Line(points={{1,80},{19,80}},color={0,0,127}));
+  connect(TSoiDis.y,TemBorWal.T)
+    annotation (Line(points={{31,30},{36,30},{36,16},{48,16}},color={0,0,127}));
+  connect(QBorHol.port_b,TemBorWal.port)
+    annotation (Line(points={{4.44089e-16,0},{0,0},{0,4},{80,4},{80,16},{70,16}},color={191,0,0}));
+  connect(TSoiDis.y,AveTBor.u)
+    annotation (Line(points={{31,30},{36,30},{36,44},{48,44}},color={0,0,127}));
+  connect(AveTBor.y,TBorAve)
+    annotation (Line(points={{71,44},{110,44}},color={0,0,127}));
   annotation (
-    Diagram(
+    Icon(
       coordinateSystem(
         preserveAspectRatio=false,
-        extent={{-140,-80},{120,100}})),
-    Icon(
+        extent={{-100,-100},{100,100}}),
       graphics={
         Rectangle(
-          extent={{-100,-100},{100,100}},
-          lineColor={0,0,127},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Polygon(
-          points={{-62,-14},{-62,-14}},
-          lineColor={238,46,47},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Polygon(
-          points={{80,-60},{-80,-60},{-80,60},{-60,60},{-60,0},{-40,0},{-40,20},{0,0},{0,20},{40,0},{40,20},{80,0},{80,-60}},
-          lineColor={95,95,95},
-          fillColor={238,46,47},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{46,-38},{58,-26}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{62,-38},{74,-26}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{62,-54},{74,-42}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{46,-54},{58,-42}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{22,-54},{34,-42}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{6,-54},{18,-42}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{6,-38},{18,-26}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{22,-38},{34,-26}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{-18,-54},{-6,-42}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{-34,-54},{-22,-42}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{-34,-38},{-22,-26}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Rectangle(
-          extent={{-18,-38},{-6,-26}},
-          lineColor={255,255,255},
-          fillColor={255,255,255},
-          fillPattern=FillPattern.Solid),
-        Text(
-          extent={{-149,-114},{151,-154}},
-          lineColor={0,0,255},
-          textString="%name")}),
+          extent={{-100,60},{100,-66}},
+          lineColor={0,0,0},
+          fillColor={234,210,210},
+          fillPattern=FillPattern.Solid),
+        Ellipse(
+          extent={{-88,-6},{-32,-62}},
+          lineColor={0,0,0},
+          fillColor={223,188,190},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{-82,-12},{-38,-56}},
+          lineColor={0,0,0},
+          fillColor={0,0,255},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{-88,54},{-32,-2}},
+          lineColor={0,0,0},
+          fillColor={223,188,190},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{-82,48},{-38,4}},
+          lineColor={0,0,0},
+          fillColor={0,0,255},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{-26,54},{30,-2}},
+          lineColor={0,0,0},
+          fillColor={223,188,190},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{-20,48},{24,4}},
+          lineColor={0,0,0},
+          fillColor={0,0,255},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{-28,-6},{28,-62}},
+          lineColor={0,0,0},
+          fillColor={223,188,190},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{-22,-12},{22,-56}},
+          lineColor={0,0,0},
+          fillColor={0,0,255},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{36,56},{92,0}},
+          lineColor={0,0,0},
+          fillColor={223,188,190},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{42,50},{86,6}},
+          lineColor={0,0,0},
+          fillColor={0,0,255},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{38,-4},{94,-60}},
+          lineColor={0,0,0},
+          fillColor={223,188,190},
+          fillPattern=FillPattern.Forward),
+        Ellipse(
+          extent={{44,-10},{88,-54}},
+          lineColor={0,0,0},
+          fillColor={0,0,255},
+          fillPattern=FillPattern.Forward)}),
+    Diagram(
+      coordinateSystem(
+        preserveAspectRatio=false,
+        extent={{-100,-100},{100,100}})),
     Documentation(
       info="<html>
-   <p>
-   This model presents a heating water central plant for the distrcit systems application.
-   </p>
-   </html>",
+<p>
+This model simulates a borefield containing one or multiple boreholes
+using the parameters in the <code>borFieDat</code> record.
+</p>
+<p>
+Heat transfer to the soil is modeled using only one borehole heat exchanger
+(To be added in an extended model). The
+fluid mass flow rate into the borehole is divided to reflect the per-borehole
+fluid mass flow rate. The borehole model calculates the dynamics within the
+borehole itself using an axial discretization and a resistance-capacitance
+network for the internal thermal resistances between the individual pipes and
+between each pipe and the borehole wall.
+</p>
+<p>
+The thermal interaction between the borehole wall and the surrounding soil
+is modeled using
+<a href=\"modelica://Buildings.Fluid.Geothermal.Borefields.BaseClasses.HeatTransfer.GroundTemperatureResponse\">
+Buildings.Fluid.Geothermal.Borefields.BaseClasses.HeatTransfer.GroundTemperatureResponse</a>,
+which uses a cell-shifting load aggregation technique to calculate the borehole wall
+temperature after calculating and/or read (from a previous calculation) the borefield's thermal response factor.
+</p>
+</html>",
       revisions="<html>
-   <ul>
-   <li>
-   June 30, 2020, by Hagar Elarga:<br/>
-   First implementation.
-   </li>
-   </ul>
-   </html>"));
-end CentralHeatingPlant;
+<ul>
+<li>
+April 9, 2021, by Michael Wetter:<br/>
+Corrected placement of <code>each</code> keyword.<br/>
+See <a href=\"https://github.com/lbl-srg/modelica-buildings/pull/2440\">Buildings, PR #2440</a>.
+</li>
+<li>
+August 25, 2020, by Filip Jorissen:<br/>
+Switched port connections for <code>masFloDiv</code>.
+See <a href=\"https://github.com/ibpsa/modelica-ibpsa/issues/41\">#41</a>.
+</li>
+<li>
+March 24, 2020, by Damien Picard:<br/>
+Propagated flowReversal into <code>masFloDiv</code> and <code>masFloMul</code>.
+</li>
+<li>
+June 7, 2019, by Massimo Cimmino:<br/>
+Converted instances that are not of interest to user to be <code>protected</code>.
+</li>
+<li>
+June 4, 2019, by Massimo Cimmino:<br/>
+Added an output for the average borehole wall temperature.
+See
+<a href=\"https://github.com/ibpsa/modelica-ibpsa/issues/1107\">#1107</a>.
+</li>
+<li>
+April 11, 2019, by Filip Jorissen:<br/>
+Added <code>choicesAllMatching</code> for <code>borFieDat</code>.
+See <a href=\"https://github.com/ibpsa/modelica-ibpsa/issues/1117\">#1117</a>.
+</li>
+<li>
+January 18, 2019, by Jianjun Hu:<br/>
+Limited the media choice to water and glycolWater.
+See <a href=\"https://github.com/ibpsa/modelica-ibpsa/issues/1050\">#1050</a>.
+</li>
+<li>
+July 2018, by Alex Laferri&egrave;re:<br/>
+Changed into a partial model and changed documentation to reflect the new approach
+used by the borefield models.
+</li>
+<li>
+July 2014, by Damien Picard:<br/>
+First implementation.
+</li>
+</ul>
+</html>"));
+end Borefield;
 {% endraw %}
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlant_Instance.mopt` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlant_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/HeatingWaterPumpSpeed.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingWaterPumpSpeed.mo`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     "Total mass flowrate of heating water pumps"
     annotation (Placement(transformation(extent={{-120,34},{-100,54}}),iconTransformation(extent={{-120,34},{-100,54}})));
   Buildings.Controls.OBC.CDL.Interfaces.RealInput dpMea(
     final unit="Pa")
     "Measured pressure difference"
     annotation (Placement(transformation(extent={{-120,-60},{-100,-40}}),iconTransformation(extent={{-120,-60},{-100,-40}})));
   Buildings.Controls.OBC.CDL.Interfaces.RealOutput y[numPum](
-    unit="1",
-    min=0,
-    max=1)
+    each unit="1",
+    each min=0,
+    each max=1)
     "Pump speed signal"
     annotation (Placement(transformation(extent={{100,-10},{120,10}})));
   Modelica.Blocks.Math.Product pumSpe[numPum]
     "Output pump speed"
     annotation (Placement(transformation(extent={{34,-10},{54,10}})));
   Buildings.Applications.BaseClasses.Controls.VariableSpeedPumpStage pumStaCon(
     tWai=tWai,
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallelInterface.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallelInterface.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/model_connectors/plants/templates/ValveParameters.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/model_connectors/plants/templates/ValveParameters.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mo` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mo`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-within GMT_Lib.DHC.Components.CentralPlant.Cooling;
 model CoolingPlant
   "This example is to validate template Central Cooling Plant component model."
     extends Buildings.Experimental.DHC.CentralPlants.Cooling.Examples.Plant(
     redeclare Buildings.Fluid.Chillers.Data.ElectricEIR.ElectricEIRChiller_York_YT_1055kW_5_96COP_Vanes perChi(
       mEva_flow_nominal=mCHW_flow_nominal,
       mCon_flow_nominal=mCW_flow_nominal,
       QEva_flow_nominal=QChi_nominal),
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-within GMT_Lib.DHC.Components.CentralPlant.Cooling; model CoolingPlant "This
-example is to validate template Central Cooling Plant component model." extends
+model CoolingPlant "This example is to validate template Central Cooling Plant
+component model." extends
 Buildings.Experimental.DHC.CentralPlants.Cooling.Examples.Plant( redeclare
 Buildings.Fluid.Chillers.Data.ElectricEIR.ElectricEIRChiller_York_YT_1055kW_5_96COP_Vanes
 perChi( mEva_flow_nominal=mCHW_flow_nominal,
 mCon_flow_nominal=mCW_flow_nominal, QEva_flow_nominal=QChi_nominal), redeclare
 Buildings.Experimental.DHC.CentralPlants.Cooling.Plant pla, dTApp=3,
 mCHW_flow_nominal=18.3, dpCHW_nominal=44.8*1000, mMin_flow=0.03,
 mCW_flow_nominal=34.7, dpCW_nominal=46.2*1000, PFan_nominal=4999,
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mos` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mos`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mot`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-within GMT_Lib.DHC.Components.Plants.Cooling.CoolingPlant;
 model CoolingPlant
   "Isolated central cooling plant template model."
   extends Buildings.Experimental.DHC.Plants.Cooling.Examples.ElectricChillerParallel(
   redeclare {$ chiller_performance $} perChi(
     mEva_flow_nominal=mCHW_flow_nominal,
     mCon_flow_nominal=mCW_flow_nominal,
     QEva_flow_nominal=QChi_nominal),
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-within GMT_Lib.DHC.Components.Plants.Cooling.CoolingPlant; model CoolingPlant
-"Isolated central cooling plant template model." extends
+model CoolingPlant "Isolated central cooling plant template model." extends
 Buildings.Experimental.DHC.Plants.Cooling.Examples.ElectricChillerParallel
 ( redeclare {$ chiller_performance $} perChi
 ( mEva_flow_nominal=mCHW_flow_nominal, mCon_flow_nominal=mCW_flow_nominal,
 QEva_flow_nominal=QChi_nominal), redeclare {$ plant_type $} pla, dTApp={$
 delta_temp_approach $}, mCHW_flow_nominal={$ chw_mass_flow_nominal $},
 dpCHW_nominal={$ chw_pressure_drop_nominal $}, mMin_flow={$
 chiller_water_flow_minimum $}, mCW_flow_nominal={$ cw_mass_flow_nominal $},
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/ACLine.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/ACLine.mot`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-within {{ project_name }}.ACLine;
 model AC{{ data["model_name"] }}
   "Isolated AC distribution line template model for GMT level 1 testing"
   parameter Modelica.Units.SI.Length l={{ data["length"] }};
   parameter Modelica.Units.SI.Power P_nominal={{ data["ampacity"] }};
   parameter Modelica.Units.SI.Voltage V_nominal={{ data["nominal_voltage"] }};
-  redeclare {{ data["commercial_line_type"] }} commercialCable;{% raw %}
+  parameter {{ data["commercial_line_type"] }} cable;{% raw %}
   extends
     Buildings.Electrical.AC.ThreePhasesBalanced.Lines.Examples.ACLineMedium(
   line_1(
       mode=Buildings.Electrical.Types.CableMode.commercial,
   l=l,
-  commercialCable=commercialCable,
+  commercialCable=cable,
   P_nominal=P_nominal,
   V_nominal=V_nominal),
   line_2a(
       mode=Buildings.Electrical.Types.CableMode.commercial,
   l=l,
-  commercialCable=commercialCable,
+  commercialCable=cable,
   P_nominal=P_nominal,
   V_nominal=V_nominal),
   line_2b(
       mode=Buildings.Electrical.Types.CableMode.commercial,
   l=l,
-  commercialCable=commercialCable,
+  commercialCable=cable,
   P_nominal=P_nominal,
   V_nominal=V_nominal),
   line_3a(
       mode=Buildings.Electrical.Types.CableMode.commercial,
   l=l,
-  commercialCable=commercialCable,
+  commercialCable=cable,
   P_nominal=P_nominal,
   V_nominal=V_nominal),
   line_3b(
       mode=Buildings.Electrical.Types.CableMode.commercial,
   l=l,
-  commercialCable=commercialCable,
+  commercialCable=cable,
   P_nominal=P_nominal,
   V_nominal=V_nominal),
   line_sc(
       mode=Buildings.Electrical.Types.CableMode.commercial,
   l=l,
-  commercialCable=commercialCable,
+  commercialCable=cable,
   P_nominal=P_nominal,
   V_nominal=V_nominal)
   );
 annotation (
     Icon(
       coordinateSystem(
         preserveAspectRatio=false)),
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
-within {{ project_name }}.ACLine; model AC{{ data["model_name"] }} "Isolated AC
-distribution line template model for GMT level 1 testing" parameter
-Modelica.Units.SI.Length l={{ data["length"] }}; parameter
-Modelica.Units.SI.Power P_nominal={{ data["ampacity"] }}; parameter
-Modelica.Units.SI.Voltage V_nominal={{ data["nominal_voltage"] }}; redeclare {
-{ data["commercial_line_type"] }} commercialCable;{% raw %} extends
+model AC{{ data["model_name"] }} "Isolated AC distribution line template model
+for GMT level 1 testing" parameter Modelica.Units.SI.Length l={{ data["length"]
+}}; parameter Modelica.Units.SI.Power P_nominal={{ data["ampacity"] }};
+parameter Modelica.Units.SI.Voltage V_nominal={{ data["nominal_voltage"] }};
+parameter {{ data["commercial_line_type"] }} cable;{% raw %} extends
 Buildings.Electrical.AC.ThreePhasesBalanced.Lines.Examples.ACLineMedium( line_1
 ( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
-commercialCable=commercialCable, P_nominal=P_nominal, V_nominal=V_nominal),
-line_2a( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
-commercialCable=commercialCable, P_nominal=P_nominal, V_nominal=V_nominal),
-line_2b( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
-commercialCable=commercialCable, P_nominal=P_nominal, V_nominal=V_nominal),
-line_3a( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
-commercialCable=commercialCable, P_nominal=P_nominal, V_nominal=V_nominal),
-line_3b( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
-commercialCable=commercialCable, P_nominal=P_nominal, V_nominal=V_nominal),
-line_sc( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
-commercialCable=commercialCable, P_nominal=P_nominal, V_nominal=V_nominal) );
-annotation ( Icon( coordinateSystem( preserveAspectRatio=false)), Diagram
+commercialCable=cable, P_nominal=P_nominal, V_nominal=V_nominal), line_2a
+( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
+commercialCable=cable, P_nominal=P_nominal, V_nominal=V_nominal), line_2b
+( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
+commercialCable=cable, P_nominal=P_nominal, V_nominal=V_nominal), line_3a
+( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
+commercialCable=cable, P_nominal=P_nominal, V_nominal=V_nominal), line_3b
+( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
+commercialCable=cable, P_nominal=P_nominal, V_nominal=V_nominal), line_sc
+( mode=Buildings.Electrical.Types.CableMode.commercial, l=l,
+commercialCable=cable, P_nominal=P_nominal, V_nominal=V_nominal) ); annotation
+( Icon( coordinateSystem( preserveAspectRatio=false)), Diagram
 ( coordinateSystem( preserveAspectRatio=false)), experiment( StopTime=86400,
 Tolerance=1e-06), Documentation( info="
 This model validates the AC distribution line template model implemented in
 Buildings.Electrical.AC.ThreePhasesBalanced.Lines.Examples.ACLine.mot.
 ", revisions="
     * March 8, 2022 by Mingzhe Liu:
       First implementation.
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/Lines.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/Lines.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/PVPanels.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/PVPanels.mot`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-within {{ project_name }}.PVPanels;
 model {{ data['model_name'] }}
   "Isolated PV panels template model for GMT level 1 testing"
   parameter Modelica.Units.SI.Area A = {{ data["net_surface_area_m2"] }};
   parameter Modelica.Units.SI.Voltage V_nominal = {{ data["nominal_voltage_V"] }};
   parameter Modelica.Units.SI.Angle til = {{ data["surface_tilt_deg"] }};
   parameter Modelica.Units.SI.Angle azi = {{ data["surface_azimuth_deg"] }};{% raw %}
   extends Buildings.Electrical.AC.ThreePhasesBalanced.Sources.Examples.PVPanels(
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-within {{ project_name }}.PVPanels; model {{ data['model_name'] }} "Isolated PV
-panels template model for GMT level 1 testing" parameter Modelica.Units.SI.Area
-A = {{ data["net_surface_area_m2"] }}; parameter Modelica.Units.SI.Voltage
-V_nominal = {{ data["nominal_voltage_V"] }}; parameter Modelica.Units.SI.Angle
-til = {{ data["surface_tilt_deg"] }}; parameter Modelica.Units.SI.Angle azi = {
-{ data["surface_azimuth_deg"] }};{% raw %} extends
+model {{ data['model_name'] }} "Isolated PV panels template model for GMT level
+1 testing" parameter Modelica.Units.SI.Area A = {{ data["net_surface_area_m2"]
+}}; parameter Modelica.Units.SI.Voltage V_nominal = {{ data
+["nominal_voltage_V"] }}; parameter Modelica.Units.SI.Angle til = {{ data
+["surface_tilt_deg"] }}; parameter Modelica.Units.SI.Angle azi = {{ data
+["surface_azimuth_deg"] }};{% raw %} extends
 Buildings.Electrical.AC.ThreePhasesBalanced.Sources.Examples.PVPanels
 ( pvOriented( A=A, V_nominal=V_nominal, til=til, azi=azi)); annotation ( Icon
 ( coordinateSystem( preserveAspectRatio=false)), Diagram( coordinateSystem
 ( preserveAspectRatio=false)), experiment( StopTime=86400, Tolerance=1e-06),
 Documentation( info="
 This model validates the pv panels template model implemented in
 Buildings.Electrical.AC.ThreePhasesBalanced.Sources.Examples.PVPanels.mot.
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/WindTurbine.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/WindTurbine.mot`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-within {{ project_name }}.WindTurbine;
 model {{ data["model_name"] }}
   "Isolated wind turbine template model for GMT level 1 testing"
   parameter Real scale={{ data["scaling_factor"] }} "Scale factor";
   parameter Modelica.Units.SI.Length h={{ data["height_over_ground"] }} "Height over ground";
   parameter Modelica.Units.SI.Voltage V_nominal={{ data["nominal_voltage"] }} "Nominal voltage";
   parameter Real table[:,2]={{ data["power_curve"] }} "Table of generated power (first column is wind speed, second column is power)";
   {% raw %}
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-within {{ project_name }}.WindTurbine; model {{ data["model_name"] }} "Isolated
-wind turbine template model for GMT level 1 testing" parameter Real scale={
-{ data["scaling_factor"] }} "Scale factor"; parameter Modelica.Units.SI.Length
-h={{ data["height_over_ground"] }} "Height over ground"; parameter
-Modelica.Units.SI.Voltage V_nominal={{ data["nominal_voltage"] }} "Nominal
-voltage"; parameter Real table[:,2]={{ data["power_curve"] }} "Table of
-generated power (first column is wind speed, second column is power)"; {% raw
-%} extends
+model {{ data["model_name"] }} "Isolated wind turbine template model for GMT
+level 1 testing" parameter Real scale={{ data["scaling_factor"] }} "Scale
+factor"; parameter Modelica.Units.SI.Length h={{ data["height_over_ground"] }}
+"Height over ground"; parameter Modelica.Units.SI.Voltage V_nominal={{ data
+["nominal_voltage"] }} "Nominal voltage"; parameter Real table[:,2]={{ data
+["power_curve"] }} "Table of generated power (first column is wind speed,
+second column is power)"; {% raw %} extends
 Buildings.Electrical.AC.ThreePhasesBalanced.Sources.Examples.WindTurbine( tur
 ( scale=scale, h=h, table=table, V_nominal=V_nominal)); annotation ( Icon
 ( coordinateSystem( preserveAspectRatio=false)), Diagram( coordinateSystem
 ( preserveAspectRatio=false)), experiment( StopTime=86400, Tolerance=1e-06),
 Documentation( info="
 This model validates the wind turbine template model implemented in
 Buildings.Electrical.AC.ThreePhasesBalanced.Sources.Examples.WindTurbine.mot.
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/community_pv.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/community_pv.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/wind_turbines.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/wind_turbines.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/RenewableSources.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/RenewableSources.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/csv_modelica.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/csv_modelica.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/input_parser.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/input_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import os
+from pathlib import Path
+from typing import Union
 
 from jinja2 import Environment, FileSystemLoader
 
 from geojson_modelica_translator.jinja_filters import ALL_CUSTOM_FILTERS
 
 
 class PackageParser(object):
@@ -32,23 +34,26 @@
                     os.path.dirname(os.path.abspath(__file__)), "templates"
                 )
             )
         )
         self.template_env.filters.update(ALL_CUSTOM_FILTERS)
 
     @classmethod
-    def new_from_template(cls, path, name, order, within=None):
-        """
-        Create new package data based on the package.mo template. If within is not specified, then it is
+    def new_from_template(cls, path: Union[str, Path], name: str, order: list[str], within: str = None) -> "PackageParser":
+        """Create new package data based on the package.mo template. If within is not specified, then it is
         assumed that this is a top level package and will load from the package_base template.
 
-        :param path: string, the path where the resulting files will be saved to.
-        :param name: string, the name of the model
-        :param order: list, ordered list of which models will be loaded (saved to package.order)
-        :param within: string, (optional), name where this package is within.
+        Args:
+            path (str): the path where the resulting package file and order will be saved to.
+            name (str): the name of the model
+            order (list[str]): ordered list of which models will be loaded (saved to package.order)
+            within (str, optional): name where this package is within.. Defaults to None.
+
+        Returns:
+            PackageParser: object of the package parser
         """
         klass = PackageParser(path)
         if within:
             template = klass.template_env.get_template("package.mot")
         else:
             template = klass.template_env.get_template("package_base.mot")
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/model_connectors/templates/RunSpawnBuilding.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/model_connectors/templates/RunSpawnBuilding.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/model_connectors/templates/spawn_fmu.mot` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/model_connectors/templates/spawn_fmu.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/modelica/modelica_runner.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/modelica/modelica_runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,264 +1,314 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import logging
 import os
 import shutil
 import subprocess
-from ast import Str
 from glob import glob
 from pathlib import Path
 from typing import Union
 
+from jinja2 import Environment, FileSystemLoader, StrictUndefined
+
+from geojson_modelica_translator.jinja_filters import ALL_CUSTOM_FILTERS
+
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     level=logging.INFO,
     format='%(asctime)s - %(levelname)s: %(message)s',
     datefmt='%d-%b-%y %H:%M:%S',
 )
 
 
 class ModelicaRunner(object):
     """
-    Class to run Modelica models. This is a very simple implementation of what needs to be
-    a full CLI to run Modelica easily. At the moment, this probably only works on Linux/Mac
-    and perhaps in Windows with Docker.
-    For Ubuntu, here is the installation instruction: https://docs.docker.com/engine/install/ubuntu/
-
-    # TODO: test in windows
-    # Document how to install Docker
+    Class to run Modelica models.
     """
+    ACTION_LOG_MAP = {
+        'compile': 'Compiling mo file',  # creates an FMU
+        'compile_and_run': 'Compile and run the mo file',
+        'run': 'Running FMU',
+    }
 
     def __init__(self, modelica_lib_path=None):
         """
         Initialize the runner with data needed for simulation
 
         :param modelica_lib_path: string, Path to the MBL to run against
         """
         # check if the user has defined a MODELICAPATH, is so, then use that.
         if os.environ.get('MODELICAPATH', None):
             print('Using predefined MODELICAPATH')
             self.modelica_lib_path = os.environ['MODELICAPATH']
             logger.debug(f'MODELICAPATH: {self.modelica_lib_path}')
         else:
             self.modelica_lib_path = modelica_lib_path
-        local_path = os.path.dirname(os.path.abspath(__file__))
-        self.spawn_docker_path = os.path.join(local_path, 'lib', 'runner', 'spawn_docker.sh')
+        local_path = Path(__file__).parent.resolve()
+        self.om_docker_path = local_path / 'lib' / 'runner' / 'om_docker.sh'
 
         # Verify that docker is up and running
         r = subprocess.call(['docker', 'ps'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         self.docker_configured = r == 0
 
-    def _verify_docker_run_capability(self, file_to_run):
+    def _verify_docker_run_capability(self, file_to_load: Union[str, Path, None]):
+        """Verify that docker is configured on the host computer correctly before running
+
+        Args:
+            file_to_load (Union[str, Path]): Can be a file path or a modelica path
+
+        Raises:
+            SystemExit: _description_
+            SystemExit: _description_
+        """
         if not self.docker_configured:
             raise SystemExit('Docker not configured on host computer, unable to run')
 
-        if not os.path.exists(file_to_run):
-            raise SystemExit(f'File not found to run {file_to_run}')
+        # If there is a file to load (meaning that we aren't loading from the library),
+        # then check that it exists
+        if file_to_load and not os.path.exists(file_to_load):
+            raise SystemExit(f'File not found to run {file_to_load}')
 
-        if not os.path.isfile(file_to_run):
-            raise SystemExit(f'Expecting to run a file, not a folder in {file_to_run}')
-
-    def _verify_run_path_for_docker(self, run_path: Str, file_to_run: Str) -> Path:
-        """if there is no run_path, then run it in the same directory as the
+    def _verify_run_path_for_docker(self, run_path: Union[str, Path, None], file_to_run: Union[str, Path, None]) -> Path:
+        """If there is no run_path, then run it in the same directory as the
         file being run. This works fine for simple Modelica projects but typically
         the run_path needs to be a few levels higher in order to include other
         project dependencies (e.g., multiple mo files).
+
+        Args:
+            run_path (str): directory of where to run the simulation
+            file_to_run (str): the name of the file to run. This should be the fully
+                               qualified path to the file.
+
+        Raises:
+            SystemExit: Throw an exception if the run_path or file_to_run has spaces in it
+
+        Returns:
+            Path: Return the run_path as a Path object
         """
         if not run_path:
-            run_path = os.path.dirname(file_to_run)
-        run_path = Path(run_path)
+            run_path = os.path.dirname(file_to_run)  # type: ignore
+        new_run_path = Path(run_path)
 
         # Modelica can't handle spaces in project name or path
-        if (len(str(run_path).split()) > 1) or (len(str(file_to_run).split()) > 1):
+        if (len(str(new_run_path).split()) > 1) or (len(str(file_to_run).split()) > 1):
             raise SystemExit(
                 f"\nModelica does not support spaces in project names or paths. "
-                f"You used '{run_path}' for run path and {file_to_run} for model project name. "
+                f"You used '{new_run_path}' for run path and {file_to_run} for model project name. "
                 "Please update your directory path or model name to not include spaces anywhere.")
-        return run_path
+        return new_run_path
 
-    def _copy_over_docker_resources(self, run_path: Path) -> None:
-        """Copy over ipython and jmodelica needed to run the simulation
-        """
-        new_spawn_docker = os.path.join(run_path, os.path.basename(self.spawn_docker_path))
-        shutil.copyfile(self.spawn_docker_path, new_spawn_docker)
-        os.chmod(new_spawn_docker, 0o775)
+    def _copy_over_docker_resources(self, run_path: Path, filename: Union[str, Path, None], model_name: str, **kwargs) -> None:
+        """Copy over files needed to run the simulation, this includes
+        the generation of the OpenModelica scripts to load and compile/run
+        the simulation.
+
+        If passing the start, stop, and step times, then at least start and stop must be supplied to
+        update the simuation to use these values instead of the defaults.
+
+        Args:
+            run_path (Path): Path where the model will be run, this is where the files will be copied.
+            filename (str): name of the file that will be loaded (e.g., BouncingBall.mo, package.mo)
+            model_name (str): name of the model to run (e.g., BouncingBall, Districts.DistrictModel)
+        """
+        # read in the start, stop, and step times
+        project_in_library = kwargs.get('project_in_library', False)
+        start_time = kwargs.get('start_time', None)
+        stop_time = kwargs.get('stop_time', None)
+        step_size = kwargs.get('step_size', None)
+
+        # initialize the templating framework (Jinja2)
+        template_env = Environment(
+            loader=FileSystemLoader(searchpath=Path(__file__).parent.resolve() / 'lib' / 'runner'),
+            undefined=StrictUndefined
+        )
+        template_env.filters.update(ALL_CUSTOM_FILTERS)
+        template = template_env.get_template('simulate.most')
+        model_data = {
+            "project_in_library": project_in_library,
+            "file_to_load": Path(filename).name if filename else None,
+            "model_name": model_name,
+            "use_default_time_params": False if start_time is not None and stop_time is not None else True,
+            "start_time": start_time,
+            "stop_time": stop_time,
+            "step_size": step_size,
+        }
+        with open(run_path / 'simulate.mos', 'w') as f:
+            f.write(template.render(**model_data))
+        template = template_env.get_template('compile_fmu.most')
+        with open(run_path / 'compile_fmu.mos', 'w') as f:
+            f.write(template.render(**model_data))
+
+        # new om_docker.sh file name
+        new_om_docker = run_path / self.om_docker_path.name
+        shutil.copyfile(self.om_docker_path, new_om_docker)
+        os.chmod(new_om_docker, 0o775)
 
-    def _subprocess_call_to_docker(self, run_path: Path, file_to_run: Str, action: Str, compiler: Str = 'optimica') -> int:
+    def _subprocess_call_to_docker(self, run_path: Union[str, Path], action: str) -> int:
         """Call out to a subprocess to run the command in docker
 
-        :param file_to_run: string, name of the file or directory to simulate
-        :param run_path: string, location where the Modelica simulatio or compilation will start
-        :param action: string, action to run either compile_and_run, compile, or run
-        :param compiler: string, compiler to use
-        :returns: int, exit code of the subprocess
-        """
-        action_log_map = {
-            'compile_and_run': 'Compiling mo file and running FMU',
-            'compile': 'Compiling mo file',
-            'run': 'Running FMU',
-        }
-        # Verify that the action is in the list of valid actions
-        assert action in action_log_map.keys(), \
-            f'Invalid action of {action} in _subprocess_call_to_docker, needs to be {[k for k in action_log_map.keys()]}'
-
-        valid_compilers = ['optimica']  # , 'jmodelica', 'openmodelica'
-        assert compiler in valid_compilers, \
-            f'Invalid compiler of {compiler} in _subprocess_call_to_docker, needs to be {valid_compilers}'
+        Args:
+            run_path (Path): local path where the Modelica simulation or compilation will start
+            action (str):  action to run either compile_and_run, compile, or run
 
+        Returns:
+            int: exit code of the subprocess
+        """
         # Set up the run content
         curdir = os.getcwd()
         os.chdir(run_path)
         stdout_log = open('stdout.log', 'w')
         try:
             # get the relative difference between the file to run and the path which everything is running in.
             # make sure to simulate at a directory above the project directory!
 
             # Use slashes for the location of the model to run. We can make these periods `.replace(os.sep, '.')`
             # but must strip off the .mo extension on the model to run
-            run_model = Path(file_to_run).relative_to(run_path)
-            logger.info(f"{action_log_map[action]}: {run_model} in {run_path}")
-            exec_call = ['./spawn_docker.sh', action, run_model, run_path, compiler]
+            # run_model = Path(file_to_run).relative_to(run_path)
+            exec_call = ['./om_docker.sh', action]
             logger.debug(f"Calling {exec_call}")
             p = subprocess.Popen(
-                exec_call,
+                exec_call,  # type: ignore
                 stdout=stdout_log,
                 stderr=subprocess.STDOUT,
                 cwd=run_path
             )
+            # Uncomment this section and rebuild the container in order to pause the container
+            # to inpsect the container and test commands.
+            # import time
+            # time.sleep(10000)  # wait for the subprocess to start
             logger.debug(f"Subprocess command executed, waiting for completion... \nArgs used: {p.args}")
             exitcode = p.wait()
         finally:
             os.chdir(curdir)
             stdout_log.close()
             logger.debug('Closed stdout.log')
 
         return exitcode
 
-    def run_in_docker(self, file_to_run: Str, run_path: Str = None, project_name: Str = None) -> Union[bool, str]:
-        """
-        Run the Modelica project in a docker-based environment. Results are saved into the path of the
-        file that was selected to run.
+    def run_in_docker(self, action: str, model_name: str, file_to_load: Union[str, Path, None] = None,
+                      run_path: Union[str, Path, None] = None, **kwargs) -> tuple[bool, Union[str, Path]]:
+        """Run the Modelica project in a docker-based environment. The action will determine
+        what type of run will be conducted. This method supports either a file path pointing to the package to load, or a modelica path which is a period separated path. Results are saved into run_path.
 
         stdout.log will store both stdout and stderr of the simulations
 
-        :param file_to_run: string, name of the file (could be directory?) to simulate
-        :param run_path: string, location where the Modelica simulation will start
-        :param project_name: string, name of the project being simulated. Will be used to determine name of results directory
-        :returns: tuple(bool, str), success status and path to the results directory
-        """
-        self._verify_docker_run_capability(file_to_run)
-        run_path = self._verify_run_path_for_docker(run_path, file_to_run)
-
-        if not project_name:
-            project_name = os.path.splitext(os.path.basename(file_to_run))[0]
-
-        self._copy_over_docker_resources(run_path)
+        Args:
+            action (str): The action to run, must be one of compile_and_run, compile, or run
+            model_name (str): The name of the model to be simulated (this is the name within Modelica)
+            file_to_load (str, Path): The file path or a modelica path to be simulated
+            run_path (str, optional): location where the Modelica simulation will start. Defaults to None.
+            kwargs: additional arugments to pass to the runner which can include
+                project_in_library (bool): whether the project is in a library or not
+                start_time (float): start time of the simulation
+                stop_time (float): stop time of the simulation
+                step_size (float): step size of the simulation
 
-        exitcode = self._subprocess_call_to_docker(run_path, file_to_run, 'compile_and_run')
-
-        logger.debug('removing temporary files')
-        # Cleanup all of the temporary files that get created
-        self._cleanup_path(run_path)
-
-        logger.debug('moving results to results directory')
-        # get the location of the results path
-        results_path = Path(run_path / f'{project_name}_results')
-        self.move_results(run_path, results_path, project_name)
-        return (exitcode == 0, results_path)
-
-    def compile_in_docker(self, file_to_run: Str, save_path: Str = None) -> bool:
-        """Build/compile the Modelica project in a docker-based environment using JModelica. The resulting
-        FMU is saved to the save_path.
-
-        stdout.log will store both stdout and stderr of the simulations
-
-        :param file_to_run: string, name of the file (could be directory?) to simulate
-        :param run_psave_pathath: string, location where the Modelica FMU will be saved
-        :returns: bool, success status
+        Returns:
+            tuple[bool, str]: success status and path to the results directory
         """
-        self._verify_docker_run_capability(file_to_run)
-        save_path = self._verify_run_path_for_docker(save_path, file_to_run)
-
-        self._copy_over_docker_resources(save_path)
-
-        exitcode = self._subprocess_call_to_docker(save_path, file_to_run, 'compile')
-
-        # Cleanup all of the temporary files that get created
-        logger.debug('removing temporary files')
-        self._cleanup_path(save_path)
-
-        logger.debug('moving results to results directory')
-        return exitcode == 0
-
-    def run_fmu_in_docker(self, file_to_run: Str, run_path: Str = None):
-        """Run the FMU in a docker-based environment. Results are saved into the path of the
-        file that was selected to run.
-
-        stdout.log will store both stdout and stderr of the simulations
-
-        :param file_to_run: string, name of the file (could be directory?) to simulate
-        :param run_path: string, location where the Modelica simulation will start
-        :param project_name: string, name of the project being simulated. Will be used to determine name of results
-                                     directory
-        :return: tuple(bool, str), success status and path to the results directory
-        """
-        self._verify_docker_run_capability(file_to_run)
-        run_path = self._verify_run_path_for_docker(run_path, file_to_run)
-        project_name = os.path.splitext(os.path.basename(file_to_run))[0]
+        # Verify that the action is in the list of valid actions
+        if action not in ModelicaRunner.ACTION_LOG_MAP:
+            raise SystemExit(f'Invalid action {action}, must be one of {list(ModelicaRunner.ACTION_LOG_MAP.keys())}')
 
-        self._copy_over_docker_resources(run_path)
+        self._verify_docker_run_capability(file_to_load)
+        verified_run_path = self._verify_run_path_for_docker(run_path, file_to_load)
 
-        exitcode = self._subprocess_call_to_docker(run_path, file_to_run, 'run')
+        self._copy_over_docker_resources(
+            verified_run_path, file_to_load, model_name, **kwargs
+        )
+
+        exitcode = self._subprocess_call_to_docker(verified_run_path, action)
+
+        logger.debug('checking stdout.log for errors')
+        # Check the stdout.log file for errors
+        with open(verified_run_path / 'stdout.log', 'r') as f:
+            stdout_log = f.read()
+            if 'Failed to build model' in stdout_log:
+                logger.error('Model failed to build')
+                exitcode = 1
+            elif 'The simulation finished successfully' in stdout_log:
+                logger.info('Model ran successfully')
+                exitcode = 0
+            elif action == 'compile':
+                logger.info('Model compiled successfully -- no errors')
+                exitcode = 0
+            else:
+                logger.error('Model failed to run -- unknown error')
+                exitcode = 1
 
         logger.debug('removing temporary files')
         # Cleanup all of the temporary files that get created
-        self._cleanup_path(run_path)
+        self._cleanup_path(verified_run_path, model_name)
 
         logger.debug('moving results to results directory')
         # get the location of the results path
-        results_path = Path(run_path / f'{project_name}_results')
-        self.move_results(run_path, results_path, project_name)
+        results_path = Path(verified_run_path / f'{model_name}_results')
+        self.move_results(verified_run_path, results_path, model_name)
         return (exitcode == 0, results_path)
 
-    def move_results(self, from_path: Path, to_path: Path, project_name: Str = None) -> None:
+    def move_results(self, from_path: Path, to_path: Path, model_name: Union[str, None] = None) -> None:
         """This method moves the results of the simulation that are known for now.
         This method moves only specific files (stdout.log for now), plus all files and folders beginning
         with the "{project_name}_" name.
 
         :param from_path: pathlib.Path, where the files will move from
         :param to_path: pathlib.Path, where the files will be saved. Will be created if does not exist.
-        :param project_name: string, name of the project ran in run_in_docker method
+        :param model_name: string, name of the project ran in run_in_docker method
         :return: None
         """
         # if there are results, they will simply be overwritten (for now).
         to_path.mkdir(parents=True, exist_ok=True)
 
         files_to_move = [
             'stdout.log',
         ]
+        if model_name is not None:
+            files_to_move.append(f'{model_name}.log',)
+            files_to_move.append(f'{model_name}.fmu',)
+            files_to_move.append(f"{model_name.replace('.', '_')}.log",)
+            files_to_move.append(f"{model_name.replace('.', '_')}_FMU.log",)
 
         for to_move in from_path.iterdir():
             if not to_move == to_path:
-                if (to_move.name in files_to_move) or to_move.name.startswith(f'{project_name}_'):
+                if (to_move.name in files_to_move) or to_move.name.startswith(f'{model_name}_'):
                     # typecast back to strings for the shutil method.
                     shutil.move(str(to_move), str(to_path / to_move.name))
 
-    def _cleanup_path(self, path: Path) -> None:
+    def _cleanup_path(self, path: Path, model_name: str) -> None:
         """Clean up the files in the path that was presumably used to run the simulation
         """
         remove_files = [
-            'spawn_docker.sh',
+            'om_docker.sh',
+            'compile_fmu.mos',
+            'simulate.mos',
+            f'{model_name}',
+            f'{model_name}.makefile',
+            f"{model_name.replace('.', '_')}_info.json",
+            f"{model_name.replace('.', '_')}_FMU.makefile",
+            f"{model_name.replace('.', '_')}_FMU.libs",
         ]
 
         for f in remove_files:
             if os.path.exists(os.path.join(path, f)):
                 os.remove(os.path.join(path, f))
 
+        # glob for the .c, .h, .o, .bin files to remove
+        remove_files_glob = [
+            f'{model_name}*.c',
+            f'{model_name}*.h',
+            f'{model_name}*.o',
+            f'{model_name}*.bin',
+        ]
+        for pattern in remove_files_glob:
+            for f in glob(os.path.join(path, pattern)):
+                os.remove(f)
+
+        # The below was a result from jmodelica and can *most likely* be removed
         for g in glob(os.path.join(path, 'tmp-simulation-*')):
             logger.debug(f"Removing tmp-simulation files {g}")
             # This is a complete hack but the name of the other folder that gets created is the
             # globbed directory without the tmp-simulation
             eplus_path = os.path.join(path, os.path.basename(g).replace('tmp-simulation-', ''))
             if os.path.exists(eplus_path):
                 shutil.rmtree(eplus_path)
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/scaffold.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/scaffold.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,29 +38,49 @@
         self.districts_path = None
         self.scripts_path = None
         self.networks_path = None
         self.overwrite = overwrite
 
         # clear out the project path
         self.project_path = os.path.join(self.root_dir, self.project_name)
+        self.package_path = os.path.join(self.project_path, "package.mo")
         if os.path.exists(self.project_path):
             if not self.overwrite:
                 raise Exception("Directory already exists and overwrite is false for %s" % self.project_path)
             else:
                 shutil.rmtree(self.project_path)
 
-    def create(self):
-        """run the scaffolding"""
+    def create(self, ignore_paths=[]):
+        """run the scaffolding to create the directory structure for DES systems
+
+        Args:
+            ignore_paths (list, optional): List of paths NOT to create. Choose from Loads, Substations, Plants, Districts, Networks. Defaults to [].
+        """
+        # initialize all of path objects
+        self.loads_path = None
+        self.substations_path = None
+        self.plants_path = None
+        self.districts_path = None
+        self.networks_path = None
 
         # leverage the ModelicaPath function
-        self.loads_path = ModelicaPath("Loads", root_dir=self.project_path, overwrite=self.overwrite)
-        self.substations_path = ModelicaPath("Substations", root_dir=self.project_path, overwrite=self.overwrite)
-        self.plants_path = ModelicaPath("Plants", root_dir=self.project_path, overwrite=self.overwrite)
-        self.districts_path = ModelicaPath("Districts", root_dir=self.project_path, overwrite=self.overwrite)
-        self.networks_path = ModelicaPath("Networks", root_dir=self.project_path, overwrite=self.overwrite)
+        if 'Loads' not in ignore_paths:
+            self.loads_path = ModelicaPath("Loads", root_dir=self.project_path, overwrite=self.overwrite)
+
+        if 'Substations' not in ignore_paths:
+            self.substations_path = ModelicaPath("Substations", root_dir=self.project_path, overwrite=self.overwrite)
+
+        if 'Plants' not in ignore_paths:
+            self.plants_path = ModelicaPath("Plants", root_dir=self.project_path, overwrite=self.overwrite)
+
+        if 'Districts' not in ignore_paths:
+            self.districts_path = ModelicaPath("Districts", root_dir=self.project_path, overwrite=self.overwrite)
+
+        if 'Networks' not in ignore_paths:
+            self.networks_path = ModelicaPath("Networks", root_dir=self.project_path, overwrite=self.overwrite)
 
     def clear_or_create_path(self, path, overwrite=False):
         if os.path.exists(path):
             if not overwrite:
                 raise Exception("Directory already exists and overwrite is false for %s" % path)
             else:
                 shutil.rmtree(path)
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/system_parameters/schema.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/system_parameters/schema.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9589984528500395%*

 * *Differences: {"'definitions'": "{'time_series_model_parameters': {'properties': {'max_electrical_load': "*

 * *                  "OrderedDict([('description', 'Maximum electrical load from OpenStudio building "*

 * *                  "simulation. (W)'), ('type', 'number'), ('default', 0)])}}, "*

 * *                  "'central_cooling_plant_parameters': {'required': {delete: [16, 15, 14, 13, 12, "*

 * *                  "11, 10, 8, 7, 6, 5, 4, 3, 2, 1, 0]}}, 'central_heating_plant_parameters': "*

 * *                  "{'required': {delete: [6, […]*

```diff
@@ -233,31 +233,15 @@
                 "temp_setpoint_chw": {
                     "default": 5,
                     "description": "District circuit chilled water temperature setpoint. (C)",
                     "type": "number"
                 }
             },
             "required": [
-                "heat_flow_nominal",
-                "mass_chw_flow_nominal",
-                "chiller_water_flow_minimum",
-                "mass_cw_flow_nominal",
-                "chw_pump_head",
-                "cw_pump_head",
-                "pressure_drop_chw_nominal",
-                "pressure_drop_cw_nominal",
-                "pressure_drop_setpoint",
-                "temp_setpoint_chw",
-                "pressure_drop_chw_valve_nominal",
-                "pressure_drop_cw_pum_nominal",
-                "temp_air_wb_nominal",
-                "temp_cw_in_nominal",
-                "cooling_tower_water_temperature_difference_nominal",
-                "delta_temp_approach",
-                "ratio_water_air_nominal"
+                "temp_setpoint_chw"
             ],
             "type": "object"
         },
         "central_heating_plant_parameters": {
             "description": "Central heating plant with maximum number of two boilers. Parameters associated with the model.",
             "properties": {
                 "boiler_water_flow_minimum": {
@@ -296,21 +280,15 @@
                 "temp_setpoint_hhw": {
                     "default": 55,
                     "description": "District circuit heating water temperature setpoint. (C)",
                     "type": "number"
                 }
             },
             "required": [
-                "heat_flow_nominal",
-                "mass_hhw_flow_nominal",
-                "boiler_water_flow_minimum",
-                "pressure_drop_hhw_nominal",
-                "temp_setpoint_hhw",
-                "pressure_drop_hhw_valve_nominal",
-                "pressure_drop_setpoint"
+                "temp_setpoint_hhw"
             ],
             "type": "object"
         },
         "combined_heat_and_power_parameters": {
             "description": "Combined heat and power (CHP) parameters used by the microgrid model.",
             "properties": {
                 "fuel_type": {
@@ -397,14 +375,51 @@
                 "nominal_voltage": {
                     "description": "Nominal voltage (V)",
                     "type": "number"
                 }
             },
             "type": "object"
         },
+        "design_def": {
+            "description": "Design parameters used for GHE sizing.",
+            "properties": {
+                "flow_rate": {
+                    "default": 0.3,
+                    "description": "Nominal design mass flow rate. Depending on whether the flow_type attribute is set to 'borehole' or 'system', this will be the nominal flow rate for either each borehole or the entire ground heat exchanger.",
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "flow_type": {
+                    "default": "borehole",
+                    "description": "Flow type for ground heat exchanger sizing, in l/s.",
+                    "enum": [
+                        "borehole",
+                        "system"
+                    ],
+                    "type": "string"
+                },
+                "max_eft": {
+                    "default": 35,
+                    "description": "Maximum heat pump entering fluid temperature used for ground heat exchanger sizing, in Celsius.",
+                    "type": "number"
+                },
+                "min_eft": {
+                    "default": 5,
+                    "description": "Minimum heat pump entering fluid temperature used for ground heat exchanger sizing, in Celsius.",
+                    "type": "number"
+                }
+            },
+            "required": [
+                "flow_rate",
+                "flow_type",
+                "max_eft",
+                "min_eft"
+            ],
+            "type": "object"
+        },
         "diesel_generator_parameters": {
             "description": "Diesel generator parameters used by the microgrid model.",
             "properties": {
                 "nominal_power_generation": {
                     "description": "Nominal power generation (W)",
                     "type": "number"
                 },
@@ -597,22 +612,81 @@
                 "heating_controller_y_max",
                 "heating_controller_y_min"
             ],
             "type": "object"
         },
         "fifth_gen_ets_parameters": {
             "properties": {
+                "chilled_water_supply_temp": {
+                    "default": 5,
+                    "description": "Chilled water supply temperature. (C)",
+                    "type": "number"
+                },
+                "cop_heat_pump_cooling": {
+                    "default": 3.5,
+                    "description": "COP of heat pump for cooling water production.",
+                    "type": "number"
+                },
+                "cop_heat_pump_heating": {
+                    "default": 2.5,
+                    "description": "COP of heat pump for heating water production.",
+                    "type": "number"
+                },
+                "ets_pump_flow_rate": {
+                    "default": 0.0005,
+                    "description": "Design volume flow rate of the ETS pump. (m3/s)",
+                    "type": "number"
+                },
+                "ets_pump_head": {
+                    "default": 10000,
+                    "description": "Design head pressure of the ETS pump. (Pa)",
+                    "type": "number"
+                },
+                "fan_design_flow_rate": {
+                    "default": 0.25,
+                    "description": "Design volume flow rate of the load-side fan. (m3/s)",
+                    "type": "number"
+                },
+                "fan_design_head": {
+                    "default": 150,
+                    "description": "Design head pressure of the load-side fan. (Pa)",
+                    "type": "number"
+                },
+                "hot_water_supply_temp": {
+                    "default": 50,
+                    "description": "Heating water supply temperature. (C)",
+                    "type": "number"
+                },
+                "pump_design_head": {
+                    "default": 150000,
+                    "description": "Design head pressure of the ambient loop pump. (Pa)",
+                    "type": "number"
+                },
+                "pump_flow_rate": {
+                    "default": 0.01,
+                    "description": "Design volume flow rate of the ambient loop pump. (m3/s)",
+                    "type": "number"
+                },
                 "supply_water_temperature_building": {
                     "default": 15,
                     "description": "Water supply temperature building side. (C)",
                     "type": "number"
                 }
             },
             "required": [
-                "supply_water_temperature_building"
+                "supply_water_temperature_building",
+                "chilled_water_supply_temp",
+                "hot_water_supply_temp",
+                "cop_heat_pump_heating",
+                "pump_flow_rate",
+                "pump_design_head",
+                "ets_pump_flow_rate",
+                "ets_pump_head",
+                "fan_design_flow_rate",
+                "fan_design_head"
             ]
         },
         "fifth_generation_def": {
             "properties": {
                 "fifth_generation": {
                     "properties": {
                         "central_cooling_plant_parameters": {
@@ -630,22 +704,60 @@
                                     "properties": {
                                         "building_id": {
                                             "description": "This is the geojson_id that is defined in the building object."
                                         }
                                     }
                                 }
                             ]
+                        },
+                        "ghe_parameters": {
+                            "$ref": "#/definitions/ghe_parameters"
                         }
                     }
                 }
             },
             "required": [
                 "fifth_generation"
             ]
         },
+        "fluid_def": {
+            "description": "Fluid properties for Ground Heat Exchanger sizing",
+            "properties": {
+                "concentration_percent": {
+                    "default": 0,
+                    "description": "The concentration of circulation fluid in percent, from 0-60.",
+                    "maximum": 60,
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "fluid_name": {
+                    "default": "Water",
+                    "description": "Circulating fluid parameters for ground heat exchanger sizing.",
+                    "enum": [
+                        "Water",
+                        "EthylAlcohol",
+                        "EthyleneGlycol",
+                        "MethylAlcohol",
+                        "PropyleneGlycol"
+                    ],
+                    "type": "string"
+                },
+                "temperature": {
+                    "default": 20,
+                    "description": "Average design fluid temperature at peak conditions, in C.",
+                    "type": "number"
+                }
+            },
+            "required": [
+                "fluid_name",
+                "concentration_percent",
+                "temperature"
+            ],
+            "type": "object"
+        },
         "fourth_generation_def": {
             "properties": {
                 "fourth_generation": {
                     "properties": {
                         "central_cooling_plant_parameters": {
                             "$ref": "#/definitions/central_cooling_plant_parameters"
                         },
@@ -669,14 +781,199 @@
                     }
                 }
             },
             "required": [
                 "fourth_generation"
             ]
         },
+        "geometric_constraints_def": {
+            "description": "Geometric constraints for GHE and boreholes.",
+            "properties": {
+                "b_max": {
+                    "default": 10,
+                    "description": "Maximum borehole-to-borehole spacing, in meters.",
+                    "type": "number"
+                },
+                "b_min": {
+                    "default": 3,
+                    "description": "Minimum borehole-to-borehole spacing, in meters.",
+                    "type": "number"
+                },
+                "max_height": {
+                    "default": 200,
+                    "description": "Maximum height, or depth, of each borehole heat exchanger, in meters.",
+                    "type": "number"
+                },
+                "method": {
+                    "default": "rectangle",
+                    "description": "GHE sizing method",
+                    "enum": [
+                        "nearsquare",
+                        "rectangle"
+                    ],
+                    "type": "string"
+                },
+                "min_height": {
+                    "default": 100,
+                    "description": "Minimum height, or depth, of each borehole heat exchanger, in meters.",
+                    "type": "number"
+                }
+            },
+            "required": [
+                "b_min",
+                "b_max",
+                "max_height",
+                "min_height",
+                "method"
+            ],
+            "type": "object"
+        },
+        "ghe_parameters": {
+            "description": "Parameters associated with Ground Heat Exchangers.",
+            "properties": {
+                "design": {
+                    "$ref": "#/definitions/design_def"
+                },
+                "fluid": {
+                    "$ref": "#/definitions/fluid_def"
+                },
+                "geometric_constraints": {
+                    "$ref": "#/definitions/geometric_constraints_def"
+                },
+                "ghe_dir": {
+                    "description": "Results directory for GHE Designer",
+                    "type": "string"
+                },
+                "ghe_specific_params": {
+                    "description": "Specific properties for each Ground Heat Exchanger",
+                    "items": {
+                        "$ref": "#/definitions/ghe_specific_params_def"
+                    },
+                    "type": "array"
+                },
+                "grout": {
+                    "$ref": "#/definitions/grout_def"
+                },
+                "pipe": {
+                    "$ref": "#/definitions/pipe_def"
+                },
+                "simulation": {
+                    "$ref": "#/definitions/simulation_def"
+                },
+                "soil": {
+                    "$ref": "#/definitions/soil_def"
+                },
+                "version": {
+                    "description": "Version of GHE Designer",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "ghe_specific_params",
+                "soil",
+                "pipe",
+                "fluid",
+                "grout",
+                "simulation",
+                "geometric_constraints",
+                "design"
+            ],
+            "type": "object"
+        },
+        "ghe_specific_params_def": {
+            "description": "The properties associated with each Ground Heat Exchanger instance",
+            "properties": {
+                "borehole": {
+                    "additionalProperties": true,
+                    "description": "Borehole properties for Ground Heat Exchanger sizing.",
+                    "properties": {
+                        "buried_depth": {
+                            "default": 1.2,
+                            "description": "The depth below the ground surface to the top of the borehole, in meters.",
+                            "type": "number"
+                        },
+                        "diameter": {
+                            "default": 0.15,
+                            "description": "The diameter of the borehole, in meters.",
+                            "type": "number"
+                        },
+                        "length_of_boreholes": {
+                            "description": "The length of the borehole (in meters), determined from Thermal Network sizing.",
+                            "type": "number"
+                        },
+                        "number_of_boreholes": {
+                            "description": "Number of boreholes on the site, determined from Thermal Network sizing",
+                            "type": "number"
+                        }
+                    },
+                    "required": [
+                        "buried_depth",
+                        "diameter"
+                    ],
+                    "type": "object"
+                },
+                "ghe_geometric_params": {
+                    "description": "The length and width of the Ground Heat Exchanger determined from the GeoJSON Feature File.",
+                    "properties": {
+                        "length_of_ghe": {
+                            "description": "Horizontal surface length allowed for the ground heat exchanger, in meters.",
+                            "type": "number"
+                        },
+                        "width_of_ghe": {
+                            "description": "Horizontal surface width allowed for the ground heat exchanger, in meters.",
+                            "type": "number"
+                        }
+                    },
+                    "required": [
+                        "length_of_ghe",
+                        "width_of_ghe"
+                    ],
+                    "type": "object"
+                },
+                "ghe_id": {
+                    "description": "Feature ID of GHE from GeoJSON Feature File.",
+                    "type": "string"
+                },
+                "ground_loads": {
+                    "description": "Heat rejection or extraction loads (in Watts) of the ground heat exchanger. \n\n Determined from the Thermal Network sizing, and used for ground heat exchanger sizing.\n\n Heat extraction loads are positive, and heat rejection loads are negative.",
+                    "items": {
+                        "type": "number"
+                    },
+                    "type": "array"
+                }
+            },
+            "required": [
+                "ghe_id",
+                "ghe_geometric_params",
+                "borehole"
+            ],
+            "type": "object"
+        },
+        "grout_def": {
+            "description": "Grout properties used for ground heat exchanger sizing.",
+            "properties": {
+                "conductivity": {
+                    "default": 2,
+                    "description": "Grout thermal conductivity, in W/m-K.",
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "rho_cp": {
+                    "default": 4408000,
+                    "description": "Grout volumetric heat capacity, in J/m^3-K.",
+                    "minimum": 0,
+                    "type": "number"
+                }
+            },
+            "required": [
+                "conductivity",
+                "rho_cp"
+            ],
+            "type": "object"
+        },
         "optimization_definition": {
             "additionalProperties": false,
             "description": "[unused] Optimization approach for the topology optimization problem",
             "properties": {
                 "optimization_approach": {
                     "enum": [
                         "Black box",
@@ -684,14 +981,74 @@
                     ],
                     "type": "string"
                 }
             },
             "title": "defaults",
             "type": "object"
         },
+        "pipe_def": {
+            "description": "Pipe properties for Ground Heat Exchanger sizing",
+            "properties": {
+                "arrangement": {
+                    "default": "singleutube",
+                    "description": "Arrangement of the pipes.",
+                    "enum": [
+                        "singleutube",
+                        "coaxial",
+                        "doubleutube"
+                    ],
+                    "type": "string"
+                },
+                "conductivity": {
+                    "default": 0.4,
+                    "description": "The conductivity of the pipe material, in W/m-K.",
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "inner_diameter": {
+                    "default": 0.0269,
+                    "description": "The diameter of the inner pipe surface, in meters.",
+                    "type": "number"
+                },
+                "outer_diameter": {
+                    "default": 0.0334,
+                    "description": "The diameter of the outer pipe surface, in meters.",
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "rho_cp": {
+                    "default": 1542000,
+                    "description": "The volumetric heat capacity of the pipe material, in J/m^3-K",
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "roughness": {
+                    "default": 1e-06,
+                    "description": "The surface roughness of the pipe, in meters.",
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "shank_spacing": {
+                    "default": 0.0277,
+                    "description": "The spacing between the U-tube legs, as referenced from outer surface of the pipes (i.e. not referenced from each pipes respective centerline), in meters.",
+                    "minimum": 0,
+                    "type": "number"
+                }
+            },
+            "required": [
+                "inner_diameter",
+                "outer_diameter",
+                "shank_spacing",
+                "roughness",
+                "conductivity",
+                "rho_cp",
+                "arrangement"
+            ],
+            "type": "object"
+        },
         "power_converter_parameters": {
             "description": "Power converter parameters used by the microgrid model.",
             "properties": {
                 "RMS_voltage_ratio": {
                     "description": "Ratio of RMS voltage on low side/high side",
                     "type": "number"
                 },
@@ -811,14 +1168,55 @@
                 "temp_setpoint_cooling",
                 "temp_setpoint_heating",
                 "temp_hw_supply",
                 "fraction_latent_person"
             ],
             "type": "object"
         },
+        "simulation_def": {
+            "description": "Simulation parameters use for ground heat exchanger sizing.",
+            "properties": {
+                "num_months": {
+                    "default": 240,
+                    "description": "Length of ground heat exchanger sizing period, in months.",
+                    "minimum": 0,
+                    "type": "integer"
+                }
+            },
+            "required": [
+                "num_months"
+            ],
+            "type": "object"
+        },
+        "soil_def": {
+            "description": "Soil properties for Ground Heat Exchanger sizing",
+            "properties": {
+                "conductivity": {
+                    "default": 2,
+                    "description": "The conductivity of the soil, in units of W/m-K.",
+                    "type": "number"
+                },
+                "rho_cp": {
+                    "default": 2600000,
+                    "description": "The volumetric heat capacity of the soil, in units of J/m^3-K",
+                    "type": "number"
+                },
+                "undisturbed_temp": {
+                    "default": 15,
+                    "description": "The undisturbed average soil temperature, in units of degrees Celsius.",
+                    "type": "number"
+                }
+            },
+            "required": [
+                "conductivity",
+                "rho_cp",
+                "undisturbed_temp"
+            ],
+            "type": "object"
+        },
         "spawn_model_parameters": {
             "additionalProperties": false,
             "description": "Parameters associated with spawn models.",
             "properties": {
                 "has_electric_cooling": {
                     "default": false,
                     "description": "Whether the building has electric cooling.",
@@ -1118,14 +1516,19 @@
                     "type": "boolean"
                 },
                 "has_liquid_heating": {
                     "default": true,
                     "description": "Whether the building has liquid heating.",
                     "type": "boolean"
                 },
+                "max_electrical_load": {
+                    "default": 0,
+                    "description": "Maximum electrical load from OpenStudio building simulation. (W)",
+                    "type": "number"
+                },
                 "temp_chw_return": {
                     "default": 12,
                     "description": "Chilled water return temperature. (C)",
                     "type": "number"
                 },
                 "temp_chw_supply": {
                     "default": 7,
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/system_parameters/system_parameters.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/system_parameters/system_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import json
 import logging
 import os
 from copy import deepcopy
 from pathlib import Path
+from typing import Union
 
 import pandas as pd
 import requests
 from jsonpath_ng.ext import parse
-from jsonschema.validators import _LATEST_VERSION as LatestValidator
+from jsonschema.validators import Draft202012Validator as LatestValidator
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     level=logging.INFO,
     format='%(asctime)s - %(levelname)s: %(message)s',
     datefmt='%d-%b-%y %H:%M:%S',
 )
@@ -41,63 +42,62 @@
         Read in the system design parameter file
 
         :param filename: string, (optional) path to file to load
         """
         # load the schema for validation
         schema = Path(__file__).parent / "schema.json"
         self.schema = json.loads(schema.read_text())
-        self.data = {}
+        self.param_template = {}
         self.filename = filename
 
         if self.filename:
             if Path(self.filename).is_file():
                 with open(self.filename, "r") as f:
-                    self.data = json.load(f)
+                    self.param_template = json.load(f)
             else:
                 raise Exception(f"System design parameters file does not exist: {self.filename}")
 
             errors = self.validate()
             if len(errors) != 0:
                 raise Exception(f"Invalid system parameter file. Errors: {errors}")
 
             self.resolve_paths()
 
-        self.param_template = {}
         self.sys_param_filename = None
 
     @classmethod
     def loadd(cls, d, validate_on_load=True):
         """
         Create a system parameters instance from a dictionary
         :param d: dict, system parameter data
 
         :return: object, SystemParameters
         """
         sp = cls()
-        sp.data = d
+        sp.param_template = d
 
         if validate_on_load:
             errors = sp.validate()
             if len(errors) != 0:
                 raise Exception(f"Invalid system parameter file. Errors: {errors}")
 
         return sp
 
     def resolve_paths(self):
         """Resolve the paths in the file to be absolute if they were defined as relative. This method uses
-        the JSONPath (with ext) to find if the value exists in the self.data object. If so, it then uses
+        the JSONPath (with ext) to find if the value exists in the self.param_template object. If so, it then uses
         the set_param which navigates the JSON tree to set the value as needed."""
         filepath = Path(self.filename).parent.resolve()
 
         for pe in self.PATH_ELEMENTS:
-            matches = parse(pe["json_path"]).find(self.data)
+            matches = parse(pe["json_path"]).find(self.param_template)
             for index, match in enumerate(matches):
                 # print(f"Index {index} to update match {match.path} | {match.value} | {match.context}")
                 new_path = Path(filepath) / match.value
-                parse(str(match.full_path)).update(self.data, new_path.as_posix())
+                parse(str(match.full_path)).update(self.param_template, new_path.as_posix())
 
     # def resolve_defaults(self):
     #     """This method will expand the default data blocks into all the subsequent custom sections. If the value is
     #     specificed in the custom block then that will be used, otherwise the default value will be replaced"""
     #     pass
 
     def get_default(self, jsonpath, default=None):
@@ -121,15 +121,15 @@
         :param default: variant, (optional) value to return if can't find the result
         :return: variant, the value from the data
         """
         if jsonpath is None or jsonpath == "":
             return None
 
         # If this is the first entry into the method, then set the data to the
-        data = data or self.data
+        data = data or self.param_template
         matches = parse(jsonpath).find(data)
 
         default_value = default
         if impute_default:
             default_value = self.get_default(jsonpath, default)
 
         results = []
@@ -156,35 +156,35 @@
 
         :param building_id: string, id of the building to look up in the custom section of the system parameters
         :param jsonpath: string, jsonpath formatted string to return
         :param default: variant, (optional) value to return if can't find the result
         :return: variant, the value from the data
         """
 
-        for b in self.data.get("buildings", []):
+        for b in self.param_template.get("buildings", []):
             if b.get("geojson_id", None) == building_id:
                 return self.get_param(jsonpath, data=b)
         else:
             raise SystemExit("No building_id submitted. Please retry and include the feature_id")
 
     def validate(self):
         """
         Validate an instance against a loaded schema
 
         :param instance: dict, json instance to validate
         :return: validation results
         """
         results = []
         v = LatestValidator(self.schema)
-        for error in sorted(v.iter_errors(self.data), key=str):
+        for error in sorted(v.iter_errors(self.param_template), key=str):
             results.append(error.message)
 
         return results
 
-    def download_weatherfile(self, filename, save_directory: str) -> str:
+    def download_weatherfile(self, filename, save_directory: str) -> Union[str, Path]:
         """Download the MOS or EPW weather file from energyplus.net
 
         This routine downloads the weather file, either an MOS or EPW, which is selected based
         on the file extension.
 
             filename, str: Name of weather file to download, e.g., USA_NY_Buffalo-Greater.Buffalo.Intl.AP.725280_TMY3.mos
             save_directory, str: Location where to save the downloaded content. The path must exist before downloading.
@@ -722,17 +722,18 @@
 
         # Grab building load filepaths from sdk output
         for thing in scenario_dir.iterdir():
             if thing.is_dir():
                 for item in thing.iterdir():
                     if item.is_dir():
                         if str(item).endswith('_export_time_series_modelica'):
-                            measure_list.append(Path(item) / "building_loads.csv")
+                            measure_list.append(Path(item) / "building_loads.csv")  # used for mfrt
                         elif str(item).endswith('_export_modelica_loads'):
-                            measure_list.append(Path(item) / "modelica.mos")
+                            measure_list.append(Path(item) / "modelica.mos")  # space heating/cooling & water heating
+                            measure_list.append(Path(item) / "building_loads.csv")  # used for max electricity load
 
         # Get each feature id from the SDK FeatureFile
         building_ids = []
         with open(feature_file) as json_file:
             sdk_input = json.load(json_file)
             weather_filename = sdk_input['project']['weather_filename']
             weather_path = self.sys_param_filename.parent / weather_filename
@@ -778,14 +779,21 @@
                         building['ets_indirect_parameters']['nominal_mass_flow_building'] = float(building_nominal_mfrt)
                     except KeyError:
                         # If massFlowRateHeating is not in the export_time_series_modelica output, just skip this step.
                         # It probably won't be in the export for hpxml residential buildings, at least as of 2022-06-29
                         logger.info("mass-flow-rate heating is not present. It is not expected in residential buildings. Skipping.")
                         continue
                 district_nominal_mfrt += building_nominal_mfrt
+                if measure_file_path.suffix == '.csv' and measure_folder_name.endswith('_export_modelica_loads'):
+                    try:
+                        building_loads = pd.read_csv(measure_file_path, usecols=['ElectricityFacility'])  # usecols to make the df small
+                    except ValueError:  # hack to handle the case where there is no ElectricityFacility column in the csv
+                        continue
+                    max_electricity_load = int(building_loads['ElectricityFacility'].max())
+                    building['load_model_parameters']['time_series']['max_electrical_load'] = max_electricity_load
 
         # Remove template buildings that weren't used or don't have successful simulations with modelica outputs
         # TODO: Another place where we only support time series for now.
         building_list = [x for x in building_list if not x['load_model_parameters']
                          ['time_series']['filepath'].endswith("populated")]
         if len(building_list) == 0:
             raise SystemExit("No Modelica files found. Modelica files are expected to be found within each feature in folders "
@@ -813,15 +821,15 @@
                         "Run opendss and reopt-feature post-processing in the UO SDK for a full-featured microgrid.")
         try:
             self.process_microgrid_inputs(scenario_dir)
         except UnboundLocalError:
             raise SystemExit(f"\nError: No scenario_optimization.json file found in {scenario_dir}\n"
                              "Perhaps you haven't run REopt post-processing step in the UO sdk?")
 
-        # save
+        # save the file to disk
         self.save()
 
     def save(self):
         """
         Write the system parameters file with param_template and save
         """
         with open(self.sys_param_filename, 'w') as outfile:
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/system_parameters/time_series_microgrid_template.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/system_parameters/time_series_microgrid_template.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999141483516484%*

 * *Differences: {"'buildings'": "{0: {'load_model_parameters': {'time_series': {'max_electrical_load': 0}}}}"}*

```diff
@@ -31,14 +31,15 @@
                     "delta_temp_air_cooling": 10,
                     "delta_temp_air_heating": 18,
                     "filepath": "To be populated",
                     "has_electric_cooling": false,
                     "has_electric_heating": false,
                     "has_liquid_cooling": true,
                     "has_liquid_heating": true,
+                    "max_electrical_load": 0,
                     "temp_chw_return": 12,
                     "temp_chw_supply": 7,
                     "temp_hw_return": 35,
                     "temp_hw_supply": 40,
                     "temp_setpoint_cooling": 24,
                     "temp_setpoint_heating": 20
                 }
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/system_parameters/time_series_template.json` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/system_parameters/time_series_template.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999404761904762%*

 * *Differences: {"'buildings'": "{0: {'load_model_parameters': {'time_series': {'max_electrical_load': 0}}}}"}*

```diff
@@ -28,14 +28,15 @@
                     "delta_temp_air_cooling": 10,
                     "delta_temp_air_heating": 18,
                     "filepath": "To be populated",
                     "has_electric_cooling": false,
                     "has_electric_heating": false,
                     "has_liquid_cooling": true,
                     "has_liquid_heating": true,
+                    "max_electrical_load": 0,
                     "temp_chw_return": 12,
                     "temp_chw_supply": 7,
                     "temp_hw_return": 35,
                     "temp_hw_supply": 40,
                     "temp_setpoint_cooling": 24,
                     "temp_setpoint_heating": 20
                 }
```

### Comparing `geojson_modelica_translator-0.4.1/geojson_modelica_translator/utils.py` & `geojson_modelica_translator-0.5.0/geojson_modelica_translator/utils.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/management/check_sys_params.py` & `geojson_modelica_translator-0.5.0/management/check_sys_params.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/management/data/baseline_geojson.json` & `geojson_modelica_translator-0.5.0/management/data/baseline_geojson.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/management/data/baseline_sys_params.json` & `geojson_modelica_translator-0.5.0/management/data/baseline_sys_params.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/management/data/baseline_weather.mos` & `geojson_modelica_translator-0.5.0/management/data/baseline_weather.mos`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/management/format_modelica_files.py` & `geojson_modelica_translator-0.5.0/management/format_modelica_files.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/management/uo_des.py` & `geojson_modelica_translator-0.5.0/management/uo_des.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,22 +172,25 @@
         default = ./model_from_sdk
 
     \f
     :param modelica_project: Path, name & location of modelica project, possibly created with this cli
     """
     run_path = Path(modelica_project).resolve()
     project_name = run_path.stem
-    file_to_run = run_path / 'Districts' / 'DistrictEnergySystem.mo'
 
     if len(str(run_path).split()) > 1:  # Modelica can't handle spaces in project name or path
         raise SystemExit(
             f"\n'{run_path}' failed. Modelica does not support spaces in project names or paths. "
             "Please update your directory tree to not include spaces in any name")
 
     # setup modelica runner
     mr = ModelicaRunner()
-    mr.run_in_docker(file_to_run, run_path=run_path.parent, project_name=project_name)
+    mr.run_in_docker('compile_and_run',
+                     f'{project_name}.Districts.DistrictEnergySystem',
+                     file_to_load=run_path / 'package.mo',
+                     run_path=run_path
+                     )
 
-    if (run_path.parent / f'{project_name}_results' / f'{project_name}_Districts_DistrictEnergySystem_result.mat').exists():
+    if (run_path.parent / f'{project_name}/{project_name}.Districts.DistrictEnergySystem_results' / f'{project_name}_Districts_DistrictEnergySystem_res.mat').exists():
         print(f"\nModelica model {project_name} ran successfully")
     else:
         raise SystemExit(f"\n{project_name} failed. Check the error log at {project_name}_results/stdout.log for more info.")
```

### Comparing `geojson_modelica_translator-0.4.1/management/update_schemas.py` & `geojson_modelica_translator-0.5.0/management/update_schemas.py`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.4.1/pyproject.toml` & `geojson_modelica_translator-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geojson-modelica-translator"
-version = "0.4.1"
+version = "0.5.0"
 description = "Package for converting GeoJSON to Modelica models for Urban Scale Analyses."
 authors = ["URBANopt DES Team <nicholas.long@nrel.gov>"]
 license = "BSD-4-Clause"
 
 readme = "README.rst"
 
 homepage = "https://docs.urbanopt.net"
@@ -13,52 +13,52 @@
 keywords = ["URBANopt", "Modelica", "GeoJSON", "Physics-based Modeling"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 packages = [
     { include = "management" },
     { include = "geojson_modelica_translator"}
 ]
 
 [tool.poetry.dependencies]
 # Urbanopt SDK requires Python 3.10 as of UOv0.9.0
-python = ">=3.8, <3.11"
+python = ">=3.9, <3.12"
 BuildingsPy = "4.0.0"
 click = "8.1.3"
-geojson = "2.5.0"
+geojson = "^3.0.0"
 jinja2 = "3.1.2"
 jsonpath-ng = "1.5.3"
 jsonschema = "~4.17"
-modelica-builder = "^0.2.2"
-pandas = "1.5.2"
-requests = "2.27.1"
+modelica-builder = "^0.2.3"
+pandas = "2.0.2"
+requests = "^2.28"
 teaser = "0.7.5"
 #teaser = { git = "https://github.com/urbanopt/TEASER.git", branch = "development"}
 
 
 [tool.poetry.dev-dependencies]
 autopep8 = "~2.0"
 coveralls = "~3.3"
-mypy = "~0.961"
-pre-commit = "~2.21"
-pytest = "~7.2"
+mypy = "~1.2"
+pre-commit = "~3.2"
+pytest = "~7.3"
 pytest-cov = "~4.0"
+# don't update sphinx right now
 sphinx = "~5.0"
 sphinx_rtd_theme = "~1.0.0"
 sphinx-jsonschema = "~1.19"
 syrupy = "~3.0"
 toml = "~0.10"
-tox = "~4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 multi_line_output = 3
```

### Comparing `geojson_modelica_translator-0.4.1/PKG-INFO` & `geojson_modelica_translator-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: geojson-modelica-translator
-Version: 0.4.1
+Version: 0.5.0
 Summary: Package for converting GeoJSON to Modelica models for Urban Scale Analyses.
 Home-page: https://docs.urbanopt.net
 License: BSD-4-Clause
 Keywords: URBANopt,Modelica,GeoJSON,Physics-based Modeling
 Author: URBANopt DES Team
 Author-email: nicholas.long@nrel.gov
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: BuildingsPy (==4.0.0)
 Requires-Dist: click (==8.1.3)
-Requires-Dist: geojson (==2.5.0)
+Requires-Dist: geojson (>=3.0.0,<4.0.0)
 Requires-Dist: jinja2 (==3.1.2)
 Requires-Dist: jsonpath-ng (==1.5.3)
 Requires-Dist: jsonschema (>=4.17,<4.18)
-Requires-Dist: modelica-builder (>=0.2.2,<0.3.0)
-Requires-Dist: pandas (==1.5.2)
-Requires-Dist: requests (==2.27.1)
+Requires-Dist: modelica-builder (>=0.2.3,<0.3.0)
+Requires-Dist: pandas (==2.0.2)
+Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: teaser (==0.7.5)
 Project-URL: Documentation, https://docs.urbanopt.net/geojson-modelica-translator/
 Project-URL: Repository, https://github.com/urbanopt/geojson-modelica-translator
 Description-Content-Type: text/x-rst
 
 GeoJSON Modelica Translator (GMT)
 ---------------------------------
```

