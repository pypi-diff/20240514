# Comparing `tmp/zepben.evolve-0.38.0b7-py3-none-any.whl.zip` & `tmp/zepben.evolve-0.38.0b8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,334 +1,344 @@
-Zip file size: 437836 bytes, number of entries: 332
--rw-r--r--  2.0 unx    19009 b- defN 24-Mar-27 06:33 zepben/evolve/__init__.py
--rw-r--r--  2.0 unx     1387 b- defN 24-Mar-27 06:33 zepben/evolve/exceptions.py
--rw-r--r--  2.0 unx     1132 b- defN 24-Mar-27 06:33 zepben/evolve/types.py
--rw-r--r--  2.0 unx     4576 b- defN 24-Mar-27 06:33 zepben/evolve/util.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/__init__.py
--rw-r--r--  2.0 unx     7148 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/database_reader.py
--rw-r--r--  2.0 unx     6108 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/database_writer.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/__init__.py
--rw-r--r--  2.0 unx     5275 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/base_cim_reader.py
--rw-r--r--  2.0 unx     2991 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/base_service_reader.py
--rw-r--r--  2.0 unx     4510 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/customer_cim_reader.py
--rw-r--r--  2.0 unx     1761 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/customer_service_reader.py
--rw-r--r--  2.0 unx     3245 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/diagram_cim_reader.py
--rw-r--r--  2.0 unx     1041 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/diagram_service_reader.py
--rw-r--r--  2.0 unx      733 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/metadata_collection_reader.py
--rw-r--r--  2.0 unx     1088 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/metadata_entry_reader.py
--rw-r--r--  2.0 unx    80182 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/network_cim_reader.py
--rw-r--r--  2.0 unx    12684 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/network_service_reader.py
--rw-r--r--  2.0 unx     6872 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/readers/result_set.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/__init__.py
--rw-r--r--  2.0 unx     1009 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/column.py
--rw-r--r--  2.0 unx    12102 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/database_tables.py
--rw-r--r--  2.0 unx      403 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/exceptions.py
--rw-r--r--  2.0 unx     1164 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/metadata_tables.py
--rw-r--r--  2.0 unx     5820 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/sqlite_table.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/__init__.py
--rw-r--r--  2.0 unx     1484 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/assetorganisationroles_association_tables.py
--rw-r--r--  2.0 unx     2295 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/circuit_association_tables.py
--rw-r--r--  2.0 unx     1561 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/customeragreements_association_tables.py
--rw-r--r--  2.0 unx     3547 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/equipment_association_tables.py
--rw-r--r--  2.0 unx     1696 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py
--rw-r--r--  2.0 unx     1435 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py
--rw-r--r--  2.0 unx     1572 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/protection_equipment_protected_switches.py
--rw-r--r--  2.0 unx     1409 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/__init__.py
--rw-r--r--  2.0 unx     2240 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py
--rw-r--r--  2.0 unx     9391 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py
--rw-r--r--  2.0 unx     5681 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/common_tables.py
--rw-r--r--  2.0 unx     1705 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/customer_tables.py
--rw-r--r--  2.0 unx     1912 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/metering_tables.py
--rw-r--r--  2.0 unx      494 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/operations_tables.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/__init__.py
--rw-r--r--  2.0 unx     5266 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/__init__.py
--rw-r--r--  2.0 unx     1995 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/auxiliaryequipment_tables.py
--rw-r--r--  2.0 unx     8442 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/core_tables.py
--rw-r--r--  2.0 unx     3113 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/diagramlayout_tables.py
--rw-r--r--  2.0 unx     2454 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py
--rw-r--r--  2.0 unx     2581 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/protection_tables.py
--rw-r--r--  2.0 unx     1205 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/__init__.py
--rw-r--r--  2.0 unx     1226 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/conductor_tables.py
--rw-r--r--  2.0 unx      710 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/connector_tables.py
--rw-r--r--  2.0 unx      458 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/container_tables.py
--rw-r--r--  2.0 unx    16832 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/energyconnection_tables.py
--rw-r--r--  2.0 unx     1845 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/perlength_tables.py
--rw-r--r--  2.0 unx     2325 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py
--rw-r--r--  2.0 unx     8640 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/transformer_tables.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/__init__.py
--rw-r--r--  2.0 unx     2114 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/production_tables.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/__init__.py
--rw-r--r--  2.0 unx     1515 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/feeder_tables.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/__init__.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/__init__.py
--rw-r--r--  2.0 unx      454 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/production_tables.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/__init__.py
--rw-r--r--  2.0 unx     5263 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/base_cim_writer.py
--rw-r--r--  2.0 unx     2995 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/base_service_writer.py
--rw-r--r--  2.0 unx     4752 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/customer_cim_writer.py
--rw-r--r--  2.0 unx     1393 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/customer_service_writer.py
--rw-r--r--  2.0 unx     2657 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/diagram_cim_writer.py
--rw-r--r--  2.0 unx     1004 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/diagram_service_writer.py
--rw-r--r--  2.0 unx      904 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/metadata_collection_writer.py
--rw-r--r--  2.0 unx     1257 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/metadata_entry_writer.py
--rw-r--r--  2.0 unx    77362 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/network_cim_writer.py
--rw-r--r--  2.0 unx     8548 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/network_service_writer.py
--rw-r--r--  2.0 unx     1430 b- defN 24-Mar-27 06:33 zepben/evolve/database/sqlite/writers/utils.py
--rw-r--r--  2.0 unx      302 b- defN 24-Mar-27 06:33 zepben/evolve/examples/__init__.py
--rw-r--r--  2.0 unx     5062 b- defN 24-Mar-27 06:33 zepben/evolve/examples/simple_test_network.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/__init__.py
--rw-r--r--  2.0 unx     7357 b- defN 24-Mar-27 06:33 zepben/evolve/model/phases.py
--rw-r--r--  2.0 unx     1502 b- defN 24-Mar-27 06:33 zepben/evolve/model/resistance_reactance.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/busbranch/__init__.py
--rw-r--r--  2.0 unx    47076 b- defN 24-Mar-27 06:33 zepben/evolve/model/busbranch/bus_branch.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/__init__.py
--rw-r--r--  2.0 unx     1398 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/no_load_test.py
--rw-r--r--  2.0 unx     1445 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/open_circuit_test.py
--rw-r--r--  2.0 unx     4220 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/power_transformer_info.py
--rw-r--r--  2.0 unx     1877 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py
--rw-r--r--  2.0 unx      927 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py
--rw-r--r--  2.0 unx      550 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/switch_info.py
--rw-r--r--  2.0 unx     5904 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py
--rw-r--r--  2.0 unx     4395 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py
--rw-r--r--  2.0 unx      860 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/wire_info.py
--rw-r--r--  2.0 unx     1015 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assetinfo/wire_material_kind.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assets/__init__.py
--rw-r--r--  2.0 unx     4019 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assets/asset.py
--rw-r--r--  2.0 unx      845 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assets/asset_info.py
--rw-r--r--  2.0 unx      588 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assets/asset_organisation_role.py
--rw-r--r--  2.0 unx     3009 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assets/pole.py
--rw-r--r--  2.0 unx     1157 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assets/streetlight.py
--rw-r--r--  2.0 unx      635 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/assets/structure.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/common/__init__.py
--rw-r--r--  2.0 unx     1570 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/common/document.py
--rw-r--r--  2.0 unx     7841 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/common/location.py
--rw-r--r--  2.0 unx      531 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/common/organisation.py
--rw-r--r--  2.0 unx      838 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/common/organisation_role.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/customers/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/customers/customer.py
--rw-r--r--  2.0 unx     4260 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/customers/customer_agreement.py
--rw-r--r--  2.0 unx     1474 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/customers/customer_kind.py
--rw-r--r--  2.0 unx     3336 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/customers/pricing_structure.py
--rw-r--r--  2.0 unx      763 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/customers/tariff.py
--rw-r--r--  2.0 unx      244 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/__init__.py
--rw-r--r--  2.0 unx      244 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py
--rw-r--r--  2.0 unx     4000 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_relay_info.py
--rw-r--r--  2.0 unx     1859 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py
--rw-r--r--  2.0 unx     1250 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py
--rw-r--r--  2.0 unx      993 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py
--rw-r--r--  2.0 unx     1098 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py
--rw-r--r--  2.0 unx     1202 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/ratio.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/metering/__init__.py
--rw-r--r--  2.0 unx    11269 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/metering/metering.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/operations/__init__.py
--rw-r--r--  2.0 unx     3889 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61968/operations/operational_restriction.py
--rw-r--r--  2.0 unx      248 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/__init__.py
--rw-r--r--  2.0 unx      249 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/__init__.py
--rw-r--r--  2.0 unx     1475 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/auxiliary_equipment.py
--rw-r--r--  2.0 unx     1489 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/current_transformer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer.py
--rw-r--r--  2.0 unx      811 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer_kind.py
--rw-r--r--  2.0 unx      588 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/sensor.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/__init__.py
--rw-r--r--  2.0 unx      556 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/base_voltage.py
--rw-r--r--  2.0 unx     7135 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/conducting_equipment.py
--rw-r--r--  2.0 unx     3645 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/connectivity_node.py
--rw-r--r--  2.0 unx      592 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/connectivity_node_container.py
--rw-r--r--  2.0 unx    14195 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/equipment.py
--rw-r--r--  2.0 unx    15682 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/equipment_container.py
--rw-r--r--  2.0 unx     8261 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/identified_object.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/name.py
--rw-r--r--  2.0 unx     7475 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/name_type.py
--rw-r--r--  2.0 unx     7033 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/phase_code.py
--rw-r--r--  2.0 unx     1250 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/power_system_resource.py
--rw-r--r--  2.0 unx     6734 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/regions.py
--rw-r--r--  2.0 unx    10120 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/substation.py
--rw-r--r--  2.0 unx     6717 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/core/terminal.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/diagramlayout/__init__.py
--rw-r--r--  2.0 unx    10307 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_layout.py
--rw-r--r--  2.0 unx      748 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_style.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/diagramlayout/orientation_kind.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/domain/__init__.py
--rw-r--r--  2.0 unx    17065 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/domain/unit_symbol.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/equivalents/__init__.py
--rw-r--r--  2.0 unx     5374 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_branch.py
--rw-r--r--  2.0 unx      641 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_equipment.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/meas/__init__.py
--rw-r--r--  2.0 unx      963 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/meas/control.py
--rw-r--r--  2.0 unx      576 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/meas/iopoint.py
--rw-r--r--  2.0 unx     4294 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/meas/measurement.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/meas/value.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/protection/__init__.py
--rw-r--r--  2.0 unx     1465 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/protection/current_relay.py
--rw-r--r--  2.0 unx     4777 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/protection/protection_equipment.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/scada/__init__.py
--rw-r--r--  2.0 unx      737 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/scada/remote_control.py
--rw-r--r--  2.0 unx      587 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/scada/remote_point.py
--rw-r--r--  2.0 unx      734 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/scada/remote_source.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/__init__.py
--rw-r--r--  2.0 unx     2433 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py
--rw-r--r--  2.0 unx     1385 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/breaker.py
--rw-r--r--  2.0 unx     1413 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/connectors.py
--rw-r--r--  2.0 unx      672 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/disconnector.py
--rw-r--r--  2.0 unx     1929 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py
--rw-r--r--  2.0 unx     7483 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py
--rw-r--r--  2.0 unx     6517 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/energy_source.py
--rw-r--r--  2.0 unx     1977 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py
--rw-r--r--  2.0 unx      595 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/fuse.py
--rw-r--r--  2.0 unx      611 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/jumper.py
--rw-r--r--  2.0 unx      492 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/line.py
--rw-r--r--  2.0 unx      584 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py
--rw-r--r--  2.0 unx     1904 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/per_length.py
--rw-r--r--  2.0 unx      884 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py
--rw-r--r--  2.0 unx    24976 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py
--rw-r--r--  2.0 unx    30217 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py
--rw-r--r--  2.0 unx     4386 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/protected_switch.py
--rw-r--r--  2.0 unx      582 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/recloser.py
--rw-r--r--  2.0 unx     8103 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/regulating_control.py
--rw-r--r--  2.0 unx     1168 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/regulating_control_mode_kind.py
--rw-r--r--  2.0 unx     3658 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py
--rw-r--r--  2.0 unx     4955 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/switch.py
--rw-r--r--  2.0 unx     2112 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/tap_changer_control.py
--rw-r--r--  2.0 unx     1045 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/transformer_cooling_type.py
--rw-r--r--  2.0 unx     2219 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/transformer_star_impedance.py
--rw-r--r--  2.0 unx     1544 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/vector_group.py
--rw-r--r--  2.0 unx      786 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/winding_connection.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/generation/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/generation/production/__init__.py
--rw-r--r--  2.0 unx      809 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/generation/production/battery_state_kind.py
--rw-r--r--  2.0 unx     2215 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/base/wires/generation/production/power_electronics_unit.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/__init__.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/feeder/__init__.py
--rw-r--r--  2.0 unx     5385 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/feeder/circuit.py
--rw-r--r--  2.0 unx     7542 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py
--rw-r--r--  2.0 unx     7636 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/protection/__init__.py
--rw-r--r--  2.0 unx      746 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/protection/power_direction_kind.py
--rw-r--r--  2.0 unx      768 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/protection/protection_kind.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/wires/__init__.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/__init__.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/__init__.py
--rw-r--r--  2.0 unx      426 b- defN 24-Mar-27 06:33 zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/ev_charging_unit.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/__init__.py
--rw-r--r--  2.0 unx      960 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/__init__.py
--rw-r--r--  2.0 unx    18023 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/base_service.py
--rw-r--r--  2.0 unx    16620 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/base_service_comparator.py
--rw-r--r--  2.0 unx     1189 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/difference.py
--rw-r--r--  2.0 unx    22895 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/reference_resolvers.py
--rw-r--r--  2.0 unx    20762 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/resolver.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/meta/__init__.py
--rw-r--r--  2.0 unx      461 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/meta/data_source.py
--rw-r--r--  2.0 unx      804 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/meta/metadata_collection.py
--rw-r--r--  2.0 unx     1481 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/meta/metadata_translations.py
--rw-r--r--  2.0 unx      601 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/meta/service_info.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/translator/__init__.py
--rw-r--r--  2.0 unx     3420 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/translator/base_cim2proto.py
--rw-r--r--  2.0 unx     3938 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/translator/base_proto2cim.py
--rw-r--r--  2.0 unx     2924 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/translator/service_differences.py
--rw-r--r--  2.0 unx     2410 b- defN 24-Mar-27 06:33 zepben/evolve/services/common/translator/util.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/customer/__init__.py
--rw-r--r--  2.0 unx     1922 b- defN 24-Mar-27 06:33 zepben/evolve/services/customer/customer_service_comparator.py
--rw-r--r--  2.0 unx      467 b- defN 24-Mar-27 06:33 zepben/evolve/services/customer/customers.py
--rw-r--r--  2.0 unx     1044 b- defN 24-Mar-27 06:33 zepben/evolve/services/customer/translator/__init__.py
--rw-r--r--  2.0 unx     2760 b- defN 24-Mar-27 06:33 zepben/evolve/services/customer/translator/customer_cim2proto.py
--rw-r--r--  2.0 unx     3379 b- defN 24-Mar-27 06:33 zepben/evolve/services/customer/translator/customer_proto2cim.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/diagram/__init__.py
--rw-r--r--  2.0 unx     1486 b- defN 24-Mar-27 06:33 zepben/evolve/services/diagram/diagram_service_comparator.py
--rw-r--r--  2.0 unx     4598 b- defN 24-Mar-27 06:33 zepben/evolve/services/diagram/diagrams.py
--rw-r--r--  2.0 unx      508 b- defN 24-Mar-27 06:33 zepben/evolve/services/diagram/translator/__init__.py
--rw-r--r--  2.0 unx     2237 b- defN 24-Mar-27 06:33 zepben/evolve/services/diagram/translator/diagram_cim2proto.py
--rw-r--r--  2.0 unx     2463 b- defN 24-Mar-27 06:33 zepben/evolve/services/diagram/translator/diagram_proto2cim.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/measurement/__init__.py
--rw-r--r--  2.0 unx     1207 b- defN 24-Mar-27 06:33 zepben/evolve/services/measurement/measurements.py
--rw-r--r--  2.0 unx      261 b- defN 24-Mar-27 06:33 zepben/evolve/services/measurement/translator/__init__.py
--rw-r--r--  2.0 unx     1832 b- defN 24-Mar-27 06:33 zepben/evolve/services/measurement/translator/measurement_cim2proto.py
--rw-r--r--  2.0 unx     1951 b- defN 24-Mar-27 06:33 zepben/evolve/services/measurement/translator/measurement_proto2cim.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/__init__.py
--rw-r--r--  2.0 unx     6279 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/network_extensions.py
--rw-r--r--  2.0 unx    10634 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/network_service.py
--rw-r--r--  2.0 unx    42979 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/network_service_comparator.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/__init__.py
--rw-r--r--  2.0 unx     3654 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/find.py
--rw-r--r--  2.0 unx     5623 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/find_swer_equipment.py
--rw-r--r--  2.0 unx    16173 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/tracing.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/util.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/__init__.py
--rw-r--r--  2.0 unx      775 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step.py
--rw-r--r--  2.0 unx     2394 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step_tracker.py
--rw-r--r--  2.0 unx     8474 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/connected_equipment_trace.py
--rw-r--r--  2.0 unx     1162 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/connected_equipment_traversal.py
--rw-r--r--  2.0 unx     4223 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/connectivity_result.py
--rw-r--r--  2.0 unx     2671 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/connectivity_trace.py
--rw-r--r--  2.0 unx     1212 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/connectivity_tracker.py
--rw-r--r--  2.0 unx     5162 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/limited_connected_equipment_trace.py
--rw-r--r--  2.0 unx     3872 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/phase_paths.py
--rw-r--r--  2.0 unx     9998 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_connected.py
--rw-r--r--  2.0 unx     2862 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_internal.py
--rw-r--r--  2.0 unx    11472 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/transformer_phase_paths.py
--rw-r--r--  2.0 unx    10412 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/xy_candidate_phase_paths.py
--rw-r--r--  2.0 unx      583 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/connectivity/xy_phase_step.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/__init__.py
--rw-r--r--  2.0 unx     5997 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py
--rw-r--r--  2.0 unx     6053 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py
--rw-r--r--  2.0 unx     3246 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/associated_terminal_trace.py
--rw-r--r--  2.0 unx     1477 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/associated_terminal_tracker.py
--rw-r--r--  2.0 unx     3990 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/direction_status.py
--rw-r--r--  2.0 unx     2546 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/feeder_direction.py
--rw-r--r--  2.0 unx     7410 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/remove_direction.py
--rw-r--r--  2.0 unx     6757 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/feeder/set_direction.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/phases/__init__.py
--rw-r--r--  2.0 unx    10311 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/phases/phase_inferrer.py
--rw-r--r--  2.0 unx     3428 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/phases/phase_status.py
--rw-r--r--  2.0 unx     2628 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/phases/phase_step.py
--rw-r--r--  2.0 unx     2014 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/phases/phase_step_tracker.py
--rw-r--r--  2.0 unx     6251 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/phases/phase_trace.py
--rw-r--r--  2.0 unx     5510 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/phases/remove_phases.py
--rw-r--r--  2.0 unx    12798 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/phases/set_phases.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/traversals/__init__.py
--rw-r--r--  2.0 unx     1642 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/traversals/basic_tracker.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/traversals/basic_traversal.py
--rw-r--r--  2.0 unx     6585 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/traversals/branch_recursive_tracing.py
--rw-r--r--  2.0 unx     5164 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/traversals/queue.py
--rw-r--r--  2.0 unx     1775 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/traversals/tracker.py
--rw-r--r--  2.0 unx     8650 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/traversals/traversal.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/tree/__init__.py
--rw-r--r--  2.0 unx     4454 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/tree/downstream_tree.py
--rw-r--r--  2.0 unx     1780 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/tree/tree_node.py
--rw-r--r--  2.0 unx     1167 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/tracing/tree/tree_node_tracker.py
--rw-r--r--  2.0 unx    22426 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/translator/__init__.py
--rw-r--r--  2.0 unx    65188 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/translator/network_cim2proto.py
--rw-r--r--  2.0 unx    78124 b- defN 24-Mar-27 06:33 zepben/evolve/services/network/translator/network_proto2cim.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/__init__.py
--rw-r--r--  2.0 unx      427 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/exceptions.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/get/__init__.py
--rw-r--r--  2.0 unx     9348 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/get/consumer.py
--rw-r--r--  2.0 unx     5425 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/get/customer_consumer.py
--rw-r--r--  2.0 unx     5032 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/get/diagram_consumer.py
--rw-r--r--  2.0 unx    38079 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/get/network_consumer.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/get/hierarchy/__init__.py
--rw-r--r--  2.0 unx     1047 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/get/hierarchy/data.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/grpc/__init__.py
--rw-r--r--  2.0 unx      801 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/grpc/auth_token_plugin.py
--rw-r--r--  2.0 unx     9451 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/grpc/connect.py
--rw-r--r--  2.0 unx     4020 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/grpc/grpc.py
--rw-r--r--  2.0 unx     7664 b- defN 24-Mar-27 06:33 zepben/evolve/streaming/grpc/grpc_channel_builder.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 06:33 zepben/evolve/testing/__init__.py
--rw-r--r--  2.0 unx    28552 b- defN 24-Mar-27 06:33 zepben/evolve/testing/test_network_builder.py
--rw-r--r--  2.0 unx     3238 b- defN 24-Mar-27 06:33 zepben/evolve/testing/test_traversal.py
--rw-r--r--  2.0 unx    16725 b- defN 24-Mar-27 06:37 zepben.evolve-0.38.0b7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2299 b- defN 24-Mar-27 06:37 zepben.evolve-0.38.0b7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 06:37 zepben.evolve-0.38.0b7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-27 06:37 zepben.evolve-0.38.0b7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    38855 b- defN 24-Mar-27 06:37 zepben.evolve-0.38.0b7.dist-info/RECORD
-332 files, 1567154 bytes uncompressed, 372432 bytes compressed:  76.2%
+Zip file size: 456706 bytes, number of entries: 342
+-rw-r--r--  2.0 unx    19853 b- defN 24-Mar-27 11:04 zepben/evolve/__init__.py
+-rw-r--r--  2.0 unx     1387 b- defN 24-Mar-27 11:04 zepben/evolve/exceptions.py
+-rw-r--r--  2.0 unx     1132 b- defN 24-Mar-27 11:04 zepben/evolve/types.py
+-rw-r--r--  2.0 unx     4576 b- defN 24-Mar-27 11:04 zepben/evolve/util.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/__init__.py
+-rw-r--r--  2.0 unx     7148 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/database_reader.py
+-rw-r--r--  2.0 unx     6108 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/database_writer.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/__init__.py
+-rw-r--r--  2.0 unx     5275 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/base_cim_reader.py
+-rw-r--r--  2.0 unx     2991 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/base_service_reader.py
+-rw-r--r--  2.0 unx     4510 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/customer_cim_reader.py
+-rw-r--r--  2.0 unx     1761 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/customer_service_reader.py
+-rw-r--r--  2.0 unx     3245 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/diagram_cim_reader.py
+-rw-r--r--  2.0 unx     1041 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/diagram_service_reader.py
+-rw-r--r--  2.0 unx      733 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/metadata_collection_reader.py
+-rw-r--r--  2.0 unx     1088 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/metadata_entry_reader.py
+-rw-r--r--  2.0 unx    88904 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/network_cim_reader.py
+-rw-r--r--  2.0 unx    14696 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/network_service_reader.py
+-rw-r--r--  2.0 unx     6872 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/readers/result_set.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/__init__.py
+-rw-r--r--  2.0 unx     1009 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/column.py
+-rw-r--r--  2.0 unx    13135 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/database_tables.py
+-rw-r--r--  2.0 unx      403 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/exceptions.py
+-rw-r--r--  2.0 unx     1164 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/metadata_tables.py
+-rw-r--r--  2.0 unx     5820 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/sqlite_table.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/__init__.py
+-rw-r--r--  2.0 unx     1484 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/assetorganisationroles_association_tables.py
+-rw-r--r--  2.0 unx     2295 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/circuit_association_tables.py
+-rw-r--r--  2.0 unx     1561 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/customeragreements_association_tables.py
+-rw-r--r--  2.0 unx     3547 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/equipment_association_tables.py
+-rw-r--r--  2.0 unx     1696 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/protection_relay_functions_protected_switches.py
+-rw-r--r--  2.0 unx     1426 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/protection_relay_functions_sensors.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/protection_relay_schemes_protection_relay_functions.py
+-rw-r--r--  2.0 unx     1409 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/__init__.py
+-rw-r--r--  2.0 unx     2240 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py
+-rw-r--r--  2.0 unx     9391 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py
+-rw-r--r--  2.0 unx     5681 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/common_tables.py
+-rw-r--r--  2.0 unx     1705 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/customer_tables.py
+-rw-r--r--  2.0 unx     1912 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/metering_tables.py
+-rw-r--r--  2.0 unx      494 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/operations_tables.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/__init__.py
+-rw-r--r--  2.0 unx     5311 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/__init__.py
+-rw-r--r--  2.0 unx     1995 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/auxiliaryequipment_tables.py
+-rw-r--r--  2.0 unx     8442 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/core_tables.py
+-rw-r--r--  2.0 unx     3113 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/diagramlayout_tables.py
+-rw-r--r--  2.0 unx     2454 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py
+-rw-r--r--  2.0 unx     2581 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py
+-rw-r--r--  2.0 unx     7143 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/protection_tables.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/__init__.py
+-rw-r--r--  2.0 unx     1226 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/conductor_tables.py
+-rw-r--r--  2.0 unx      710 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/connector_tables.py
+-rw-r--r--  2.0 unx      458 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/container_tables.py
+-rw-r--r--  2.0 unx    17861 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/energyconnection_tables.py
+-rw-r--r--  2.0 unx     1845 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/perlength_tables.py
+-rw-r--r--  2.0 unx     2775 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py
+-rw-r--r--  2.0 unx     8640 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/transformer_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/__init__.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/production_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/__init__.py
+-rw-r--r--  2.0 unx     1515 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/feeder_tables.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/__init__.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/__init__.py
+-rw-r--r--  2.0 unx      454 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/production_tables.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/__init__.py
+-rw-r--r--  2.0 unx     5263 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/base_cim_writer.py
+-rw-r--r--  2.0 unx     2995 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/base_service_writer.py
+-rw-r--r--  2.0 unx     4752 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/customer_cim_writer.py
+-rw-r--r--  2.0 unx     1393 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/customer_service_writer.py
+-rw-r--r--  2.0 unx     2657 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/diagram_cim_writer.py
+-rw-r--r--  2.0 unx     1004 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/diagram_service_writer.py
+-rw-r--r--  2.0 unx      904 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/metadata_collection_writer.py
+-rw-r--r--  2.0 unx     1257 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/metadata_entry_writer.py
+-rw-r--r--  2.0 unx    86260 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/network_cim_writer.py
+-rw-r--r--  2.0 unx     9809 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/network_service_writer.py
+-rw-r--r--  2.0 unx     1430 b- defN 24-Mar-27 11:04 zepben/evolve/database/sqlite/writers/utils.py
+-rw-r--r--  2.0 unx      302 b- defN 24-Mar-27 11:04 zepben/evolve/examples/__init__.py
+-rw-r--r--  2.0 unx     5062 b- defN 24-Mar-27 11:04 zepben/evolve/examples/simple_test_network.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/__init__.py
+-rw-r--r--  2.0 unx     7357 b- defN 24-Mar-27 11:04 zepben/evolve/model/phases.py
+-rw-r--r--  2.0 unx     1502 b- defN 24-Mar-27 11:04 zepben/evolve/model/resistance_reactance.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/busbranch/__init__.py
+-rw-r--r--  2.0 unx    47076 b- defN 24-Mar-27 11:04 zepben/evolve/model/busbranch/bus_branch.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/__init__.py
+-rw-r--r--  2.0 unx     1398 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/no_load_test.py
+-rw-r--r--  2.0 unx     1445 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/open_circuit_test.py
+-rw-r--r--  2.0 unx     4220 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/power_transformer_info.py
+-rw-r--r--  2.0 unx     1877 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py
+-rw-r--r--  2.0 unx      927 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py
+-rw-r--r--  2.0 unx      550 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/switch_info.py
+-rw-r--r--  2.0 unx     5904 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py
+-rw-r--r--  2.0 unx     4395 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py
+-rw-r--r--  2.0 unx      860 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/wire_info.py
+-rw-r--r--  2.0 unx     1015 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assetinfo/wire_material_kind.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assets/__init__.py
+-rw-r--r--  2.0 unx     4019 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assets/asset.py
+-rw-r--r--  2.0 unx      845 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assets/asset_info.py
+-rw-r--r--  2.0 unx      588 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assets/asset_organisation_role.py
+-rw-r--r--  2.0 unx     3009 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assets/pole.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assets/streetlight.py
+-rw-r--r--  2.0 unx      635 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/assets/structure.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/common/__init__.py
+-rw-r--r--  2.0 unx     1570 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/common/document.py
+-rw-r--r--  2.0 unx     7841 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/common/location.py
+-rw-r--r--  2.0 unx      531 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/common/organisation.py
+-rw-r--r--  2.0 unx      838 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/common/organisation_role.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/customers/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/customers/customer.py
+-rw-r--r--  2.0 unx     4260 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/customers/customer_agreement.py
+-rw-r--r--  2.0 unx     1474 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/customers/customer_kind.py
+-rw-r--r--  2.0 unx     3336 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/customers/pricing_structure.py
+-rw-r--r--  2.0 unx      763 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/customers/tariff.py
+-rw-r--r--  2.0 unx      244 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/__init__.py
+-rw-r--r--  2.0 unx      244 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py
+-rw-r--r--  2.0 unx     1859 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py
+-rw-r--r--  2.0 unx     1250 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py
+-rw-r--r--  2.0 unx     4360 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/relay_info.py
+-rw-r--r--  2.0 unx      993 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py
+-rw-r--r--  2.0 unx     1098 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py
+-rw-r--r--  2.0 unx     1202 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/infiec61968/infcommon/ratio.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/metering/__init__.py
+-rw-r--r--  2.0 unx    11269 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/metering/metering.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/operations/__init__.py
+-rw-r--r--  2.0 unx     3889 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61968/operations/operational_restriction.py
+-rw-r--r--  2.0 unx      248 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/__init__.py
+-rw-r--r--  2.0 unx      249 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/__init__.py
+-rw-r--r--  2.0 unx     1475 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/auxiliary_equipment.py
+-rw-r--r--  2.0 unx     1489 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/current_transformer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer.py
+-rw-r--r--  2.0 unx      811 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer_kind.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/sensor.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/__init__.py
+-rw-r--r--  2.0 unx      556 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/base_voltage.py
+-rw-r--r--  2.0 unx     7135 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/conducting_equipment.py
+-rw-r--r--  2.0 unx     3645 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/connectivity_node.py
+-rw-r--r--  2.0 unx      592 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/connectivity_node_container.py
+-rw-r--r--  2.0 unx    14195 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/equipment.py
+-rw-r--r--  2.0 unx    15682 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/equipment_container.py
+-rw-r--r--  2.0 unx     8261 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/identified_object.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/name.py
+-rw-r--r--  2.0 unx     7475 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/name_type.py
+-rw-r--r--  2.0 unx     7033 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/phase_code.py
+-rw-r--r--  2.0 unx     1250 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/power_system_resource.py
+-rw-r--r--  2.0 unx     6734 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/regions.py
+-rw-r--r--  2.0 unx    10120 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/substation.py
+-rw-r--r--  2.0 unx     6717 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/core/terminal.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/diagramlayout/__init__.py
+-rw-r--r--  2.0 unx    10307 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_layout.py
+-rw-r--r--  2.0 unx      748 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_style.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/diagramlayout/orientation_kind.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/domain/__init__.py
+-rw-r--r--  2.0 unx    17065 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/domain/unit_symbol.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/equivalents/__init__.py
+-rw-r--r--  2.0 unx     5374 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_branch.py
+-rw-r--r--  2.0 unx      641 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_equipment.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/meas/__init__.py
+-rw-r--r--  2.0 unx      963 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/meas/control.py
+-rw-r--r--  2.0 unx      576 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/meas/iopoint.py
+-rw-r--r--  2.0 unx     4294 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/meas/measurement.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/meas/value.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/protection/__init__.py
+-rw-r--r--  2.0 unx      920 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/protection/current_relay.py
+-rw-r--r--  2.0 unx     2561 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/protection/distance_relay.py
+-rw-r--r--  2.0 unx    18678 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/protection/protection_relay_function.py
+-rw-r--r--  2.0 unx     4228 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/protection/protection_relay_scheme.py
+-rw-r--r--  2.0 unx     3848 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/protection/protection_relay_system.py
+-rw-r--r--  2.0 unx      963 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/protection/relay_setting.py
+-rw-r--r--  2.0 unx      696 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/protection/voltage_relay.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/scada/__init__.py
+-rw-r--r--  2.0 unx      737 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/scada/remote_control.py
+-rw-r--r--  2.0 unx      587 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/scada/remote_point.py
+-rw-r--r--  2.0 unx      734 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/scada/remote_source.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/__init__.py
+-rw-r--r--  2.0 unx     2433 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py
+-rw-r--r--  2.0 unx     1385 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/breaker.py
+-rw-r--r--  2.0 unx     1413 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/connectors.py
+-rw-r--r--  2.0 unx      672 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/disconnector.py
+-rw-r--r--  2.0 unx     1929 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py
+-rw-r--r--  2.0 unx     7483 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py
+-rw-r--r--  2.0 unx     6517 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/energy_source.py
+-rw-r--r--  2.0 unx     1977 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py
+-rw-r--r--  2.0 unx      831 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/fuse.py
+-rw-r--r--  2.0 unx      573 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/ground.py
+-rw-r--r--  2.0 unx      535 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/ground_disconnector.py
+-rw-r--r--  2.0 unx      611 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/jumper.py
+-rw-r--r--  2.0 unx      492 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/line.py
+-rw-r--r--  2.0 unx      584 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py
+-rw-r--r--  2.0 unx     1904 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/per_length.py
+-rw-r--r--  2.0 unx      884 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py
+-rw-r--r--  2.0 unx    24976 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py
+-rw-r--r--  2.0 unx    31160 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py
+-rw-r--r--  2.0 unx     4181 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/protected_switch.py
+-rw-r--r--  2.0 unx      582 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/recloser.py
+-rw-r--r--  2.0 unx     8338 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/regulating_control.py
+-rw-r--r--  2.0 unx     1168 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/regulating_control_mode_kind.py
+-rw-r--r--  2.0 unx     1635 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/series_compensator.py
+-rw-r--r--  2.0 unx     3658 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py
+-rw-r--r--  2.0 unx     4955 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/switch.py
+-rw-r--r--  2.0 unx     2112 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/tap_changer_control.py
+-rw-r--r--  2.0 unx     1045 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/transformer_cooling_type.py
+-rw-r--r--  2.0 unx     2219 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/transformer_star_impedance.py
+-rw-r--r--  2.0 unx     1544 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/vector_group.py
+-rw-r--r--  2.0 unx      786 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/winding_connection.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/generation/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/generation/production/__init__.py
+-rw-r--r--  2.0 unx      809 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/generation/production/battery_state_kind.py
+-rw-r--r--  2.0 unx     2215 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/base/wires/generation/production/power_electronics_unit.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/__init__.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/feeder/__init__.py
+-rw-r--r--  2.0 unx     5385 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/feeder/circuit.py
+-rw-r--r--  2.0 unx     7542 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py
+-rw-r--r--  2.0 unx     7636 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/protection/__init__.py
+-rw-r--r--  2.0 unx      746 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/protection/power_direction_kind.py
+-rw-r--r--  2.0 unx     2711 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/protection/protection_kind.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/wires/__init__.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/__init__.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/__init__.py
+-rw-r--r--  2.0 unx      426 b- defN 24-Mar-27 11:04 zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/ev_charging_unit.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/__init__.py
+-rw-r--r--  2.0 unx      960 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/__init__.py
+-rw-r--r--  2.0 unx    18023 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/base_service.py
+-rw-r--r--  2.0 unx    16620 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/base_service_comparator.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/difference.py
+-rw-r--r--  2.0 unx    24212 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/reference_resolvers.py
+-rw-r--r--  2.0 unx    22825 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/resolver.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/meta/__init__.py
+-rw-r--r--  2.0 unx      461 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/meta/data_source.py
+-rw-r--r--  2.0 unx      804 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/meta/metadata_collection.py
+-rw-r--r--  2.0 unx     1481 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/meta/metadata_translations.py
+-rw-r--r--  2.0 unx      601 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/meta/service_info.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/translator/__init__.py
+-rw-r--r--  2.0 unx     3420 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/translator/base_cim2proto.py
+-rw-r--r--  2.0 unx     3938 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/translator/base_proto2cim.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/translator/service_differences.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-Mar-27 11:04 zepben/evolve/services/common/translator/util.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/customer/__init__.py
+-rw-r--r--  2.0 unx     1922 b- defN 24-Mar-27 11:04 zepben/evolve/services/customer/customer_service_comparator.py
+-rw-r--r--  2.0 unx      467 b- defN 24-Mar-27 11:04 zepben/evolve/services/customer/customers.py
+-rw-r--r--  2.0 unx     1044 b- defN 24-Mar-27 11:04 zepben/evolve/services/customer/translator/__init__.py
+-rw-r--r--  2.0 unx     2760 b- defN 24-Mar-27 11:04 zepben/evolve/services/customer/translator/customer_cim2proto.py
+-rw-r--r--  2.0 unx     3379 b- defN 24-Mar-27 11:04 zepben/evolve/services/customer/translator/customer_proto2cim.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/diagram/__init__.py
+-rw-r--r--  2.0 unx     1486 b- defN 24-Mar-27 11:04 zepben/evolve/services/diagram/diagram_service_comparator.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-Mar-27 11:04 zepben/evolve/services/diagram/diagrams.py
+-rw-r--r--  2.0 unx      508 b- defN 24-Mar-27 11:04 zepben/evolve/services/diagram/translator/__init__.py
+-rw-r--r--  2.0 unx     2237 b- defN 24-Mar-27 11:04 zepben/evolve/services/diagram/translator/diagram_cim2proto.py
+-rw-r--r--  2.0 unx     2463 b- defN 24-Mar-27 11:04 zepben/evolve/services/diagram/translator/diagram_proto2cim.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/measurement/__init__.py
+-rw-r--r--  2.0 unx     1207 b- defN 24-Mar-27 11:04 zepben/evolve/services/measurement/measurements.py
+-rw-r--r--  2.0 unx      261 b- defN 24-Mar-27 11:04 zepben/evolve/services/measurement/translator/__init__.py
+-rw-r--r--  2.0 unx     1832 b- defN 24-Mar-27 11:04 zepben/evolve/services/measurement/translator/measurement_cim2proto.py
+-rw-r--r--  2.0 unx     1951 b- defN 24-Mar-27 11:04 zepben/evolve/services/measurement/translator/measurement_proto2cim.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/__init__.py
+-rw-r--r--  2.0 unx     6279 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/network_extensions.py
+-rw-r--r--  2.0 unx    10634 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/network_service.py
+-rw-r--r--  2.0 unx    46822 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/network_service_comparator.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/__init__.py
+-rw-r--r--  2.0 unx     3654 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/find.py
+-rw-r--r--  2.0 unx     5623 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/find_swer_equipment.py
+-rw-r--r--  2.0 unx    16173 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/tracing.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/util.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/__init__.py
+-rw-r--r--  2.0 unx      775 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step.py
+-rw-r--r--  2.0 unx     2394 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step_tracker.py
+-rw-r--r--  2.0 unx     8474 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/connected_equipment_trace.py
+-rw-r--r--  2.0 unx     1162 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/connected_equipment_traversal.py
+-rw-r--r--  2.0 unx     4223 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/connectivity_result.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/connectivity_trace.py
+-rw-r--r--  2.0 unx     1212 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/connectivity_tracker.py
+-rw-r--r--  2.0 unx     5162 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/limited_connected_equipment_trace.py
+-rw-r--r--  2.0 unx     3872 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/phase_paths.py
+-rw-r--r--  2.0 unx     9998 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_connected.py
+-rw-r--r--  2.0 unx     2862 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_internal.py
+-rw-r--r--  2.0 unx    11472 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/transformer_phase_paths.py
+-rw-r--r--  2.0 unx    10412 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/xy_candidate_phase_paths.py
+-rw-r--r--  2.0 unx      583 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/connectivity/xy_phase_step.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/__init__.py
+-rw-r--r--  2.0 unx     5997 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py
+-rw-r--r--  2.0 unx     3246 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/associated_terminal_trace.py
+-rw-r--r--  2.0 unx     1477 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/associated_terminal_tracker.py
+-rw-r--r--  2.0 unx     3990 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/direction_status.py
+-rw-r--r--  2.0 unx     2546 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/feeder_direction.py
+-rw-r--r--  2.0 unx     7410 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/remove_direction.py
+-rw-r--r--  2.0 unx     6757 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/feeder/set_direction.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/phases/__init__.py
+-rw-r--r--  2.0 unx    10311 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/phases/phase_inferrer.py
+-rw-r--r--  2.0 unx     3428 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/phases/phase_status.py
+-rw-r--r--  2.0 unx     2628 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/phases/phase_step.py
+-rw-r--r--  2.0 unx     2014 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/phases/phase_step_tracker.py
+-rw-r--r--  2.0 unx     6251 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/phases/phase_trace.py
+-rw-r--r--  2.0 unx     5510 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/phases/remove_phases.py
+-rw-r--r--  2.0 unx    12798 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/phases/set_phases.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/traversals/__init__.py
+-rw-r--r--  2.0 unx     1642 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/traversals/basic_tracker.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/traversals/basic_traversal.py
+-rw-r--r--  2.0 unx     6585 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/traversals/branch_recursive_tracing.py
+-rw-r--r--  2.0 unx     5164 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/traversals/queue.py
+-rw-r--r--  2.0 unx     1775 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/traversals/tracker.py
+-rw-r--r--  2.0 unx     8650 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/traversals/traversal.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/tree/__init__.py
+-rw-r--r--  2.0 unx     4454 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/tree/downstream_tree.py
+-rw-r--r--  2.0 unx     1780 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/tree/tree_node.py
+-rw-r--r--  2.0 unx     1167 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/tracing/tree/tree_node_tracker.py
+-rw-r--r--  2.0 unx    23636 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/translator/__init__.py
+-rw-r--r--  2.0 unx    70246 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/translator/network_cim2proto.py
+-rw-r--r--  2.0 unx    84542 b- defN 24-Mar-27 11:04 zepben/evolve/services/network/translator/network_proto2cim.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/__init__.py
+-rw-r--r--  2.0 unx      427 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/exceptions.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/get/__init__.py
+-rw-r--r--  2.0 unx     9348 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/get/consumer.py
+-rw-r--r--  2.0 unx     5425 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/get/customer_consumer.py
+-rw-r--r--  2.0 unx     5032 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/get/diagram_consumer.py
+-rw-r--r--  2.0 unx    38507 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/get/network_consumer.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/get/hierarchy/__init__.py
+-rw-r--r--  2.0 unx     1047 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/get/hierarchy/data.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/grpc/__init__.py
+-rw-r--r--  2.0 unx      801 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/grpc/auth_token_plugin.py
+-rw-r--r--  2.0 unx     9451 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/grpc/connect.py
+-rw-r--r--  2.0 unx     4020 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/grpc/grpc.py
+-rw-r--r--  2.0 unx     7664 b- defN 24-Mar-27 11:04 zepben/evolve/streaming/grpc/grpc_channel_builder.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Mar-27 11:04 zepben/evolve/testing/__init__.py
+-rw-r--r--  2.0 unx    28552 b- defN 24-Mar-27 11:04 zepben/evolve/testing/test_network_builder.py
+-rw-r--r--  2.0 unx     3238 b- defN 24-Mar-27 11:04 zepben/evolve/testing/test_traversal.py
+-rw-r--r--  2.0 unx    16725 b- defN 24-Mar-27 11:08 zepben.evolve-0.38.0b8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2301 b- defN 24-Mar-27 11:08 zepben.evolve-0.38.0b8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 11:08 zepben.evolve-0.38.0b8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Mar-27 11:08 zepben.evolve-0.38.0b8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    40147 b- defN 24-Mar-27 11:08 zepben.evolve-0.38.0b8.dist-info/RECORD
+342 files, 1656602 bytes uncompressed, 389094 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -93,15 +93,21 @@
 
 Filename: zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py
 Comment: 
 
-Filename: zepben/evolve/database/sqlite/tables/associations/protection_equipment_protected_switches.py
+Filename: zepben/evolve/database/sqlite/tables/associations/protection_relay_functions_protected_switches.py
+Comment: 
+
+Filename: zepben/evolve/database/sqlite/tables/associations/protection_relay_functions_sensors.py
+Comment: 
+
+Filename: zepben/evolve/database/sqlite/tables/associations/protection_relay_schemes_protection_relay_functions.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py
 Comment: 
 
 Filename: zepben/evolve/database/sqlite/tables/iec61968/__init__.py
 Comment: 
@@ -357,23 +363,23 @@
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/__init__.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py
 Comment: 
 
-Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_relay_info.py
-Comment: 
-
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/relay_info.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py
@@ -507,15 +513,30 @@
 
 Filename: zepben/evolve/model/cim/iec61970/base/protection/__init__.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/protection/current_relay.py
 Comment: 
 
-Filename: zepben/evolve/model/cim/iec61970/base/protection/protection_equipment.py
+Filename: zepben/evolve/model/cim/iec61970/base/protection/distance_relay.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/protection/protection_relay_function.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/protection/protection_relay_scheme.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/protection/protection_relay_system.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/protection/relay_setting.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/protection/voltage_relay.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/scada/__init__.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/scada/remote_control.py
 Comment: 
@@ -552,14 +573,20 @@
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/fuse.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/base/wires/ground.py
+Comment: 
+
+Filename: zepben/evolve/model/cim/iec61970/base/wires/ground_disconnector.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61970/base/wires/jumper.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/line.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py
@@ -585,14 +612,17 @@
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/regulating_control.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/regulating_control_mode_kind.py
 Comment: 
 
+Filename: zepben/evolve/model/cim/iec61970/base/wires/series_compensator.py
+Comment: 
+
 Filename: zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py
 Comment: 
 
 Filename: zepben/evolve/model/cim/iec61970/base/wires/switch.py
@@ -975,23 +1005,23 @@
 
 Filename: zepben/evolve/testing/test_network_builder.py
 Comment: 
 
 Filename: zepben/evolve/testing/test_traversal.py
 Comment: 
 
-Filename: zepben.evolve-0.38.0b7.dist-info/LICENSE
+Filename: zepben.evolve-0.38.0b8.dist-info/LICENSE
 Comment: 
 
-Filename: zepben.evolve-0.38.0b7.dist-info/METADATA
+Filename: zepben.evolve-0.38.0b8.dist-info/METADATA
 Comment: 
 
-Filename: zepben.evolve-0.38.0b7.dist-info/WHEEL
+Filename: zepben.evolve-0.38.0b8.dist-info/WHEEL
 Comment: 
 
-Filename: zepben.evolve-0.38.0b7.dist-info/top_level.txt
+Filename: zepben.evolve-0.38.0b8.dist-info/top_level.txt
 Comment: 
 
-Filename: zepben.evolve-0.38.0b7.dist-info/RECORD
+Filename: zepben.evolve-0.38.0b8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zepben/evolve/__init__.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 # We need to import SinglePhaseKind before anything uses PhaseCode to prevent cyclic dependencies.
 from zepben.evolve.model.cim.iec61970.base.wires.single_phase_kind import *
@@ -26,15 +26,15 @@
 from zepben.evolve.model.cim.iec61968.assetinfo.no_load_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.open_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.short_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.shunt_compensator_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.switch_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_end_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_tank_info import *
-from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import *
+from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.relay_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.potential_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.transformer_construction_kind import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.transformer_function_kind import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infcommon.ratio import *
 from zepben.evolve.model.cim.iec61968.metering.metering import *
 from zepben.evolve.model.cim.iec61968.common.organisation import *
@@ -55,24 +55,32 @@
 from zepben.evolve.model.cim.iec61970.base.diagramlayout.orientation_kind import *
 from zepben.evolve.model.cim.iec61970.base.diagramlayout.diagram_style import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_point import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_source import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_control import *
 from zepben.evolve.model.cim.iec61970.base.domain.unit_symbol import *
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.auxiliary_equipment import *
-from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_function import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_scheme import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_system import *
 from zepben.evolve.model.cim.iec61970.base.protection.current_relay import *
+from zepben.evolve.model.cim.iec61970.base.protection.distance_relay import *
+from zepben.evolve.model.cim.iec61970.base.protection.voltage_relay import *
+from zepben.evolve.model.cim.iec61970.base.protection.relay_setting import *
+from zepben.evolve.model.cim.iec61970.base.wires.ground import *
+from zepben.evolve.model.cim.iec61970.base.wires.ground_disconnector import *
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.power_electronics_unit import *
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.battery_state_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.line import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import *
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import *
 from zepben.evolve.model.cim.iec61970.base.wires.per_length import *
 from zepben.evolve.model.cim.iec61970.base.wires.vector_group import *
 from zepben.evolve.model.cim.iec61970.base.wires.winding_connection import *
+from zepben.evolve.model.cim.iec61970.base.wires.series_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.shunt_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source_phase import *
 from zepben.evolve.model.cim.iec61970.base.wires.phase_shunt_connection_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.connectors import *
 from zepben.evolve.model.cim.iec61970.base.wires.switch import *
@@ -211,15 +219,17 @@
 from zepben.evolve.database.sqlite.tables.associations.loop_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.circuit_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.customeragreements_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.equipment_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.usagepoints_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.assetorganisationroles_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.pricingstructure_association_tables import *
-from zepben.evolve.database.sqlite.tables.associations.protection_equipment_protected_switches import *
+from zepben.evolve.database.sqlite.tables.associations.protection_relay_functions_protected_switches import *
+from zepben.evolve.database.sqlite.tables.associations.protection_relay_functions_sensors import *
+from zepben.evolve.database.sqlite.tables.associations.protection_relay_schemes_protection_relay_functions import *
 from zepben.evolve.database.sqlite.tables.iec61968.common_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.asset_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.customer_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.infiec61968.infassetinfo_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.metering_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.assetinfo_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.operations_tables import *
```

## zepben/evolve/exceptions.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 
 class MissingReferenceException(Exception):
```

## zepben/evolve/types.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Callable, Optional, TypeVar
```

## zepben/evolve/util.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/database/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/database_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import logging
 import sqlite3
 from sqlite3 import Connection, Cursor
```

## zepben/evolve/database/sqlite/database_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import logging
 import os
 import sqlite3
```

## zepben/evolve/database/sqlite/readers/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/readers/base_cim_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import logging
 from typing import Callable, Optional, Type, TypeVar
```

## zepben/evolve/database/sqlite/readers/base_service_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import logging
 from sqlite3 import Cursor
 from typing import Callable, Type, TypeVar
```

## zepben/evolve/database/sqlite/readers/customer_cim_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Callable
 
 from zepben.evolve import BaseCIMReader, CustomerService, Agreement, TableAgreements, ResultSet, TableCustomers, Customer, CustomerKind, \
```

## zepben/evolve/database/sqlite/readers/customer_service_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import BaseServiceReader, TableOrganisations, TableCustomers, TableCustomerAgreements, TablePricingStructures, TableTariffs, \
     TableCustomerAgreementsPricingStructures, TablePricingStructuresTariffs, CustomerCIMReader
```

## zepben/evolve/database/sqlite/readers/diagram_cim_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Callable
 
 from zepben.evolve import BaseCIMReader, TableDiagrams, ResultSet, Diagram, DiagramStyle, OrientationKind, TableDiagramObjects, DiagramObject, \
```

## zepben/evolve/database/sqlite/readers/diagram_service_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from zepben.evolve import BaseServiceReader, TableDiagrams, TableDiagramObjects, TableDiagramObjectPoints, DiagramCIMReader
 
 __all__ = ["DiagramServiceReader"]
```

## zepben/evolve/database/sqlite/readers/metadata_collection_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import BaseServiceReader, MetadataEntryReader, TableMetadataDataSources
```

## zepben/evolve/database/sqlite/readers/metadata_entry_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import datetime
 from typing import Callable
```

## zepben/evolve/database/sqlite/readers/network_cim_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 # 
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from datetime import datetime
 from typing import Callable, Optional
 
@@ -32,18 +32,23 @@
     TablePowerTransformers, PowerTransformer, VectorGroup, TablePowerTransformerEnds, PowerTransformerEnd, ProtectedSwitch, TableProtectedSwitches, \
     TableRatioTapChangers, RatioTapChanger, TransformerEnd, TableReclosers, Recloser, RegulatingCondEq, TableRegulatingCondEq, ShuntCompensator, \
     TableShuntCompensators, Switch, TableSwitches, TapChanger, TableTapChangers, TableTransformerEnds, TransformerStarImpedance, \
     TableTransformerStarImpedance, TableCircuits, Circuit, Loop, TableLoops, TableAssetOrganisationRolesAssets, TableEquipmentEquipmentContainers, \
     TableEquipmentOperationalRestrictions, TableEquipmentUsagePoints, TableUsagePointsEndDevices, TableCircuitsSubstations, TableCircuitsTerminals, \
     TablePotentialTransformers, PotentialTransformer, PotentialTransformerKind, PotentialTransformerInfo, Sensor, TableSensors, TableCurrentTransformers, \
     CurrentTransformer, CurrentTransformerInfo, TableCurrentTransformerInfo, TablePotentialTransformerInfo, TableLoopsSubstations, LoopSubstationRelationship, \
-    LvFeeder, TableLvFeeders, CurrentRelayInfo, TableCurrentRelayInfo, SwitchInfo, TableSwitchInfo, ProtectionEquipment, TableProtectionEquipment, \
-    ProtectionKind, PowerDirectionKind, TableCurrentRelays, CurrentRelay, TableProtectionEquipmentProtectedSwitches, TableRecloseDelays, TableEvChargingUnits, \
-    EvChargingUnit, RegulatingControl, TableRegulatingControls, RegulatingControlModeKind, TapChangerControl, TableTapChangerControls, \
-    TablePowerTransformerEndRatings, TransformerCoolingType, TransformerEndRatedS
+    LvFeeder, TableLvFeeders, RelayInfo, TableRelayInfo, SwitchInfo, TableSwitchInfo, TableProtectionRelayFunctions, \
+    ProtectionKind, PowerDirectionKind, TableCurrentRelays, CurrentRelay, TableProtectionRelayFunctionsProtectedSwitches, TableRecloseDelays, \
+    TableEvChargingUnits, EvChargingUnit, RegulatingControl, TableRegulatingControls, RegulatingControlModeKind, TapChangerControl, TableTapChangerControls, \
+    TablePowerTransformerEndRatings, TransformerCoolingType, TableProtectionRelayFunctionThresholds, TableDistanceRelays, \
+    TableVoltageRelays, TableProtectionRelayFunctionTimeLimits, TableProtectionRelaySystems, TableProtectionRelaySchemes, TableGrounds, \
+    TableGroundDisconnectors, TableSeriesCompensators, TableProtectionRelayFunctionsSensors, TableProtectionRelaySchemesProtectionRelayFunctions, \
+    ProtectionRelayScheme, ProtectionRelaySystem, RelaySetting, DistanceRelay, ProtectionRelayFunction, VoltageRelay, Ground, GroundDisconnector, \
+    SeriesCompensator
+
 from zepben.evolve.services.common.resolver import rce_regulating_control
 
 __all__ = ["NetworkCIMReader"]
 
 
 class NetworkCIMReader(BaseCIMReader):
 
@@ -279,20 +284,21 @@
             rs.get_string(table.state_or_province.query_index, "")
         )
 
         return None if town_detail.all_fields_null_or_empty() else town_detail
 
     # ************ IEC61968 infIEC61968 InfAssetInfo ************
 
-    def load_current_relay_info(self, table: TableCurrentRelayInfo, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
-        current_relay_info = CurrentRelayInfo(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+    def load_relay_info(self, table: TableRelayInfo, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        relay_info = RelayInfo(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
-        current_relay_info.curve_setting = rs.get_string(table.curve_setting.query_index, None)
+        relay_info.curve_setting = rs.get_string(table.curve_setting.query_index, None)
+        relay_info.reclose_fast = rs.get_boolean(table.reclose_fast.query_index, None)
 
-        return self._load_asset_info(current_relay_info, table, rs) and self._add_or_throw(current_relay_info)
+        return self._load_asset_info(relay_info, table, rs) and self._add_or_throw(relay_info)
 
     def load_current_transformer_info(self, table: TableCurrentTransformerInfo, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         current_transformer_info = CurrentTransformerInfo(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         current_transformer_info.accuracy_class = rs.get_string(table.accuracy_class.query_index, None)
         current_transformer_info.accuracy_limit = rs.get_double(table.accuracy_limit.query_index, None)
         current_transformer_info.core_count = rs.get_int(table.core_count.query_index, None)
@@ -318,19 +324,19 @@
         potential_transformer_info.rated_voltage = rs.get_int(table.rated_voltage.query_index, None)
         potential_transformer_info.secondary_ratio = rs.get_double(table.secondary_ratio.query_index, None)
 
         return self._load_asset_info(potential_transformer_info, table, rs) and self._add_or_throw(potential_transformer_info)
 
     def load_reclose_delays(self, table: TableRecloseDelays, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         # Note TableRecloseDelays.selectSql ensures we process ratings in the correct order.
-        current_relay_info_mrid = rs.get_string(table.current_relay_info_mrid.query_index)
+        relay_info_mrid = rs.get_string(table.relay_info_mrid.query_index)
         reclose_delay = rs.get_double(table.reclose_delay.query_index)
-        set_last_mrid(f"{current_relay_info_mrid}.s{reclose_delay}")
-        cri = self._ensure_get(current_relay_info_mrid, CurrentRelayInfo)
-        cri.add_delay(reclose_delay)
+        set_last_mrid(f"{relay_info_mrid}.s{reclose_delay}")
+        ri = self._ensure_get(relay_info_mrid, RelayInfo)
+        ri.add_delay(reclose_delay)
 
         return True
 
     # ************ IEC61968 METERING ************
 
     def _load_end_device(self, end_device: EndDevice, table: TableEndDevices, rs: ResultSet) -> bool:
         end_device.customer_mrid = rs.get_string(table.customer_mrid.query_index, None)
@@ -567,25 +573,94 @@
 
     def load_current_relay(self, table: TableCurrentRelays, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         current_relay = CurrentRelay(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         current_relay.current_limit_1 = rs.get_double(table.current_limit_1.query_index, None)
         current_relay.inverse_time_flag = rs.get_boolean(table.inverse_time_flag.query_index, None)
         current_relay.time_delay_1 = rs.get_double(table.time_delay_1.query_index, None)
-        current_relay.asset_info = self._ensure_get(rs.get_string(table.current_relay_info_mrid.query_index, None), WireInfo)
 
-        return self._load_protection_equipment(current_relay, table, rs) and self._add_or_throw(current_relay)
+        return self._load_protection_relay_function(current_relay, table, rs) and self._add_or_throw(current_relay)
+
+    def load_distance_relay(self, table: TableDistanceRelays, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        distance_relay = DistanceRelay(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+
+        distance_relay.backward_blind = rs.get_double(table.backward_blind.query_index, None)
+        distance_relay.backward_reach = rs.get_double(table.backward_reach.query_index, None)
+        distance_relay.backward_reactance = rs.get_double(table.backward_reactance.query_index, None)
+        distance_relay.forward_blind = rs.get_double(table.forward_blind.query_index, None)
+        distance_relay.forward_reach = rs.get_double(table.forward_reach.query_index, None)
+        distance_relay.forward_reactance = rs.get_double(table.forward_reactance.query_index, None)
+        distance_relay.operation_phase_angle1 = rs.get_double(table.operation_phase_angle1.query_index, None)
+        distance_relay.operation_phase_angle2 = rs.get_double(table.operation_phase_angle2.query_index, None)
+        distance_relay.operation_phase_angle3 = rs.get_double(table.operation_phase_angle3.query_index, None)
+
+        return self._load_protection_relay_function(distance_relay, table, rs) and self._add_or_throw(distance_relay)
+
+    def _load_protection_relay_function(self, protection_relay_function: ProtectionRelayFunction, table: TableProtectionRelayFunctions, rs: ResultSet) -> bool:
+        protection_relay_function.asset_info = self._ensure_get(rs.get_string(table.relay_info_mrid.query_index, None), RelayInfo)
+        protection_relay_function.model = rs.get_string(table.model.query_index, None)
+        protection_relay_function.reclosing = rs.get_boolean(table.reclosing.query_index, None)
+        protection_relay_function.relay_delay_time = rs.get_double(table.relay_delay_time.query_index, None)
+        protection_relay_function.protection_kind = ProtectionKind[rs.get_string(table.protection_kind.query_index)]
+        protection_relay_function.directable = rs.get_boolean(table.directable.query_index, None)
+        protection_relay_function.power_direction = PowerDirectionKind[rs.get_string(table.power_direction.query_index)]
+
+        return self._load_power_system_resource(protection_relay_function, table, rs)
+
+    def load_protection_relay_function_thresholds(self, table: TableProtectionRelayFunctionThresholds, rs: ResultSet,
+                                                  set_last_mrid: Callable[[str], str]) -> bool:
+        protection_relay_function_mrid = rs.get_string(table.protection_relay_function_mrid.query_index)
+
+        protection_relay_function = self._ensure_get(protection_relay_function_mrid, ProtectionRelayFunction)
+
+        sequence_number = rs.get_int(table.sequence_number.query_index)
+        unit_symbol = UnitSymbol[rs.get_string(table.unit_symbol.query_index)]
+        value = rs.get_double(table.value.query_index)
+        name = rs.get_string(table.name_.query_index, None)
+
+        set_last_mrid(f"{protection_relay_function_mrid}.s{sequence_number}")
+
+        new_relay_setting = RelaySetting(unit_symbol, value, name)
+
+        protection_relay_function.add_threshold(new_relay_setting, sequence_number)
+
+        return True
+
+    def load_protection_relay_function_time_limits(self, table: TableProtectionRelayFunctionTimeLimits, rs: ResultSet,
+                                                   set_last_mrid: Callable[[str], str]) -> bool:
+        protection_relay_function_mrid = rs.get_string(table.protection_relay_function_mrid.query_index)
+
+        protection_relay_function = self._ensure_get(protection_relay_function_mrid, ProtectionRelayFunction)
+
+        sequence_number = rs.get_int(table.sequence_number.query_index)
+        time_limit = rs.get_double(table.time_limit.query_index)
+
+        set_last_mrid(f"{protection_relay_function_mrid} time limit {sequence_number}")
+
+        protection_relay_function.add_time_limit(time_limit, sequence_number)
+
+        return True
+
+    def load_protection_relay_scheme(self, table: TableProtectionRelaySchemes, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        protection_relay_scheme = ProtectionRelayScheme(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+        protection_relay_scheme.system = self._ensure_get(rs.get_string(table.system_mrid.query_index, None), ProtectionRelaySystem)
+        if protection_relay_scheme.system is not None:
+            protection_relay_scheme.system.add_scheme(protection_relay_scheme)
+        return self._load_identified_object(protection_relay_scheme, table, rs) and self._add_or_throw(protection_relay_scheme)
+
+    def load_protection_relay_system(self, table: TableProtectionRelaySystems, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        protection_relay_system = ProtectionRelaySystem(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+        protection_relay_system.protection_kind = ProtectionKind[rs.get_string(table.protection_kind.query_index)]
+
+        return self._load_equipment(protection_relay_system, table, rs) and self._add_or_throw(protection_relay_system)
 
-    def _load_protection_equipment(self, protection_equipment: ProtectionEquipment, table: TableProtectionEquipment, rs: ResultSet) -> bool:
-        protection_equipment.relay_delay_time = rs.get_double(table.relay_delay_time.query_index, None)
-        protection_equipment.protection_kind = ProtectionKind[rs.get_string(table.protection_kind.query_index)]
-        protection_equipment.directable = rs.get_boolean(table.directable.query_index, None)
-        protection_equipment.power_direction = PowerDirectionKind[rs.get_string(table.power_direction.query_index)]
+    def load_voltage_relay(self, table: TableVoltageRelays, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        voltage_relay = VoltageRelay(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
-        return self._load_equipment(protection_equipment, table, rs)
+        return self._load_protection_relay_function(voltage_relay, table, rs) and self._add_or_throw(voltage_relay)
 
     # ************ IEC61970 BASE SCADA ************
 
     def load_remote_control(self, table: TableRemoteControls, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         remote_control = RemoteControl(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         remote_control.control = self._ensure_get(rs.get_string(table.control_mrid.query_index, None), Control)
@@ -750,17 +825,28 @@
 
         energy_source_phase.phase = SinglePhaseKind[rs.get_string(table.phase.query_index)]
 
         return self._load_power_system_resource(energy_source_phase, table, rs) and self._add_or_throw(energy_source_phase)
 
     def load_fuse(self, table: TableFuses, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         fuse = Fuse(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+        fuse.function = self._ensure_get(rs.get_string(table.function_mrid.query_index, None), ProtectionRelayFunction)
 
         return self._load_switch(fuse, table, rs) and self._add_or_throw(fuse)
 
+    def load_ground(self, table: TableGrounds, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        ground = Ground(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+
+        return self._load_conducting_equipment(ground, table, rs) and self._add_or_throw(ground)
+
+    def load_ground_disconnector(self, table: TableGroundDisconnectors, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        ground_disconnector = GroundDisconnector(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+
+        return self._load_switch(ground_disconnector, table, rs) and self._add_or_throw(ground_disconnector)
+
     def load_jumper(self, table: TableJumpers, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         jumper = Jumper(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
 
         return self._load_switch(jumper, table, rs) and self._add_or_throw(jumper)
 
     def load_junction(self, table: TableJunctions, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
         junction = Junction(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
@@ -931,18 +1017,31 @@
         regulating_control.mode = RegulatingControlModeKind[rs.get_string(table.mode.query_index)]
         regulating_control.monitored_phase = PhaseCode[rs.get_string(table.monitored_phase.query_index)]
         regulating_control.target_deadband = rs.get_double(table.target_deadband.query_index, None)
         regulating_control.target_value = rs.get_double(table.target_value.query_index, None)
         regulating_control.enabled = rs.get_boolean(table.enabled.query_index, None)
         regulating_control.max_allowed_target_value = rs.get_double(table.max_allowed_target_value.query_index, None)
         regulating_control.min_allowed_target_value = rs.get_double(table.min_allowed_target_value.query_index, None)
+        regulating_control.rated_current = rs.get_double(table.rated_current.query_index, None)
         regulating_control.terminal = self._ensure_get(rs.get_string(table.terminal_mrid.query_index, None), Terminal)
 
         return self._load_power_system_resource(regulating_control, table, rs)
 
+    def load_series_compensator(self, table: TableSeriesCompensators, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        series_compensator = SeriesCompensator(mrid=set_last_mrid(rs.get_string(table.mrid.query_index)))
+
+        series_compensator.r = rs.get_double(table.r.query_index, None)
+        series_compensator.r0 = rs.get_double(table.r0.query_index, None)
+        series_compensator.x = rs.get_double(table.x.query_index, None)
+        series_compensator.x0 = rs.get_double(table.x0.query_index, None)
+        series_compensator.varistor_rated_current = rs.get_int(table.varistor_rated_current.query_index, None)
+        series_compensator.varistor_voltage_threshold = rs.get_int(table.varistor_voltage_threshold.query_index, None)
+
+        return self._load_conducting_equipment(series_compensator, table, rs) and self._add_or_throw(series_compensator)
+
     def _load_shunt_compensator(self, shunt_compensator: ShuntCompensator, table: TableShuntCompensators, rs: ResultSet) -> bool:
         shunt_compensator.asset_info = self._ensure_get(rs.get_string(table.shunt_compensator_info_mrid.query_index, None), ShuntCompensatorInfo)
 
         shunt_compensator.grounded = rs.get_boolean(table.grounded.query_index)
         shunt_compensator.nom_u = rs.get_int(table.nom_u.query_index, None)
         shunt_compensator.phase_connection = PhaseShuntConnectionKind[rs.get_string(table.phase_connection.query_index)]
         shunt_compensator.sections = rs.get_double(table.sections.query_index, None)
@@ -1159,22 +1258,49 @@
             loop.add_substation(substation)
         elif relationship == LoopSubstationRelationship.SUBSTATION_ENERGIZES_LOOP:
             substation.add_energized_loop(loop)
             loop.add_energizing_substation(substation)
 
         return True
 
-    def load_protection_equipment_protected_switch(self, table: TableProtectionEquipmentProtectedSwitches, rs: ResultSet,
+    def load_protection_equipment_protected_switch(self, table: TableProtectionRelayFunctionsProtectedSwitches, rs: ResultSet,
                                                    set_last_mrid: Callable[[str], str]) -> bool:
-        protection_equipment_mrid = set_last_mrid(rs.get_string(table.protection_equipment_mrid.query_index))
-        set_last_mrid(f"{protection_equipment_mrid}-to-UNKNOWN")
+        protection_relay_function_mrid = rs.get_string(table.protection_relay_function_mrid.query_index)
+        set_last_mrid(f"{protection_relay_function_mrid}-to-UNKNOWN")
 
         protected_switch_mrid = rs.get_string(table.protected_switch_mrid.query_index)
-        set_last_mrid(f"{protection_equipment_mrid}-to-{protected_switch_mrid}")
+        set_last_mrid(f"{protection_relay_function_mrid}-to-{protected_switch_mrid}")
 
-        protection_equipment = self._base_service.get(protection_equipment_mrid, ProtectionEquipment)
+        protection_relay_function = self._base_service.get(protection_relay_function_mrid, ProtectionRelayFunction)
         protected_switch = self._base_service.get(protected_switch_mrid, ProtectedSwitch)
 
-        protection_equipment.add_protected_switch(protected_switch)
-        protected_switch.add_operated_by_protection_equipment(protection_equipment)
+        protection_relay_function.add_protected_switch(protected_switch)
+        protected_switch.add_relay_function(protection_relay_function)
+        return True
+
+    def load_protection_relay_functions_sensors(self, table: TableProtectionRelayFunctionsSensors, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        protection_relay_function_mrid = rs.get_string(table.protection_relay_function_mrid.query_index)
+        set_last_mrid(f"{protection_relay_function_mrid}-to-UNKNOWN")
+
+        sensor_mrid = rs.get_string(table.sensor_mrid.query_index)
+        set_last_mrid(f"{protection_relay_function_mrid}-to-{sensor_mrid}")
+
+        protection_relay_function = self._base_service.get(protection_relay_function_mrid, ProtectionRelayFunction)
+        sensor = self._base_service.get(sensor_mrid, Sensor)
+
+        protection_relay_function.add_sensor(sensor)
+        sensor.add_relay_function(protection_relay_function)  # I feel like there was a resolver for this somewhere? oh maybe for pb
+        return True
+
+    def load_protection_relay_schemes_protection_relay_functions(self, table: TableProtectionRelaySchemesProtectionRelayFunctions, rs: ResultSet, set_last_mrid: Callable[[str], str]) -> bool:
+        protection_relay_scheme_mrid = rs.get_string(table.protection_relay_scheme_mrid.query_index)
+        set_last_mrid(f"{protection_relay_scheme_mrid}-to-UNKNOWN")
+
+        protection_relay_function_mrid = rs.get_string(table.protection_relay_function_mrid.query_index)
+        set_last_mrid(f"{protection_relay_scheme_mrid}-to-{protection_relay_function_mrid}")
+
+        protection_relay_scheme = self._base_service.get(protection_relay_scheme_mrid, ProtectionRelayScheme)
+        protection_relay_function = self._base_service.get(protection_relay_function_mrid, ProtectionRelayFunction)
 
+        protection_relay_scheme.add_function(protection_relay_function)
+        protection_relay_function.add_scheme(protection_relay_scheme)
         return True
```

## zepben/evolve/database/sqlite/readers/network_service_reader.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import BaseServiceReader, TableCableInfo, TableOverheadWireInfo, TablePowerTransformerInfo, TableTransformerTankInfo, TableNoLoadTests, \
     TableOpenCircuitTests, TableShortCircuitTests, TableShuntCompensatorInfo, TableTransformerEndInfo, TableLocations, TableOrganisations, TableAssetOwners, \
@@ -11,17 +11,19 @@
     TablePowerElectronicsConnection, TablePowerElectronicsConnectionPhases, TableBatteryUnit, TablePhotoVoltaicUnit, TablePowerElectronicsWindUnit, \
     TableAcLineSegments, TableBreakers, TableLoadBreakSwitches, TableBusbarSections, TableDisconnectors, TableEnergyConsumers, TableEnergyConsumerPhases, \
     TableEnergySources, TableEnergySourcePhases, TableFuses, TableJumpers, TableJunctions, TableLinearShuntCompensators, TablePowerTransformers, \
     TableReclosers, TableTerminals, TableTransformerStarImpedance, TablePowerTransformerEnds, TableRatioTapChangers, TableFaultIndicators, TableFeeders, \
     TableLoops, TableCircuits, TablePositionPoints, TableLocationStreetAddresses, TableAssetOrganisationRolesAssets, TableUsagePointsEndDevices, \
     TableEquipmentUsagePoints, TableEquipmentOperationalRestrictions, TableEquipmentEquipmentContainers, TableCircuitsSubstations, TableCircuitsTerminals, \
     TableLoopsSubstations, TableControls, TableRemoteControls, TableRemoteSources, TableAnalogs, TableAccumulators, TableDiscretes, TableLvFeeders, \
-    TableCurrentTransformers, TablePotentialTransformers, TableCurrentTransformerInfo, TablePotentialTransformerInfo, TableCurrentRelayInfo, \
-    TableCurrentRelays, TableSwitchInfo, TableProtectionEquipmentProtectedSwitches, TableRecloseDelays, TableEvChargingUnits, TableTapChangerControls, \
-    TablePowerTransformerEndRatings
+    TableCurrentTransformers, TablePotentialTransformers, TableCurrentTransformerInfo, TablePotentialTransformerInfo, TableRelayInfo, \
+    TableCurrentRelays, TableSwitchInfo, TableProtectionRelayFunctionsProtectedSwitches, TableRecloseDelays, TableEvChargingUnits, TableTapChangerControls, \
+    TablePowerTransformerEndRatings, TableProtectionRelayFunctionThresholds, TableDistanceRelays, TableVoltageRelays, TableProtectionRelayFunctionTimeLimits, \
+    TableProtectionRelaySystems, TableProtectionRelaySchemes, TableGrounds, TableGroundDisconnectors, TableSeriesCompensators, \
+    TableProtectionRelayFunctionsSensors, TableProtectionRelaySchemesProtectionRelayFunctions
 from zepben.evolve.database.sqlite.readers.network_cim_reader import NetworkCIMReader
 
 __all__ = ["NetworkServiceReader"]
 
 
 class NetworkServiceReader(BaseServiceReader):
     """
@@ -39,15 +41,15 @@
         status = status and self._load_each(TableOpenCircuitTests, "open circuit tests", reader.load_open_circuit_test)
         status = status and self._load_each(TableShortCircuitTests, "short circuit tests", reader.load_short_circuit_test)
         status = status and self._load_each(TableShuntCompensatorInfo, "shunt compensator info", reader.load_shunt_compensator_info)
         status = status and self._load_each(TableSwitchInfo, "switch info", reader.load_switch_info)
         status = status and self._load_each(TableTransformerEndInfo, "transformer end info", reader.load_transformer_end_info)
         status = status and self._load_each(TableCurrentTransformerInfo, "current transformer info", reader.load_current_transformer_info)
         status = status and self._load_each(TablePotentialTransformerInfo, "potential transformer info", reader.load_potential_transformer_info)
-        status = status and self._load_each(TableCurrentRelayInfo, "current relay info", reader.load_current_relay_info)
+        status = status and self._load_each(TableRelayInfo, "relay info", reader.load_relay_info)
         status = status and self._load_each(TableRecloseDelays, "reclose delays", reader.load_reclose_delays)
         status = status and self._load_each(TableLocations, "locations", reader.load_location)
         status = status and self._load_each(TableOrganisations, "organisations", reader.load_organisation)
         status = status and self._load_each(TableAssetOwners, "asset owners", reader.load_asset_owner)
         status = status and self._load_each(TablePoles, "poles", reader.load_pole)
         status = status and self._load_each(TableStreetlights, "streetlights", reader.load_streetlight)
         status = status and self._load_each(TableMeters, "meters", reader.load_meter)
@@ -62,22 +64,31 @@
         status = status and self._load_each(TablePerLengthSequenceImpedances, "per length sequence impedances", reader.load_per_length_sequence_impedance)
         status = status and self._load_each(TableEquivalentBranches, "equivalent branches", reader.load_equivalent_branch)
         status = status and self._load_each(TableAcLineSegments, "AC line segments", reader.load_ac_line_segment)
         status = status and self._load_each(TableBreakers, "breakers", reader.load_breaker)
         status = status and self._load_each(TableLoadBreakSwitches, "load break switches", reader.load_load_break_switch)
         status = status and self._load_each(TableBusbarSections, "busbar sections", reader.load_busbar_section)
         status = status and self._load_each(TableCurrentRelays, "current relays", reader.load_current_relay)
+        status = status and self._load_each(TableDistanceRelays, "distance relays", reader.load_distance_relay)
+        status = status and self._load_each(TableVoltageRelays, "voltage relays", reader.load_voltage_relay)
+        status = status and self._load_each(TableProtectionRelayFunctionThresholds, "protection relay function thresholds", reader.load_protection_relay_function_thresholds)
+        status = status and self._load_each(TableProtectionRelayFunctionTimeLimits, "protection relay function time limits", reader.load_protection_relay_function_time_limits)
+        status = status and self._load_each(TableProtectionRelaySystems, "protection relay system", reader.load_protection_relay_system)
+        status = status and self._load_each(TableProtectionRelaySchemes, "protection relay scheme", reader.load_protection_relay_scheme)
         status = status and self._load_each(TableDisconnectors, "disconnectors", reader.load_disconnector)
         status = status and self._load_each(TableEnergyConsumers, "energy consumers", reader.load_energy_consumer)
         status = status and self._load_each(TableEnergyConsumerPhases, "energy consumer phases", reader.load_energy_consumer_phase)
         status = status and self._load_each(TableEnergySources, "energy sources", reader.load_energy_source)
         status = status and self._load_each(TableEnergySourcePhases, "energy source phases", reader.load_energy_source_phase)
         status = status and self._load_each(TableFuses, "fuses", reader.load_fuse)
         status = status and self._load_each(TableJumpers, "jumpers", reader.load_jumper)
         status = status and self._load_each(TableJunctions, "junctions", reader.load_junction)
+        status = status and self._load_each(TableGrounds, "grounds", reader.load_ground)
+        status = status and self._load_each(TableGroundDisconnectors, "ground disconnectors", reader.load_ground_disconnector)
+        status = status and self._load_each(TableSeriesCompensators, "series compensators", reader.load_series_compensator)
         status = status and self._load_each(TableLinearShuntCompensators, "linear shunt compensators", reader.load_linear_shunt_compensator)
         status = status and self._load_each(TablePowerTransformers, "power transformers", reader.load_power_transformer)
         status = status and self._load_each(TableReclosers, "reclosers", reader.load_recloser)
         status = status and self._load_each(TablePowerElectronicsConnection, "power electronics connection", reader.load_power_electronics_connection)
         status = status and self._load_each(TableTerminals, "terminals", reader.load_terminal)
         status = status and self._load_each(TableTapChangerControls, "tap changer controls", reader.load_tap_changer_control)
         status = status and self._load_each(TablePowerElectronicsConnectionPhases, "power electronics connection phases", reader.load_power_electronics_connection_phase)
@@ -111,22 +122,32 @@
             reader.load_equipment_operational_restriction
         )
         status = status and self._load_each(
             TableEquipmentEquipmentContainers,
             "equipment to equipment container associations",
             reader.load_equipment_equipment_container
         )
+        status = status and self._load_each(TableCircuitsSubstations, "circuit to substation associations", reader.load_circuit_substation)
+        status = status and self._load_each(TableCircuitsTerminals, "circuit to terminal associations", reader.load_circuit_terminal)
+        status = status and self._load_each(TableLoopsSubstations, "loop to substation associations", reader.load_loop_substation)
         status = status and self._load_each(
-            TableProtectionEquipmentProtectedSwitches,
+            TableProtectionRelayFunctionsProtectedSwitches,
             "protection equipment to protected switch associations",
             reader.load_protection_equipment_protected_switch
         )
-        status = status and self._load_each(TableCircuitsSubstations, "circuit to substation associations", reader.load_circuit_substation)
-        status = status and self._load_each(TableCircuitsTerminals, "circuit to terminal associations", reader.load_circuit_terminal)
-        status = status and self._load_each(TableLoopsSubstations, "loop to substation associations", reader.load_loop_substation)
+        status = status and self._load_each(
+            TableProtectionRelayFunctionsSensors,
+            "protection equipment to sensor associations",
+            reader.load_protection_relay_functions_sensors
+        )
+        status = status and self._load_each(
+            TableProtectionRelaySchemesProtectionRelayFunctions,
+            "protection relay scheme to protection relay function associations",
+            reader.load_protection_relay_schemes_protection_relay_functions
+        )
         status = status and self._load_each(TableControls, "controls", reader.load_control)
         status = status and self._load_each(TableRemoteControls, "remote controls", reader.load_remote_control)
         status = status and self._load_each(TableRemoteSources, "remote sources", reader.load_remote_source)
         status = status and self._load_each(TableAnalogs, "analogs", reader.load_analog)
         status = status and self._load_each(TableAccumulators, "accumulators", reader.load_accumulator)
         status = status and self._load_each(TableDiscretes, "discretes", reader.load_discrete)
```

## zepben/evolve/database/sqlite/readers/result_set.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from datetime import datetime
 from typing import Any, Optional, Union, Type, TypeVar, List
```

## zepben/evolve/database/sqlite/tables/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/column.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 
 from dataclassy import dataclass
```

## zepben/evolve/database/sqlite/tables/database_tables.py

```diff
@@ -1,24 +1,26 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from sqlite3 import Cursor
 from typing import Dict, TypeVar, Type, Any, Optional
 
 from dataclassy import dataclass
 
-from zepben.evolve import TableProtectionEquipmentProtectedSwitches
 from zepben.evolve.database.sqlite.tables.associations.assetorganisationroles_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.circuit_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.customeragreements_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.equipment_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.loop_association_tables import *
 from zepben.evolve.database.sqlite.tables.associations.pricingstructure_association_tables import *
+from zepben.evolve.database.sqlite.tables.associations.protection_relay_functions_protected_switches import *
+from zepben.evolve.database.sqlite.tables.associations.protection_relay_schemes_protection_relay_functions import *
+from zepben.evolve.database.sqlite.tables.associations.protection_relay_functions_sensors import *
 from zepben.evolve.database.sqlite.tables.associations.usagepoints_association_tables import *
 from zepben.evolve.database.sqlite.tables.exceptions import MissingTableConfigException, SqlException
 from zepben.evolve.database.sqlite.tables.iec61968.asset_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.assetinfo_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.common_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.customer_tables import *
 from zepben.evolve.database.sqlite.tables.iec61968.infiec61968.infassetinfo_tables import *
@@ -63,39 +65,41 @@
         TableBusbarSections: TableBusbarSections(),
         TableCableInfo: TableCableInfo(),
         TableCircuits: TableCircuits(),
         TableCircuitsSubstations: TableCircuitsSubstations(),
         TableCircuitsTerminals: TableCircuitsTerminals(),
         TableConnectivityNodes: TableConnectivityNodes(),
         TableControls: TableControls(),
-        TableCurrentRelayInfo: TableCurrentRelayInfo(),
         TableCurrentRelays: TableCurrentRelays(),
         TableCurrentTransformerInfo: TableCurrentTransformerInfo(),
         TableCurrentTransformers: TableCurrentTransformers(),
         TableCustomerAgreements: TableCustomerAgreements(),
         TableCustomerAgreementsPricingStructures: TableCustomerAgreementsPricingStructures(),
         TableCustomers: TableCustomers(),
         TableDiagramObjectPoints: TableDiagramObjectPoints(),
         TableDiagramObjects: TableDiagramObjects(),
         TableDiagrams: TableDiagrams(),
         TableDisconnectors: TableDisconnectors(),
         TableDiscretes: TableDiscretes(),
+        TableDistanceRelays: TableDistanceRelays(),
         TableEnergyConsumerPhases: TableEnergyConsumerPhases(),
         TableEnergyConsumers: TableEnergyConsumers(),
         TableEnergySourcePhases: TableEnergySourcePhases(),
         TableEnergySources: TableEnergySources(),
         TableEquipmentEquipmentContainers: TableEquipmentEquipmentContainers(),
         TableEquipmentOperationalRestrictions: TableEquipmentOperationalRestrictions(),
         TableEquipmentUsagePoints: TableEquipmentUsagePoints(),
         TableEquivalentBranches: TableEquivalentBranches(),
         TableEvChargingUnits: TableEvChargingUnits(),
         TableFaultIndicators: TableFaultIndicators(),
         TableFeeders: TableFeeders(),
         TableFuses: TableFuses(),
         TableGeographicalRegions: TableGeographicalRegions(),
+        TableGrounds: TableGrounds(),
+        TableGroundDisconnectors: TableGroundDisconnectors(),
         TableJumpers: TableJumpers(),
         TableJunctions: TableJunctions(),
         TableLinearShuntCompensators: TableLinearShuntCompensators(),
         TableLoadBreakSwitches: TableLoadBreakSwitches(),
         TableLocationStreetAddresses: TableLocationStreetAddresses(),
         TableLocations: TableLocations(),
         TableLoops: TableLoops(),
@@ -121,20 +125,28 @@
         TablePowerElectronicsWindUnit: TablePowerElectronicsWindUnit(),
         TablePowerTransformerEnds: TablePowerTransformerEnds(),
         TablePowerTransformerEndRatings: TablePowerTransformerEndRatings(),
         TablePowerTransformerInfo: TablePowerTransformerInfo(),
         TablePowerTransformers: TablePowerTransformers(),
         TablePricingStructures: TablePricingStructures(),
         TablePricingStructuresTariffs: TablePricingStructuresTariffs(),
-        TableProtectionEquipmentProtectedSwitches: TableProtectionEquipmentProtectedSwitches(),
+        TableProtectionRelayFunctionThresholds: TableProtectionRelayFunctionThresholds(),
+        TableProtectionRelayFunctionTimeLimits: TableProtectionRelayFunctionTimeLimits(),
+        TableProtectionRelayFunctionsProtectedSwitches: TableProtectionRelayFunctionsProtectedSwitches(),
+        TableProtectionRelayFunctionsSensors: TableProtectionRelayFunctionsSensors(),
+        TableProtectionRelaySchemes: TableProtectionRelaySchemes(),
+        TableProtectionRelaySchemesProtectionRelayFunctions: TableProtectionRelaySchemesProtectionRelayFunctions(),
+        TableProtectionRelaySystems: TableProtectionRelaySystems(),
         TableRatioTapChangers: TableRatioTapChangers(),
         TableReclosers: TableReclosers(),
         TableRecloseDelays: TableRecloseDelays(),
+        TableRelayInfo: TableRelayInfo(),
         TableRemoteControls: TableRemoteControls(),
         TableRemoteSources: TableRemoteSources(),
+        TableSeriesCompensators: TableSeriesCompensators(),
         TableShortCircuitTests: TableShortCircuitTests(),
         TableShuntCompensatorInfo: TableShuntCompensatorInfo(),
         TableSites: TableSites(),
         TableStreetlights: TableStreetlights(),
         TableSubGeographicalRegions: TableSubGeographicalRegions(),
         TableSubstations: TableSubstations(),
         TableSwitchInfo: TableSwitchInfo(),
@@ -143,14 +155,15 @@
         TableTerminals: TableTerminals(),
         TableTransformerEndInfo: TableTransformerEndInfo(),
         TableTransformerStarImpedance: TableTransformerStarImpedance(),
         TableTransformerTankInfo: TableTransformerTankInfo(),
         TableUsagePoints: TableUsagePoints(),
         TableUsagePointsEndDevices: TableUsagePointsEndDevices(),
         TableVersion: TableVersion(),
+        TableVoltageRelays: TableVoltageRelays(),
     }
 
 
 @dataclass(slots=True)
 class PreparedStatement(object):
     statement: str
     _values: Dict[int, Any] = dict()
```

## zepben/evolve/database/sqlite/tables/exceptions.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 __all__ = ["MissingTableConfigException", "SqlException"]
```

## zepben/evolve/database/sqlite/tables/metadata_tables.py

```diff
@@ -1,23 +1,23 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.sqlite_table import SqliteTable
 
 __all__ = ["TableVersion", "TableMetadataDataSources"]
 
 
 class TableVersion(SqliteTable):
     version: Column = None
 
-    SUPPORTED_VERSION = 48
+    SUPPORTED_VERSION = 49
 
     def __init__(self):
         self.version = self._create_column("version", "TEXT", Nullable.NOT_NULL)
 
     def name(self) -> str:
         return "version"
```

## zepben/evolve/database/sqlite/tables/sqlite_table.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 import inspect
```

## zepben/evolve/database/sqlite/tables/associations/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/associations/assetorganisationroles_association_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
```

## zepben/evolve/database/sqlite/tables/associations/circuit_association_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
```

## zepben/evolve/database/sqlite/tables/associations/customeragreements_association_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
```

## zepben/evolve/database/sqlite/tables/associations/equipment_association_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
```

## zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 from typing import List
```

## zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import List
```

## zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import List
```

## zepben/evolve/database/sqlite/tables/iec61968/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61968.common_tables import TableOrganisationRoles
```

## zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
```

## zepben/evolve/database/sqlite/tables/iec61968/common_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 from typing import List
```

## zepben/evolve/database/sqlite/tables/iec61968/customer_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import List
```

## zepben/evolve/database/sqlite/tables/iec61968/metering_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61968.asset_tables import TableAssetContainers
```

## zepben/evolve/database/sqlite/tables/iec61968/operations_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.iec61968.common_tables import TableDocuments
```

## zepben/evolve/database/sqlite/tables/iec61968/infiec61968/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py

```diff
@@ -1,58 +1,60 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve import SqliteTable
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61968.asset_tables import TableAssetInfo
 
-__all__ = ["TableCurrentRelayInfo", "TableCurrentTransformerInfo", "TablePotentialTransformerInfo", "TableRecloseDelays"]
+__all__ = ["TableRelayInfo", "TableCurrentTransformerInfo", "TablePotentialTransformerInfo", "TableRecloseDelays"]
 
 
 class TableRecloseDelays(SqliteTable):
-    current_relay_info_mrid: Column = None
+    relay_info_mrid: Column = None
     reclose_delay: Column = None
     sequence_number: Column = None
 
     def __init__(self):
         super(TableRecloseDelays, self).__init__()
-        self.current_relay_info_mrid = self._create_column("current_relay_info_mrid", "TEXT", Nullable.NOT_NULL)
+        self.relay_info_mrid = self._create_column("relay_info_mrid", "TEXT", Nullable.NOT_NULL)
         self.reclose_delay = self._create_column("reclose_delay", "NUMBER", Nullable.NOT_NULL)
         self.sequence_number = self._create_column("sequence_number", "INTEGER", Nullable.NOT_NULL)
 
     def name(self) -> str:
         return "reclose_delays"
 
     def unique_index_columns(self) -> List[List[Column]]:
         cols = super(TableRecloseDelays, self).unique_index_columns()
-        cols.append([self.current_relay_info_mrid, self.sequence_number])
+        cols.append([self.relay_info_mrid, self.sequence_number])
         return cols
 
     def non_unique_index_columns(self) -> List[List[Column]]:
         cols = super(TableRecloseDelays, self).non_unique_index_columns()
-        cols.append([self.current_relay_info_mrid])
+        cols.append([self.relay_info_mrid])
         return cols
 
     def select_sql(self):
-        return super(TableRecloseDelays, self).select_sql() + " ORDER BY current_relay_info_mrid, sequence_number ASC;"
+        return super(TableRecloseDelays, self).select_sql() + " ORDER BY relay_info_mrid, sequence_number ASC;"
 
 
-class TableCurrentRelayInfo(TableAssetInfo):
+class TableRelayInfo(TableAssetInfo):
     curve_setting: Column = None
+    reclose_fast: Column = None
 
     def __init__(self):
-        super(TableCurrentRelayInfo, self).__init__()
+        super(TableRelayInfo, self).__init__()
         self.curve_setting = self._create_column("curve_setting", "TEXT", Nullable.NULL)
+        self.reclose_fast = self._create_column("reclose_fast", "BOOLEAN", Nullable.NULL)
 
     def name(self) -> str:
-        return "current_relay_info"
+        return "relay_info"
 
 
 class TableCurrentTransformerInfo(TableAssetInfo):
     accuracy_class: Column = None
     accuracy_limit: Column = None
     core_count: Column = None
     ct_class: Column = None
```

## zepben/evolve/database/sqlite/tables/iec61970/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61970/base/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61970/base/auxiliaryequipment_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableEquipment
```

## zepben/evolve/database/sqlite/tables/iec61970/base/core_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
```

## zepben/evolve/database/sqlite/tables/iec61970/base/diagramlayout_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import List
```

## zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from zepben.evolve import Column, TableConductingEquipment, Nullable
 
 __all__ = ["TableEquivalentBranches", "TableEquivalentEquipment"]
```

## zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import List
```

## zepben/evolve/database/sqlite/tables/iec61970/base/protection_tables.py

```diff
@@ -1,41 +1,157 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
+from typing import List
+
+from zepben.evolve import SqliteTable
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
-from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableEquipment, TableIdentifiedObjects
+from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableEquipment, TableIdentifiedObjects, TablePowerSystemResources
 
-__all__ = ["TableProtectionEquipment", "TableCurrentRelays"]
+__all__ = ["TableProtectionRelayFunctions", "TableCurrentRelays", "TableProtectionRelaySystems", "TableDistanceRelays",
+           "TableProtectionRelayFunctionThresholds", "TableProtectionRelayFunctionTimeLimits", "TableProtectionRelaySchemes", "TableVoltageRelays"]
 
 
 # noinspection PyAbstractClass
-class TableProtectionEquipment(TableEquipment):
+class TableProtectionRelayFunctions(TablePowerSystemResources):
+    model: Column = None
+    reclosing: Column = None
     relay_delay_time: Column = None
     protection_kind: Column = None
     directable: Column = None
     power_direction: Column = None
+    relay_info_mrid: Column = None
 
     def __init__(self):
-        super(TableProtectionEquipment, self).__init__()
+        super(TableProtectionRelayFunctions, self).__init__()
+        self.model = self._create_column("model", "TEXT", Nullable.NULL)
+        self.reclosing = self._create_column("reclosing", "BOOLEAN", Nullable.NULL)
         self.relay_delay_time = self._create_column("relay_delay_time", "NUMBER", Nullable.NULL)
         self.protection_kind = self._create_column("protection_kind", "TEXT", Nullable.NOT_NULL)
         self.directable = self._create_column("directable", "BOOLEAN", Nullable.NULL)
         self.power_direction = self._create_column("power_direction", "TEXT", Nullable.NOT_NULL)
+        self.relay_info_mrid = self._create_column("relay_info_mrid", "TEXT", Nullable.NULL)
 
 
-class TableCurrentRelays(TableProtectionEquipment):
+class TableCurrentRelays(TableProtectionRelayFunctions):
     current_limit_1: Column = None
     inverse_time_flag: Column = None
     time_delay_1: Column = None
-    current_relay_info_mrid: Column = None
 
     def __init__(self):
         super(TableCurrentRelays, self).__init__()
         self.current_limit_1 = self._create_column("current_limit_1", "NUMBER", Nullable.NULL)
         self.inverse_time_flag = self._create_column("inverse_time_flag", "BOOLEAN", Nullable.NULL)
         self.time_delay_1 = self._create_column("time_delay_1", "NUMBER", Nullable.NULL)
-        self.current_relay_info_mrid = self._create_column("current_relay_info_mrid", "TEXT", Nullable.NULL)
 
     def name(self) -> str:
         return "current_relays"
+
+
+class TableDistanceRelays(TableProtectionRelayFunctions):
+    backward_blind: Column = None
+    backward_reach: Column = None
+    backward_reactance: Column = None
+    forward_blind: Column = None
+    forward_reach: Column = None
+    forward_reactance: Column = None
+    operation_phase_angle1: Column = None
+    operation_phase_angle2: Column = None
+    operation_phase_angle3: Column = None
+
+    def __init__(self):
+        super(TableDistanceRelays, self).__init__()
+        self.backward_blind = self._create_column("backward_blind", "NUMBER", Nullable.NULL)
+        self.backward_reach = self._create_column("backward_reach", "NUMBER", Nullable.NULL)
+        self.backward_reactance = self._create_column("backward_reactance", "NUMBER", Nullable.NULL)
+        self.forward_blind = self._create_column("forward_blind", "NUMBER", Nullable.NULL)
+        self.forward_reach = self._create_column("forward_reach", "NUMBER", Nullable.NULL)
+        self.forward_reactance = self._create_column("forward_reactance", "NUMBER", Nullable.NULL)
+        self.operation_phase_angle1 = self._create_column("operation_phase_angle1", "NUMBER", Nullable.NULL)
+        self.operation_phase_angle2 = self._create_column("operation_phase_angle2", "NUMBER", Nullable.NULL)
+        self.operation_phase_angle3 = self._create_column("operation_phase_angle3", "NUMBER", Nullable.NULL)
+
+    def name(self) -> str:
+        return "distance_relays"
+
+
+class TableProtectionRelayFunctionThresholds(SqliteTable):
+    protection_relay_function_mrid: Column = None
+    sequence_number: Column = None
+    unit_symbol: Column = None
+    value: Column = None
+    name_: Column = None
+
+    def __init__(self):
+        super(TableProtectionRelayFunctionThresholds, self).__init__()
+        self.protection_relay_function_mrid = self._create_column("protection_relay_function_mrid", "TEXT", Nullable.NOT_NULL)
+        self.sequence_number = self._create_column("sequence_number", "INTEGER", Nullable.NOT_NULL)
+        self.unit_symbol = self._create_column("unit_symbol", "TEXT", Nullable.NOT_NULL)
+        self.value = self._create_column("value", "NUMBER", Nullable.NOT_NULL)
+        self.name_ = self._create_column("name", "TEXT", Nullable.NULL)
+
+    def name(self) -> str:
+        return "protection_relay_function_thresholds"
+
+    def unique_index_columns(self) -> List[List[Column]]:
+        cols = super(TableProtectionRelayFunctionThresholds, self).unique_index_columns()
+        cols.append([self.protection_relay_function_mrid, self.sequence_number])
+        return cols
+
+    def non_unique_index_columns(self) -> List[List[Column]]:
+        cols = super(TableProtectionRelayFunctionThresholds, self).non_unique_index_columns()
+        cols.append([self.protection_relay_function_mrid])
+        return cols
+
+
+class TableProtectionRelayFunctionTimeLimits(SqliteTable):
+    protection_relay_function_mrid: Column = None
+    sequence_number: Column = None
+    time_limit: Column = None
+
+    def __init__(self):
+        super(TableProtectionRelayFunctionTimeLimits, self).__init__()
+        self.protection_relay_function_mrid = self._create_column("protection_relay_function_mrid", "TEXT", Nullable.NOT_NULL)
+        self.sequence_number = self._create_column("sequence_number", "INTEGER", Nullable.NOT_NULL)
+        self.time_limit = self._create_column("time_limit", "NUMBER", Nullable.NOT_NULL)
+
+    def name(self) -> str:
+        return "protection_relay_function_time_limits"
+
+    def unique_index_columns(self) -> List[List[Column]]:
+        cols = super(TableProtectionRelayFunctionTimeLimits, self).unique_index_columns()
+        cols.append([self.protection_relay_function_mrid, self.sequence_number])
+        return cols
+
+    def non_unique_index_columns(self) -> List[List[Column]]:
+        cols = super(TableProtectionRelayFunctionTimeLimits, self).non_unique_index_columns()
+        cols.append([self.protection_relay_function_mrid])
+        return cols
+
+
+class TableProtectionRelaySchemes(TableIdentifiedObjects):
+    system_mrid: Column = None
+
+    def __init__(self):
+        super(TableProtectionRelaySchemes, self).__init__()
+        self.system_mrid = self._create_column("system_mrid", "TEXT", Nullable.NULL)
+
+    def name(self) -> str:
+        return "protection_relay_schemes"
+
+
+class TableProtectionRelaySystems(TableEquipment):
+    protection_kind: Column = None
+
+    def __init__(self):
+        super(TableProtectionRelaySystems, self).__init__()
+        self.protection_kind = self._create_column("protection_kind", "TEXT", Nullable.NOT_NULL)
+
+    def name(self) -> str:
+        return "protection_relay_systems"
+
+
+class TableVoltageRelays(TableProtectionRelayFunctions):
+    def name(self) -> str:
+        return "voltage_relays"
```

## zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableIdentifiedObjects
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/conductor_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableConductingEquipment
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/connector_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableConductingEquipment
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/container_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableEquipmentContainers
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/energyconnection_tables.py

```diff
@@ -1,21 +1,21 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableConductingEquipment, TablePowerSystemResources
 
 __all__ = ["TableEnergyConnections", "TableEnergyConsumerPhases", "TableEnergyConsumers", "TableEnergySources", "TableEnergySourcePhases",
            "TableRegulatingCondEq", "TableShuntCompensators", "TableLinearShuntCompensators", "TablePowerElectronicsConnection",
-           "TablePowerElectronicsConnectionPhases", "TableRegulatingControls", "TableTapChangerControls"]
+           "TablePowerElectronicsConnectionPhases", "TableRegulatingControls", "TableTapChangerControls", "TableSeriesCompensators"]
 
 
 # noinspection PyAbstractClass
 class TableEnergyConnections(TableConductingEquipment):
     pass
 
 
@@ -299,26 +299,28 @@
     mode: Column = None
     monitored_phase: Column = None
     target_deadband: Column = None
     target_value: Column = None
     enabled: Column = None
     max_allowed_target_value: Column = None
     min_allowed_target_value: Column = None
+    rated_current: Column = None
     terminal_mrid: Column = None
 
     def __init__(self):
         super(TableRegulatingControls, self).__init__()
         self.discrete = self._create_column("discrete", "BOOLEAN", Nullable.NULL)
         self.mode = self._create_column("mode", "TEXT", Nullable.NOT_NULL)
         self.monitored_phase = self._create_column("monitored_phase", "TEXT", Nullable.NOT_NULL)
         self.target_deadband = self._create_column("target_deadband", "NUMBER", Nullable.NULL)
         self.target_value = self._create_column("target_value", "NUMBER", Nullable.NULL)
         self.enabled = self._create_column("enabled", "BOOLEAN", Nullable.NULL)
         self.max_allowed_target_value = self._create_column("max_allowed_target_value", "NUMBER", Nullable.NULL)
         self.min_allowed_target_value = self._create_column("min_allowed_target_value", "NUMBER", Nullable.NULL)
+        self.rated_current = self._create_column("rated_current", "NUMBER", Nullable.NULL)
         self.terminal_mrid = self._create_column("terminal_mrid", "TEXT", Nullable.NULL)
 
 
 class TableTapChangerControls(TableRegulatingControls):
     limit_voltage: Column = None
     line_drop_compensation: Column = None
     line_drop_r: Column = None
@@ -339,7 +341,27 @@
         self.reverse_line_drop_x = self._create_column("reverse_line_drop_x", "NUMBER", Nullable.NULL)
         self.forward_ldc_blocking = self._create_column("forward_ldc_blocking", "BOOLEAN", Nullable.NULL)
         self.time_delay = self._create_column("time_delay", "NUMBER", Nullable.NULL)
         self.co_generation_enabled = self._create_column("co_generation_enabled", "BOOLEAN", Nullable.NULL)
 
     def name(self) -> str:
         return "tap_changer_controls"
+
+class TableSeriesCompensators(TableConductingEquipment):
+    r: Column = None
+    r0: Column = None
+    x: Column = None
+    x0: Column = None
+    varistor_rated_current: Column = None
+    varistor_voltage_threshold: Column = None
+
+    def __init__(self):
+        super(TableSeriesCompensators, self).__init__()
+        self.r = self._create_column("r", "NUMBER", Nullable.NULL)
+        self.r0 = self._create_column("r0", "NUMBER", Nullable.NULL)
+        self.x = self._create_column("x", "NUMBER", Nullable.NULL)
+        self.x0 = self._create_column("x0", "NUMBER", Nullable.NULL)
+        self.varistor_rated_current = self._create_column("varistor_rated_current", "INTEGER", Nullable.NULL)
+        self.varistor_voltage_threshold = self._create_column("varistor_voltage_threshold", "INTEGER", Nullable.NULL)
+
+    def name(self) -> str:
+        return "series_compensators"
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/perlength_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableIdentifiedObjects
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py

```diff
@@ -1,18 +1,18 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.iec61970.base.core_tables import TableConductingEquipment
 
 __all__ = ["TableSwitches", "TableProtectedSwitches", "TableFuses", "TableLoadBreakSwitches", "TableBreakers", "TableReclosers", "TableJumpers",
-           "TableDisconnectors"]
+           "TableDisconnectors", "TableGrounds", "TableGroundDisconnectors"]
 
 
 # noinspection PyAbstractClass
 class TableSwitches(TableConductingEquipment):
     normal_open: Column = None
     open: Column = None
     rated_current: Column = None
@@ -48,14 +48,20 @@
 
 class TableDisconnectors(TableSwitches):
     def name(self) -> str:
         return "disconnectors"
 
 
 class TableFuses(TableSwitches):
+    function_mrid: Column = None
+
+    def __init__(self):
+        super(TableFuses, self).__init__()
+        self.function_mrid = self._create_column("function_mrid", "TEXT", Nullable.NULL)
+
     def name(self) -> str:
         return "fuses"
 
 
 class TableJumpers(TableSwitches):
     def name(self) -> str:
         return "jumpers"
@@ -66,7 +72,18 @@
         return "load_break_switches"
 
 
 class TableReclosers(TableProtectedSwitches):
     def name(self) -> str:
         return "reclosers"
 
+
+class TableGroundDisconnectors(TableSwitches):
+
+    def name(self) -> str:
+        return "ground_disconnectors"
+
+
+class TableGrounds(TableConductingEquipment):
+
+    def name(self) -> str:
+        return "grounds"
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/transformer_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import List
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/production_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
```

## zepben/evolve/database/sqlite/tables/iec61970/infiec61970/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2021 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61970/infiec61970/feeder_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Nullable, Column
```

## zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2021 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2021 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/production_tables.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import TablePowerElectronicsUnit
```

## zepben/evolve/database/sqlite/writers/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/database/sqlite/writers/base_cim_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/database/sqlite/writers/base_service_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import logging
 from traceback import format_exc
 from typing import Callable, TypeVar, Generic, Type
```

## zepben/evolve/database/sqlite/writers/customer_cim_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.database.sqlite.tables.associations.customeragreements_association_tables import TableCustomerAgreementsPricingStructures
 from zepben.evolve.database.sqlite.tables.associations.pricingstructure_association_tables import TablePricingStructuresTariffs
```

## zepben/evolve/database/sqlite/writers/customer_service_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import CustomerCIMWriter, Organisation, Customer, CustomerAgreement, PricingStructure, Tariff, CustomerService
 from zepben.evolve.database.sqlite.writers.base_service_writer import BaseServiceWriter
```

## zepben/evolve/database/sqlite/writers/diagram_cim_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import DiagramObject, TableDiagramObjects, Diagram, TableDiagrams, DiagramObjectPoint, TableDiagramObjectPoints
 from zepben.evolve.database.sqlite.writers.base_cim_writer import BaseCIMWriter
```

## zepben/evolve/database/sqlite/writers/diagram_service_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import DiagramObject, Diagram, DiagramService
 from zepben.evolve.database.sqlite.writers.base_service_writer import BaseServiceWriter
```

## zepben/evolve/database/sqlite/writers/metadata_collection_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import logging
 
 from zepben.evolve import MetadataCollection, MetadataEntryWriter
```

## zepben/evolve/database/sqlite/writers/metadata_entry_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from sqlite3 import Cursor
 
 from dataclassy import dataclass
```

## zepben/evolve/database/sqlite/writers/network_cim_writer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import CableInfo, TableCableInfo, PreparedStatement, WireInfo, TableWireInfo, AssetInfo, TableOverheadWireInfo, OverheadWireInfo, \
     PowerTransformerInfo, TablePowerTransformerInfo, TableAcDcTerminals, AcDcTerminal, BaseVoltage, TableBaseVoltages, TableConductingEquipment, \
@@ -28,18 +28,22 @@
     Streetlight, TableStreetlights, Location, TableLocations, TableLocationStreetAddressField, StreetAddress, TableLocationStreetAddresses, PositionPoint, \
     TablePositionPoints, TableStreetAddresses, TableTownDetails, TownDetail, StreetDetail, TableEndDevices, Meter, TableMeters, TableUsagePoints, \
     OperationalRestriction, TableOperationalRestrictions, TableFaultIndicators, TableAuxiliaryEquipment, AuxiliaryEquipment, FaultIndicator, \
     TableMeasurements, Measurement, Analog, TableAnalogs, Accumulator, TableAccumulators, Discrete, TableDiscretes, Control, TableControls, TableIoPoints, \
     IoPoint, TableRemotePoints, RemotePoint, RemoteControl, TableRemoteControls, RemoteSource, TableRemoteSources, ShuntCompensatorInfo, \
     CurrentTransformer, TableSensors, Sensor, TableCurrentTransformers, PotentialTransformer, TablePotentialTransformers, CurrentTransformerInfo, \
     TableCurrentTransformerInfo, PotentialTransformerInfo, TablePotentialTransformerInfo, TableShuntCompensatorInfo, EquivalentBranch, EquivalentEquipment, \
-    Recloser, TableReclosers, TableEquipmentOperationalRestrictions, TableLvFeeders, LvFeeder, TableSwitchInfo, SwitchInfo, TableCurrentRelayInfo, \
-    CurrentRelayInfo, CurrentRelay, ProtectionEquipment, TableProtectionEquipment, TableCurrentRelays, TableProtectionEquipmentProtectedSwitches, \
+    Recloser, TableReclosers, TableEquipmentOperationalRestrictions, TableLvFeeders, LvFeeder, TableSwitchInfo, SwitchInfo, TableRelayInfo, \
+    RelayInfo, CurrentRelay, TableProtectionRelayFunctions, TableCurrentRelays, TableProtectionRelayFunctionsProtectedSwitches, \
     TableRecloseDelays, EvChargingUnit, TableEvChargingUnits, TableRegulatingControls, RegulatingControl, TapChangerControl, TableTapChangerControls, \
-    TransformerEndRatedS, TablePowerTransformerEndRatings
+    TablePowerTransformerEndRatings, TableGrounds, TableGroundDisconnectors, SeriesCompensator, TableSeriesCompensators, \
+    ProtectionRelayFunction, RelaySetting, TableProtectionRelayFunctionThresholds, TableProtectionRelayFunctionTimeLimits, TableVoltageRelays, \
+    TableDistanceRelays, TableProtectionRelaySchemes, TableProtectionRelaySystems, TableProtectionRelayFunctionsSensors, \
+    TableProtectionRelaySchemesProtectionRelayFunctions, DistanceRelay, ProtectionRelayScheme, ProtectionRelaySystem, VoltageRelay, Ground, GroundDisconnector
+
 from zepben.evolve.database.sqlite.tables.iec61970.base.equivalent_tables import TableEquivalentBranches, TableEquivalentEquipment
 from zepben.evolve.database.sqlite.writers.base_cim_writer import BaseCIMWriter
 
 __all__ = ["NetworkCIMWriter"]
 
 
 class NetworkCIMWriter(BaseCIMWriter):
@@ -275,30 +279,31 @@
         self.insert_street_detail(table, insert, street_address.street_detail)
         self.insert_town_detail(table, insert, street_address.town_detail)
 
         return self._try_execute_single_update(insert, street_id, description)
 
     # ************ IEC61968 infIEC61968 InfAssetInfo ************
 
-    def save_current_relay_info(self, current_relay_info: CurrentRelayInfo) -> bool:
-        table = self.database_tables.get_table(TableCurrentRelayInfo)
-        insert = self.database_tables.get_insert(TableCurrentRelayInfo)
+    def save_relay_info(self, relay_info: RelayInfo) -> bool:
+        table = self.database_tables.get_table(TableRelayInfo)
+        insert = self.database_tables.get_insert(TableRelayInfo)
 
         delay_table = self.database_tables.get_table(TableRecloseDelays)
-        if current_relay_info.reclose_delays:
-            for idx, delay in enumerate(current_relay_info.reclose_delays):
+        if relay_info.reclose_delays:
+            for idx, delay in enumerate(relay_info.reclose_delays):
                 delay_insert = self.database_tables.get_insert(TableRecloseDelays)
-                delay_insert.add_value(delay_table.current_relay_info_mrid.query_index, current_relay_info.mrid)
+                delay_insert.add_value(delay_table.relay_info_mrid.query_index, relay_info.mrid)
                 delay_insert.add_value(delay_table.sequence_number.query_index, idx)
                 delay_insert.add_value(delay_table.reclose_delay.query_index, delay)
-                self._try_execute_single_update(delay_insert, f"{current_relay_info.mrid}-rd-{idx}", "reclose delay")
+                self._try_execute_single_update(delay_insert, f"{relay_info.mrid}-rd-{idx}", "reclose delay")
 
-        insert.add_value(table.curve_setting.query_index, current_relay_info.curve_setting)
+        insert.add_value(table.curve_setting.query_index, relay_info.curve_setting)
+        insert.add_value(table.reclose_fast.query_index, relay_info.reclose_fast)
 
-        return self._save_asset_info(table, insert, current_relay_info, "current relay info")
+        return self._save_asset_info(table, insert, relay_info, "relay info")
 
     # ************ IEC61968 infIEC61968 InfAssetInfo ************
 
     def save_current_transformer_info(self, current_transformer_info: CurrentTransformerInfo):
         table = self.database_tables.get_table(TableCurrentTransformerInfo)
         insert = self.database_tables.get_insert(TableCurrentTransformerInfo)
 
@@ -550,26 +555,102 @@
     def save_current_relay(self, current_relay: CurrentRelay) -> bool:
         table = self.database_tables.get_table(TableCurrentRelays)
         insert = self.database_tables.get_insert(TableCurrentRelays)
 
         insert.add_value(table.current_limit_1.query_index, current_relay.current_limit_1)
         insert.add_value(table.inverse_time_flag.query_index, current_relay.inverse_time_flag)
         insert.add_value(table.time_delay_1.query_index, current_relay.time_delay_1)
-        insert.add_value(table.current_relay_info_mrid.query_index, self._mrid_or_none(current_relay.current_relay_info))
 
-        return self._save_protection_equipment(table, insert, current_relay, "current relay")
+        return self._save_protection_relay_function(table, insert, current_relay, "current relay")
 
-    def _save_protection_equipment(self, table: TableProtectionEquipment, insert: PreparedStatement, protection_equipment: ProtectionEquipment,
-                                   description: str) -> bool:
-        insert.add_value(table.relay_delay_time.query_index, protection_equipment.relay_delay_time)
-        insert.add_value(table.protection_kind.query_index, protection_equipment.protection_kind.short_name)
-        insert.add_value(table.directable.query_index, protection_equipment.directable)
-        insert.add_value(table.power_direction.query_index, protection_equipment.power_direction.short_name)
+    def save_distance_relay(self, distance_relay: DistanceRelay) -> bool:
+        table = self.database_tables.get_table(TableDistanceRelays)
+        insert = self.database_tables.get_insert(TableDistanceRelays)
+
+        insert.add_value(table.backward_blind.query_index, distance_relay.backward_blind)
+        insert.add_value(table.backward_reach.query_index, distance_relay.backward_reach)
+        insert.add_value(table.backward_reactance.query_index, distance_relay.backward_reactance)
+        insert.add_value(table.forward_blind.query_index, distance_relay.forward_blind)
+        insert.add_value(table.forward_reach.query_index, distance_relay.forward_reach)
+        insert.add_value(table.forward_reactance.query_index, distance_relay.forward_reactance)
+        insert.add_value(table.operation_phase_angle1.query_index, distance_relay.operation_phase_angle1)
+        insert.add_value(table.operation_phase_angle2.query_index, distance_relay.operation_phase_angle2)
+        insert.add_value(table.operation_phase_angle3.query_index, distance_relay.operation_phase_angle3)
+
+        return self._save_protection_relay_function(table, insert, distance_relay, "distance relay")
+
+    def _save_protection_relay_function(self, table: TableProtectionRelayFunctions, insert: PreparedStatement,
+                                        protection_relay_function: ProtectionRelayFunction,
+                                        description: str) -> bool:
+        insert.add_value(table.model.query_index, protection_relay_function.model)
+        insert.add_value(table.reclosing.query_index, protection_relay_function.reclosing)
+        insert.add_value(table.relay_delay_time.query_index, protection_relay_function.relay_delay_time)
+        insert.add_value(table.protection_kind.query_index, protection_relay_function.protection_kind.short_name)
+        insert.add_value(table.directable.query_index, protection_relay_function.directable)
+        insert.add_value(table.power_direction.query_index, protection_relay_function.power_direction.short_name)
+        insert.add_value(table.relay_info_mrid.query_index, self._mrid_or_none(protection_relay_function.asset_info))
+
+        status = True
+        for protected_switch in protection_relay_function.protected_switches:
+            status = status and self._save_protection_relay_function_protected_switch(protection_relay_function, protected_switch)
+        for sensor in protection_relay_function.sensors:
+            status = status and self._save_protection_relay_function_sensor(protection_relay_function, sensor)
+        for sequence_number, threshold in enumerate(protection_relay_function.thresholds):
+            status = status and self.save_protection_relay_threshold(protection_relay_function, sequence_number, threshold)
+        for sequence_number, time_limit in enumerate(protection_relay_function.time_limits):
+            status = status and self.save_protection_relay_time_limit(protection_relay_function, sequence_number, time_limit)
+
+        return status and self._save_power_system_resource(table, insert, protection_relay_function, description)
+
+    def save_protection_relay_threshold(self, protection_relay_function: ProtectionRelayFunction, sequence_number: int, threshold: RelaySetting) -> bool:
+        table = self.database_tables.get_table(TableProtectionRelayFunctionThresholds)
+        insert = self.database_tables.get_insert(TableProtectionRelayFunctionThresholds)
+
+        insert.add_value(table.protection_relay_function_mrid.query_index, protection_relay_function.mrid)
+        insert.add_value(table.sequence_number.query_index, sequence_number)
+        insert.add_value(table.unit_symbol.query_index, threshold.unit_symbol.short_name)
+        insert.add_value(table.value.query_index, threshold.value)
+        insert.add_value(table.name_.query_index, threshold.name)
+
+        return self._try_execute_single_update(insert, f"{protection_relay_function.mrid}-threshold{sequence_number}", "protection relay function threshold")
+
+    def save_protection_relay_time_limit(self, protection_relay_function: ProtectionRelayFunction, sequence_number: int, time_limit: float) -> bool:
+        table = self.database_tables.get_table(TableProtectionRelayFunctionTimeLimits)
+        insert = self.database_tables.get_insert(TableProtectionRelayFunctionTimeLimits)
+
+        insert.add_value(table.protection_relay_function_mrid.query_index, protection_relay_function.mrid)
+        insert.add_value(table.sequence_number.query_index, sequence_number)
+        insert.add_value(table.time_limit.query_index, time_limit)
+
+        return self._try_execute_single_update(insert, f"{protection_relay_function.mrid}-time_limit{sequence_number}", "protection relay function time limit")
+
+    def save_protection_relay_scheme(self, protection_relay_scheme: ProtectionRelayScheme) -> bool:
+        table = self.database_tables.get_table(TableProtectionRelaySchemes)
+        insert = self.database_tables.get_insert(TableProtectionRelaySchemes)
+
+        insert.add_value(table.system_mrid.query_index, self._mrid_or_none(protection_relay_scheme.system))
+
+        status = True
+        for function in protection_relay_scheme.functions:
+            status = status and self._save_protection_relay_scheme_protection_relay_function(protection_relay_scheme, function)
+        return status and self._save_identified_object(table, insert, protection_relay_scheme,  "protection relay scheme")
+
+    def save_protection_relay_system(self, protection_relay_system: ProtectionRelaySystem) -> bool:
+        table = self.database_tables.get_table(TableProtectionRelaySystems)
+        insert = self.database_tables.get_insert(TableProtectionRelaySystems)
+
+        insert.add_value(table.protection_kind.query_index, protection_relay_system.protection_kind.short_name)
+
+        return self._save_equipment(table, insert, protection_relay_system, "protection relay system")
+
+    def save_voltage_relay(self, voltage_relay: VoltageRelay) -> bool:
+        table = self.database_tables.get_table(TableVoltageRelays)
+        insert = self.database_tables.get_insert(TableVoltageRelays)
 
-        return self._save_equipment(table, insert, protection_equipment, description)
+        return self._save_protection_relay_function(table, insert, voltage_relay, "voltage relay")
 
     # ************ IEC61970 BASE WIRES ************
 
     def _save_power_electronics_unit(self, table: TablePowerElectronicsUnit, insert: PreparedStatement, power_electronics_unit: PowerElectronicsUnit,
                                      description: str) -> bool:
         insert.add_value(table.power_electronics_connection_mrid.query_index, self._mrid_or_none(power_electronics_unit.power_electronics_connection))
         insert.add_value(table.max_p.query_index, power_electronics_unit.max_p)
@@ -717,16 +798,30 @@
 
         return self._save_power_system_resource(table, insert, energy_source_phase, "energy source phase")
 
     def save_fuse(self, fuse: Fuse) -> bool:
         table = self.database_tables.get_table(TableFuses)
         insert = self.database_tables.get_insert(TableFuses)
 
+        insert.add_value(table.function_mrid.query_index, self._mrid_or_none(fuse.function))
+
         return self._save_switch(table, insert, fuse, "fuse")
 
+    def save_ground(self, ground: Ground) -> bool:
+        table = self.database_tables.get_table(TableGrounds)
+        insert = self.database_tables.get_insert(TableGrounds)
+
+        return self._save_conducting_equipment(table, insert, ground, "ground")
+
+    def save_ground_disconnector(self, ground_disconnector: GroundDisconnector) -> bool:
+        table = self.database_tables.get_table(TableGroundDisconnectors)
+        insert = self.database_tables.get_insert(TableGroundDisconnectors)
+
+        return self._save_switch(table, insert, ground_disconnector, "ground disconnector")
+
     def save_jumper(self, jumper: Jumper) -> bool:
         table = self.database_tables.get_table(TableJumpers)
         insert = self.database_tables.get_insert(TableJumpers)
 
         return self._save_switch(table, insert, jumper, "jumper")
 
     def save_junction(self, junction: Junction) -> bool:
@@ -864,19 +959,15 @@
             self._try_execute_single_update(ratings_insert, f"{power_transformer_end.mrid}-{it.cooling_type.short_name}-{it.rated_s}", "transformer end ratedS")
 
         return self._save_transformer_end(table, insert, power_transformer_end, "power transformer end")
 
     def _save_protected_switch(self, table: TableProtectedSwitches, insert: PreparedStatement, protected_switch: ProtectedSwitch, description: str) -> bool:
         insert.add_value(table.breaking_capacity.query_index, protected_switch.breaking_capacity)
 
-        status = True
-        for pe in protected_switch.operated_by_protection_equipment:
-            status = status and self._save_protection_equipment_protected_switch(pe, protected_switch)
-
-        return status and self._save_switch(table, insert, protected_switch, description)
+        return self._save_switch(table, insert, protected_switch, description)
 
     def save_ratio_tap_changer(self, ratio_tap_changer: RatioTapChanger) -> bool:
         table = self.database_tables.get_table(TableRatioTapChangers)
         insert = self.database_tables.get_insert(TableRatioTapChangers)
 
         insert.add_value(table.transformer_end_mrid.query_index, self._mrid_or_none(ratio_tap_changer.transformer_end))
         insert.add_value(table.step_voltage_increment.query_index, ratio_tap_changer.step_voltage_increment)
@@ -901,18 +992,32 @@
         insert.add_value(table.mode.query_index, regulating_control.mode.short_name)
         insert.add_value(table.monitored_phase.query_index, regulating_control.monitored_phase.short_name)
         insert.add_value(table.target_deadband.query_index, regulating_control.target_deadband)
         insert.add_value(table.target_value.query_index, regulating_control.target_value)
         insert.add_value(table.enabled.query_index, regulating_control.enabled)
         insert.add_value(table.max_allowed_target_value.query_index, regulating_control.max_allowed_target_value)
         insert.add_value(table.min_allowed_target_value.query_index, regulating_control.min_allowed_target_value)
+        insert.add_value(table.rated_current.query_index, regulating_control.rated_current)
         insert.add_value(table.terminal_mrid.query_index, self._mrid_or_none(regulating_control.terminal))
 
         return self._save_power_system_resource(table, insert, regulating_control, description)
 
+    def save_series_compensator(self, series_compensator: SeriesCompensator) -> bool:
+        table = self.database_tables.get_table(TableSeriesCompensators)
+        insert = self.database_tables.get_insert(TableSeriesCompensators)
+
+        insert.add_value(table.r.query_index, series_compensator.r)
+        insert.add_value(table.r0.query_index, series_compensator.r0)
+        insert.add_value(table.x.query_index, series_compensator.x)
+        insert.add_value(table.x0.query_index, series_compensator.x0)
+        insert.add_value(table.varistor_rated_current.query_index, series_compensator.varistor_rated_current)
+        insert.add_value(table.varistor_voltage_threshold.query_index, series_compensator.varistor_voltage_threshold)
+
+        return self._save_conducting_equipment(table, insert, series_compensator, "series compensator")
+
     def _save_shunt_compensator(self, table: TableShuntCompensators, insert: PreparedStatement, shunt_compensator: ShuntCompensator, description: str) -> bool:
         insert.add_value(table.shunt_compensator_info_mrid.query_index, self._mrid_or_none(shunt_compensator.shunt_compensator_info))
         insert.add_value(table.grounded.query_index, shunt_compensator.grounded)
         insert.add_value(table.nom_u.query_index, shunt_compensator.nom_u)
         insert.add_value(table.phase_connection.query_index, shunt_compensator.phase_connection.short_name)
         insert.add_value(table.sections.query_index, shunt_compensator.sections)
 
@@ -1156,16 +1261,37 @@
 
         insert.add_value(table.loop_mrid.query_index, loop.mrid)
         insert.add_value(table.substation_mrid.query_index, substation.mrid)
         insert.add_value(table.relationship.query_index, relationship.short_name)
 
         return self._try_execute_single_update(insert, f"{loop.mrid}-to-{substation.mrid}", f"loop to substation association")
 
-    def _save_protection_equipment_protected_switch(self, protection_equipment: ProtectionEquipment, protected_switch: ProtectedSwitch) -> bool:
-        table = self.database_tables.get_table(TableProtectionEquipmentProtectedSwitches)
-        insert = self.database_tables.get_insert(TableProtectionEquipmentProtectedSwitches)
+    def _save_protection_relay_function_protected_switch(self, protection_relay_function: ProtectionRelayFunction, protected_switch: ProtectedSwitch) -> bool:
+        table = self.database_tables.get_table(TableProtectionRelayFunctionsProtectedSwitches)
+        insert = self.database_tables.get_insert(TableProtectionRelayFunctionsProtectedSwitches)
 
-        insert.add_value(table.protection_equipment_mrid.query_index, protection_equipment.mrid)
+        insert.add_value(table.protection_relay_function_mrid.query_index, protection_relay_function.mrid)
         insert.add_value(table.protected_switch_mrid.query_index, protected_switch.mrid)
 
-        return self._try_execute_single_update(insert, f"{protection_equipment.mrid}-to-{protected_switch.mrid}",
+        return self._try_execute_single_update(insert, f"{protection_relay_function.mrid}-to-{protected_switch.mrid}",
                                                "protection equipment to protected switch association")
+
+    def _save_protection_relay_function_sensor(self, protection_relay_function: ProtectionRelayFunction, sensor: Sensor) -> bool:
+        table = self.database_tables.get_table(TableProtectionRelayFunctionsSensors)
+        insert = self.database_tables.get_insert(TableProtectionRelayFunctionsSensors)
+
+        insert.add_value(table.protection_relay_function_mrid.query_index, protection_relay_function.mrid)
+        insert.add_value(table.sensor_mrid.query_index, sensor.mrid)
+
+        return self._try_execute_single_update(insert, f"{protection_relay_function.mrid}-to-{sensor.mrid}",
+                                               "sensor to protected switch association")
+
+    def _save_protection_relay_scheme_protection_relay_function(self, protection_relay_scheme: ProtectionRelayScheme,
+                                                                protection_relay_function: ProtectionRelayFunction) -> bool:
+        table = self.database_tables.get_table(TableProtectionRelaySchemesProtectionRelayFunctions)
+        insert = self.database_tables.get_insert(TableProtectionRelaySchemesProtectionRelayFunctions)
+
+        insert.add_value(table.protection_relay_scheme_mrid.query_index, protection_relay_scheme.mrid)
+        insert.add_value(table.protection_relay_function_mrid.query_index, protection_relay_function.mrid)
+
+        return self._try_execute_single_update(insert, f"{protection_relay_scheme.mrid}-to-{protection_relay_function.mrid}",
+                                               "protection relay function to protection relay function association")
```

## zepben/evolve/database/sqlite/writers/network_service_writer.py

```diff
@@ -1,26 +1,34 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import NetworkService, CableInfo, OverheadWireInfo, PowerTransformerInfo, TransformerTankInfo, NoLoadTest, OpenCircuitTest, \
     ShortCircuitTest, ShuntCompensatorInfo, TransformerEndInfo, AssetOwner, Pole, Streetlight, Location, Organisation, Meter, UsagePoint, \
     OperationalRestriction, FaultIndicator, BaseVoltage, ConnectivityNode, Feeder, GeographicalRegion, Site, SubGeographicalRegion, Substation, Terminal, \
     EquivalentBranch, PhotoVoltaicUnit, AcLineSegment, Breaker, LoadBreakSwitch, BusbarSection, Disconnector, EnergyConsumer, EnergyConsumerPhase, \
     EnergySource, EnergySourcePhase, Fuse, Jumper, Junction, LinearShuntCompensator, PerLengthSequenceImpedance, PowerElectronicsConnection, \
     PowerElectronicsConnectionPhase, PowerTransformer, PowerTransformerEnd, RatioTapChanger, Recloser, TransformerStarImpedance, Circuit, Loop, Analog, \
     Accumulator, Discrete, Control, RemoteControl, RemoteSource, BatteryUnit, PowerElectronicsWindUnit, LvFeeder, CurrentTransformerInfo, \
-    PotentialTransformerInfo, CurrentTransformer, PotentialTransformer, CurrentRelayInfo, CurrentRelay, SwitchInfo, EvChargingUnit, TapChangerControl
+    PotentialTransformerInfo, CurrentTransformer, PotentialTransformer, RelayInfo, CurrentRelay, SwitchInfo, EvChargingUnit, TapChangerControl, \
+    SeriesCompensator
 from zepben.evolve.database.sqlite.writers.base_service_writer import BaseServiceWriter
 from zepben.evolve.database.sqlite.writers.network_cim_writer import NetworkCIMWriter
 
 __all__ = ["NetworkServiceWriter"]
 
+from zepben.evolve.model.cim.iec61970.base.protection.distance_relay import DistanceRelay
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_scheme import ProtectionRelayScheme
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_system import ProtectionRelaySystem
+from zepben.evolve.model.cim.iec61970.base.protection.voltage_relay import VoltageRelay
+from zepben.evolve.model.cim.iec61970.base.wires.ground import Ground
+from zepben.evolve.model.cim.iec61970.base.wires.ground_disconnector import GroundDisconnector
+
 
 class NetworkServiceWriter(BaseServiceWriter):
 
     def save(self, service: NetworkService, writer: NetworkCIMWriter) -> bool:
         status = super(NetworkServiceWriter, self).save(service, writer)
 
         status = status and self._save_all(service, CableInfo, writer.save_cable_info)
@@ -84,13 +92,20 @@
         status = status and self._save_all(service, Control, writer.save_control)
         status = status and self._save_all(service, RemoteControl, writer.save_remote_control)
         status = status and self._save_all(service, RemoteSource, writer.save_remote_source)
         status = status and self._save_all(service, CurrentTransformerInfo, writer.save_current_transformer_info)
         status = status and self._save_all(service, PotentialTransformerInfo, writer.save_potential_transformer_info)
         status = status and self._save_all(service, CurrentTransformer, writer.save_current_transformer)
         status = status and self._save_all(service, PotentialTransformer, writer.save_potential_transformer)
-        status = status and self._save_all(service, CurrentRelayInfo, writer.save_current_relay_info)
+        status = status and self._save_all(service, RelayInfo, writer.save_relay_info)
         status = status and self._save_all(service, CurrentRelay, writer.save_current_relay)
         status = status and self._save_all(service, TapChangerControl, writer.save_tap_changer_control)
         status = status and self._save_all(service, EvChargingUnit, writer.save_ev_charging_unit)
+        status = status and self._save_all(service, DistanceRelay, writer.save_distance_relay)
+        status = status and self._save_all(service, ProtectionRelayScheme, writer.save_protection_relay_scheme)
+        status = status and self._save_all(service, ProtectionRelaySystem, writer.save_protection_relay_system)
+        status = status and self._save_all(service, VoltageRelay, writer.save_voltage_relay)
+        status = status and self._save_all(service, Ground, writer.save_ground)
+        status = status and self._save_all(service, GroundDisconnector, writer.save_ground_disconnector)
+        status = status and self._save_all(service, SeriesCompensator, writer.save_series_compensator)
 
         return status
```

## zepben/evolve/database/sqlite/writers/utils.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import logging
 from sqlite3 import Cursor
 from typing import Optional, Callable, Any
```

## zepben/evolve/examples/__init__.py

```diff
@@ -1,7 +1,7 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.examples.simple_test_network import *
```

## zepben/evolve/examples/simple_test_network.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 __all__ = ["simple_test_network"]
 
 from typing import List
```

## zepben/evolve/model/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/phases.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
```

## zepben/evolve/model/resistance_reactance.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, Callable, TYPE_CHECKING
```

## zepben/evolve/model/busbranch/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/busbranch/bus_branch.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import abc
 from collections import Counter
 from dataclasses import dataclass, field
```

## zepben/evolve/model/cim/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/assetinfo/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/assetinfo/no_load_test.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional
 
 from zepben.evolve import TransformerTest
```

## zepben/evolve/model/cim/iec61968/assetinfo/open_circuit_test.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional
 
 from zepben.evolve import TransformerTest
```

## zepben/evolve/model/cim/iec61968/assetinfo/power_transformer_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import List, Optional, Generator
```

## zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional
 
 from zepben.evolve import TransformerTest
```

## zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional
```

## zepben/evolve/model/cim/iec61968/assetinfo/switch_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional
 
 from zepben.evolve.model.cim.iec61968.assets.asset_info import AssetInfo
```

## zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 import math
```

## zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, List, Generator, TYPE_CHECKING
```

## zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional
 
 from zepben.evolve.model.cim.iec61970.base.core.identified_object import IdentifiedObject
```

## zepben/evolve/model/cim/iec61968/assetinfo/wire_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/assetinfo/wire_material_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61968/assets/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/assets/asset.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/assets/asset_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.model.cim.iec61970.base.core.identified_object import IdentifiedObject
```

## zepben/evolve/model/cim/iec61968/assets/asset_organisation_role.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.model.cim.iec61968.common.organisation_role import OrganisationRole
```

## zepben/evolve/model/cim/iec61968/assets/pole.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/assets/streetlight.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/assets/structure.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/common/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/common/document.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from datetime import datetime
 from typing import Optional
```

## zepben/evolve/model/cim/iec61968/common/location.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/common/organisation.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.model.cim.iec61970.base.core.identified_object import IdentifiedObject
```

## zepben/evolve/model/cim/iec61968/common/organisation_role.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/customers/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/customers/customer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/customers/customer_agreement.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/customers/customer_kind.py

```diff
@@ -1,10 +1,10 @@
 
 
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61968/customers/pricing_structure.py

```diff
@@ -1,10 +1,10 @@
 
 
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/customers/tariff.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/infiec61968/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
```

## zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
```

## zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py

```diff
@@ -1,10 +1,10 @@
 
 
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/infiec61968/infcommon/ratio.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from dataclassy import dataclass
 
 __all__ = ["Ratio"]
```

## zepben/evolve/model/cim/iec61968/metering/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/metering/metering.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61968/operations/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61968/operations/operational_restriction.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/__init__.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/__init__.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/auxiliary_equipment.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/current_transformer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
```

## zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
```

## zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 
 __all__ = ["PotentialTransformerKind"]
```

## zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/sensor.py

```diff
@@ -1,16 +1,89 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
+from __future__ import annotations
+
+from typing import Generator, Optional, List, TYPE_CHECKING, Iterable
+from zepben.evolve.util import ngen, nlen, get_by_mrid, safe_remove
+if TYPE_CHECKING:
+    from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_function import ProtectionRelayFunction
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.auxiliary_equipment import AuxiliaryEquipment
 
 __all__ = ["Sensor"]
 
 
 class Sensor(AuxiliaryEquipment):
     """
     This class describes devices that transform a measured quantity into signals that can be presented at displays,
     used in control or be recorded.
     """
-    pass
+
+    _relay_functions: Optional[List[ProtectionRelayFunction]] = None
+    """The relay functions influenced by this [Sensor]."""
+
+    def __init__(self, relay_functions: Iterable[ProtectionRelayFunction] = None, **kwargs):
+        super(Sensor, self).__init__(**kwargs)
+        if relay_functions is not None:
+            for relay_function in relay_functions:
+                self.add_relay_function(relay_function)
+
+    @property
+    def relay_functions(self) -> Generator[ProtectionRelayFunction, None, None]:
+        """
+        Yields all the :class:`ProtectionRelayFunction` that are influenced by this :class:`Sensor`.
+
+        :return: A generator that iterates over all ProtectionRelayFunction influenced by this Sensor.
+        """
+        return ngen(self._relay_functions)
+
+    def num_relay_functions(self) -> int:
+        """
+        Get the number of :class:`ProtectionRelayFunction` that are influenced by this :class:`Sensor`.
+
+        :return: The number of ProtectionRelayFunction influenced by this Sensor.
+        """
+        return nlen(self._relay_functions)
+
+    def get_relay_function(self, mrid: str) -> Optional[ProtectionRelayFunction]:
+        """
+        Get a :class:`ProtectionRelayFunction` that are influenced by this :class:`Sensor`.
+
+        :param mrid: The mRID of the desired ProtectionRelayFunction
+        :return: The ProtectionRelayFunction with the specified mRID if it exists, otherwise None.
+        """
+        return get_by_mrid(self._relay_functions, mrid)
+
+    def add_relay_function(self, protection_relay_function: ProtectionRelayFunction) -> Sensor:
+        """
+        Associate this :class:`Sensor` with a :class:`ProtectionRelayFunction` it is influencing.
+
+        :param protection_relay_function: The ProtectionRelayFunction to associate with this Sensor.
+        :return: A reference to this Sensor for fluent use.
+        """
+        if self._validate_reference(protection_relay_function, self.get_relay_function, "A ProtectionRelayFunction"):
+            return self
+
+        self._relay_functions = list() if self._relay_functions is None else self._relay_functions
+        self._relay_functions.append(protection_relay_function)
+        return self
+
+    def remove_relay_function(self, protection_relay_function: ProtectionRelayFunction) -> Sensor:
+        """
+        Disassociate this :class:`Sensor` from a :class:`ProtectionRelayFunction` it is influencing.
+
+        :param protection_relay_function: The ProtectionRelayFunction to disassociate from this Sensor.
+        :return: A reference to this Sensor for fluent use.
+        """
+        self._relay_functions = safe_remove(self._relay_functions, protection_relay_function)
+        return self
+
+    def clear_relay_function(self) -> Sensor:
+        """
+        Disassociate all :class:`ProtectionRelayFunction` from this :class:`Sensor`.
+
+        :return: A reference to this Sensor for fluent use.
+        """
+        self._relay_functions = None
+        return self
```

## zepben/evolve/model/cim/iec61970/base/core/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/core/base_voltage.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.model.cim.iec61970.base.core.identified_object import IdentifiedObject
```

## zepben/evolve/model/cim/iec61970/base/core/conducting_equipment.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/connectivity_node.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/connectivity_node_container.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/equipment.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/equipment_container.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/identified_object.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/name.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/name_type.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/phase_code.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum, unique
 from typing import List, Set, Union
```

## zepben/evolve/model/cim/iec61970/base/core/power_system_resource.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/regions.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/substation.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/core/terminal.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/diagramlayout/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_layout.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_style.py

```diff
@@ -1,10 +1,10 @@
 
 
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61970/base/diagramlayout/orientation_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61970/base/domain/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/domain/unit_symbol.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61970/base/equivalents/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_branch.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_equipment.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/meas/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/meas/control.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/meas/iopoint.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.model.cim.iec61970.base.core.identified_object import IdentifiedObject
```

## zepben/evolve/model/cim/iec61970/base/meas/measurement.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/meas/value.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from datetime import datetime
 from typing import Optional
```

## zepben/evolve/model/cim/iec61970/base/protection/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/protection/current_relay.py

```diff
@@ -1,37 +1,23 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
-from typing import Optional
+from typing import Optional, TYPE_CHECKING
 
-from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import CurrentRelayInfo
-from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import ProtectionEquipment
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_function import ProtectionRelayFunction
 
 __all__ = ["CurrentRelay"]
 
 
-class CurrentRelay(ProtectionEquipment):
+class CurrentRelay(ProtectionRelayFunction):
     """A device that checks current flow values in any direction or designated direction."""
 
     current_limit_1: Optional[float] = None
     """Current limit number 1 for inverse time pickup in amperes."""
 
     inverse_time_flag: Optional[bool] = None
     """Set true if the current relay has inverse time characteristic."""
 
     time_delay_1: Optional[float] = None
     """Inverse time delay number 1 for current limit number 1 in seconds."""
-
-    @property
-    def current_relay_info(self) -> Optional[CurrentRelayInfo]:
-        """Datasheet information for this :class:`CurrentRelay`."""
-        return self.asset_info
-
-    @current_relay_info.setter
-    def current_relay_info(self, cri: Optional[CurrentRelayInfo]):
-        """
-        Set the :class:`CurrentRelayInfo` for this :class:`CurrentRelay`
-        :param cri: The CurrentRelayInfo for this CurrentRelay
-        """
-        self.asset_info = cri
```

## zepben/evolve/model/cim/iec61970/base/scada/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/scada/remote_control.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import Optional
```

## zepben/evolve/model/cim/iec61970/base/scada/remote_point.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.model.cim.iec61970.base.core.identified_object import IdentifiedObject
```

## zepben/evolve/model/cim/iec61970/base/scada/remote_source.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import Optional
```

## zepben/evolve/model/cim/iec61970/base/wires/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import Optional
```

## zepben/evolve/model/cim/iec61970/base/wires/breaker.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/connectors.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/disconnector.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional
```

## zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/energy_source.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/fuse.py

```diff
@@ -1,19 +1,25 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
 
+from typing import Optional
+
 from zepben.evolve import Switch
 
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_function import ProtectionRelayFunction
+
 __all__ = ["Fuse"]
 
 
 class Fuse(Switch):
     """
     An overcurrent protective device with a circuit opening fusible part that is heated and severed by the passage of
     overcurrent through it. A fuse is considered a switching device because it breaks current.
     """
-    pass
+
+    function: Optional[ProtectionRelayFunction] = None
+    """The function implemented by this Fuse"""
```

## zepben/evolve/model/cim/iec61970/base/wires/jumper.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/line.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.model.cim.iec61970.base.core.equipment_container import EquipmentContainer
```

## zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/per_length.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional
 
 from zepben.evolve.model.cim.iec61970.base.core.identified_object import IdentifiedObject
```

## zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, List, Generator, TYPE_CHECKING
```

## zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
 
@@ -192,29 +192,49 @@
 
     x_ground: Optional[float] = None
     """(for Yn and Zn connections) Reactive part of neutral impedance where 'grounded' is true"""
 
     ratio_tap_changer: Optional[RatioTapChanger] = None
     """Ratio tap changer associated with this transformer end."""
 
-    terminal: Optional[Terminal] = None
+    _terminal: Optional[Terminal] = None
     """The terminal of the transformer that this end is associated with"""
 
     base_voltage: Optional[BaseVoltage] = None
     """Base voltage of the transformer end.  This is essential for PU calculation."""
 
     end_number: int = 0
     """Number for this transformer end, corresponding to the end’s order in the power transformer vector group or phase angle clock number. 
     Highest voltage winding should be 1. Each end within a power transformer should have a unique subsequent end number. 
     Note the transformer end number need not match the terminal sequence number."""
 
     star_impedance: Optional[TransformerStarImpedance] = None
     """(accurate for 2- or 3-winding transformers only) Pi-model impedances of this transformer end. By convention, for a two winding transformer, the full
      values of the transformer should be entered on the high voltage end (endNumber=1)."""
 
+    def __init__(self, terminal: Optional[Terminal] = None, **kwargs):
+        super(TransformerEnd, self).__init__(**kwargs)
+        if terminal is not None:
+            self.terminal = terminal
+
+    @property
+    def terminal(self) -> Optional[Terminal]:
+        """
+        The terminal of the transformer that this end is associated with
+        """
+        return self._terminal
+
+    @terminal.setter
+    def terminal(self, value: Optional[Terminal]):
+        if value is not None:
+            require(value.conducting_equipment is None or isinstance(value.conducting_equipment, PowerTransformer),
+                    lambda: f"Cannot assign {self.__class__.__name__}[{self.mrid}] to {value.__class__.__name__}[{value.mrid}], which is connected to a " +
+                            f"{value.conducting_equipment.__class__.__name__}[{value.conducting_equipment.mrid}] rather than a PowerTransformer.")
+            self._terminal = value
+
 
 @dataclass(slots=True)
 class TransformerEndRatedS:
     cooling_type: TransformerCoolingType
     rated_s: int
```

## zepben/evolve/model/cim/iec61970/base/wires/protected_switch.py

```diff
@@ -1,98 +1,96 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
 
 from typing import Optional, List, Generator, TYPE_CHECKING, Iterable
 
 from zepben.evolve.model.cim.iec61970.base.wires.switch import Switch
 from zepben.evolve.util import get_by_mrid, ngen, nlen, safe_remove
 
 if TYPE_CHECKING:
-    from zepben.evolve import ProtectionEquipment
-
+    from zepben.evolve import ProtectionRelayFunction
 
 __all__ = ["ProtectedSwitch"]
 
 
 class ProtectedSwitch(Switch):
     """
-    A ProtectedSwitch is a switching device that can be operated by ProtectionEquipment.
+    A ProtectedSwitch is a switching device that can be operated by :class:`ProtectionRelayFunction`.
     """
 
     breaking_capacity: Optional[int] = None
     """The maximum fault current in amps a breaking device can break safely under prescribed conditions of use."""
 
-    _operated_by_protection_equipment: Optional[List[ProtectionEquipment]] = None
+    _relay_functions: Optional[List[ProtectionRelayFunction]] = None
 
     def __init__(
         self,
-        operated_by_protection_equipment: Iterable[ProtectionEquipment] = None,
+        relay_functions: Iterable[ProtectionRelayFunction] = None,
         **kwargs
     ):
         super(ProtectedSwitch, self).__init__(**kwargs)
 
         # breaking_capacity is handled via dataclassy.
-        if operated_by_protection_equipment is not None:
-            for protection_equipment in operated_by_protection_equipment:
-                self.add_operated_by_protection_equipment(protection_equipment)
+        if relay_functions is not None:
+            for relay_function in relay_functions:
+                self.add_relay_function(relay_function)
 
     @property
-    def operated_by_protection_equipment(self) -> Generator[ProtectionEquipment, None, None]:
+    def relay_functions(self) -> Generator[ProtectionRelayFunction, None, None]:
         """
-        Yields all :class:`ProtectionEquipment` operating this :class:`ProtectedSwitch`.
+        Yields all :class:`ProtectionRelayFunctions<ProtectionRelayFunction>` operating this :class:`ProtectedSwitch`.
 
-        :return: A generator that iterates over all ProtectionEquipment operating this ProtectedSwitch.
+        :return: A generator that iterates over all :class:`ProtectionRelayFunctions<ProtectionRelayFunction>` operating this :class:`ProtectedSwitch`.
         """
-        return ngen(self._operated_by_protection_equipment)
+        return ngen(self._relay_functions)
 
-    def num_operated_by_protection_equipment(self) -> int:
+    def num_relay_functions(self) -> int:
         """
-        Get the number of :class:`ProtectionEquipment` operating this :class:`ProtectedSwitch`.
+        Get the number of :class:`ProtectionRelayFunctions<ProtectionRelayFunction>` operating this :class:`ProtectedSwitch`.
 
-        :return: The number of ProtectionEquipment operating this ProtectedSwitch.
+        :return: The number of :class:`ProtectionRelayFunctions<ProtectionRelayFunction>` operating this :class:`ProtectedSwitch`.
         """
-        return nlen(self._operated_by_protection_equipment)
+        return nlen(self._relay_functions)
 
-    def get_operated_by_protection_equipment(self, mrid: str) -> Optional[ProtectionEquipment]:
+    def get_relay_function(self, mrid: str) -> Optional[ProtectionRelayFunction]:
         """
-        Get a :class:`ProtectionEquipment` operating this :class:`ProtectedSwitch` with the specified `mrid`.
+        Get a :class:`ProtectionRelayFunction` operating this :class:`ProtectedSwitch` with the specified `mrid`.
 
-        :param mrid: The mRID of the desired ProtectionEquipment
-        :return: The ProtectionEquipment with the specified mRID if it exists, otherwise None.
+        :param mrid: The mRID of the desired :class:`ProtectionRelayFunction`
+        :return: The :class:`ProtectionRelayFunction` with the specified mRID if it exists, otherwise None.
         """
-        return get_by_mrid(self._operated_by_protection_equipment, mrid)
+        return get_by_mrid(self._relay_functions, mrid)
 
-    def add_operated_by_protection_equipment(self, operated_by_protection_equipment: ProtectionEquipment) -> ProtectedSwitch:
+    def add_relay_function(self, relay_function: ProtectionRelayFunction) -> ProtectedSwitch:
         """
-        Associate this :class:`ProtectedSwitch` with a :class:`ProtectionEquipment` operating it.
-        :param operated_by_protection_equipment: The ProtectionEquipment to associate with this ProtectedSwitch.
-        :return: A reference to this ProtectedSwitch for fluent use.
+        Associate this :class:`ProtectedSwitch` with a :class:`ProtectionRelayFunction` operating it.
+        :param relay_function: The :class:`ProtectionRelayFunction` to associate with this :class:`ProtectedSwitch`.
+        :return: A reference to this :class:`ProtectedSwitch` for fluent use.
         """
-        if self._validate_reference(operated_by_protection_equipment, self.get_operated_by_protection_equipment, "A ProtectionEquipment"):
+        if self._validate_reference(relay_function, self.get_relay_function, "A ProtectionRelayFunction"):
             return self
 
-        self._operated_by_protection_equipment = list() if self._operated_by_protection_equipment is None else self._operated_by_protection_equipment
-        self._operated_by_protection_equipment.append(operated_by_protection_equipment)
-
+        self._relay_functions = list() if self._relay_functions is None else self._relay_functions
+        self._relay_functions.append(relay_function)
         return self
 
-    def remove_operated_by_protection_equipment(self, operated_by_protection_equipment: Optional[ProtectionEquipment]) -> ProtectedSwitch:
+    def remove_relay_function(self, relay_function: Optional[ProtectionRelayFunction]) -> ProtectedSwitch:
         """
-        Disassociate this :class:`ProtectedSwitch` from a :class:`ProtectionEquipment`.
-        :param operated_by_protection_equipment: The ProtectionEquipment to disassociate from this ProtectedSwitch.
-        :return: A reference to this ProtectedSwitch for fluent use.
+        Disassociate this :class:`ProtectedSwitch` from a :class:`ProtectionRelayFunction`.
+        :param relay_function: The :class:`ProtectionRelayFunction` to disassociate from this :class:`ProtectedSwitch`.
+        :return: A reference to this :class:`ProtectedSwitch` for fluent use.
         """
-        self._operated_by_protection_equipment = safe_remove(self._operated_by_protection_equipment, operated_by_protection_equipment)
+        self._relay_functions = safe_remove(self._relay_functions, relay_function)
         return self
 
-    def clear_operated_by_protection_equipment(self) -> ProtectedSwitch:
+    def clear_relay_functions(self) -> ProtectedSwitch:
         """
-        Disassociate all :class:`ProtectionEquipment` from this :class:`ProtectedSwitch`.
-        :return: A reference to this ProtectedSwitch for fluent use.
+        Disassociate all :class:`ProtectionRelayFunction` from this :class:`ProtectedSwitch`.
+        :return: A reference to this :class:`ProtectedSwitch` for fluent use.
         """
-        self._operated_by_protection_equipment = None
+        self._relay_functions = None
         return self
```

## zepben/evolve/model/cim/iec61970/base/wires/recloser.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/regulating_control.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 from typing import Optional, List, Generator, Iterable, TYPE_CHECKING
 
@@ -75,14 +75,18 @@
 
     max_allowed_target_value: Optional[float] = None
     """Maximum allowed target value (RegulatingControl.targetValue)."""
 
     min_allowed_target_value: Optional[float] = None
     """Minimum allowed target value (RegulatingControl.targetValue)."""
 
+    rated_current: Optional[float] = None
+    """The rated current of associated CT in amps for this RegulatingControl. Forms the base used to convert Line Drop Compensation settings from ohms to 
+    voltage."""
+
     terminal: Optional[Terminal] = None
     """
     The terminal associated with this regulating control. The terminal is associated instead of a node, since the terminal could connect into either a 
     topological node or a connectivity node. Sometimes it is useful to model regulation at a terminal of a bus bar object.
     """
 
     _regulating_cond_eq: Optional[List[RegulatingCondEq]] = None
@@ -128,20 +132,21 @@
         :return: A reference to this RegulatingControl for fluent use.
         """
         if self._validate_reference(regulating_cond_eq, self.get_regulating_cond_eq, "A RegulatingCondEq"):
             return self
 
         self._regulating_cond_eq = list() if self._regulating_cond_eq is None else self._regulating_cond_eq
         self._regulating_cond_eq.append(regulating_cond_eq)
+        return self
 
     def remove_regulating_cond_eq(self, regulating_cond_eq: Optional[RegulatingCondEq]) -> RegulatingControl:
         """
         Disassociate this :class:`RegulatingControl` from a :class:`RegulatingCondEq`.
 
-        :param regulating_cond_eq: The RegulatingCondEq to disassociate from this RegulatingControl
+        :param regulating_cond_eq: The RegulatingCondEq to disassociate from this RegulatingControl.
         :return: A reference to this RegulatingControl for fluent use.
         """
         self._regulating_cond_eq = safe_remove(self._regulating_cond_eq, regulating_cond_eq)
         return self
 
     def clear_regulating_cond_eq(self) -> RegulatingControl:
         """
```

## zepben/evolve/model/cim/iec61970/base/wires/regulating_control_mode_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 
 __all__ = ["RegulatingControlModeKind"]
```

## zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional
 
 from zepben.evolve import ShuntCompensatorInfo
```

## zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
 from typing import Union
```

## zepben/evolve/model/cim/iec61970/base/wires/switch.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/base/wires/tap_changer_control.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional
```

## zepben/evolve/model/cim/iec61970/base/wires/transformer_cooling_type.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 
 __all__ = ["TransformerCoolingType"]
```

## zepben/evolve/model/cim/iec61970/base/wires/transformer_star_impedance.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
```

## zepben/evolve/model/cim/iec61970/base/wires/vector_group.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61970/base/wires/winding_connection.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/model/cim/iec61970/base/wires/generation/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/wires/generation/production/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/base/wires/generation/production/battery_state_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 
 __all__ = ["BatteryStateKind"]
```

## zepben/evolve/model/cim/iec61970/base/wires/generation/production/power_electronics_unit.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional
 
 from zepben.evolve.model.cim.iec61970.base.core.equipment import Equipment
```

## zepben/evolve/model/cim/iec61970/infiec61970/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/infiec61970/feeder/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/infiec61970/feeder/circuit.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, Generator, List, TYPE_CHECKING
```

## zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/model/cim/iec61970/infiec61970/protection/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/infiec61970/protection/power_direction_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 
 __all__ = ["PowerDirectionKind"]
```

## zepben/evolve/model/cim/iec61970/infiec61970/protection/protection_kind.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from enum import Enum
 
 __all__ = ["ProtectionKind"]
@@ -10,28 +10,97 @@
 
 class ProtectionKind(Enum):
     """The kind of protection being provided by this protection equipment."""
 
     UNKNOWN = 0
     """Unknown"""
 
-    EF = 1
-    """Earth Fault"""
+    JG = 1
+    """Overcurrent"""
 
-    SEF = 2
-    """Sensitive Earth Fault"""
+    JGG = 2
+    """Instantaneous"""
 
-    OC = 3
-    """Overcurrent"""
+    JGGG = 3
+    """Instantaneous"""
+
+    JT = 4
+    """Thermal overload"""
+
+    J0 = 5
+    """Ground overcurrent"""
+
+    J0GG = 6
+    """Instantaneous ground overcurrent"""
+
+    SEF = 7
+    """Sensitive earth fault"""
+
+    VG = 8
+    """Overvoltage"""
+
+    VGG = 9
+    """Instantaneous overvoltage"""
+
+    VL = 10
+    """Undervoltage"""
+
+    VLL = 11
+    """Instantaneous"""
+
+    V0G = 12
+    """Zero-sequence overvoltage"""
+
+    V0GG = 13
+    """Instantaneous zero-sequence overvoltage"""
+
+    JDIFF = 14
+    """Differential Current"""
+
+    FREQ = 15
+    """Under frequency"""
+
+    FREQG = 16
+    """Over frequency"""
+
+    ZL = 17
+    """Phase distance"""
+
+    Z0L = 18
+    """Ground distance"""
+
+    LE = 19
+    """Load encroachment"""
+
+    J2G = 20
+    """Negative-sequence overcurrent"""
+
+    MULTI_FUNCTION = 21
+    """A multifunctional relay for universal usages"""
+
+    GROUND_CURRENT = 22
+    """A device used to monitor and protect electrical equipment from damage caused by ground faults"""
+
+    GROUND_VOLTAGE = 23
+    """A device used to detect contact accidents between an electric path and ground caused by arc ground faults"""
+
+    NETWORK_PROTECTOR = 24
+    """Is a special self-contained air breaker or switching unit having a full complement of current, potential and control transformers, as well as relay functionality."""
+
+    DISTANCE = 25
+    """A device used to detect faults on long-distance lines, pinpointing not only the fault condition but also measuring the distance between the current sensing mechanism and the fault location in the wire."""
+
+    NEGATIVE_OVERCURRENT = 26
+    """A device used to protect generators from the unbalanced load by detecting negative sequence current."""
 
-    IOC = 4
-    """Instantaneous Overcurrent"""
+    POWER = 27
+    """A device that uses an electromagnet to open or close a circuit when the input (coil) is correctly excited"""
 
-    IEF = 5
-    """Instantaneous Earth Fault"""
+    SECTIONALIZER = 28
+    """A device that automatically isolates a faulted section of line from the rest of the distribution system"""
 
-    REF = 6
-    """Restricted Earth Fault"""
+    AUTO_TRANSFORMER = 29
+    """A device used to regulate the voltage of transmission lines and can also be used to transform voltages."""
 
     @property
     def short_name(self):
         return str(self)[15:]
```

## zepben/evolve/model/cim/iec61970/infiec61970/wires/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/ev_charging_unit.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import PowerElectronicsUnit
```

## zepben/evolve/services/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/common/__init__.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.protobuf.cim.iec61968.common.Document_pb2 import Document as PBDocument
 from zepben.protobuf.cim.iec61968.common.OrganisationRole_pb2 import OrganisationRole as PBOrganisationRole
```

## zepben/evolve/services/common/base_service.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/common/base_service_comparator.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from math import isnan
 from types import MemberDescriptorType
 from typing import get_type_hints, Dict, Type, Callable, Any, TypeVar, Optional, Union, List, Tuple
```

## zepben/evolve/services/common/difference.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from dataclasses import dataclass, field
 from typing import Optional, Any, List, Dict, TypeVar
```

## zepben/evolve/services/common/reference_resolvers.py

```diff
@@ -1,20 +1,19 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
 
 from typing import Callable, Optional
 
 from dataclassy import dataclass
 
-
 from zepben.evolve.model.cim.iec61968.assetinfo.no_load_test import NoLoadTest
 from zepben.evolve.model.cim.iec61968.assetinfo.open_circuit_test import OpenCircuitTest
 from zepben.evolve.model.cim.iec61968.assetinfo.power_transformer_info import PowerTransformerInfo
 from zepben.evolve.model.cim.iec61968.assetinfo.short_circuit_test import ShortCircuitTest
 from zepben.evolve.model.cim.iec61968.assetinfo.shunt_compensator_info import ShuntCompensatorInfo
 from zepben.evolve.model.cim.iec61968.assetinfo.switch_info import SwitchInfo
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_end_info import TransformerEndInfo
@@ -27,44 +26,47 @@
 from zepben.evolve.model.cim.iec61968.common.location import Location
 from zepben.evolve.model.cim.iec61968.common.organisation import Organisation
 from zepben.evolve.model.cim.iec61968.common.organisation_role import OrganisationRole
 from zepben.evolve.model.cim.iec61968.customers.customer import Customer
 from zepben.evolve.model.cim.iec61968.customers.customer_agreement import CustomerAgreement
 from zepben.evolve.model.cim.iec61968.customers.pricing_structure import PricingStructure
 from zepben.evolve.model.cim.iec61968.customers.tariff import Tariff
-from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import CurrentRelayInfo
+from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.relay_info import RelayInfo
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_transformer_info import CurrentTransformerInfo
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.potential_transformer_info import PotentialTransformerInfo
 from zepben.evolve.model.cim.iec61968.metering.metering import EndDevice, UsagePoint
 from zepben.evolve.model.cim.iec61968.operations.operational_restriction import OperationalRestriction
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.auxiliary_equipment import AuxiliaryEquipment
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.current_transformer import CurrentTransformer
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.potential_transformer import PotentialTransformer
+from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.sensor import Sensor
 from zepben.evolve.model.cim.iec61970.base.core.base_voltage import BaseVoltage
 from zepben.evolve.model.cim.iec61970.base.core.conducting_equipment import ConductingEquipment
 from zepben.evolve.model.cim.iec61970.base.core.connectivity_node import ConnectivityNode
 from zepben.evolve.model.cim.iec61970.base.core.equipment import Equipment
 from zepben.evolve.model.cim.iec61970.base.core.equipment_container import Feeder, EquipmentContainer
 from zepben.evolve.model.cim.iec61970.base.core.identified_object import IdentifiedObject
 from zepben.evolve.model.cim.iec61970.base.core.power_system_resource import PowerSystemResource
 from zepben.evolve.model.cim.iec61970.base.core.regions import GeographicalRegion, SubGeographicalRegion
 from zepben.evolve.model.cim.iec61970.base.core.substation import Substation
 from zepben.evolve.model.cim.iec61970.base.core.terminal import Terminal
 from zepben.evolve.model.cim.iec61970.base.diagramlayout.diagram_layout import Diagram, DiagramObject
 from zepben.evolve.model.cim.iec61970.base.meas.control import Control
 from zepben.evolve.model.cim.iec61970.base.meas.measurement import Measurement
-from zepben.evolve.model.cim.iec61970.base.protection.current_relay import CurrentRelay
-from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import ProtectionEquipment
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_function import ProtectionRelayFunction
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_scheme import ProtectionRelayScheme
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_system import ProtectionRelaySystem
 from zepben.evolve.model.cim.iec61970.base.scada.remote_control import RemoteControl
 from zepben.evolve.model.cim.iec61970.base.scada.remote_source import RemoteSource
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import AcLineSegment, Conductor
 from zepben.evolve.model.cim.iec61970.base.wires.energy_connection import RegulatingCondEq
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import EnergyConsumer, EnergyConsumerPhase
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import EnergySource
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source_phase import EnergySourcePhase
+from zepben.evolve.model.cim.iec61970.base.wires.fuse import Fuse
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.power_electronics_unit import PowerElectronicsUnit
 from zepben.evolve.model.cim.iec61970.base.wires.per_length import PerLengthSequenceImpedance
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import PowerElectronicsConnectionPhase, PowerElectronicsConnection
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import PowerTransformer, PowerTransformerEnd, RatioTapChanger, TransformerEnd, TapChanger
 from zepben.evolve.model.cim.iec61970.base.wires.protected_switch import ProtectedSwitch
 from zepben.evolve.model.cim.iec61970.base.wires.regulating_control import RegulatingControl
 from zepben.evolve.model.cim.iec61970.base.wires.shunt_compensator import ShuntCompensator
@@ -87,17 +89,18 @@
     "sgr_to_gr_resolver", "sgr_to_sub_resolver", "sub_to_feeder_resolver", "sub_to_sgr_resolver", "sub_to_circuit_resolver", "sub_to_eloop_resolver",
     "sub_to_loop_resolver", "term_to_ce_resolver", "term_to_cn_resolver", "te_to_term_resolver", "te_to_bv_resolver", "te_to_rtc_resolver", "up_to_ed_resolver",
     "up_to_eq_resolver", "up_to_loc_resolver", "circuit_to_loop_resolver", "circuit_to_sub_resolver", "circuit_to_term_resolver", "loop_to_circuit_resolver",
     "loop_to_esub_resolver", "loop_to_sub_resolver", "BoundReferenceResolver", "ReferenceResolver", "UnresolvedReference", "tei_to_tti_resolver",
     "tti_to_tei_resolver", "tei_to_tsi_resolver", "tsi_to_tei_resolver", "te_to_tsi_resolver", "pti_to_tti_resolver", "peu_to_pec_resolver",
     "pec_to_peu_resolver", "pecphase_to_pec_resolver", "pec_to_pecphase_resolver", "tei_to_ee_nlt_resolver", "tei_to_ee_sct_resolver", "tei_to_ge_sct_resolver",
     "tei_to_oe_oct_resolver", "tei_to_ee_oct_resolver", "shunt_compensator_to_shunt_compensator_info_resolver", "lvfeeder_to_nht_resolver",
-    "lvfeeder_to_nef_resolver", "ct_to_cti_resolver", "vt_to_vti_resolver", "pe_to_ps_resolver", "ps_to_pe_resolver", "switch_to_switch_info_resolver",
-    "current_relay_to_current_relay_info_resolver", "rc_to_rce_resolver", "rce_to_rc_resolver", "rc_to_term_resolver", "tc_to_tcc_resolver"
-]
+    "lvfeeder_to_nef_resolver", "ct_to_cti_resolver", "vt_to_vti_resolver", "prf_to_psw_resolver", "psw_to_prf_resolver", "switch_to_switch_info_resolver",
+    "prf_to_relay_info_resolver", "rc_to_rce_resolver", "rce_to_rc_resolver", "rc_to_term_resolver", "tc_to_tcc_resolver", "prf_to_psw_resolver",
+    "psw_to_prf_resolver", "prf_to_sen_resolver", "sen_to_prf_resolver", "prf_to_prscheme_resolver", "prscheme_to_prf_resolver", "prscheme_to_prsystem_resolver",
+    "prsystem_to_prscheme_resolver", "fuse_to_prf_resolver"]
 
 
 @dataclass(frozen=True, eq=False, slots=True)
 class ReferenceResolver(object):
     from_class: type
     to_class: type
     resolve: Callable[[IdentifiedObject, IdentifiedObject], None]
@@ -187,15 +190,15 @@
 aux_equip_to_term_resolver = ReferenceResolver(AuxiliaryEquipment, Terminal, lambda t, r: setattr(t, 'terminal', r))
 
 cond_equip_to_bv_resolver = ReferenceResolver(ConductingEquipment, BaseVoltage, lambda t, r: setattr(t, 'base_voltage', r))
 cond_equip_to_terminal_resolver = ReferenceResolver(ConductingEquipment, Terminal, _resolve_ce_term)
 
 conductor_to_wire_info_resolver = ReferenceResolver(Conductor, WireInfo, lambda t, r: setattr(t, 'asset_info', r))
 
-current_relay_to_current_relay_info_resolver = ReferenceResolver(CurrentRelay, CurrentRelayInfo, lambda t, r: setattr(t, 'asset_info', r))
+prf_to_relay_info_resolver = ReferenceResolver(ProtectionRelayFunction, RelayInfo, lambda t, r: setattr(t, 'asset_info', r))
 
 powertransformer_to_power_transformer_info_resolver = ReferenceResolver(PowerTransformer, PowerTransformerInfo, lambda t, r: setattr(t, 'asset_info', r))
 
 shunt_compensator_to_shunt_compensator_info_resolver = ReferenceResolver(ShuntCompensator, ShuntCompensatorInfo, lambda t, r: setattr(t, 'asset_info', r))
 
 switch_to_switch_info_resolver = ReferenceResolver(Switch, SwitchInfo, lambda t, r: setattr(t, 'asset_info', r))
 
@@ -310,16 +313,27 @@
 tei_to_oe_oct_resolver = ReferenceResolver(TransformerEndInfo, OpenCircuitTest, lambda t, r: setattr(t, 'open_end_open_circuit_tests', r))
 tei_to_ee_oct_resolver = ReferenceResolver(TransformerEndInfo, OpenCircuitTest, lambda t, r: setattr(t, 'energised_end_open_circuit_tests', r))
 
 # To avoid confusion with PowerTransformer shortened as "pt", PotentialTransformer is shortened to "vt".
 ct_to_cti_resolver = ReferenceResolver(CurrentTransformer, CurrentTransformerInfo, lambda t, r: setattr(t, 'asset_info', r))
 vt_to_vti_resolver = ReferenceResolver(PotentialTransformer, PotentialTransformerInfo, lambda t, r: setattr(t, 'asset_info', r))
 
-pe_to_ps_resolver = ReferenceResolver(ProtectionEquipment, ProtectedSwitch, lambda t, r: t.add_protected_switch(r))
-ps_to_pe_resolver = ReferenceResolver(ProtectedSwitch, ProtectionEquipment, lambda t, r: t.add_operated_by_protection_equipment(r))
+prf_to_psw_resolver = ReferenceResolver(ProtectionRelayFunction, ProtectedSwitch, lambda t, r: t.add_protected_switch(r))
+psw_to_prf_resolver = ReferenceResolver(ProtectedSwitch, ProtectionRelayFunction, lambda t, r: t.add_relay_function(r))
+
+prf_to_sen_resolver = ReferenceResolver(ProtectionRelayFunction, Sensor, lambda t, r: t.add_sensor(r))
+sen_to_prf_resolver = ReferenceResolver(Sensor, ProtectionRelayFunction, lambda t, r: t.add_relay_function(r))
+
+prf_to_prscheme_resolver = ReferenceResolver(ProtectionRelayFunction, ProtectionRelayScheme, lambda t, r: t.add_scheme(r))
+prscheme_to_prf_resolver = ReferenceResolver(ProtectionRelayScheme, ProtectionRelayFunction, lambda t, r: t.add_function(r))
+
+prscheme_to_prsystem_resolver = ReferenceResolver(ProtectionRelayScheme, ProtectionRelaySystem, lambda t, r: setattr(t, 'system', r))
+prsystem_to_prscheme_resolver = ReferenceResolver(ProtectionRelaySystem, ProtectionRelayScheme, lambda t, r: t.add_scheme(r))
+
+fuse_to_prf_resolver = ReferenceResolver(Fuse, ProtectionRelayFunction, lambda t, r: setattr(t, 'function', r))
 
 rce_to_rc_resolver = ReferenceResolver(RegulatingCondEq, RegulatingControl, lambda t, r: setattr(t, 'regulating_control', r))
 rc_to_rce_resolver = ReferenceResolver(RegulatingControl, RegulatingCondEq, lambda t, r: t.add_regulating_cond_eq(r))
 
 rc_to_term_resolver = ReferenceResolver(RegulatingControl, Terminal, lambda t, r: setattr(t, 'terminal', r))
 
 tc_to_tcc_resolver = ReferenceResolver(TapChanger, TapChangerControl, lambda t, r: setattr(t, 'tap_changer_control', r))
```

## zepben/evolve/services/common/resolver.py

```diff
@@ -1,488 +1,523 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
 
 from zepben.evolve import AcLineSegment, Asset, AuxiliaryEquipment, ConductingEquipment, Conductor, PowerTransformer, Pole, Streetlight, ConnectivityNode, \
     Control, Customer, CustomerAgreement, Diagram, DiagramObject, EndDevice, Equipment, EquipmentContainer, EnergyConsumer, EnergyConsumerPhase, EnergySource, \
     EnergySourcePhase, Feeder, GeographicalRegion, Measurement, OperationalRestriction, OrganisationRole, PowerSystemResource, PowerTransformerEnd, \
     PricingStructure, RatioTapChanger, RemoteControl, RemoteSource, SubGeographicalRegion, Substation, Terminal, TransformerEnd, UsagePoint, Circuit, Loop, \
     PowerElectronicsUnit, PowerElectronicsConnectionPhase, PowerElectronicsConnection, TransformerTankInfo, TransformerEndInfo, PowerTransformerInfo, \
-    TransformerStarImpedance, ShuntCompensator, LvFeeder, PotentialTransformer, CurrentTransformer, ProtectionEquipment, ProtectedSwitch, Switch, CurrentRelay, \
-    RegulatingControl, RegulatingCondEq, TapChanger
+    TransformerStarImpedance, ShuntCompensator, LvFeeder, PotentialTransformer, CurrentTransformer, ProtectedSwitch, Switch, RegulatingControl, \
+    RegulatingCondEq, TapChanger, ProtectionRelayFunction, ProtectionRelayScheme, ProtectionRelaySystem, Sensor, Fuse
 from zepben.evolve.services.common.reference_resolvers import *
 
-__all__ = ["per_length_sequence_impedance", "organisation_roles", "at_location", "ae_terminal", "ce_base_voltage", "ce_terminals",
-           "asset_info", "streetlights", "pole", "cn_terminals", "remote_control", "agreements", "customer",
-           "pricing_structures", "power_transformer_info",
-           "diagram_objects", "diagram", "service_location", "ed_usage_points", "containers", "current_containers",
-           "operational_restrictions",
-           "eq_usage_points", "ec_equipment", "ec_phases", "energy_consumer", "es_phases", "energy_source",
-           "normal_energizing_substation", "normal_head_terminal", "sub_geographical_regions", "remote_source",
-           "or_equipment", "organisation",
-           "psr_location", "ends", "power_transformer", "tariffs", "transformer_end", "control", "measurement",
-           "geographical_region", "substations",
-           "normal_energized_feeders", "sub_geographical_region", "conducting_equipment", "connectivity_node",
-           "te_base_voltage", "ratio_tap_changer",
-           "te_terminal", "end_devices", "up_equipment", "usage_point_location", "shunt_compensator_info",
-           "transformer_end_info", "power_transformer_info_transformer_tank_info", "transformer_star_impedance",
-           "star_impedance_transformer_end_info", "transformer_end_transformer_star_impedance", "normal_energized_lv_feeders",
-           "normal_energizing_feeders", "lv_feeder_normal_head_terminal", "normal_energizing_feeders", "protected_switches", "tc_tap_changer_control",
-           "rce_regulating_control", "rc_regulating_cond_eq"]
+__all__ = ["ae_terminal", "agreements", "at_location", "ce_base_voltage", "ce_terminals", "circuits", "cn_terminals", "conducting_equipment",
+           "connectivity_node", "containers", "control", "current_containers", "current_transformer_info", "customer", "diagram", "diagram_objects",
+           "ec_equipment", "ec_phases", "ed_usage_points", "end_devices", "end_substation", "end_terminal", "ends", "energised_end_no_load_tests",
+           "energised_end_open_circuit_tests", "energised_end_short_circuit_tests", "energy_consumer", "energy_source", "eq_usage_points", "es_phases",
+           "fuse_function", "geographical_region", "grounded_end_short_circuit_tests", "loop", "loop_circuits", "loop_energizing_substations",
+           "loop_substations", "loops", "lv_feeder_normal_head_terminal", "measurement", "normal_energized_feeders", "normal_energized_loops",
+           "normal_energized_lv_feeders", "normal_energizing_feeders", "normal_energizing_substation", "normal_head_terminal", "open_end_open_circuit_tests",
+           "operational_restrictions", "or_equipment", "organisation", "organisation_roles", "per_length_sequence_impedance",
+           "phase_power_electronics_connection", "pole", "potential_transformer_info", "power_electronics_connection_phase", "power_electronics_unit",
+           "power_transformer", "power_transformer_info", "power_transformer_info_transformer_tank_info", "prf_protected_switch", "prf_scheme",
+           "prf_sensor", "pricing_structures", "prscheme_function", "prscheme_system", "prsystem_scheme", "ps_relay_function", "psr_location",
+           "ratio_tap_changer", "rc_regulating_cond_eq", "rc_terminal", "rce_regulating_control", "relay_info", "remote_control", "remote_source",
+           "sen_relay_function", "service_location", "shunt_compensator_info", "star_impedance_transformer_end_info", "streetlights",
+           "sub_geographical_region", "sub_geographical_regions", "substations", "switch_info", "tariffs", "tc_tap_changer_control", "te_base_voltage",
+           "te_terminal", "transformer_end", "transformer_end_info", "transformer_end_transformer_star_impedance", "transformer_star_impedance",
+           "transformer_tank_info", "unit_power_electronics_connection", "up_equipment", "usage_point_location", "wire_info"]
 
 
-def per_length_sequence_impedance(ac_line_segment: AcLineSegment):
+def ae_terminal(auxiliary_equipment: AuxiliaryEquipment) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(ac_line_segment, acls_to_plsi_resolver, None)
+    return BoundReferenceResolver(auxiliary_equipment, aux_equip_to_term_resolver, None)
 
 
-def organisation_roles(asset: Asset) -> BoundReferenceResolver:
+def agreements(c: Customer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(asset, asset_to_asset_org_role_resolver, None)
+    return BoundReferenceResolver(c, cust_to_custagr_resolver, custagr_to_cust_resolver)
 
 
 def at_location(asset: Asset) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(asset, asset_to_location_resolver, None)
 
 
-def ae_terminal(auxiliary_equipment: AuxiliaryEquipment) -> BoundReferenceResolver:
-    # noinspection PyArgumentList
-    return BoundReferenceResolver(auxiliary_equipment, aux_equip_to_term_resolver, None)
-
-
 def ce_base_voltage(ce: ConductingEquipment) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(ce, cond_equip_to_bv_resolver, None)
 
 
 def ce_terminals(ce: ConductingEquipment) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(ce, cond_equip_to_terminal_resolver, term_to_ce_resolver)
 
 
-def asset_info(conductor: Conductor) -> BoundReferenceResolver:
-    # noinspection PyArgumentList
-    return BoundReferenceResolver(conductor, conductor_to_wire_info_resolver, None)
-
-
-def current_relay_info(cr: CurrentRelay) -> BoundReferenceResolver:
-    # noinspection PyArgumentList
-    return BoundReferenceResolver(cr, current_relay_to_current_relay_info_resolver, None)
-
-
-def power_transformer_info(pt: PowerTransformer) -> BoundReferenceResolver:
+def circuits(substation: Substation) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(pt, powertransformer_to_power_transformer_info_resolver, None)
+    return BoundReferenceResolver(substation, sub_to_circuit_resolver, circuit_to_sub_resolver)
 
 
-def shunt_compensator_info(sc: ShuntCompensator) -> BoundReferenceResolver:
+def cn_terminals(cn: ConnectivityNode) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(sc, shunt_compensator_to_shunt_compensator_info_resolver, None)
+    return BoundReferenceResolver(cn, conn_node_to_term_resolver, term_to_cn_resolver)
 
 
-def switch_info(switch: Switch) -> BoundReferenceResolver:
+def conducting_equipment(terminal: Terminal) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(switch, switch_to_switch_info_resolver, None)
+    return BoundReferenceResolver(terminal, term_to_ce_resolver, cond_equip_to_terminal_resolver)
 
 
-def streetlights(p: Pole) -> BoundReferenceResolver:
+def connectivity_node(terminal: Terminal) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(p, pole_to_streetlight_resolver, streetlight_to_pole_resolver)
+    return BoundReferenceResolver(terminal, term_to_cn_resolver, conn_node_to_term_resolver)
 
 
-def pole(streetlight: Streetlight) -> BoundReferenceResolver:
+def containers(equipment: Equipment) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(streetlight, streetlight_to_pole_resolver, pole_to_streetlight_resolver)
+    return BoundReferenceResolver(equipment, eq_to_ec_resolver, ec_to_eq_resolver)
 
 
-def cn_terminals(cn: ConnectivityNode) -> BoundReferenceResolver:
+def control(rc: RemoteControl) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(cn, conn_node_to_term_resolver, term_to_cn_resolver)
+    return BoundReferenceResolver(rc, rc_to_cont_resolver, control_to_remote_control_resolver)
 
 
-def remote_control(c: Control) -> BoundReferenceResolver:
+def current_containers(equipment: Equipment) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(c, control_to_remote_control_resolver, rc_to_cont_resolver)
+    return BoundReferenceResolver(equipment, eq_to_curcontainer_resolver, ec_to_curequipment_resolver)
 
 
-def agreements(c: Customer) -> BoundReferenceResolver:
+def current_transformer_info(current_transformer: CurrentTransformer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(c, cust_to_custagr_resolver, custagr_to_cust_resolver)
+    return BoundReferenceResolver(current_transformer, ct_to_cti_resolver, None)
 
 
 def customer(customer_agreement: CustomerAgreement) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(customer_agreement, custagr_to_cust_resolver, cust_to_custagr_resolver)
 
 
-def pricing_structures(customer_agreement: CustomerAgreement) -> BoundReferenceResolver:
+def diagram(diagram_object: DiagramObject) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(customer_agreement, custagr_to_ps_resolver, None)
+    return BoundReferenceResolver(diagram_object, diagobj_to_diag_resolver, diag_to_diagobj_resolver)
 
 
 def diagram_objects(d: Diagram) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(d, diag_to_diagobj_resolver, diagobj_to_diag_resolver)
 
 
-def diagram(diagram_object: DiagramObject) -> BoundReferenceResolver:
+def ec_equipment(equipment_container: EquipmentContainer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(diagram_object, diagobj_to_diag_resolver, diag_to_diagobj_resolver)
+    return BoundReferenceResolver(equipment_container, ec_to_eq_resolver, eq_to_ec_resolver)
 
 
-def service_location(end_device: EndDevice) -> BoundReferenceResolver:
+def ec_phases(ec: EnergyConsumer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(end_device, ed_to_loc_resolver, None)
+    return BoundReferenceResolver(ec, ec_to_ecp_resolver, ecp_to_ec_resolver)
 
 
 def ed_usage_points(end_device: EndDevice) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(end_device, ed_to_up_resolver, up_to_ed_resolver)
 
 
-def containers(equipment: Equipment) -> BoundReferenceResolver:
+def end_devices(usage_point: UsagePoint) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(equipment, eq_to_ec_resolver, ec_to_eq_resolver)
+    return BoundReferenceResolver(usage_point, up_to_ed_resolver, ed_to_up_resolver)
 
 
-def current_containers(equipment: Equipment) -> BoundReferenceResolver:
+def end_substation(circuit: Circuit) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(equipment, eq_to_curcontainer_resolver, ec_to_curequipment_resolver)
+    return BoundReferenceResolver(circuit, circuit_to_sub_resolver, sub_to_circuit_resolver)
 
 
-def operational_restrictions(equipment: Equipment) -> BoundReferenceResolver:
+def end_terminal(circuit: Circuit) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(equipment, eq_to_or_resolver, or_to_eq_resolver)
+    return BoundReferenceResolver(circuit, circuit_to_term_resolver, None)
 
 
-def eq_usage_points(equipment: Equipment) -> BoundReferenceResolver:
+def ends(pt: PowerTransformer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(equipment, eq_to_up_resolver, up_to_eq_resolver)
+    return BoundReferenceResolver(pt, pt_to_pte_resolver, pte_to_pt_resolver)
 
 
-def ec_equipment(equipment_container: EquipmentContainer) -> BoundReferenceResolver:
+def energised_end_no_load_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(equipment_container, ec_to_eq_resolver, eq_to_ec_resolver)
+    return BoundReferenceResolver(tei, tei_to_ee_nlt_resolver, None)
 
 
-def ec_phases(ec: EnergyConsumer) -> BoundReferenceResolver:
+def energised_end_open_circuit_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(ec, ec_to_ecp_resolver, ecp_to_ec_resolver)
+    return BoundReferenceResolver(tei, tei_to_ee_oct_resolver, None)
+
+
+def energised_end_short_circuit_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(tei, tei_to_ee_sct_resolver, None)
 
 
 def energy_consumer(energy_consumer_phase: EnergyConsumerPhase) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(energy_consumer_phase, ecp_to_ec_resolver, ec_to_ecp_resolver)
 
 
+def energy_source(energy_source_phase: EnergySourcePhase) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(energy_source_phase, esp_to_es_resolver, es_to_esp_resolver)
+
+
+def eq_usage_points(equipment: Equipment) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(equipment, eq_to_up_resolver, up_to_eq_resolver)
+
+
 def es_phases(es: EnergySource) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(es, es_to_esp_resolver, esp_to_es_resolver)
 
 
-def energy_source(energy_source_phase: EnergySourcePhase) -> BoundReferenceResolver:
+def fuse_function(fuse: Fuse) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(energy_source_phase, esp_to_es_resolver, es_to_esp_resolver)
+    return BoundReferenceResolver(fuse, fuse_to_prf_resolver, None)
 
 
-def normal_energizing_substation(feeder: Feeder) -> BoundReferenceResolver:
+def geographical_region(sgr: SubGeographicalRegion) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(feeder, feeder_to_nes_resolver, sub_to_feeder_resolver)
+    return BoundReferenceResolver(sgr, sgr_to_gr_resolver, gr_to_sgr_resolver)
 
 
-def normal_head_terminal(feeder: Feeder) -> BoundReferenceResolver:
+def grounded_end_short_circuit_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(feeder, feeder_to_nht_resolver, None)
+    return BoundReferenceResolver(tei, tei_to_ge_sct_resolver, None)
 
 
-def normal_energized_lv_feeders(feeder: Feeder) -> BoundReferenceResolver:
+def loop(circuit: Circuit) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(feeder, feeder_to_nelvf_resolver, lvfeeder_to_nef_resolver)
+    return BoundReferenceResolver(circuit, circuit_to_loop_resolver, loop_to_circuit_resolver)
 
 
-def sub_geographical_regions(gr: GeographicalRegion) -> BoundReferenceResolver:
+def loop_circuits(l_: Loop) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(gr, gr_to_sgr_resolver, sgr_to_gr_resolver)
+    return BoundReferenceResolver(l_, loop_to_circuit_resolver, circuit_to_loop_resolver)
 
 
-def remote_source(m: Measurement) -> BoundReferenceResolver:
+def loop_energizing_substations(l_: Loop) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(m, meas_to_rs_resolver, rs_to_meas_resolver)
+    return BoundReferenceResolver(l_, loop_to_esub_resolver, sub_to_eloop_resolver)
 
 
-def or_equipment(operational_restriction: OperationalRestriction) -> BoundReferenceResolver:
+def loop_substations(l_: Loop) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(operational_restriction, or_to_eq_resolver, eq_to_or_resolver)
+    return BoundReferenceResolver(l_, loop_to_sub_resolver, sub_to_loop_resolver)
 
 
-def organisation(organisation_role: OrganisationRole) -> BoundReferenceResolver:
+def loops(substation: Substation) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(organisation_role, orgr_to_org_resolver, None)
+    return BoundReferenceResolver(substation, sub_to_loop_resolver, loop_to_sub_resolver)
 
 
-def psr_location(power_system_resource: PowerSystemResource) -> BoundReferenceResolver:
+def lv_feeder_normal_head_terminal(lv_feeder: LvFeeder) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(power_system_resource, psr_to_loc_resolver, None)
+    return BoundReferenceResolver(lv_feeder, lvfeeder_to_nht_resolver, None)
 
 
-def ends(pt: PowerTransformer) -> BoundReferenceResolver:
+def measurement(rs: RemoteSource) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(pt, pt_to_pte_resolver, pte_to_pt_resolver)
+    return BoundReferenceResolver(rs, rs_to_meas_resolver, meas_to_rs_resolver)
 
 
-def power_transformer(power_transformer_end: PowerTransformerEnd) -> BoundReferenceResolver:
+def normal_energized_feeders(substation: Substation) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(power_transformer_end, pte_to_pt_resolver, pt_to_pte_resolver)
+    return BoundReferenceResolver(substation, sub_to_feeder_resolver, feeder_to_nes_resolver)
 
 
-def tariffs(pricing_structure: PricingStructure) -> BoundReferenceResolver:
+def normal_energized_loops(substation: Substation) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(pricing_structure, ps_to_tariff_resolver, None)
+    return BoundReferenceResolver(substation, sub_to_eloop_resolver, loop_to_esub_resolver)
 
 
-def transformer_end(rtt: RatioTapChanger) -> BoundReferenceResolver:
+def normal_energized_lv_feeders(feeder: Feeder) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(rtt, rtc_to_te_resolver, te_to_rtc_resolver)
+    return BoundReferenceResolver(feeder, feeder_to_nelvf_resolver, lvfeeder_to_nef_resolver)
 
 
-def control(rc: RemoteControl) -> BoundReferenceResolver:
+def normal_energizing_feeders(lv_feeder: LvFeeder) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(rc, rc_to_cont_resolver, control_to_remote_control_resolver)
+    return BoundReferenceResolver(lv_feeder, lvfeeder_to_nef_resolver, feeder_to_nelvf_resolver)
 
 
-def measurement(rs: RemoteSource) -> BoundReferenceResolver:
+def normal_energizing_substation(feeder: Feeder) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(rs, rs_to_meas_resolver, meas_to_rs_resolver)
+    return BoundReferenceResolver(feeder, feeder_to_nes_resolver, sub_to_feeder_resolver)
 
 
-def geographical_region(sgr: SubGeographicalRegion) -> BoundReferenceResolver:
+def normal_head_terminal(feeder: Feeder) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(sgr, sgr_to_gr_resolver, gr_to_sgr_resolver)
+    return BoundReferenceResolver(feeder, feeder_to_nht_resolver, None)
 
 
-def substations(sgr: SubGeographicalRegion) -> BoundReferenceResolver:
+def open_end_open_circuit_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(sgr, sgr_to_sub_resolver, sub_to_sgr_resolver)
+    return BoundReferenceResolver(tei, tei_to_oe_oct_resolver, None)
 
 
-def normal_energized_feeders(substation: Substation) -> BoundReferenceResolver:
+def operational_restrictions(equipment: Equipment) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(substation, sub_to_feeder_resolver, feeder_to_nes_resolver)
+    return BoundReferenceResolver(equipment, eq_to_or_resolver, or_to_eq_resolver)
 
 
-def sub_geographical_region(substation: Substation) -> BoundReferenceResolver:
+def or_equipment(operational_restriction: OperationalRestriction) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(substation, sub_to_sgr_resolver, sgr_to_sub_resolver)
+    return BoundReferenceResolver(operational_restriction, or_to_eq_resolver, eq_to_or_resolver)
 
 
-def circuits(substation: Substation) -> BoundReferenceResolver:
+def organisation(organisation_role: OrganisationRole) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(substation, sub_to_circuit_resolver, circuit_to_sub_resolver)
+    return BoundReferenceResolver(organisation_role, orgr_to_org_resolver, None)
 
 
-def normal_energized_loops(substation: Substation) -> BoundReferenceResolver:
+def organisation_roles(asset: Asset) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(substation, sub_to_eloop_resolver, loop_to_esub_resolver)
+    return BoundReferenceResolver(asset, asset_to_asset_org_role_resolver, None)
 
 
-def loops(substation: Substation) -> BoundReferenceResolver:
+def per_length_sequence_impedance(ac_line_segment: AcLineSegment):
     # noinspection PyArgumentList
-    return BoundReferenceResolver(substation, sub_to_loop_resolver, loop_to_sub_resolver)
+    return BoundReferenceResolver(ac_line_segment, acls_to_plsi_resolver, None)
 
 
-def conducting_equipment(terminal: Terminal) -> BoundReferenceResolver:
+def phase_power_electronics_connection(pec: PowerElectronicsConnectionPhase) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(terminal, term_to_ce_resolver, cond_equip_to_terminal_resolver)
+    return BoundReferenceResolver(pec, pecphase_to_pec_resolver, pec_to_pecphase_resolver)
 
 
-def connectivity_node(terminal: Terminal) -> BoundReferenceResolver:
+def pole(streetlight: Streetlight) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(terminal, term_to_cn_resolver, conn_node_to_term_resolver)
+    return BoundReferenceResolver(streetlight, streetlight_to_pole_resolver, pole_to_streetlight_resolver)
 
 
-def te_base_voltage(te: TransformerEnd) -> BoundReferenceResolver:
+def potential_transformer_info(potential_transformer: PotentialTransformer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(te, te_to_bv_resolver, None)
+    return BoundReferenceResolver(potential_transformer, vt_to_vti_resolver, None)
 
 
-def ratio_tap_changer(te: TransformerEnd) -> BoundReferenceResolver:
+def power_electronics_connection_phase(pec: PowerElectronicsConnection) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(te, te_to_rtc_resolver, rtc_to_te_resolver)
+    return BoundReferenceResolver(pec, pec_to_pecphase_resolver, pecphase_to_pec_resolver)
 
 
-def te_terminal(te: TransformerEnd) -> BoundReferenceResolver:
+def power_electronics_unit(pec: PowerElectronicsConnection) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(te, te_to_term_resolver, None)
+    return BoundReferenceResolver(pec, pec_to_peu_resolver, peu_to_pec_resolver)
 
 
-def end_devices(usage_point: UsagePoint) -> BoundReferenceResolver:
+def power_transformer(power_transformer_end: PowerTransformerEnd) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(usage_point, up_to_ed_resolver, ed_to_up_resolver)
+    return BoundReferenceResolver(power_transformer_end, pte_to_pt_resolver, pt_to_pte_resolver)
 
 
-def up_equipment(usage_point: UsagePoint) -> BoundReferenceResolver:
+def power_transformer_info(pt: PowerTransformer) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(usage_point, up_to_eq_resolver, eq_to_up_resolver)
+    return BoundReferenceResolver(pt, powertransformer_to_power_transformer_info_resolver, None)
 
 
-def usage_point_location(usage_point: UsagePoint) -> BoundReferenceResolver:
+def power_transformer_info_transformer_tank_info(pti: PowerTransformerInfo) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(usage_point, up_to_loc_resolver, None)
+    return BoundReferenceResolver(pti, pti_to_tti_resolver, None)
 
 
-def loop(circuit: Circuit) -> BoundReferenceResolver:
+def prf_protected_switch(prf: ProtectionRelayFunction) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(circuit, circuit_to_loop_resolver, loop_to_circuit_resolver)
+    return BoundReferenceResolver(prf, prf_to_psw_resolver, psw_to_prf_resolver)
 
 
-def end_terminal(circuit: Circuit) -> BoundReferenceResolver:
+def prf_scheme(prf: ProtectionRelayFunction) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(circuit, circuit_to_term_resolver, None)
+    return BoundReferenceResolver(prf, prf_to_prscheme_resolver, prscheme_to_prf_resolver)
 
 
-def end_substation(circuit: Circuit) -> BoundReferenceResolver:
+def prf_sensor(prf: ProtectionRelayFunction) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(circuit, circuit_to_sub_resolver, sub_to_circuit_resolver)
+    return BoundReferenceResolver(prf, prf_to_sen_resolver, sen_to_prf_resolver)
 
 
-def loop_circuits(l_: Loop) -> BoundReferenceResolver:
+def pricing_structures(customer_agreement: CustomerAgreement) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(l_, loop_to_circuit_resolver, circuit_to_loop_resolver)
+    return BoundReferenceResolver(customer_agreement, custagr_to_ps_resolver, None)
 
 
-def loop_substations(l_: Loop) -> BoundReferenceResolver:
+def prscheme_function(prscheme: ProtectionRelayScheme) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(l_, loop_to_sub_resolver, sub_to_loop_resolver)
+    return BoundReferenceResolver(prscheme, prscheme_to_prf_resolver, prf_to_prscheme_resolver)
 
 
-def loop_energizing_substations(l_: Loop) -> BoundReferenceResolver:
+def prscheme_system(prscheme: ProtectionRelayScheme) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(l_, loop_to_esub_resolver, sub_to_eloop_resolver)
+    return BoundReferenceResolver(prscheme, prscheme_to_prsystem_resolver, prsystem_to_prscheme_resolver)
 
 
-def lv_feeder_normal_head_terminal(lv_feeder: LvFeeder) -> BoundReferenceResolver:
+def prsystem_scheme(prsystem: ProtectionRelaySystem) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(lv_feeder, lvfeeder_to_nht_resolver, None)
+    return BoundReferenceResolver(prsystem, prsystem_to_prscheme_resolver, prscheme_to_prsystem_resolver)
 
 
-def normal_energizing_feeders(lv_feeder: LvFeeder) -> BoundReferenceResolver:
+def ps_relay_function(ps: ProtectedSwitch) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(lv_feeder, lvfeeder_to_nef_resolver, feeder_to_nelvf_resolver)
+    return BoundReferenceResolver(ps, psw_to_prf_resolver, prf_to_psw_resolver)
 
 
-def unit_power_electronics_connection(pec: PowerElectronicsUnit) -> BoundReferenceResolver:
+def psr_location(power_system_resource: PowerSystemResource) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(pec, peu_to_pec_resolver, pec_to_peu_resolver)
+    return BoundReferenceResolver(power_system_resource, psr_to_loc_resolver, None)
 
 
-def phase_power_electronics_connection(pec: PowerElectronicsConnectionPhase) -> BoundReferenceResolver:
+def ratio_tap_changer(te: TransformerEnd) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(pec, pecphase_to_pec_resolver, pec_to_pecphase_resolver)
+    return BoundReferenceResolver(te, te_to_rtc_resolver, rtc_to_te_resolver)
 
 
-def power_electronics_unit(pec: PowerElectronicsConnection) -> BoundReferenceResolver:
+def rc_regulating_cond_eq(regulating_control: RegulatingControl) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(pec, pec_to_peu_resolver, peu_to_pec_resolver)
+    return BoundReferenceResolver(regulating_control, rc_to_rce_resolver, rce_to_rc_resolver)
 
 
-def power_electronics_connection_phase(pec: PowerElectronicsConnection) -> BoundReferenceResolver:
+def rc_terminal(rc: RegulatingControl) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(pec, pec_to_pecphase_resolver, pecphase_to_pec_resolver)
+    return BoundReferenceResolver(rc, rc_to_term_resolver, None)
 
 
-def transformer_end_info(tti: TransformerTankInfo) -> BoundReferenceResolver:
+def rce_regulating_control(regulating_cond_eq: RegulatingCondEq) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tti, tti_to_tei_resolver, tei_to_tti_resolver)
+    return BoundReferenceResolver(regulating_cond_eq, rce_to_rc_resolver, rc_to_rce_resolver)
 
 
-def transformer_tank_info(tei: TransformerEndInfo) -> BoundReferenceResolver:
+def relay_info(prf: ProtectionRelayFunction) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tei, tei_to_tti_resolver, tti_to_tei_resolver)
+    return BoundReferenceResolver(prf, prf_to_relay_info_resolver, None)
 
 
-def power_transformer_info_transformer_tank_info(pti: PowerTransformerInfo) -> BoundReferenceResolver:
+def remote_control(c: Control) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(pti, pti_to_tti_resolver, None)
+    return BoundReferenceResolver(c, control_to_remote_control_resolver, rc_to_cont_resolver)
 
 
-def transformer_star_impedance(tei: TransformerEndInfo) -> BoundReferenceResolver:
+def remote_source(m: Measurement) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tei, tei_to_tsi_resolver, tsi_to_tei_resolver)
+    return BoundReferenceResolver(m, meas_to_rs_resolver, rs_to_meas_resolver)
+
+
+def sen_relay_function(sen: Sensor) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(sen, sen_to_prf_resolver, prf_to_sen_resolver)
+
+
+def service_location(end_device: EndDevice) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(end_device, ed_to_loc_resolver, None)
+
+
+def shunt_compensator_info(sc: ShuntCompensator) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(sc, shunt_compensator_to_shunt_compensator_info_resolver, None)
 
 
 def star_impedance_transformer_end_info(tsi: TransformerStarImpedance) -> BoundReferenceResolver:
     # noinspection PyArgumentList
     return BoundReferenceResolver(tsi, tsi_to_tei_resolver, tei_to_tsi_resolver)
 
 
-def transformer_end_transformer_star_impedance(te: TransformerEnd) -> BoundReferenceResolver:
+def streetlights(p: Pole) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(te, te_to_tsi_resolver, None)
+    return BoundReferenceResolver(p, pole_to_streetlight_resolver, streetlight_to_pole_resolver)
 
 
-def energised_end_no_load_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
+def sub_geographical_region(substation: Substation) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tei, tei_to_ee_nlt_resolver, None)
+    return BoundReferenceResolver(substation, sub_to_sgr_resolver, sgr_to_sub_resolver)
 
 
-def energised_end_short_circuit_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
+def sub_geographical_regions(gr: GeographicalRegion) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tei, tei_to_ee_sct_resolver, None)
+    return BoundReferenceResolver(gr, gr_to_sgr_resolver, sgr_to_gr_resolver)
 
 
-def grounded_end_short_circuit_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
+def substations(sgr: SubGeographicalRegion) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tei, tei_to_ge_sct_resolver, None)
+    return BoundReferenceResolver(sgr, sgr_to_sub_resolver, sub_to_sgr_resolver)
 
 
-def open_end_open_circuit_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
+def switch_info(switch: Switch) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tei, tei_to_oe_oct_resolver, None)
+    return BoundReferenceResolver(switch, switch_to_switch_info_resolver, None)
 
 
-def energised_end_open_circuit_tests(tei: TransformerEndInfo) -> BoundReferenceResolver:
+def tariffs(pricing_structure: PricingStructure) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tei, tei_to_ee_oct_resolver, None)
+    return BoundReferenceResolver(pricing_structure, ps_to_tariff_resolver, None)
 
 
-def current_transformer_info(current_transformer: CurrentTransformer) -> BoundReferenceResolver:
+def tc_tap_changer_control(tap_changer: TapChanger) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(current_transformer, ct_to_cti_resolver, None)
+    return BoundReferenceResolver(tap_changer, tc_to_tcc_resolver, None)
 
 
-def potential_transformer_info(potential_transformer: PotentialTransformer) -> BoundReferenceResolver:
+def te_base_voltage(te: TransformerEnd) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(potential_transformer, vt_to_vti_resolver, None)
+    return BoundReferenceResolver(te, te_to_bv_resolver, None)
 
 
-def protected_switches(protection_equipment: ProtectionEquipment) -> BoundReferenceResolver:
+def te_terminal(te: TransformerEnd) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(protection_equipment, pe_to_ps_resolver, ps_to_pe_resolver)
+    return BoundReferenceResolver(te, te_to_term_resolver, None)
 
 
-def operated_by_protection_equipment(protected_switch: ProtectedSwitch) -> BoundReferenceResolver:
+def transformer_end(rtt: RatioTapChanger) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(protected_switch, ps_to_pe_resolver, pe_to_ps_resolver)
+    return BoundReferenceResolver(rtt, rtc_to_te_resolver, te_to_rtc_resolver)
 
-def rc_regulating_cond_eq(regulating_control: RegulatingControl) -> BoundReferenceResolver:
+
+def transformer_end_info(tti: TransformerTankInfo) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(regulating_control, rc_to_rce_resolver, rce_to_rc_resolver)
+    return BoundReferenceResolver(tti, tti_to_tei_resolver, tei_to_tti_resolver)
 
 
-def rce_regulating_control(regulating_cond_eq: RegulatingCondEq) -> BoundReferenceResolver:
+def transformer_end_transformer_star_impedance(te: TransformerEnd) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(regulating_cond_eq, rce_to_rc_resolver, rc_to_rce_resolver)
+    return BoundReferenceResolver(te, te_to_tsi_resolver, None)
 
 
-def tc_tap_changer_control(tap_changer: TapChanger) -> BoundReferenceResolver:
+def transformer_star_impedance(tei: TransformerEndInfo) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(tap_changer, tc_to_tcc_resolver, None)
+    return BoundReferenceResolver(tei, tei_to_tsi_resolver, tsi_to_tei_resolver)
 
 
-def rc_terminal(rc: RegulatingControl) -> BoundReferenceResolver:
+def transformer_tank_info(tei: TransformerEndInfo) -> BoundReferenceResolver:
     # noinspection PyArgumentList
-    return BoundReferenceResolver(rc, rc_to_term_resolver, None)
+    return BoundReferenceResolver(tei, tei_to_tti_resolver, tti_to_tei_resolver)
+
+
+def unit_power_electronics_connection(pec: PowerElectronicsUnit) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(pec, peu_to_pec_resolver, pec_to_peu_resolver)
+
+
+def up_equipment(usage_point: UsagePoint) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(usage_point, up_to_eq_resolver, eq_to_up_resolver)
+
+
+def usage_point_location(usage_point: UsagePoint) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(usage_point, up_to_loc_resolver, None)
+
+
+def wire_info(conductor: Conductor) -> BoundReferenceResolver:
+    # noinspection PyArgumentList
+    return BoundReferenceResolver(conductor, conductor_to_wire_info_resolver, None)
```

## zepben/evolve/services/common/meta/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/common/meta/data_source.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from datetime import datetime
```

## zepben/evolve/services/common/meta/metadata_collection.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List, Generator
 
 from dataclassy import dataclass
```

## zepben/evolve/services/common/meta/metadata_translations.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from google.protobuf.timestamp_pb2 import Timestamp as PBTimestamp
 from zepben.protobuf.metadata.metadata_data_pb2 import DataSource as PBDataSource
 from zepben.protobuf.metadata.metadata_data_pb2 import ServiceInfo as PBServiceInfo
```

## zepben/evolve/services/common/meta/service_info.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 from dataclassy import dataclass
 from typing import TYPE_CHECKING, List
```

## zepben/evolve/services/common/translator/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/common/translator/base_cim2proto.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
```

## zepben/evolve/services/common/translator/base_proto2cim.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from abc import ABCMeta
 from typing import Optional
```

## zepben/evolve/services/common/translator/service_differences.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Callable, Optional, Set, Dict, Generator, Tuple, Any, Iterable
 
 from zepben.evolve import IdentifiedObject
```

## zepben/evolve/services/common/translator/util.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Optional, Dict
 
 # noinspection PyPackageRequirements
```

## zepben/evolve/services/customer/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/customer/customer_service_comparator.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from zepben.evolve import BaseServiceComparator, ObjectDifference, Customer, CustomerAgreement, PricingStructure, Tariff
```

## zepben/evolve/services/customer/customers.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve.services.common.base_service import BaseService
```

## zepben/evolve/services/customer/translator/__init__.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.protobuf.cim.iec61968.common.Agreement_pb2 import Agreement
 from zepben.protobuf.cim.iec61968.customers.CustomerAgreement_pb2 import CustomerAgreement
```

## zepben/evolve/services/customer/translator/customer_cim2proto.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.protobuf.cim.iec61968.common.Agreement_pb2 import Agreement as PBAgreement
 from zepben.protobuf.cim.iec61968.customers.CustomerAgreement_pb2 import CustomerAgreement as PBCustomerAgreement
```

## zepben/evolve/services/customer/translator/customer_proto2cim.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/diagram/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/diagram/diagram_service_comparator.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from zepben.evolve import BaseServiceComparator, ObjectDifference, Diagram, DiagramObject
```

## zepben/evolve/services/diagram/diagrams.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import Dict, List
```

## zepben/evolve/services/diagram/translator/__init__.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.protobuf.cim.iec61970.base.diagramlayout.DiagramObject_pb2 import DiagramObject
 from zepben.protobuf.cim.iec61970.base.diagramlayout.Diagram_pb2 import Diagram
```

## zepben/evolve/services/diagram/translator/diagram_cim2proto.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.protobuf.cim.iec61970.base.diagramlayout.DiagramObjectPoint_pb2 import DiagramObjectPoint as PBDiagramObjectPoint
 from zepben.protobuf.cim.iec61970.base.diagramlayout.DiagramObject_pb2 import DiagramObject as PBDiagramObject
```

## zepben/evolve/services/diagram/translator/diagram_proto2cim.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.protobuf.cim.iec61970.base.diagramlayout.DiagramObjectPoint_pb2 import DiagramObjectPoint as PBDiagramObjectPoint
 from zepben.protobuf.cim.iec61970.base.diagramlayout.DiagramObject_pb2 import DiagramObject as PBDiagramObject
```

## zepben/evolve/services/measurement/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/measurement/measurements.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import List, Optional, Generator, TYPE_CHECKING
```

## zepben/evolve/services/measurement/translator/__init__.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 __all__ = []
```

## zepben/evolve/services/measurement/translator/measurement_cim2proto.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from zepben.protobuf.cim.iec61970.base.meas.MeasurementValue_pb2 import MeasurementValue as PBMeasurementValue
 from zepben.protobuf.cim.iec61970.base.meas.AccumulatorValue_pb2 import AccumulatorValue as PBAccumulatorValue
 from zepben.protobuf.cim.iec61970.base.meas.AnalogValue_pb2 import AnalogValue as PBAnalogValue
```

## zepben/evolve/services/measurement/translator/measurement_proto2cim.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.protobuf.cim.iec61970.base.meas.MeasurementValue_pb2 import MeasurementValue as PBMeasurementValue
 from zepben.protobuf.cim.iec61970.base.meas.AccumulatorValue_pb2 import AccumulatorValue as PBAccumulatorValue
```

## zepben/evolve/services/network/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/network/network_extensions.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
```

## zepben/evolve/services/network/network_service.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/network_service_comparator.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https:#mozilla.org/MPL/2.0/.
 from dataclasses import dataclass
 from typing import Callable, Optional, Any
 
@@ -11,15 +11,16 @@
     AuxiliaryEquipment, FaultIndicator, BaseVoltage, ConductingEquipment, ConnectivityNode, Equipment, EquipmentContainer, Feeder, GeographicalRegion, \
     PowerSystemResource, Site, SubGeographicalRegion, Substation, Terminal, PowerElectronicsUnit, BatteryUnit, PhotoVoltaicUnit, PowerElectronicsWindUnit, \
     Breaker, LoadBreakSwitch, BusbarSection, Conductor, Disconnector, EnergyConsumer, EnergyConsumerPhase, EnergySource, EnergySourcePhase, Fuse, Jumper, \
     Junction, LinearShuntCompensator, PerLengthSequenceImpedance, PowerElectronicsConnection, PowerElectronicsConnectionPhase, PowerTransformer, \
     PowerTransformerEnd, RatioTapChanger, Recloser, RegulatingCondEq, ShuntCompensator, TapChanger, TransformerEnd, TransformerStarImpedance, Circuit, \
     Loop, SinglePhaseKind, ValueDifference, PhaseCode, Control, Measurement, Analog, Accumulator, Discrete, RemoteControl, RemoteSource, EquivalentBranch, \
     Switch, ShuntCompensatorInfo, LvFeeder, CurrentTransformerInfo, PotentialTransformerInfo, CurrentTransformer, PotentialTransformer, SwitchInfo, \
-    CurrentRelayInfo, CurrentRelay, ProtectionEquipment, ProtectedSwitch, EvChargingUnit, RegulatingControl, TapChangerControl
+    RelayInfo, CurrentRelay, ProtectedSwitch, EvChargingUnit, RegulatingControl, TapChangerControl, ProtectionRelayFunction, DistanceRelay, VoltageRelay, \
+    ProtectionRelayScheme, ProtectionRelaySystem, Sensor, Ground, GroundDisconnector, SeriesCompensator
 from zepben.evolve.services.common.base_service_comparator import BaseServiceComparator
 from zepben.evolve.services.common.translator.service_differences import ObjectDifference
 
 
 @dataclass
 class NetworkServiceComparatorOptions:
     compare_terminals: bool = True
@@ -225,19 +226,19 @@
 
         return self._compare_identified_object(diff)
 
     #####################################
     # IEC61968 infIEC61968 InfAssetInfo #
     #####################################
 
-    def _compare_current_relay_info(self, source: CurrentRelayInfo, target: CurrentRelayInfo) -> ObjectDifference:
+    def _compare_relay_info(self, source: RelayInfo, target: RelayInfo) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
-        self._compare_values(diff, CurrentRelayInfo.curve_setting)
-        self._compare_indexed_value_collections(diff, CurrentRelayInfo.reclose_delays)
+        self._compare_values(diff, RelayInfo.curve_setting, RelayInfo.reclose_fast)
+        self._compare_indexed_value_collections(diff, RelayInfo.reclose_delays)
 
         return self._compare_asset_info(diff)
 
     def _compare_current_transformer_info(self, source: CurrentTransformerInfo, target: CurrentTransformerInfo) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_values(
@@ -327,28 +328,32 @@
 
         return self._compare_equipment(diff)
 
     def _compare_current_transformer(self, source: CurrentTransformer, target: CurrentTransformer) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_values(diff, CurrentTransformer.core_burden)
+        self._compare_id_references(diff, CurrentTransformer.current_transformer_info)
 
         return self._compare_sensor(diff)
 
     def _compare_fault_indicator(self, source: FaultIndicator, target: FaultIndicator) -> ObjectDifference:
         return self._compare_auxiliary_equipment(ObjectDifference(source, target))
 
     def _compare_potential_transformer(self, source: PotentialTransformer, target: PotentialTransformer) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_values(diff, PotentialTransformer.type)
+        self._compare_id_references(diff, PotentialTransformer.potential_transformer_info)
 
         return self._compare_sensor(diff)
 
     def _compare_sensor(self, diff: ObjectDifference) -> ObjectDifference:
+        self._compare_id_reference_collections(diff, Sensor.relay_functions)
+
         return self._compare_auxiliary_equipment(diff)
 
     ######################
     # IEC61970 BASE CORE #
     ######################
 
     def _compare_ac_dc_terminal(self, diff: ObjectDifference) -> ObjectDifference:
@@ -525,20 +530,76 @@
 
     def _compare_current_relay(self, source: CurrentRelay, target: CurrentRelay) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_values(diff, CurrentRelay.inverse_time_flag)
         self._compare_floats(diff, CurrentRelay.current_limit_1, CurrentRelay.time_delay_1)
 
-        return self._compare_protection_equipment(diff)
+        return self._compare_protection_relay_function(diff)
+
+    def _compare_distance_relay(self, source: DistanceRelay, target: DistanceRelay) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+
+        self._compare_floats(
+            diff,
+            DistanceRelay.backward_blind,
+            DistanceRelay.backward_reach,
+            DistanceRelay.backward_reactance,
+            DistanceRelay.forward_blind,
+            DistanceRelay.forward_reach,
+            DistanceRelay.forward_reactance,
+            DistanceRelay.operation_phase_angle1,
+            DistanceRelay.operation_phase_angle2,
+            DistanceRelay.operation_phase_angle3,
+        )
+
+        return self._compare_protection_relay_function(diff)
+
+    def _compare_voltage_relay(self, source: VoltageRelay, target: VoltageRelay) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+
+        return self._compare_protection_relay_function(diff)
 
-    def _compare_protection_equipment(self, diff: ObjectDifference) -> ObjectDifference:
-        self._compare_values(diff, ProtectionEquipment.protection_kind, ProtectionEquipment.directable, ProtectionEquipment.power_direction)
-        self._compare_floats(diff, ProtectionEquipment.relay_delay_time)
-        self._compare_id_reference_collections(diff, ProtectionEquipment.protected_switches)
+    def _compare_protection_relay_function(self, diff: ObjectDifference) -> ObjectDifference:
+        self._compare_values(
+            diff,
+            ProtectionRelayFunction.model,
+            ProtectionRelayFunction.reclosing,
+            ProtectionRelayFunction.protection_kind,
+            ProtectionRelayFunction.directable,
+            ProtectionRelayFunction.power_direction
+        )
+        self._compare_floats(diff, ProtectionRelayFunction.relay_delay_time)
+        self._compare_indexed_value_collections(
+            diff,
+            ProtectionRelayFunction.time_limits,
+            ProtectionRelayFunction.thresholds
+        )
+        self._compare_id_reference_collections(
+            diff,
+            ProtectionRelayFunction.protected_switches,
+            ProtectionRelayFunction.sensors,
+            ProtectionRelayFunction.schemes,
+        )
+        self._compare_id_references(diff, ProtectionRelayFunction.relay_info)
+
+        return self._compare_power_system_resource(diff)
+
+    def _compare_protection_relay_scheme(self, source: ProtectionRelayScheme, target: ProtectionRelayScheme) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+        self._compare_id_references(diff, ProtectionRelayScheme.system)
+        self._compare_id_reference_collections(diff, ProtectionRelayScheme.functions)
+
+        return self._compare_identified_object(diff)
+
+    def _compare_protection_relay_system(self, source: ProtectionRelaySystem, target: ProtectionRelaySystem) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+
+        self._compare_values(diff, ProtectionRelaySystem.protection_kind)
+        self._compare_id_reference_collections(diff, ProtectionRelaySystem.schemes)
 
         return self._compare_equipment(diff)
 
     #######################
     # IEC61970 BASE SCADA #
     #######################
 
@@ -601,14 +662,15 @@
         return self._compare_protected_switch(diff)
 
     def _compare_busbar_section(self, source: BusbarSection, target: BusbarSection) -> ObjectDifference:
         return self._compare_connector(ObjectDifference(source, target))
 
     def _compare_conductor(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_floats(diff, Conductor.length)
+        self._compare_id_references(diff, Conductor.wire_info)
 
         return self._compare_conducting_equipment(diff)
 
     def _compare_connector(self, diff: ObjectDifference) -> ObjectDifference:
         return self._compare_conducting_equipment(diff)
 
     def _compare_disconnector(self, source: Disconnector, target: Disconnector) -> ObjectDifference:
@@ -678,14 +740,22 @@
 
         self._compare_id_references(diff, EnergySourcePhase.energy_source)
         self._compare_values(diff, EnergySourcePhase.phase)
 
         return self._compare_power_system_resource(diff)
 
     def _compare_fuse(self, source: Fuse, target: Fuse) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+        self._compare_id_references(diff, Fuse.function)
+        return self._compare_switch(diff)
+
+    def _compare_ground(self, source: Ground, target: Ground) -> ObjectDifference:
+        return self._compare_conducting_equipment(ObjectDifference(source, target))
+
+    def _compare_compare_ground_disconnector(self, source: GroundDisconnector, target: GroundDisconnector) -> ObjectDifference:
         return self._compare_switch(ObjectDifference(source, target))
 
     def _compare_jumper(self, source: Jumper, target: Jumper) -> ObjectDifference:
         return self._compare_switch(ObjectDifference(source, target))
 
     def _compare_junction(self, source: Junction, target: Junction) -> ObjectDifference:
         return self._compare_connector(ObjectDifference(source, target))
@@ -787,14 +857,15 @@
 
     def _compare_power_transformer(self, source: PowerTransformer, target: PowerTransformer) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_indexed_id_reference_collections(diff, PowerTransformer.ends)
         self._compare_values(diff, PowerTransformer.vector_group, PowerTransformer.construction_kind, PowerTransformer.function)
         self._compare_floats(diff, PowerTransformer.transformer_utilisation)
+        self._compare_id_references(diff, PowerTransformer.power_transformer_info)
 
         return self._compare_conducting_equipment(diff)
 
     def _compare_power_transformer_end(self, source: PowerTransformerEnd, target: PowerTransformerEnd) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_id_references(diff, PowerTransformerEnd.power_transformer)
@@ -818,15 +889,15 @@
         )
         self._compare_indexed_value_collections(diff, PowerTransformerEnd.s_ratings)
 
         return self._compare_transformer_end(diff)
 
     def _compare_protected_switch(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_values(diff, ProtectedSwitch.breaking_capacity)
-        self._compare_id_reference_collections(diff, ProtectedSwitch.operated_by_protection_equipment)
+        self._compare_id_reference_collections(diff, ProtectedSwitch.relay_functions)
 
         return self._compare_switch(diff)
 
     def _compare_ratio_tap_changer(self, source: RatioTapChanger, target: RatioTapChanger) -> ObjectDifference:
         diff = ObjectDifference(source, target)
 
         self._compare_id_references(diff, RatioTapChanger.transformer_end)
@@ -852,31 +923,41 @@
             RegulatingControl.enabled
         )
         self._compare_floats(
             diff,
             RegulatingControl.target_deadband,
             RegulatingControl.target_value,
             RegulatingControl.max_allowed_target_value,
-            RegulatingControl.min_allowed_target_value
+            RegulatingControl.min_allowed_target_value,
+            RegulatingControl.rated_current
         )
         self._compare_id_references(diff, RegulatingControl.terminal)
         self._compare_id_reference_collections(diff, RegulatingControl.regulating_conducting_equipment)
 
         return self._compare_power_system_resource(diff)
 
+    def _compare_series_compensator(self, source: SeriesCompensator, target: SeriesCompensator) -> ObjectDifference:
+        diff = ObjectDifference(source, target)
+        self._compare_values(diff, SeriesCompensator.varistor_rated_current, SeriesCompensator.varistor_voltage_threshold)
+        self._compare_floats(diff, SeriesCompensator.r, SeriesCompensator.r0, SeriesCompensator.x, SeriesCompensator.x0)
+
+        return self._compare_conducting_equipment(diff)
+
     def _compare_shunt_compensator(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_values(diff, ShuntCompensator.grounded, ShuntCompensator.nom_u, ShuntCompensator.phase_connection)
         self._compare_floats(diff, ShuntCompensator.sections)
+        self._compare_id_references(diff, ShuntCompensator.shunt_compensator_info)
 
         return self._compare_regulating_cond_eq(diff)
 
     def _compare_switch(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_floats(diff, Switch.rated_current)
         self._add_if_different(diff, "isNormallyOpen", self._compare_open_status(diff, Switch.is_normally_open))
         self._add_if_different(diff, "isOpen", self._compare_open_status(diff, Switch.is_open))
+        self._compare_id_references(diff, Switch.switch_info)
 
         return self._compare_conducting_equipment(diff)
 
     def _compare_tap_changer(self, diff: ObjectDifference) -> ObjectDifference:
         self._compare_values(
             diff,
             TapChanger.control_enabled,
```

## zepben/evolve/services/network/tracing/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/network/tracing/find.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 from dataclassy import dataclass
 from typing import TYPE_CHECKING
```

## zepben/evolve/services/network/tracing/find_swer_equipment.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https:#mozilla.org/MPL/2.0/.
 from typing import Callable, Set, Union, Optional
 
 from zepben.evolve import ConnectedEquipmentTraversal, ConductingEquipmentStep, NetworkService, ConductingEquipment, Feeder, PowerTransformer, Switch, \
```

## zepben/evolve/services/network/tracing/tracing.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, TypeVar
```

## zepben/evolve/services/network/tracing/util.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/tracing/connectivity/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from dataclassy import dataclass
 
 from zepben.evolve import ConductingEquipment
```

## zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step_tracker.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Dict
```

## zepben/evolve/services/network/tracing/connectivity/connected_equipment_trace.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
```

## zepben/evolve/services/network/tracing/connectivity/connected_equipment_traversal.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.evolve import BasicTraversal, ConductingEquipmentStep, ConductingEquipment
```

## zepben/evolve/services/network/tracing/connectivity/connectivity_result.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/tracing/connectivity/connectivity_trace.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
```

## zepben/evolve/services/network/tracing/connectivity/connectivity_tracker.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Set, TYPE_CHECKING
```

## zepben/evolve/services/network/tracing/connectivity/limited_connected_equipment_trace.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import Callable, List, Dict, Optional
```

## zepben/evolve/services/network/tracing/connectivity/phase_paths.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Dict, List
 
 from zepben.evolve import SinglePhaseKind, PhaseCode, NominalPhasePath
```

## zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_connected.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List, Iterable, Optional, Set, Dict, Callable
 
 from zepben.evolve import Terminal, PhaseCode, SinglePhaseKind, NominalPhasePath, Queue, LifoQueue, Switch
```

## zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_internal.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Set, Optional
 
 from zepben.evolve import Terminal, PowerTransformer, SinglePhaseKind, ConnectivityResult, NominalPhasePath
```

## zepben/evolve/services/network/tracing/connectivity/transformer_phase_paths.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Dict, List
 
 from zepben.evolve import SinglePhaseKind as Phase, NominalPhasePath, PhaseCode
```

## zepben/evolve/services/network/tracing/connectivity/xy_candidate_phase_paths.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from collections import Counter
 from itertools import takewhile
 from typing import List, Dict, Tuple, Optional, Counter as CounterType
```

## zepben/evolve/services/network/tracing/connectivity/xy_phase_step.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 __all__ = ["XyPhaseStep"]
```

## zepben/evolve/services/network/tracing/feeder/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Set, Callable, Optional, Awaitable, Any
 
 from zepben.evolve import BasicTraversal
```

## zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Set, Callable, Optional, Awaitable, Any
 
 from zepben.evolve import BasicTraversal
```

## zepben/evolve/services/network/tracing/feeder/associated_terminal_trace.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import Callable, Optional, Set, List
 
 from zepben.evolve import BasicTraversal
```

## zepben/evolve/services/network/tracing/feeder/associated_terminal_tracker.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import Optional
```

## zepben/evolve/services/network/tracing/feeder/direction_status.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 __all__ = ["normal_direction", "current_direction", "DirectionStatus", "NormalDirection", "CurrentDirection"]
```

## zepben/evolve/services/network/tracing/feeder/feeder_direction.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from enum import Enum
```

## zepben/evolve/services/network/tracing/feeder/remove_direction.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from dataclassy import dataclass
 
 from zepben.evolve import FifoQueue, normal_direction, BranchRecursiveTraversal, current_direction, NetworkService, Terminal, FeederDirection
```

## zepben/evolve/services/network/tracing/feeder/set_direction.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List, Callable, Optional
 
 from zepben.evolve import BranchRecursiveTraversal, Terminal, FifoQueue, NetworkService, Feeder, FeederDirection, normally_open, \
```

## zepben/evolve/services/network/tracing/phases/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/network/tracing/phases/phase_inferrer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import logging
 from typing import Dict, Callable, List, Set, Awaitable
```

## zepben/evolve/services/network/tracing/phases/phase_status.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/tracing/phases/phase_step.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from zepben.evolve import PhaseCode
```

## zepben/evolve/services/network/tracing/phases/phase_step_tracker.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from collections import defaultdict
```

## zepben/evolve/services/network/tracing/phases/phase_trace.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Set, Iterable, Union, Optional
```

## zepben/evolve/services/network/tracing/phases/remove_phases.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/tracing/phases/set_phases.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/tracing/traversals/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/network/tracing/traversals/basic_tracker.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 __all__ = ["BasicTracker"]
```

## zepben/evolve/services/network/tracing/traversals/basic_traversal.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/tracing/traversals/branch_recursive_tracing.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/tracing/traversals/queue.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 from collections import deque
 from abc import abstractmethod, ABC
```

## zepben/evolve/services/network/tracing/traversals/tracker.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from abc import abstractmethod
```

## zepben/evolve/services/network/tracing/traversals/traversal.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/services/network/tracing/tree/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/services/network/tracing/tree/downstream_tree.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Set
```

## zepben/evolve/services/network/tracing/tree/tree_node.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional, List, Generator
```

## zepben/evolve/services/network/tracing/tree/tree_node_tracker.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Set
```

## zepben/evolve/services/network/translator/__init__.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from zepben.protobuf.cim.iec61968.assetinfo.CableInfo_pb2 import CableInfo
 from zepben.protobuf.cim.iec61968.assetinfo.NoLoadTest_pb2 import NoLoadTest
@@ -26,15 +26,15 @@
 from zepben.protobuf.cim.iec61968.assets.Structure_pb2 import Structure
 from zepben.protobuf.cim.iec61968.common.Document_pb2 import Document
 from zepben.protobuf.cim.iec61968.common.Location_pb2 import Location
 from zepben.protobuf.cim.iec61968.customers.CustomerAgreement_pb2 import CustomerAgreement
 from zepben.protobuf.cim.iec61968.customers.Customer_pb2 import Customer
 from zepben.protobuf.cim.iec61968.customers.PricingStructure_pb2 import PricingStructure
 from zepben.protobuf.cim.iec61968.customers.Tariff_pb2 import Tariff
-from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentRelayInfo_pb2 import CurrentRelayInfo
+from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.RelayInfo_pb2 import RelayInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentTransformerInfo_pb2 import CurrentTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.PotentialTransformerInfo_pb2 import PotentialTransformerInfo
 from zepben.protobuf.cim.iec61968.metering.EndDevice_pb2 import EndDevice
 from zepben.protobuf.cim.iec61968.metering.Meter_pb2 import Meter
 from zepben.protobuf.cim.iec61968.metering.UsagePoint_pb2 import UsagePoint
 from zepben.protobuf.cim.iec61968.operations.OperationalRestriction_pb2 import OperationalRestriction
 from zepben.protobuf.cim.iec61970.base.auxiliaryequipment.AuxiliaryEquipment_pb2 import AuxiliaryEquipment
@@ -64,15 +64,19 @@
 from zepben.protobuf.cim.iec61970.base.meas.Accumulator_pb2 import Accumulator
 from zepben.protobuf.cim.iec61970.base.meas.Analog_pb2 import Analog
 from zepben.protobuf.cim.iec61970.base.meas.Control_pb2 import Control
 from zepben.protobuf.cim.iec61970.base.meas.Discrete_pb2 import Discrete
 from zepben.protobuf.cim.iec61970.base.meas.IoPoint_pb2 import IoPoint
 from zepben.protobuf.cim.iec61970.base.meas.Measurement_pb2 import Measurement
 from zepben.protobuf.cim.iec61970.base.protection.CurrentRelay_pb2 import CurrentRelay
-from zepben.protobuf.cim.iec61970.base.protection.ProtectionEquipment_pb2 import ProtectionEquipment
+from zepben.protobuf.cim.iec61970.base.protection.DistanceRelay_pb2 import DistanceRelay
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelayFunction_pb2 import ProtectionRelayFunction
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelayScheme_pb2 import ProtectionRelayScheme
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelaySystem_pb2 import ProtectionRelaySystem
+from zepben.protobuf.cim.iec61970.base.protection.VoltageRelay_pb2 import VoltageRelay
 from zepben.protobuf.cim.iec61970.base.scada.RemoteControl_pb2 import RemoteControl
 from zepben.protobuf.cim.iec61970.base.scada.RemotePoint_pb2 import RemotePoint
 from zepben.protobuf.cim.iec61970.base.scada.RemoteSource_pb2 import RemoteSource
 from zepben.protobuf.cim.iec61970.base.wires.AcLineSegment_pb2 import AcLineSegment
 from zepben.protobuf.cim.iec61970.base.wires.Breaker_pb2 import Breaker
 from zepben.protobuf.cim.iec61970.base.wires.BusbarSection_pb2 import BusbarSection
 from zepben.protobuf.cim.iec61970.base.wires.Conductor_pb2 import Conductor
@@ -80,14 +84,16 @@
 from zepben.protobuf.cim.iec61970.base.wires.Disconnector_pb2 import Disconnector
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConnection_pb2 import EnergyConnection
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConsumerPhase_pb2 import EnergyConsumerPhase
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConsumer_pb2 import EnergyConsumer
 from zepben.protobuf.cim.iec61970.base.wires.EnergySourcePhase_pb2 import EnergySourcePhase
 from zepben.protobuf.cim.iec61970.base.wires.EnergySource_pb2 import EnergySource
 from zepben.protobuf.cim.iec61970.base.wires.Fuse_pb2 import Fuse
+from zepben.protobuf.cim.iec61970.base.wires.Ground_pb2 import Ground
+from zepben.protobuf.cim.iec61970.base.wires.GroundDisconnector_pb2 import GroundDisconnector
 from zepben.protobuf.cim.iec61970.base.wires.Jumper_pb2 import Jumper
 from zepben.protobuf.cim.iec61970.base.wires.Junction_pb2 import Junction
 from zepben.protobuf.cim.iec61970.base.wires.Line_pb2 import Line
 from zepben.protobuf.cim.iec61970.base.wires.LinearShuntCompensator_pb2 import LinearShuntCompensator
 from zepben.protobuf.cim.iec61970.base.wires.LoadBreakSwitch_pb2 import LoadBreakSwitch
 from zepben.protobuf.cim.iec61970.base.wires.PerLengthImpedance_pb2 import PerLengthImpedance
 from zepben.protobuf.cim.iec61970.base.wires.PerLengthLineParameter_pb2 import PerLengthLineParameter
@@ -97,14 +103,15 @@
 from zepben.protobuf.cim.iec61970.base.wires.PowerTransformerEnd_pb2 import PowerTransformerEnd
 from zepben.protobuf.cim.iec61970.base.wires.PowerTransformer_pb2 import PowerTransformer
 from zepben.protobuf.cim.iec61970.base.wires.ProtectedSwitch_pb2 import ProtectedSwitch
 from zepben.protobuf.cim.iec61970.base.wires.RatioTapChanger_pb2 import RatioTapChanger
 from zepben.protobuf.cim.iec61970.base.wires.Recloser_pb2 import Recloser
 from zepben.protobuf.cim.iec61970.base.wires.RegulatingCondEq_pb2 import RegulatingCondEq
 from zepben.protobuf.cim.iec61970.base.wires.RegulatingControl_pb2 import RegulatingControl
+from zepben.protobuf.cim.iec61970.base.wires.SeriesCompensator_pb2 import SeriesCompensator
 from zepben.protobuf.cim.iec61970.base.wires.ShuntCompensator_pb2 import ShuntCompensator
 from zepben.protobuf.cim.iec61970.base.wires.Switch_pb2 import Switch
 from zepben.protobuf.cim.iec61970.base.wires.TapChanger_pb2 import TapChanger
 from zepben.protobuf.cim.iec61970.base.wires.TapChangerControl_pb2 import TapChangerControl
 from zepben.protobuf.cim.iec61970.base.wires.TransformerEnd_pb2 import TransformerEnd
 from zepben.protobuf.cim.iec61970.base.wires.TransformerStarImpedance_pb2 import TransformerStarImpedance
 from zepben.protobuf.cim.iec61970.base.wires.generation.production.BatteryUnit_pb2 import BatteryUnit
@@ -143,15 +150,15 @@
 Streetlight.mrid = lambda self: self.at.mrid()
 Structure.mrid = lambda self: self.ac.mrid()
 Location.mrid = lambda self: self.io.mrid()
 Customer.mrid = lambda self: getattr(self, "or").mrid()
 CustomerAgreement.mrid = lambda self: self.agr.mrid()
 PricingStructure.mrid = lambda self: self.doc.mrid()
 Tariff.mrid = lambda self: self.doc.mrid()
-CurrentRelayInfo.mrid = lambda self: self.ai.mrid()
+RelayInfo.mrid = lambda self: self.ai.mrid()
 CurrentTransformerInfo.mrid = lambda self: self.ai.mrid()
 PotentialTransformerInfo.mrid = lambda self: self.ai.mrid()
 EndDevice.mrid = lambda self: self.ac.mrid()
 Meter.mrid = lambda self: self.ed.mrid()
 UsagePoint.mrid = lambda self: self.io.mrid()
 OperationalRestriction.mrid = lambda self: self.doc.mrid()
 AuxiliaryEquipment.mrid = lambda self: self.eq.mrid()
@@ -180,16 +187,20 @@
 EquivalentEquipment.mrid = lambda self: self.ce.mrid()
 Accumulator.mrid = lambda self: self.measurement.mrid()
 Analog.mrid = lambda self: self.measurement.mrid()
 Discrete.mrid = lambda self: self.measurement.mrid()
 Control.mrid = lambda self: self.ip.mrid()
 IoPoint.mrid = lambda self: self.io.mrid()
 Measurement.mrid = lambda self: self.io.mrid()
-CurrentRelay.mrid = lambda self: self.pe.mrid()
-ProtectionEquipment.mrid = lambda self: self.eq.mrid()
+CurrentRelay.mrid = lambda self: self.prf.mrid()
+DistanceRelay.mrid = lambda self: self.prf.mrid()
+ProtectionRelayFunction.mrid = lambda self: self.psr.mrid()
+ProtectionRelayScheme.mrid = lambda self: self.io.mrid()
+ProtectionRelaySystem.mrid = lambda self: self.eq.mrid()
+VoltageRelay.mrid = lambda self: self.prf.mrid()
 RemoteControl.mrid = lambda self: self.rp.mrid()
 RemotePoint.mrid = lambda self: self.io.mrid()
 RemoteSource.mrid = lambda self: self.rp.mrid()
 BatteryUnit.mrid = lambda self: self.peu.mrid()
 PhotoVoltaicUnit.mrid = lambda self: self.peu.mrid()
 PowerElectronicsUnit.mrid = lambda self: self.eq.mrid()
 PowerElectronicsWindUnit.mrid = lambda self: self.peu.mrid()
@@ -201,14 +212,16 @@
 Disconnector.mrid = lambda self: self.sw.mrid()
 EnergyConnection.mrid = lambda self: self.ce.mrid()
 EnergyConsumer.mrid = lambda self: self.ec.mrid()
 EnergyConsumerPhase.mrid = lambda self: self.psr.mrid()
 EnergySource.mrid = lambda self: self.ec.mrid()
 EnergySourcePhase.mrid = lambda self: self.psr.mrid()
 Fuse.mrid = lambda self: self.sw.mrid()
+Ground.mrid = lambda self: self.ce.mrid()
+GroundDisconnector.mrid = lambda self: self.sw.mrid()
 Jumper.mrid = lambda self: self.sw.mrid()
 Junction.mrid = lambda self: self.cn.mrid()
 Line.mrid = lambda self: self.ec.mrid()
 LinearShuntCompensator.mrid = lambda self: self.sc.mrid()
 LoadBreakSwitch.mrid = lambda self: self.ps.mrid()
 PerLengthImpedance.mrid = lambda self: self.lp.mrid()
 PerLengthLineParameter.mrid = lambda self: self.io.mrid()
@@ -218,14 +231,15 @@
 PowerElectronicsConnectionPhase.mrid = lambda self: self.psr.mrid()
 PowerTransformerEnd.mrid = lambda self: self.te.mrid()
 ProtectedSwitch.mrid = lambda self: self.sw.mrid()
 RatioTapChanger.mrid = lambda self: self.tc.mrid()
 Recloser.mrid = lambda self: self.sw.mrid()
 RegulatingCondEq.mrid = lambda self: self.ec.mrid()
 RegulatingControl.mrid = lambda self: self.psr.mrid()
+SeriesCompensator.mrid = lambda self: self.ce.mrid()
 ShuntCompensator.mrid = lambda self: self.rce.mrid()
 Switch.mrid = lambda self: self.ce.mrid()
 TapChanger.mrid = lambda self: self.psr.mrid()
 TapChangerControl.mrid = lambda self: self.rc.mrid()
 TransformerEnd.mrid = lambda self: self.io.mrid()
 Loop.mrid = lambda self: self.io.mrid()
 Circuit.mrid = lambda self: self.l.mrid()
@@ -327,20 +341,23 @@
 # normal_energizing_substation_mrid
 Feeder.normal_energizing_substation_mrid = lambda self: getattr(self, "normalEnergizingSubstationMRID", None)
 
 # per_length_sequence_impedance_mrid
 AcLineSegment.per_length_sequence_impedance_mrid = lambda self: getattr(self, "perLengthSequenceImpedanceMRID", None)
 
 # asset_info_mrid
+CurrentRelay.asset_info_mrid = lambda self: self.prf.asset_info_mrid
 ConductingEquipment.asset_info_mrid = lambda self: self.eq.asset_info_mrid()
 Conductor.asset_info_mrid = lambda self: self.ce.asset_info_mrid()
 CurrentTransformer.asset_info_mrid = lambda self: self.sn.ae.eq.asset_info_mrid()
-CurrentRelay.asset_info_mrid = lambda self: self.pe.eq.asset_info_mrid()
+DistanceRelay.asset_info_mrid = lambda self: self.prf.asset_info_mrid
 Equipment.asset_info_mrid = lambda self: self.psr.assetInfoMRID
 PotentialTransformer.asset_info_mrid = lambda self: self.sn.ae.eq.asset_info_mrid()
 PowerTransformer.asset_info_mrid = lambda self: self.ce.asset_info_mrid()
+ProtectionRelayFunction.asset_info_mrid = lambda self: self.psr.assetInfoMRID
 ShuntCompensator.asset_info_mrid = lambda self: self.rce.ec.ce.asset_info_mrid()
 Switch.asset_info_mrid = lambda self: self.ce.asset_info_mrid()
+VoltageRelay.asset_info_mrid = lambda self: self.prf.asset_info_mrid
 
 # ratio_tap_changer_mrid
 TransformerEnd.ratio_tap_changer_mrid = lambda self: getattr(self, "ratioTapChangerMRID", None)
 PowerTransformerEnd.ratio_tap_changer_mrid = lambda self: self.te.ratio_tap_changer_mrid()
```

## zepben/evolve/services/network/translator/network_cim2proto.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from zepben.protobuf.cim.iec61968.assetinfo.CableInfo_pb2 import CableInfo as PBCableInfo
 from zepben.protobuf.cim.iec61968.assetinfo.NoLoadTest_pb2 import NoLoadTest as PBNoLoadTest
 from zepben.protobuf.cim.iec61968.assetinfo.OpenCircuitTest_pb2 import OpenCircuitTest as PBOpenCircuitTest
@@ -26,15 +26,15 @@
 from zepben.protobuf.cim.iec61968.assets.Streetlight_pb2 import Streetlight as PBStreetlight
 from zepben.protobuf.cim.iec61968.assets.Structure_pb2 import Structure as PBStructure
 from zepben.protobuf.cim.iec61968.common.Location_pb2 import Location as PBLocation
 from zepben.protobuf.cim.iec61968.common.PositionPoint_pb2 import PositionPoint as PBPositionPoint
 from zepben.protobuf.cim.iec61968.common.StreetAddress_pb2 import StreetAddress as PBStreetAddress
 from zepben.protobuf.cim.iec61968.common.StreetDetail_pb2 import StreetDetail as PBStreetDetail
 from zepben.protobuf.cim.iec61968.common.TownDetail_pb2 import TownDetail as PBTownDetail
-from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentRelayInfo_pb2 import CurrentRelayInfo as PBCurrentRelayInfo
+from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.RelayInfo_pb2 import RelayInfo as PBRelayInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentTransformerInfo_pb2 import CurrentTransformerInfo as PBCurrentTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.PotentialTransformerInfo_pb2 import PotentialTransformerInfo as PBPotentialTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.TransformerConstructionKind_pb2 import TransformerConstructionKind as PBTransformerConstructionKind
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.TransformerFunctionKind_pb2 import TransformerFunctionKind as PBTransformerFunctionKind
 from zepben.protobuf.cim.iec61968.infiec61968.infcommon.Ratio_pb2 import Ratio as PBRatio
 from zepben.protobuf.cim.iec61968.metering.EndDevice_pb2 import EndDevice as PBEndDevice
 from zepben.protobuf.cim.iec61968.metering.Meter_pb2 import Meter as PBMeter
@@ -67,15 +67,20 @@
 from zepben.protobuf.cim.iec61970.base.meas.Accumulator_pb2 import Accumulator as PBAccumulator
 from zepben.protobuf.cim.iec61970.base.meas.Analog_pb2 import Analog as PBAnalog
 from zepben.protobuf.cim.iec61970.base.meas.Control_pb2 import Control as PBControl
 from zepben.protobuf.cim.iec61970.base.meas.Discrete_pb2 import Discrete as PBDiscrete
 from zepben.protobuf.cim.iec61970.base.meas.IoPoint_pb2 import IoPoint as PBIoPoint
 from zepben.protobuf.cim.iec61970.base.meas.Measurement_pb2 import Measurement as PBMeasurement
 from zepben.protobuf.cim.iec61970.base.protection.CurrentRelay_pb2 import CurrentRelay as PBCurrentRelay
-from zepben.protobuf.cim.iec61970.base.protection.ProtectionEquipment_pb2 import ProtectionEquipment as PBProtectionEquipment
+from zepben.protobuf.cim.iec61970.base.protection.DistanceRelay_pb2 import DistanceRelay as PBDistanceRelay
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelayFunction_pb2 import ProtectionRelayFunction as PBProtectionRelayFunction
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelayScheme_pb2 import ProtectionRelayScheme as PBProtectionRelayScheme
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelaySystem_pb2 import ProtectionRelaySystem as PBProtectionRelaySystem
+from zepben.protobuf.cim.iec61970.base.protection.RelaySetting_pb2 import RelaySetting as PBRelaySetting
+from zepben.protobuf.cim.iec61970.base.protection.VoltageRelay_pb2 import VoltageRelay as PBVoltageRelay
 from zepben.protobuf.cim.iec61970.base.scada.RemoteControl_pb2 import RemoteControl as PBRemoteControl
 from zepben.protobuf.cim.iec61970.base.scada.RemotePoint_pb2 import RemotePoint as PBRemotePoint
 from zepben.protobuf.cim.iec61970.base.scada.RemoteSource_pb2 import RemoteSource as PBRemoteSource
 from zepben.protobuf.cim.iec61970.base.wires.AcLineSegment_pb2 import AcLineSegment as PBAcLineSegment
 from zepben.protobuf.cim.iec61970.base.wires.Breaker_pb2 import Breaker as PBBreaker
 from zepben.protobuf.cim.iec61970.base.wires.BusbarSection_pb2 import BusbarSection as PBBusbarSection
 from zepben.protobuf.cim.iec61970.base.wires.Conductor_pb2 import Conductor as PBConductor
@@ -83,14 +88,16 @@
 from zepben.protobuf.cim.iec61970.base.wires.Disconnector_pb2 import Disconnector as PBDisconnector
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConnection_pb2 import EnergyConnection as PBEnergyConnection
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConsumerPhase_pb2 import EnergyConsumerPhase as PBEnergyConsumerPhase
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConsumer_pb2 import EnergyConsumer as PBEnergyConsumer
 from zepben.protobuf.cim.iec61970.base.wires.EnergySourcePhase_pb2 import EnergySourcePhase as PBEnergySourcePhase
 from zepben.protobuf.cim.iec61970.base.wires.EnergySource_pb2 import EnergySource as PBEnergySource
 from zepben.protobuf.cim.iec61970.base.wires.Fuse_pb2 import Fuse as PBFuse
+from zepben.protobuf.cim.iec61970.base.wires.Ground_pb2 import Ground as PBGround
+from zepben.protobuf.cim.iec61970.base.wires.GroundDisconnector_pb2 import GroundDisconnector as PBGroundDisconnector
 from zepben.protobuf.cim.iec61970.base.wires.Jumper_pb2 import Jumper as PBJumper
 from zepben.protobuf.cim.iec61970.base.wires.Junction_pb2 import Junction as PBJunction
 from zepben.protobuf.cim.iec61970.base.wires.Line_pb2 import Line as PBLine
 from zepben.protobuf.cim.iec61970.base.wires.LinearShuntCompensator_pb2 import LinearShuntCompensator as PBLinearShuntCompensator
 from zepben.protobuf.cim.iec61970.base.wires.LoadBreakSwitch_pb2 import LoadBreakSwitch as PBLoadBreakSwitch
 from zepben.protobuf.cim.iec61970.base.wires.PerLengthImpedance_pb2 import PerLengthImpedance as PBPerLengthImpedance
 from zepben.protobuf.cim.iec61970.base.wires.PerLengthLineParameter_pb2 import PerLengthLineParameter as PBPerLengthLineParameter
@@ -102,14 +109,15 @@
 from zepben.protobuf.cim.iec61970.base.wires.PowerTransformer_pb2 import PowerTransformer as PBPowerTransformer
 from zepben.protobuf.cim.iec61970.base.wires.ProtectedSwitch_pb2 import ProtectedSwitch as PBProtectedSwitch
 from zepben.protobuf.cim.iec61970.base.wires.RatioTapChanger_pb2 import RatioTapChanger as PBRatioTapChanger
 from zepben.protobuf.cim.iec61970.base.wires.Recloser_pb2 import Recloser as PBRecloser
 from zepben.protobuf.cim.iec61970.base.wires.RegulatingCondEq_pb2 import RegulatingCondEq as PBRegulatingCondEq
 from zepben.protobuf.cim.iec61970.base.wires.RegulatingControlModeKind_pb2 import RegulatingControlModeKind as PBRegulatingControlModeKind
 from zepben.protobuf.cim.iec61970.base.wires.RegulatingControl_pb2 import RegulatingControl as PBRegulatingControl
+from zepben.protobuf.cim.iec61970.base.wires.SeriesCompensator_pb2 import SeriesCompensator as PBSeriesCompensator
 from zepben.protobuf.cim.iec61970.base.wires.ShuntCompensator_pb2 import ShuntCompensator as PBShuntCompensator
 from zepben.protobuf.cim.iec61970.base.wires.SinglePhaseKind_pb2 import SinglePhaseKind as PBSinglePhaseKind
 from zepben.protobuf.cim.iec61970.base.wires.Switch_pb2 import Switch as PBSwitch
 from zepben.protobuf.cim.iec61970.base.wires.TapChanger_pb2 import TapChanger as PBTapChanger
 from zepben.protobuf.cim.iec61970.base.wires.TapChangerControl_pb2 import TapChangerControl as PBTapChangerControl
 from zepben.protobuf.cim.iec61970.base.wires.TransformerEnd_pb2 import TransformerEnd as PBTransformerEnd
 from zepben.protobuf.cim.iec61970.base.wires.TransformerEndRatedS_pb2 import TransformerEndRatedS as PBTransformerEndRatedS
@@ -127,15 +135,14 @@
 from zepben.protobuf.cim.iec61970.infiec61970.feeder.LvFeeder_pb2 import LvFeeder as PBLvFeeder
 from zepben.protobuf.cim.iec61970.infiec61970.protection.ProtectionKind_pb2 import ProtectionKind as PBProtectionKind
 from zepben.protobuf.cim.iec61970.infiec61970.protection.PowerDirectionKind_pb2 import PowerDirectionKind as PBPowerDirectionKind
 from zepben.protobuf.cim.iec61970.infiec61970.wires.generation.production.EvChargingUnit_pb2 import EvChargingUnit as PBEvChargingUnit
 from zepben.protobuf.network.model.FeederDirection_pb2 import FeederDirection as PBFeederDirection
 from google.protobuf.timestamp_pb2 import Timestamp as PBTimestamp
 
-
 from zepben.evolve.model.cim.iec61968.assetinfo.no_load_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.open_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.power_transformer_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.short_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.shunt_compensator_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.switch_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_end_info import *
@@ -145,15 +152,15 @@
 from zepben.evolve.model.cim.iec61968.assets.asset import *
 from zepben.evolve.model.cim.iec61968.assets.asset_info import *
 from zepben.evolve.model.cim.iec61968.assets.asset_organisation_role import *
 from zepben.evolve.model.cim.iec61968.assets.pole import *
 from zepben.evolve.model.cim.iec61968.assets.streetlight import *
 from zepben.evolve.model.cim.iec61968.assets.structure import *
 from zepben.evolve.model.cim.iec61968.common.location import *
-from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import *
+from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.relay_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.potential_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infcommon.ratio import *
 from zepben.evolve.model.cim.iec61968.metering.metering import *
 from zepben.evolve.model.cim.iec61968.operations.operational_restriction import *
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.auxiliary_equipment import *
 from zepben.evolve.model.cim.iec61970.base.auxiliaryequipment.current_transformer import *
@@ -171,37 +178,45 @@
 from zepben.evolve.model.cim.iec61970.base.core.terminal import *
 from zepben.evolve.model.cim.iec61970.base.equivalents.equivalent_branch import *
 from zepben.evolve.model.cim.iec61970.base.equivalents.equivalent_equipment import *
 from zepben.evolve.model.cim.iec61970.base.meas.control import *
 from zepben.evolve.model.cim.iec61970.base.meas.iopoint import *
 from zepben.evolve.model.cim.iec61970.base.meas.measurement import *
 from zepben.evolve.model.cim.iec61970.base.protection.current_relay import *
-from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import *
+from zepben.evolve.model.cim.iec61970.base.protection.distance_relay import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_function import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_scheme import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_system import *
+from zepben.evolve.model.cim.iec61970.base.protection.relay_setting import *
+from zepben.evolve.model.cim.iec61970.base.protection.voltage_relay import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_control import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_point import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import *
 from zepben.evolve.model.cim.iec61970.base.wires.breaker import *
 from zepben.evolve.model.cim.iec61970.base.wires.connectors import *
 from zepben.evolve.model.cim.iec61970.base.wires.disconnector import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source_phase import *
 from zepben.evolve.model.cim.iec61970.base.wires.fuse import *
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.power_electronics_unit import *
+from zepben.evolve.model.cim.iec61970.base.wires.ground import *
+from zepben.evolve.model.cim.iec61970.base.wires.ground_disconnector import *
 from zepben.evolve.model.cim.iec61970.base.wires.jumper import *
 from zepben.evolve.model.cim.iec61970.base.wires.line import *
 from zepben.evolve.model.cim.iec61970.base.wires.load_break_switch import *
 from zepben.evolve.model.cim.iec61970.base.wires.per_length import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import *
 from zepben.evolve.model.cim.iec61970.base.wires.protected_switch import *
 from zepben.evolve.model.cim.iec61970.base.wires.recloser import *
 from zepben.evolve.model.cim.iec61970.base.wires.regulating_control import *
+from zepben.evolve.model.cim.iec61970.base.wires.series_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.shunt_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.switch import *
 from zepben.evolve.model.cim.iec61970.base.wires.tap_changer_control import *
 from zepben.evolve.model.cim.iec61970.base.wires.transformer_star_impedance import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.circuit import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.loop import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.lv_feeder import *
@@ -211,29 +226,31 @@
     nullable_bool_settings
 
 __all__ = [
     "CimTranslationException", "cable_info_to_pb", "no_load_test_to_pb", "open_circuit_test_to_pb", "overhead_wire_info_to_pb", "power_transformer_info_to_pb",
     "short_circuit_test_to_pb", "shunt_compensator_info_to_pb", "switch_info_to_pb", "transformer_end_info_to_pb", "transformer_tank_info_to_pb",
     "transformer_test_to_pb", "wire_info_to_pb", "asset_to_pb", "asset_container_to_pb", "asset_info_to_pb", "asset_organisation_role_to_pb",
     "asset_owner_to_pb", "pole_to_pb", "streetlight_to_pb", "structure_to_pb", "location_to_pb", "position_point_to_pb", "street_address_to_pb",
-    "street_detail_to_pb", "town_detail_to_pb", "current_relay_info_to_pb", "current_transformer_info_to_pb", "potential_transformer_info_to_pb",
+    "street_detail_to_pb", "town_detail_to_pb", "relay_info_to_pb", "current_transformer_info_to_pb", "potential_transformer_info_to_pb",
     "ratio_to_pb", "end_device_to_pb", "meter_to_pb", "usage_point_to_pb", "operational_restriction_to_pb", "auxiliary_equipment_to_pb",
     "current_transformer_to_pb", "fault_indicator_to_pb", "potential_transformer_to_pb", "sensor_to_pb", "ac_dc_terminal_to_pb", "base_voltage_to_pb",
     "conducting_equipment_to_pb", "connectivity_node_to_pb", "connectivity_node_container_to_pb", "equipment_to_pb", "equipment_container_to_pb",
     "feeder_to_pb", "geographical_region_to_pb", "power_system_resource_to_pb", "site_to_pb", "sub_geographical_region_to_pb", "substation_to_pb",
     "terminal_to_pb", "equivalent_branch_to_pb", "equivalent_equipment_to_pb", "accumulator_to_pb", "analog_to_pb", "control_to_pb", "discrete_to_pb",
-    "io_point_to_pb", "measurement_to_pb", "current_relay_to_pb", "protection_equipment_to_pb", "remote_control_to_pb", "remote_point_to_pb",
+    "io_point_to_pb", "measurement_to_pb", "current_relay_to_pb", "distance_relay_to_pb", "voltage_relay_to_pb", "remote_control_to_pb", "remote_point_to_pb",
     "remote_source_to_pb", "battery_unit_to_pb", "photo_voltaic_unit_to_pb", "power_electronics_unit_to_pb", "power_electronics_wind_unit_to_pb",
     "ac_line_segment_to_pb", "breaker_to_pb", "conductor_to_pb", "connector_to_pb", "disconnector_to_pb", "energy_connection_to_pb", "energy_consumer_to_pb",
     "energy_consumer_phase_to_pb", "energy_source_to_pb", "energy_source_phase_to_pb", "fuse_to_pb", "jumper_to_pb", "junction_to_pb", "busbar_section_to_pb",
     "line_to_pb", "linear_shunt_compensator_to_pb", "load_break_switch_to_pb", "per_length_line_parameter_to_pb", "per_length_impedance_to_pb",
     "per_length_sequence_impedance_to_pb", "power_electronics_connection_to_pb", "power_electronics_connection_phase_to_pb", "power_transformer_to_pb",
     "power_transformer_end_to_pb", "protected_switch_to_pb", "ratio_tap_changer_to_pb", "recloser_to_pb", "regulating_cond_eq_to_pb", "shunt_compensator_to_pb",
     "switch_to_pb", "tap_changer_to_pb", "transformer_end_to_pb", "transformer_star_impedance_to_pb", "circuit_to_pb", "loop_to_pb", "lv_feeder_to_pb",
-    "ev_charging_unit", "transformer_end_rated_s_to_pb", "tap_changer_control_to_pb", "regulating_control_to_pb"
+    "ev_charging_unit", "transformer_end_rated_s_to_pb", "tap_changer_control_to_pb", "regulating_control_to_pb", "protection_relay_function_to_pb",
+    "protection_relay_scheme_to_pb", "protection_relay_system_to_pb", "relay_setting_to_pb", "ground_to_pb", "ground_disconnector_to_pb",
+    "series_compensator_to_pb"
 ]
 
 
 def _get_or_none(getter, obj) -> object:
     return getter(obj) if obj else None
 
 
@@ -483,18 +500,19 @@
 TownDetail.to_pb = town_detail_to_pb
 
 
 #####################################
 # IEC61968 infIEC61968 InfAssetInfo #
 #####################################
 
-def current_relay_info_to_pb(cim: CurrentRelayInfo) -> PBCurrentRelayInfo:
-    return PBCurrentRelayInfo(
+def relay_info_to_pb(cim: RelayInfo) -> PBRelayInfo:
+    return PBRelayInfo(
         ai=asset_info_to_pb(cim),
         curveSetting=cim.curve_setting,
+        **nullable_bool_settings("recloseFast", cim.reclose_fast),
         recloseDelays=cim.reclose_delays
     )
 
 
 def current_transformer_info_to_pb(cim: CurrentTransformerInfo) -> PBCurrentTransformerInfo:
     return PBCurrentTransformerInfo(
         ai=asset_info_to_pb(cim),
@@ -521,15 +539,15 @@
         primaryRatio=from_nullable_float(cim.primary_ratio),
         ptClass=cim.pt_class,
         ratedVoltage=from_nullable_int(cim.rated_voltage),
         secondaryRatio=from_nullable_float(cim.secondary_ratio)
     )
 
 
-CurrentRelayInfo.to_pb = current_relay_info_to_pb
+RelayInfo.to_pb = relay_info_to_pb
 CurrentTransformerInfo.to_pb = current_transformer_info_to_pb
 PotentialTransformerInfo.to_pb = potential_transformer_info_to_pb
 
 
 ##################################
 # IEC61968 infIEC61968 InfCommon #
 ##################################
@@ -613,15 +631,18 @@
     return PBPotentialTransformer(
         sn=sensor_to_pb(cim, True),
         type=PBPotentialTransformerKind.Value(cim.type.short_name)
     )
 
 
 def sensor_to_pb(cim: Sensor, include_asset_info: bool = False) -> PBSensor:
-    return PBSensor(ae=auxiliary_equipment_to_pb(cim, include_asset_info))
+    return PBSensor(
+        ae=auxiliary_equipment_to_pb(cim, include_asset_info),
+        relayFunctionMRIDs=[str(io.mrid) for io in cim.relay_functions],
+    )
 
 
 AuxiliaryEquipment.to_pb = auxiliary_equipment_to_pb
 CurrentTransformer.to_pb = current_transformer_to_pb
 FaultIndicator.to_pb = fault_indicator_to_pb
 PotentialTransformer.to_pb = potential_transformer_to_pb
 Sensor.to_pb = sensor_to_pb
@@ -842,34 +863,88 @@
 
 ############################
 # IEC61970 Base Protection #
 ############################
 
 def current_relay_to_pb(cim: CurrentRelay) -> PBCurrentRelay:
     return PBCurrentRelay(
-        pe=protection_equipment_to_pb(cim, True),
+        prf=protection_relay_function_to_pb(cim, True),
         currentLimit1=from_nullable_float(cim.current_limit_1),
         **nullable_bool_settings("inverseTimeFlag", cim.inverse_time_flag),
         timeDelay1=from_nullable_float(cim.time_delay_1),
     )
 
 
-def protection_equipment_to_pb(cim: ProtectionEquipment, include_asset_info: bool = False) -> PBProtectionEquipment:
-    return PBProtectionEquipment(
-        eq=equipment_to_pb(cim, include_asset_info),
+def distance_relay_to_pb(cim: DistanceRelay) -> PBDistanceRelay:
+    return PBDistanceRelay(
+        prf=protection_relay_function_to_pb(cim, True),
+        backwardBlind=from_nullable_float(cim.backward_blind),
+        backwardReach=from_nullable_float(cim.backward_reach),
+        backwardReactance=from_nullable_float(cim.backward_reactance),
+        forwardBlind=from_nullable_float(cim.forward_blind),
+        forwardReach=from_nullable_float(cim.forward_reach),
+        forwardReactance=from_nullable_float(cim.forward_reactance),
+        operationPhaseAngle1=from_nullable_float(cim.operation_phase_angle1),
+        operationPhaseAngle2=from_nullable_float(cim.operation_phase_angle2),
+        operationPhaseAngle3=from_nullable_float(cim.operation_phase_angle3)
+    )
+
+
+def protection_relay_function_to_pb(cim: ProtectionRelayFunction, include_asset_info: bool = False) -> PBProtectionRelayFunction:
+    return PBProtectionRelayFunction(
+        psr=power_system_resource_to_pb(cim, include_asset_info),
+        model=cim.model,
+        **nullable_bool_settings("reclosing", cim.reclosing),
+        timeLimits=cim.time_limits,
+        thresholds=[relay_setting_to_pb(rs) for rs in cim.thresholds],
         relayDelayTime=from_nullable_float(cim.relay_delay_time),
         protectionKind=PBProtectionKind.Value(cim.protection_kind.short_name),
         protectedSwitchMRIDs=[str(io.mrid) for io in cim.protected_switches],
         **nullable_bool_settings("directable", cim.directable),
-        powerDirection=PBPowerDirectionKind.Value(cim.power_direction.short_name)
+        powerDirection=PBPowerDirectionKind.Value(cim.power_direction.short_name),
+        sensorMRIDs=[str(io.mrid) for io in cim.sensors],
+        schemeMRIDs=[str(io.mrid) for io in cim.schemes],
+    )
+
+
+def protection_relay_scheme_to_pb(cim: ProtectionRelayScheme) -> PBProtectionRelayScheme:
+    return PBProtectionRelayScheme(
+        io=identified_object_to_pb(cim),
+        systemMRID=mrid_or_empty(cim.system),
+        functionMRIDs=[str(io.mrid) for io in cim.functions]
+    )
+
+
+def protection_relay_system_to_pb(cim: ProtectionRelaySystem) -> PBProtectionRelaySystem:
+    return PBProtectionRelaySystem(
+        eq=equipment_to_pb(cim),
+        protectionKind=PBProtectionKind.Value(cim.protection_kind.short_name),
+        schemeMRIDs=[str(io.mrid) for io in cim.schemes],
+    )
+
+
+def relay_setting_to_pb(cim: RelaySetting) -> PBRelaySetting:
+    return PBRelaySetting(
+        name=cim.name,
+        unitSymbol=PBUnitSymbol.Value(cim.unit_symbol.short_name),
+        value=from_nullable_float(cim.value)
+    )
+
+
+def voltage_relay_to_pb(cim: VoltageRelay) -> PBVoltageRelay:
+    return PBVoltageRelay(
+        prf=protection_relay_function_to_pb(cim, True),
     )
 
 
 CurrentRelay.to_pb = current_relay_to_pb
-ProtectionEquipment.to_pb = protection_equipment_to_pb
+DistanceRelay.to_pb = distance_relay_to_pb
+ProtectionRelayScheme.to_pb = protection_relay_scheme_to_pb
+ProtectionRelaySystem.to_pb = protection_relay_system_to_pb
+VoltageRelay.to_pb = voltage_relay_to_pb
 
 
 #######################
 # IEC61970 BASE SCADA #
 #######################
 
 def remote_control_to_pb(cim: RemoteControl) -> PBRemoteControl:
@@ -1031,15 +1106,30 @@
         psr=power_system_resource_to_pb(cim),
         energySourceMRID=mrid_or_empty(cim.energy_source),
         phase=PBSinglePhaseKind.Value(cim.phase.short_name)
     )
 
 
 def fuse_to_pb(cim: Fuse) -> PBFuse:
-    return PBFuse(sw=switch_to_pb(cim))
+    return PBFuse(
+        sw=switch_to_pb(cim),
+        functionMRID=mrid_or_empty(cim.function)
+    )
+
+
+def ground_to_pb(cim: Ground) -> PBGround:
+    return PBGround(
+        ce=conducting_equipment_to_pb(cim, True)
+    )
+
+
+def ground_disconnector_to_pb(cim: GroundDisconnector) -> PBGroundDisconnector:
+    return PBGroundDisconnector(
+        sw=switch_to_pb(cim)
+    )
 
 
 def jumper_to_pb(cim: Jumper) -> PBJumper:
     return PBJumper(sw=switch_to_pb(cim))
 
 
 def junction_to_pb(cim: Junction) -> PBJunction:
@@ -1166,26 +1256,38 @@
         g=from_nullable_float(cim.g),
         g0=from_nullable_float(cim.g0),
         phaseAngleClock=from_nullable_int(cim.phase_angle_clock),
         ratings=[transformer_end_rated_s_to_pb(it) for it in cim.s_ratings]
     )
 
 
+def series_compensator_to_pb(cim: SeriesCompensator) -> PBSeriesCompensator:
+    return PBSeriesCompensator(
+        ce=conducting_equipment_to_pb(cim, True),
+        r=from_nullable_float(cim.r),
+        r0=from_nullable_float(cim.r0),
+        x=from_nullable_float(cim.x),
+        x0=from_nullable_float(cim.x0),
+        varistorRatedCurrent=from_nullable_int(cim.varistor_rated_current),
+        varistorVoltageThreshold=from_nullable_int(cim.varistor_voltage_threshold),
+    )
+
+
 def transformer_end_rated_s_to_pb(cim: TransformerEndRatedS) -> PBTransformerEndRatedS:
     return PBTransformerEndRatedS(
         ratedS=cim.rated_s,
         coolingType=PBTransformerCoolingType.Value(cim.cooling_type.short_name)
     )
 
 
 def protected_switch_to_pb(cim: ProtectedSwitch) -> PBProtectedSwitch:
     return PBProtectedSwitch(
         sw=switch_to_pb(cim),
         breakingCapacity=from_nullable_int(cim.breaking_capacity),
-        operatedByProtectionEquipmentMRIDs=[str(io.mrid) for io in cim.operated_by_protection_equipment]
+        relayFunctionMRIDs=[str(io.mrid) for io in cim.relay_functions]
     )
 
 
 def ratio_tap_changer_to_pb(cim: RatioTapChanger) -> PBRatioTapChanger:
     return PBRatioTapChanger(
         tc=tap_changer_to_pb(cim),
         transformerEndMRID=mrid_or_empty(cim.transformer_end),
@@ -1212,14 +1314,15 @@
         mode=PBRegulatingControlModeKind.Value(cim.mode.short_name),
         monitoredPhase=PBPhaseCode.Value(cim.monitored_phase.short_name),
         targetDeadband=from_nullable_float(cim.target_deadband),
         targetValue=from_nullable_float(cim.target_value),
         **nullable_bool_settings("enabled", cim.enabled),
         maxAllowedTargetValue=from_nullable_float(cim.max_allowed_target_value),
         minAllowedTargetValue=from_nullable_float(cim.min_allowed_target_value),
+        ratedCurrent=from_nullable_float(cim.rated_current),
         terminalMRID=mrid_or_empty(cim.terminal),
         regulatingCondEqMRIDs=[str(io.mrid) for io in cim.regulating_conducting_equipment]
     )
 
 
 def shunt_compensator_to_pb(cim: ShuntCompensator) -> PBShuntCompensator:
     return PBShuntCompensator(
@@ -1302,14 +1405,16 @@
 Disconnector.to_pb = disconnector_to_pb
 EnergyConnection.to_pb = energy_connection_to_pb
 EnergyConsumer.to_pb = energy_consumer_to_pb
 EnergyConsumerPhase.to_pb = energy_consumer_phase_to_pb
 EnergySource.to_pb = energy_source_to_pb
 EnergySourcePhase.to_pb = energy_source_phase_to_pb
 Fuse.to_pb = fuse_to_pb
+Ground.to_pb = ground_to_pb
+GroundDisconnector.to_pb = ground_disconnector_to_pb
 Jumper.to_pb = jumper_to_pb
 Junction.to_pb = junction_to_pb
 Line.to_pb = line_to_pb
 LinearShuntCompensator.to_pb = linear_shunt_compensator_to_pb
 LoadBreakSwitch.to_pb = load_break_switch_to_pb
 PerLengthImpedance.to_pb = per_length_impedance_to_pb
 PerLengthLineParameter.to_pb = per_length_line_parameter_to_pb
@@ -1317,14 +1422,15 @@
 PowerElectronicsConnection.to_pb = power_electronics_connection_to_pb
 PowerElectronicsConnectionPhase.to_pb = power_electronics_connection_phase_to_pb
 PowerTransformer.to_pb = power_transformer_to_pb
 PowerTransformerEnd.to_pb = power_transformer_end_to_pb
 ProtectedSwitch.to_pb = protected_switch_to_pb
 RatioTapChanger.to_pb = ratio_tap_changer_to_pb
 Recloser.to_pb = recloser_to_pb
+SeriesCompensator.to_pb = series_compensator_to_pb
 RegulatingCondEq.to_pb = regulating_cond_eq_to_pb
 TapChangerControl.to_pb = tap_changer_control_to_pb
 ShuntCompensator.to_pb = shunt_compensator_to_pb
 Switch.to_pb = switch_to_pb
 TapChanger.to_pb = tap_changer_to_pb
 TransformerEnd.to_pb = transformer_end_to_pb
 TransformerEndRatedS.to_pb = transformer_end_rated_s_to_pb
```

## zepben/evolve/services/network/translator/network_proto2cim.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from typing import Optional
@@ -29,15 +29,15 @@
 from zepben.protobuf.cim.iec61968.assets.Streetlight_pb2 import Streetlight as PBStreetlight
 from zepben.protobuf.cim.iec61968.assets.Structure_pb2 import Structure as PBStructure
 from zepben.protobuf.cim.iec61968.common.Location_pb2 import Location as PBLocation
 from zepben.protobuf.cim.iec61968.common.PositionPoint_pb2 import PositionPoint as PBPositionPoint
 from zepben.protobuf.cim.iec61968.common.StreetAddress_pb2 import StreetAddress as PBStreetAddress
 from zepben.protobuf.cim.iec61968.common.StreetDetail_pb2 import StreetDetail as PBStreetDetail
 from zepben.protobuf.cim.iec61968.common.TownDetail_pb2 import TownDetail as PBTownDetail
-from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentRelayInfo_pb2 import CurrentRelayInfo as PBCurrentRelayInfo
+from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.RelayInfo_pb2 import RelayInfo as PBRelayInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.CurrentTransformerInfo_pb2 import CurrentTransformerInfo as PBCurrentTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infassetinfo.PotentialTransformerInfo_pb2 import PotentialTransformerInfo as PBPotentialTransformerInfo
 from zepben.protobuf.cim.iec61968.infiec61968.infcommon.Ratio_pb2 import Ratio as PBRatio
 from zepben.protobuf.cim.iec61968.metering.EndDevice_pb2 import EndDevice as PBEndDevice
 from zepben.protobuf.cim.iec61968.metering.Meter_pb2 import Meter as PBMeter
 from zepben.protobuf.cim.iec61968.metering.UsagePoint_pb2 import UsagePoint as PBUsagePoint
 from zepben.protobuf.cim.iec61968.operations.OperationalRestriction_pb2 import OperationalRestriction as PBOperationalRestriction
@@ -65,15 +65,20 @@
 from zepben.protobuf.cim.iec61970.base.meas.Accumulator_pb2 import Accumulator as PBAccumulator
 from zepben.protobuf.cim.iec61970.base.meas.Analog_pb2 import Analog as PBAnalog
 from zepben.protobuf.cim.iec61970.base.meas.Control_pb2 import Control as PBControl
 from zepben.protobuf.cim.iec61970.base.meas.Discrete_pb2 import Discrete as PBDiscrete
 from zepben.protobuf.cim.iec61970.base.meas.IoPoint_pb2 import IoPoint as PBIoPoint
 from zepben.protobuf.cim.iec61970.base.meas.Measurement_pb2 import Measurement as PBMeasurement
 from zepben.protobuf.cim.iec61970.base.protection.CurrentRelay_pb2 import CurrentRelay as PBCurrentRelay
-from zepben.protobuf.cim.iec61970.base.protection.ProtectionEquipment_pb2 import ProtectionEquipment as PBProtectionEquipment
+from zepben.protobuf.cim.iec61970.base.protection.DistanceRelay_pb2 import DistanceRelay as PBDistanceRelay
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelayFunction_pb2 import ProtectionRelayFunction as PBProtectionRelayFunction
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelayScheme_pb2 import ProtectionRelayScheme as PBProtectionRelayScheme
+from zepben.protobuf.cim.iec61970.base.protection.ProtectionRelaySystem_pb2 import ProtectionRelaySystem as PBProtectionRelaySystem
+from zepben.protobuf.cim.iec61970.base.protection.VoltageRelay_pb2 import VoltageRelay as PBVoltageRelay
+from zepben.protobuf.cim.iec61970.base.protection.RelaySetting_pb2 import RelaySetting as PBRelaySetting
 from zepben.protobuf.cim.iec61970.base.scada.RemoteControl_pb2 import RemoteControl as PBRemoteControl
 from zepben.protobuf.cim.iec61970.base.scada.RemotePoint_pb2 import RemotePoint as PBRemotePoint
 from zepben.protobuf.cim.iec61970.base.scada.RemoteSource_pb2 import RemoteSource as PBRemoteSource
 from zepben.protobuf.cim.iec61970.base.wires.AcLineSegment_pb2 import AcLineSegment as PBAcLineSegment
 from zepben.protobuf.cim.iec61970.base.wires.Breaker_pb2 import Breaker as PBBreaker
 from zepben.protobuf.cim.iec61970.base.wires.BusbarSection_pb2 import BusbarSection as PBBusbarSection
 from zepben.protobuf.cim.iec61970.base.wires.Conductor_pb2 import Conductor as PBConductor
@@ -81,14 +86,16 @@
 from zepben.protobuf.cim.iec61970.base.wires.Disconnector_pb2 import Disconnector as PBDisconnector
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConnection_pb2 import EnergyConnection as PBEnergyConnection
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConsumerPhase_pb2 import EnergyConsumerPhase as PBEnergyConsumerPhase
 from zepben.protobuf.cim.iec61970.base.wires.EnergyConsumer_pb2 import EnergyConsumer as PBEnergyConsumer
 from zepben.protobuf.cim.iec61970.base.wires.EnergySourcePhase_pb2 import EnergySourcePhase as PBEnergySourcePhase
 from zepben.protobuf.cim.iec61970.base.wires.EnergySource_pb2 import EnergySource as PBEnergySource
 from zepben.protobuf.cim.iec61970.base.wires.Fuse_pb2 import Fuse as PBFuse
+from zepben.protobuf.cim.iec61970.base.wires.Ground_pb2 import Ground as PBGround
+from zepben.protobuf.cim.iec61970.base.wires.GroundDisconnector_pb2 import GroundDisconnector as PBGroundDisconnector
 from zepben.protobuf.cim.iec61970.base.wires.Jumper_pb2 import Jumper as PBJumper
 from zepben.protobuf.cim.iec61970.base.wires.Junction_pb2 import Junction as PBJunction
 from zepben.protobuf.cim.iec61970.base.wires.Line_pb2 import Line as PBLine
 from zepben.protobuf.cim.iec61970.base.wires.LinearShuntCompensator_pb2 import LinearShuntCompensator as PBLinearShuntCompensator
 from zepben.protobuf.cim.iec61970.base.wires.LoadBreakSwitch_pb2 import LoadBreakSwitch as PBLoadBreakSwitch
 from zepben.protobuf.cim.iec61970.base.wires.PerLengthImpedance_pb2 import PerLengthImpedance as PBPerLengthImpedance
 from zepben.protobuf.cim.iec61970.base.wires.PerLengthLineParameter_pb2 import PerLengthLineParameter as PBPerLengthLineParameter
@@ -98,14 +105,15 @@
 from zepben.protobuf.cim.iec61970.base.wires.PowerTransformerEnd_pb2 import PowerTransformerEnd as PBPowerTransformerEnd
 from zepben.protobuf.cim.iec61970.base.wires.PowerTransformer_pb2 import PowerTransformer as PBPowerTransformer
 from zepben.protobuf.cim.iec61970.base.wires.ProtectedSwitch_pb2 import ProtectedSwitch as PBProtectedSwitch
 from zepben.protobuf.cim.iec61970.base.wires.RatioTapChanger_pb2 import RatioTapChanger as PBRatioTapChanger
 from zepben.protobuf.cim.iec61970.base.wires.Recloser_pb2 import Recloser as PBRecloser
 from zepben.protobuf.cim.iec61970.base.wires.RegulatingCondEq_pb2 import RegulatingCondEq as PBRegulatingCondEq
 from zepben.protobuf.cim.iec61970.base.wires.RegulatingControl_pb2 import RegulatingControl as PBRegulatingControl
+from zepben.protobuf.cim.iec61970.base.wires.SeriesCompensator_pb2 import SeriesCompensator as PBSeriesCompensator
 from zepben.protobuf.cim.iec61970.base.wires.ShuntCompensator_pb2 import ShuntCompensator as PBShuntCompensator
 from zepben.protobuf.cim.iec61970.base.wires.Switch_pb2 import Switch as PBSwitch
 from zepben.protobuf.cim.iec61970.base.wires.TapChanger_pb2 import TapChanger as PBTapChanger
 from zepben.protobuf.cim.iec61970.base.wires.TapChangerControl_pb2 import TapChangerControl as PBTapChangerControl
 from zepben.protobuf.cim.iec61970.base.wires.TransformerEnd_pb2 import TransformerEnd as PBTransformerEnd
 from zepben.protobuf.cim.iec61970.base.wires.TransformerEndRatedS_pb2 import TransformerEndRatedS as PBTransformerEndRatedS
 from zepben.protobuf.cim.iec61970.base.wires.TransformerStarImpedance_pb2 import TransformerStarImpedance as PBTransformerStarImpedance
@@ -114,15 +122,14 @@
 from zepben.protobuf.cim.iec61970.base.wires.generation.production.PowerElectronicsUnit_pb2 import PowerElectronicsUnit as PBPowerElectronicsUnit
 from zepben.protobuf.cim.iec61970.base.wires.generation.production.PowerElectronicsWindUnit_pb2 import PowerElectronicsWindUnit as PBPowerElectronicsWindUnit
 from zepben.protobuf.cim.iec61970.infiec61970.feeder.Circuit_pb2 import Circuit as PBCircuit
 from zepben.protobuf.cim.iec61970.infiec61970.feeder.Loop_pb2 import Loop as PBLoop
 from zepben.protobuf.cim.iec61970.infiec61970.feeder.LvFeeder_pb2 import LvFeeder as PBLvFeeder
 from zepben.protobuf.cim.iec61970.infiec61970.wires.generation.production.EvChargingUnit_pb2 import EvChargingUnit as PBEvChargingUnit
 
-from zepben.evolve import TransformerCoolingType
 from zepben.evolve.model.cim.iec61968.assetinfo.no_load_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.open_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.power_transformer_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.short_circuit_test import *
 from zepben.evolve.model.cim.iec61968.assetinfo.shunt_compensator_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.switch_info import *
 from zepben.evolve.model.cim.iec61968.assetinfo.transformer_end_info import *
@@ -133,15 +140,15 @@
 from zepben.evolve.model.cim.iec61968.assets.asset import *
 from zepben.evolve.model.cim.iec61968.assets.asset_info import *
 from zepben.evolve.model.cim.iec61968.assets.asset_organisation_role import *
 from zepben.evolve.model.cim.iec61968.assets.pole import *
 from zepben.evolve.model.cim.iec61968.assets.streetlight import *
 from zepben.evolve.model.cim.iec61968.assets.structure import *
 from zepben.evolve.model.cim.iec61968.common.location import *
-from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_relay_info import *
+from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.relay_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.current_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.potential_transformer_info import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.transformer_construction_kind import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infassetinfo.transformer_function_kind import *
 from zepben.evolve.model.cim.iec61968.infiec61968.infcommon.ratio import *
 from zepben.evolve.model.cim.iec61968.metering.metering import *
 from zepben.evolve.model.cim.iec61968.operations.operational_restriction import *
@@ -164,45 +171,54 @@
 from zepben.evolve.model.cim.iec61970.base.domain.unit_symbol import *
 from zepben.evolve.model.cim.iec61970.base.equivalents.equivalent_branch import *
 from zepben.evolve.model.cim.iec61970.base.equivalents.equivalent_equipment import *
 from zepben.evolve.model.cim.iec61970.base.meas.control import *
 from zepben.evolve.model.cim.iec61970.base.meas.iopoint import *
 from zepben.evolve.model.cim.iec61970.base.meas.measurement import *
 from zepben.evolve.model.cim.iec61970.base.protection.current_relay import *
-from zepben.evolve.model.cim.iec61970.base.protection.protection_equipment import *
+from zepben.evolve.model.cim.iec61970.base.protection.distance_relay import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_function import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_scheme import *
+from zepben.evolve.model.cim.iec61970.base.protection.protection_relay_system import *
+from zepben.evolve.model.cim.iec61970.base.protection.relay_setting import *
+from zepben.evolve.model.cim.iec61970.base.protection.voltage_relay import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_control import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_point import *
 from zepben.evolve.model.cim.iec61970.base.scada.remote_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.aclinesegment import *
 from zepben.evolve.model.cim.iec61970.base.wires.breaker import Breaker
 from zepben.evolve.model.cim.iec61970.base.wires.connectors import *
 from zepben.evolve.model.cim.iec61970.base.wires.disconnector import Disconnector
 from zepben.evolve.model.cim.iec61970.base.wires.energy_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_consumer import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source import *
 from zepben.evolve.model.cim.iec61970.base.wires.energy_source_phase import *
 from zepben.evolve.model.cim.iec61970.base.wires.fuse import Fuse
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.battery_state_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.generation.production.power_electronics_unit import *
+from zepben.evolve.model.cim.iec61970.base.wires.ground import *
+from zepben.evolve.model.cim.iec61970.base.wires.ground_disconnector import *
 from zepben.evolve.model.cim.iec61970.base.wires.jumper import Jumper
 from zepben.evolve.model.cim.iec61970.base.wires.line import *
 from zepben.evolve.model.cim.iec61970.base.wires.load_break_switch import LoadBreakSwitch
 from zepben.evolve.model.cim.iec61970.base.wires.per_length import *
 from zepben.evolve.model.cim.iec61970.base.wires.phase_shunt_connection_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_electronics_connection import *
 from zepben.evolve.model.cim.iec61970.base.wires.power_transformer import *
 from zepben.evolve.model.cim.iec61970.base.wires.protected_switch import ProtectedSwitch
 from zepben.evolve.model.cim.iec61970.base.wires.recloser import Recloser
 from zepben.evolve.model.cim.iec61970.base.wires.regulating_control import *
 from zepben.evolve.model.cim.iec61970.base.wires.regulating_control_mode_kind import *
+from zepben.evolve.model.cim.iec61970.base.wires.series_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.shunt_compensator import *
 from zepben.evolve.model.cim.iec61970.base.wires.single_phase_kind import *
 from zepben.evolve.model.cim.iec61970.base.wires.switch import *
 from zepben.evolve.model.cim.iec61970.base.wires.tap_changer_control import *
 from zepben.evolve.model.cim.iec61970.base.wires.transformer_star_impedance import *
+from zepben.evolve.model.cim.iec61970.base.wires.transformer_cooling_type import *
 from zepben.evolve.model.cim.iec61970.base.wires.vector_group import *
 from zepben.evolve.model.cim.iec61970.base.wires.winding_connection import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.circuit import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.loop import *
 from zepben.evolve.model.cim.iec61970.infiec61970.feeder.lv_feeder import *
 from zepben.evolve.model.cim.iec61970.infiec61970.protection.power_direction_kind import *
 from zepben.evolve.model.cim.iec61970.infiec61970.protection.protection_kind import *
@@ -216,30 +232,32 @@
 from zepben.evolve.services.network.tracing.feeder.feeder_direction import FeederDirection
 
 __all__ = [
     "cable_info_to_cim", "no_load_test_to_cim", "open_circuit_test_to_cim", "overhead_wire_info_to_cim", "power_transformer_info_to_cim",
     "short_circuit_test_to_cim", "shunt_compensator_info_to_cim", "switch_info_to_cim", "transformer_end_info_to_cim", "transformer_tank_info_to_cim",
     "transformer_test_to_cim", "wire_info_to_cim", "asset_to_cim", "asset_container_to_cim", "asset_info_to_cim", "asset_organisation_role_to_cim",
     "asset_owner_to_cim", "pole_to_cim", "streetlight_to_cim", "structure_to_cim", "location_to_cim", "position_point_to_cim", "street_address_to_cim",
-    "street_detail_to_cim", "town_detail_to_cim", "current_relay_info_to_cim", "current_transformer_info_to_cim", "potential_transformer_info_to_cim",
+    "street_detail_to_cim", "town_detail_to_cim", "relay_info_to_cim", "current_transformer_info_to_cim", "potential_transformer_info_to_cim",
     "ratio_to_cim", "end_device_to_cim", "meter_to_cim", "usage_point_to_cim", "operational_restriction_to_cim", "auxiliary_equipment_to_cim",
     "current_transformer_to_cim", "fault_indicator_to_cim", "potential_transformer_to_cim", "sensor_to_cim", "ac_dc_terminal_to_cim", "base_voltage_to_cim",
     "conducting_equipment_to_cim", "connectivity_node_to_cim", "connectivity_node_container_to_cim", "equipment_to_cim", "equipment_container_to_cim",
     "feeder_to_cim", "geographical_region_to_cim", "power_system_resource_to_cim", "site_to_cim", "sub_geographical_region_to_cim", "substation_to_cim",
     "terminal_to_cim", "equivalent_branch_to_cim", "equivalent_equipment_to_cim", "accumulator_to_cim", "analog_to_cim", "control_to_cim", "discrete_to_cim",
-    "io_point_to_cim", "measurement_to_cim", "current_relay_to_cim", "protection_equipment_to_cim", "remote_control_to_cim", "remote_point_to_cim",
+    "io_point_to_cim", "measurement_to_cim", "current_relay_to_cim", "protection_relay_function_to_cim", "remote_control_to_cim", "remote_point_to_cim",
     "remote_source_to_cim", "battery_unit_to_cim", "photo_voltaic_unit_to_cim", "power_electronics_unit_to_cim", "power_electronics_wind_unit_to_cim",
     "ac_line_segment_to_cim", "breaker_to_cim", "conductor_to_cim", "connector_to_cim", "disconnector_to_cim", "energy_connection_to_cim",
     "energy_consumer_to_cim", "energy_consumer_phase_to_cim", "energy_source_to_cim", "energy_source_phase_to_cim", "fuse_to_cim", "jumper_to_cim",
     "junction_to_cim", "busbar_section_to_cim", "line_to_cim", "linear_shunt_compensator_to_cim", "load_break_switch_to_cim",
     "per_length_line_parameter_to_cim", "per_length_impedance_to_cim", "per_length_sequence_impedance_to_cim", "power_electronics_connection_to_cim",
     "power_electronics_connection_phase_to_cim", "power_transformer_to_cim", "power_transformer_end_to_cim", "transformer_star_impedance_to_cim",
     "protected_switch_to_cim", "ratio_tap_changer_to_cim", "recloser_to_cim", "regulating_cond_eq_to_cim", "shunt_compensator_to_cim", "switch_to_cim",
     "tap_changer_to_cim", "transformer_end_to_cim", "circuit_to_cim", "loop_to_cim", "lv_feeder_to_cim", "ev_charging_unit_to_cim",
-    "transformer_end_rated_s_to_cim", "tap_changer_control_to_cim", "regulating_control_to_cim"
+    "transformer_end_rated_s_to_cim", "tap_changer_control_to_cim", "regulating_control_to_cim", "distance_relay_to_cim", "protection_relay_scheme_to_cim",
+    "protection_relay_system_to_cim", "relay_setting_to_cim", "voltage_relay_to_cim", "ground_to_cim", "ground_disconnector_to_cim", "series_compensator_to_cim",
+
 ]
 
 
 #######################
 # IEC61968 ASSET INFO #
 #######################
 
@@ -533,18 +551,19 @@
 PBTownDetail.to_cim = town_detail_to_cim
 
 
 #####################################
 # IEC61968 infIEC61968 InfAssetInfo #
 #####################################
 
-def current_relay_info_to_cim(pb: PBCurrentRelayInfo, network_service: NetworkService) -> Optional[CurrentRelayInfo]:
-    cim = CurrentRelayInfo(
+def relay_info_to_cim(pb: PBRelayInfo, network_service: NetworkService) -> Optional[RelayInfo]:
+    cim = RelayInfo(
         mrid=pb.mrid(),
         curve_setting=str_or_none(pb.curveSetting),
+        reclose_fast=None if pb.HasField("recloseFastNull") else pb.recloseFastSet,
         reclose_delays=list(pb.recloseDelays)
     )
 
     asset_info_to_cim(pb.ai, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
@@ -580,15 +599,15 @@
         secondary_ratio=float_or_none(pb.secondaryRatio)
     )
 
     asset_info_to_cim(pb.ai, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
-PBCurrentRelayInfo.to_cim = current_relay_info_to_cim
+PBRelayInfo.to_cim = relay_info_to_cim
 PBCurrentTransformerInfo.to_cim = current_transformer_info_to_cim
 PBPotentialTransformerInfo.to_cim = potential_transformer_info_to_cim
 
 
 ##################################
 # IEC61968 infIEC61968 InfCommon #
 ##################################
@@ -691,22 +710,23 @@
     network_service.resolve_or_defer_reference(resolver.potential_transformer_info(cim), pb.asset_info_mrid())
 
     sensor_to_cim(pb.sn, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
 def sensor_to_cim(pb: PBSensor, cim: Sensor, network_service: NetworkService):
+    for mrid in pb.relayFunctionMRIDs:
+        network_service.resolve_or_defer_reference(resolver.sen_relay_function(cim), mrid)
     auxiliary_equipment_to_cim(pb.ae, cim, network_service)
 
 
 PBAuxiliaryEquipment.to_cim = auxiliary_equipment_to_cim
 PBCurrentTransformer.to_cim = current_transformer_to_cim
 PBFaultIndicator.to_cim = fault_indicator_to_cim
 PBPotentialTransformer.to_cim = potential_transformer_to_cim
-PBSensor.to_cim = sensor_to_cim
 
 
 ######################
 # IEC61970 BASE CORE #
 ######################
 
 def ac_dc_terminal_to_cim(pb: PBAcDcTerminal, cim: AcDcTerminal, network_service: NetworkService):
@@ -969,33 +989,106 @@
     cim = CurrentRelay(
         mrid=pb.mrid(),
         current_limit_1=float_or_none(pb.currentLimit1),
         inverse_time_flag=None if pb.HasField("inverseTimeFlagNull") else pb.inverseTimeFlagSet,
         time_delay_1=float_or_none(pb.timeDelay1)
     )
 
-    network_service.resolve_or_defer_reference(resolver.current_relay_info(cim), pb.asset_info_mrid())
+    protection_relay_function_to_cim(pb.prf, cim, network_service)
+    return cim if network_service.add(cim) else None
+
 
-    protection_equipment_to_cim(pb.pe, cim, network_service)
+def distance_relay_to_cim(pb: PBDistanceRelay, network_service: NetworkService) -> Optional[DistanceRelay]:
+    cim = DistanceRelay(
+        mrid=pb.mrid(),
+        backward_blind=float_or_none(pb.backwardBlind),
+        backward_reach=float_or_none(pb.backwardReach),
+        backward_reactance=float_or_none(pb.backwardReactance),
+        forward_blind=float_or_none(pb.forwardBlind),
+        forward_reach=float_or_none(pb.forwardReach),
+        forward_reactance=float_or_none(pb.forwardReactance),
+        operation_phase_angle1=float_or_none(pb.operationPhaseAngle1),
+        operation_phase_angle2=float_or_none(pb.operationPhaseAngle2),
+        operation_phase_angle3=float_or_none(pb.operationPhaseAngle3)
+    )
+
+    protection_relay_function_to_cim(pb.prf, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
-def protection_equipment_to_cim(pb: PBProtectionEquipment, cim: ProtectionEquipment, network_service: NetworkService):
+def protection_relay_function_to_cim(pb: PBProtectionRelayFunction, cim: ProtectionRelayFunction, network_service: NetworkService):
+    cim.model = str_or_none(pb.model)
+    cim.reclosing = None if pb.HasField("reclosingNull") else pb.reclosingSet
+    for time_limit in pb.timeLimits:
+        cim.add_time_limit(time_limit)
+    for threshold in pb.thresholds:
+        cim.add_threshold(relay_setting_to_cim(threshold))
     cim.relay_delay_time = float_or_none(pb.relayDelayTime)
     cim.protection_kind = ProtectionKind(pb.protectionKind)
+    for mrid in pb.protectedSwitchMRIDs:
+        network_service.resolve_or_defer_reference(resolver.prf_protected_switch(cim), mrid)
     cim.directable = None if pb.HasField("directableNull") else pb.directableSet
     cim.power_direction = PowerDirectionKind(pb.powerDirection)
+    for mrid in pb.sensorMRIDs:
+        network_service.resolve_or_defer_reference(resolver.prf_sensor(cim), mrid)
+    for mrid in pb.schemeMRIDs:
+        network_service.resolve_or_defer_reference(resolver.prf_scheme(cim), mrid)
+    network_service.resolve_or_defer_reference(resolver.relay_info(cim), pb.asset_info_mrid())
 
-    for mrid in pb.protectedSwitchMRIDs:
-        network_service.resolve_or_defer_reference(resolver.protected_switches(cim), mrid)
+    power_system_resource_to_cim(pb.psr, cim, network_service)
+
+
+def protection_relay_scheme_to_cim(pb: PBProtectionRelayScheme, network_service: NetworkService) -> Optional[ProtectionRelayScheme]:
+    cim = ProtectionRelayScheme(
+        mrid=pb.mrid()
+    )
+
+    # TODO: I think I just throw the nullable mrid at the bound resolver safely?
+    network_service.resolve_or_defer_reference(resolver.prscheme_system(cim), pb.systemMRID)
+
+    for mrid in pb.functionMRIDs:
+        network_service.resolve_or_defer_reference(resolver.prscheme_function(cim), mrid)
+
+    identified_object_to_cim(pb.io, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
+def protection_relay_system_to_cim(pb: PBProtectionRelaySystem, network_service: NetworkService) -> Optional[ProtectionRelaySystem]:
+    cim = ProtectionRelaySystem(
+        mrid=pb.mrid(),
+        protection_kind=ProtectionKind(pb.protectionKind)
+    )
+
+    for mrid in pb.schemeMRIDs:
+        network_service.resolve_or_defer_reference(resolver.prsystem_scheme(cim), mrid)
 
     equipment_to_cim(pb.eq, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
+def relay_setting_to_cim(pb: PBRelaySetting) -> Optional[RelaySetting]:
+    return RelaySetting(
+        name=pb.name,
+        unit_symbol=unit_symbol_from_id(pb.unitSymbol),
+        value=float_or_none(pb.value)
+    )
+
+
+def voltage_relay_to_cim(pb: PBVoltageRelay, network_service: NetworkService) -> Optional[VoltageRelay]:
+    cim = VoltageRelay(pb.mrid())
+
+    protection_relay_function_to_cim(pb.prf, cim, network_service)
+    return cim if network_service.add(cim) else None
 
 
 PBCurrentRelay.to_cim = current_relay_to_cim
+PBDistanceRelay.to_cim = distance_relay_to_cim
+PBProtectionRelayScheme.to_cim = protection_relay_scheme_to_cim
+PBProtectionRelaySystem.to_cim = protection_relay_system_to_cim
+PBVoltageRelay.to_cim = voltage_relay_to_cim
 
 
 #######################
 # IEC61970 BASE SCADA #
 #######################
 
 def remote_control_to_cim(pb: PBRemoteControl, network_service: NetworkService) -> Optional[RemoteControl]:
@@ -1094,15 +1187,15 @@
     protected_switch_to_cim(pb.sw, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
 def conductor_to_cim(pb: PBConductor, cim: Conductor, network_service: NetworkService):
     cim.length = float_or_none(pb.length)
 
-    network_service.resolve_or_defer_reference(resolver.asset_info(cim), pb.asset_info_mrid())
+    network_service.resolve_or_defer_reference(resolver.wire_info(cim), pb.asset_info_mrid())
 
     conducting_equipment_to_cim(pb.ce, cim, network_service)
 
 
 def connector_to_cim(pb: PBConnector, cim: Connector, network_service: NetworkService):
     conducting_equipment_to_cim(pb.ce, cim, network_service)
 
@@ -1198,14 +1291,30 @@
     power_system_resource_to_cim(pb.psr, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
 def fuse_to_cim(pb: PBFuse, network_service: NetworkService) -> Optional[Fuse]:
     cim = Fuse(mrid=pb.mrid())
 
+    network_service.resolve_or_defer_reference(resolver.fuse_function(cim), pb.functionMRID)
+
+    switch_to_cim(pb.sw, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
+def ground_to_cim(pb: PBGround, network_service: NetworkService) -> Optional[Ground]:
+    cim = Ground(mrid=pb.mrid())
+
+    conducting_equipment_to_cim(pb.ce, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
+def ground_disconnector_to_cim(pb: PBGroundDisconnector, network_service: NetworkService) -> Optional[GroundDisconnector]:
+    cim = GroundDisconnector(mrid=pb.mrid())
+
     switch_to_cim(pb.sw, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
 def jumper_to_cim(pb: PBJumper, network_service: NetworkService) -> Optional[Jumper]:
     cim = Jumper(mrid=pb.mrid())
 
@@ -1394,16 +1503,16 @@
     identified_object_to_cim(pb.io, cim, network_service)
     return cim if network_service.add(cim) else None
 
 
 def protected_switch_to_cim(pb: PBProtectedSwitch, cim: ProtectedSwitch, network_service: NetworkService):
     cim.breaking_capacity = int_or_none(pb.breakingCapacity)
 
-    for mrid in pb.operatedByProtectionEquipmentMRIDs:
-        network_service.resolve_or_defer_reference(resolver.operated_by_protection_equipment(cim), mrid)
+    for mrid in pb.relayFunctionMRIDs:
+        network_service.resolve_or_defer_reference(resolver.ps_relay_function(cim), mrid)
 
     switch_to_cim(pb.sw, cim, network_service)
 
 
 def ratio_tap_changer_to_cim(pb: PBRatioTapChanger, network_service: NetworkService) -> Optional[RatioTapChanger]:
     cim = RatioTapChanger(
         mrid=pb.mrid(),
@@ -1435,21 +1544,37 @@
     cim.mode = RegulatingControlModeKind(pb.mode)
     cim.monitored_phase = phase_code_by_id(pb.monitoredPhase)
     cim.target_deadband = float_or_none(pb.targetDeadband)
     cim.target_value = float_or_none(pb.targetValue)
     cim.enabled = None if pb.HasField("enabledNull") else pb.enabledSet
     cim.max_allowed_target_value = float_or_none(pb.maxAllowedTargetValue)
     cim.min_allowed_target_value = float_or_none(pb.minAllowedTargetValue)
+    cim.rated_current = float_or_none(pb.ratedCurrent)
     network_service.resolve_or_defer_reference(resolver.rc_terminal(cim), pb.terminalMRID)
     for mrid in pb.regulatingCondEqMRIDs:
         network_service.resolve_or_defer_reference(resolver.rc_regulating_cond_eq(cim), mrid)
 
     power_system_resource_to_cim(pb.psr, cim, network_service)
 
 
+def series_compensator_to_cim(pb: PBSeriesCompensator, network_service: NetworkService) -> Optional[SeriesCompensator]:
+    cim = SeriesCompensator(
+        mrid=pb.mrid(),
+        r=float_or_none(pb.r),
+        r0=float_or_none(pb.r0),
+        x=float_or_none(pb.x),
+        x0=float_or_none(pb.x0),
+        varistor_rated_current=int_or_none(pb.varistorRatedCurrent),
+        varistor_voltage_threshold=int_or_none(pb.varistorVoltageThreshold)
+    )
+
+    conducting_equipment_to_cim(pb.ce, cim, network_service)
+    return cim if network_service.add(cim) else None
+
+
 def shunt_compensator_to_cim(pb: PBShuntCompensator, cim: ShuntCompensator, network_service: NetworkService):
     network_service.resolve_or_defer_reference(resolver.shunt_compensator_info(cim), pb.asset_info_mrid())
     cim.sections = float_or_none(pb.sections)
     cim.grounded = pb.grounded
     cim.nom_u = int_or_none(pb.nomU)
     cim.phase_connection = PhaseShuntConnectionKind(pb.phaseConnection)
 
@@ -1517,14 +1642,16 @@
 PBDisconnector.to_cim = disconnector_to_cim
 PBEnergyConnection.to_cim = energy_connection_to_cim
 PBEnergyConsumer.to_cim = energy_consumer_to_cim
 PBEnergyConsumerPhase.to_cim = energy_consumer_phase_to_cim
 PBEnergySource.to_cim = energy_source_to_cim
 PBEnergySourcePhase.to_cim = energy_source_phase_to_cim
 PBFuse.to_cim = fuse_to_cim
+PBGround.to_cim = ground_to_cim
+PBGroundDisconnector.to_cim = ground_disconnector_to_cim
 PBJumper.to_cim = jumper_to_cim
 PBJunction.to_cim = junction_to_cim
 PBBusbarSection.to_cim = busbar_section_to_cim
 PBLine.to_cim = line_to_cim
 PBLinearShuntCompensator.to_cim = linear_shunt_compensator_to_cim
 PBLoadBreakSwitch.to_cim = load_break_switch_to_cim
 PBPerLengthSequenceImpedance.to_cim = per_length_sequence_impedance_to_cim
@@ -1536,14 +1663,15 @@
 PBPowerTransformerEnd.to_cim = power_transformer_end_to_cim
 PBTransformerEndRatedS.to_cim = transformer_end_rated_s_to_cim
 PBTransformerStarImpedance.to_cim = transformer_star_impedance_to_cim
 PBProtectedSwitch.to_cim = protected_switch_to_cim
 PBRatioTapChanger.to_cim = ratio_tap_changer_to_cim
 PBRecloser.to_cim = recloser_to_cim
 PBRegulatingCondEq.to_cim = regulating_cond_eq_to_cim
+PBSeriesCompensator.to_cim = series_compensator_to_cim
 PBShuntCompensator.to_cim = shunt_compensator_to_cim
 PBSwitch.to_cim = switch_to_cim
 PBTapChanger.to_cim = tap_changer_to_cim
 PBTransformerEnd.to_cim = transformer_end_to_cim
 PBTapChangerControl.to_cim = tap_changer_control_to_cim
```

## zepben/evolve/streaming/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/streaming/exceptions.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 __all__ = ["GrpcConnectionException", "UnsupportedOperationException"]
```

## zepben/evolve/streaming/get/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/streaming/get/consumer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
```

## zepben/evolve/streaming/get/customer_consumer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from __future__ import annotations
```

## zepben/evolve/streaming/get/diagram_consumer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 from asyncio import get_event_loop
```

## zepben/evolve/streaming/get/network_consumer.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 
 import warnings
@@ -22,16 +22,18 @@
 from zepben.evolve import NetworkService, Feeder, IdentifiedObject, CableInfo, OverheadWireInfo, AssetOwner, \
     Organisation, Location, Meter, UsagePoint, OperationalRestriction, FaultIndicator, BaseVoltage, ConnectivityNode, GeographicalRegion, Site, \
     SubGeographicalRegion, Substation, Terminal, AcLineSegment, Breaker, Disconnector, EnergyConsumer, EnergyConsumerPhase, EnergySource, EnergySourcePhase, \
     Fuse, Jumper, Junction, LinearShuntCompensator, PerLengthSequenceImpedance, PowerTransformer, PowerTransformerEnd, RatioTapChanger, Recloser, Circuit, \
     Loop, Pole, Streetlight, Accumulator, Analog, Discrete, Control, RemoteControl, RemoteSource, PowerTransformerInfo, PowerElectronicsConnection, \
     PowerElectronicsConnectionPhase, BatteryUnit, PhotoVoltaicUnit, PowerElectronicsWindUnit, BusbarSection, LoadBreakSwitch, TransformerTankInfo, \
     TransformerEndInfo, TransformerStarImpedance, EquipmentContainer, NetworkHierarchy, MultiObjectResult, CimConsumerClient, NoLoadTest, OpenCircuitTest, \
-    ShortCircuitTest, EquivalentBranch, ShuntCompensatorInfo, LvFeeder, CurrentRelay, CurrentTransformer, CurrentRelayInfo, SwitchInfo, \
-    CurrentTransformerInfo, EvChargingUnit, TapChangerControl, ServiceInfo, PotentialTransformer, PotentialTransformerInfo
+    ShortCircuitTest, EquivalentBranch, ShuntCompensatorInfo, LvFeeder, CurrentRelay, CurrentTransformer, RelayInfo, SwitchInfo, \
+    CurrentTransformerInfo, EvChargingUnit, TapChangerControl, ServiceInfo, PotentialTransformer, DistanceRelay, VoltageRelay, ProtectionRelayScheme, \
+    ProtectionRelaySystem, GroundDisconnector, Ground, SeriesCompensator, PotentialTransformerInfo
+
 from zepben.evolve.streaming.grpc.grpc import GrpcResult
 
 __all__ = ["NetworkConsumerClient", "SyncNetworkConsumerClient"]
 
 
 MAX_64_BIT_INTEGER = 9223372036854775807
 
@@ -665,14 +667,15 @@
 
     # IEC61968 OPERATIONS #
     "operationalRestriction": OperationalRestriction,
 
     # IEC61968 InfIEC61968 ASSET INFO #
     "currentTransformerInfo": CurrentTransformerInfo,
     "potentialTransformerInfo": PotentialTransformerInfo,
+    "relayInfo": RelayInfo,
 
     # IEC61970 BASE AUXILIARY EQUIPMENT #
     "currentTransformer": CurrentTransformer,
     "faultIndicator": FaultIndicator,
     "potentialTransformer": PotentialTransformer,
 
     # IEC61970 BASE CORE #
@@ -690,14 +693,21 @@
 
     # IEC61970 BASE MEAS #
     "accumulator": Accumulator,
     "analog": Analog,
     "control": Control,
     "discrete": Discrete,
 
+    # IEC61970 BASE PROTECTION #
+    "currentRelay": CurrentRelay,
+    "distanceRelay": DistanceRelay,
+    "protectionRelayScheme": ProtectionRelayScheme,
+    "protectionRelaySystem": ProtectionRelaySystem,
+    "voltageRelay": VoltageRelay,
+
     # IEC61970 BASE SCADA #
     "remoteControl": RemoteControl,
     "remoteSource": RemoteSource,
 
     # IEC61970 BASE WIRES GENERATION PRODUCTION #
     "batteryUnit": BatteryUnit,
     "photoVoltaicUnit": PhotoVoltaicUnit,
@@ -709,32 +719,33 @@
     "busbarSection": BusbarSection,
     "disconnector": Disconnector,
     "energyConsumer": EnergyConsumer,
     "energyConsumerPhase": EnergyConsumerPhase,
     "energySource": EnergySource,
     "energySourcePhase": EnergySourcePhase,
     "fuse": Fuse,
+    "ground": Ground,
+    "groundDisconnector": GroundDisconnector,
     "jumper": Jumper,
     "junction": Junction,
     "linearShuntCompensator": LinearShuntCompensator,
     "loadBreakSwitch": LoadBreakSwitch,
     "perLengthSequenceImpedance": PerLengthSequenceImpedance,
     "powerElectronicsConnection": PowerElectronicsConnection,
     "powerElectronicsConnectionPhase": PowerElectronicsConnectionPhase,
     "powerTransformer": PowerTransformer,
     "powerTransformerEnd": PowerTransformerEnd,
     "ratioTapChanger": RatioTapChanger,
     "recloser": Recloser,
+    "seriesCompensator": SeriesCompensator,
     "tapChangerControl": TapChangerControl,
     "transformerStarImpedance": TransformerStarImpedance,
 
     # IEC61970 InfIEC61970 FEEDER #
     "circuit": Circuit,
     "loop": Loop,
     "lvFeeder": LvFeeder,
-    "currentRelay": CurrentRelay,
-    "currentRelayInfo": CurrentRelayInfo,
     "switchInfo": SwitchInfo,
 
     # IEC61970 InfIEC61970 WIRES GENERATION PRODUCTION #
     "evChargingUnit": EvChargingUnit
 }
```

## zepben/evolve/streaming/get/hierarchy/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/streaming/get/hierarchy/data.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
```

## zepben/evolve/streaming/grpc/__init__.py

```diff
@@ -1,6 +1,6 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/streaming/grpc/auth_token_plugin.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import grpc
 from zepben.auth import ZepbenTokenFetcher
```

## zepben/evolve/streaming/grpc/connect.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
```

## zepben/evolve/streaming/grpc/grpc.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
```

## zepben/evolve/streaming/grpc/grpc_channel_builder.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from abc import ABC
 from typing import Optional, List, Tuple, Any
```

## zepben/evolve/testing/__init__.py

```diff
@@ -1,5 +1,5 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
```

## zepben/evolve/testing/test_network_builder.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 try:
     from typing import Protocol
 except ImportError:
```

## zepben/evolve/testing/test_traversal.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from typing import Callable, TypeVar, Tuple, Awaitable
 from unittest.mock import Mock
```

## Comparing `zepben/evolve/database/sqlite/tables/associations/protection_equipment_protected_switches.py` & `zepben/evolve/database/sqlite/tables/associations/protection_relay_functions_protected_switches.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from typing import List
 
 from zepben.evolve.database.sqlite.tables.column import Column, Nullable
 from zepben.evolve.database.sqlite.tables.sqlite_table import SqliteTable
 
-__all__ = ["TableProtectionEquipmentProtectedSwitches"]
+__all__ = ["TableProtectionRelayFunctionsProtectedSwitches"]
 
 
-class TableProtectionEquipmentProtectedSwitches(SqliteTable):
-    protection_equipment_mrid: Column = None
+class TableProtectionRelayFunctionsProtectedSwitches(SqliteTable):
+    protection_relay_function_mrid: Column = None
     protected_switch_mrid: Column = None
 
     def __init__(self):
-        super(TableProtectionEquipmentProtectedSwitches, self).__init__()
-        self.protection_equipment_mrid = self._create_column("protection_equipment_mrid", "TEXT", Nullable.NOT_NULL)
+        super(TableProtectionRelayFunctionsProtectedSwitches, self).__init__()
+        self.protection_relay_function_mrid = self._create_column("protection_relay_function_mrid", "TEXT", Nullable.NOT_NULL)
         self.protected_switch_mrid = self._create_column("protected_switch_mrid", "TEXT", Nullable.NOT_NULL)
 
     def name(self) -> str:
-        return "protection_equipment_protected_switches"
+        return "protection_relay_functions_protected_switches"
 
     def unique_index_columns(self) -> List[List[Column]]:
-        cols = super(TableProtectionEquipmentProtectedSwitches, self).unique_index_columns()
-        cols.append([self.protection_equipment_mrid, self.protected_switch_mrid])
+        cols = super(TableProtectionRelayFunctionsProtectedSwitches, self).unique_index_columns()
+        cols.append([self.protection_relay_function_mrid, self.protected_switch_mrid])
         return cols
 
     def non_unique_index_columns(self) -> List[List[Column]]:
-        cols = super(TableProtectionEquipmentProtectedSwitches, self).non_unique_index_columns()
-        cols.append([self.protection_equipment_mrid])
+        cols = super(TableProtectionRelayFunctionsProtectedSwitches, self).non_unique_index_columns()
+        cols.append([self.protection_relay_function_mrid])
         cols.append([self.protected_switch_mrid])
         return cols
```

## Comparing `zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_relay_info.py` & `zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/relay_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,116 @@
-#  Copyright 2023 Zeppelin Bend Pty Ltd
+#  Copyright 2024 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from __future__ import annotations
 from typing import Optional, List, Generator
 
 from zepben.evolve.model.cim.iec61968.assets.asset_info import AssetInfo
 from zepben.evolve.util import ngen, nlen, safe_remove, require
 
-__all__ = ["CurrentRelayInfo"]
+__all__ = ["RelayInfo"]
 
 
-class CurrentRelayInfo(AssetInfo):
-    """Current Relay Datasheet Information."""
+class RelayInfo(AssetInfo):
+    """Relay Datasheet Information."""
 
     curve_setting: Optional[str] = None
-    """The type of curve used for the Current Relay."""
+    """The type of curve used for the Relay."""
+
+    reclose_fast: Optional[bool] = None
+    """True if reclose_delays are associated with a fast Curve, false otherwise."""
 
     _reclose_delays: Optional[List[float]] = None
 
     def __init__(self, reclose_delays: Optional[List[float]] = None, **kwargs):
-        super(CurrentRelayInfo, self).__init__(**kwargs)
+        super(RelayInfo, self).__init__(**kwargs)
         if reclose_delays:
             for index, delay in enumerate(reclose_delays):
                 self.add_delay(delay, index)
 
     @property
     def reclose_delays(self) -> Generator[float, None, None]:
         """
         The reclose delays for this curve and relay type. The index of the list is the reclose step, and the value is the overall delay time.
         """
         return ngen(self._reclose_delays)
 
     def num_delays(self) -> int:
         """
-        Get the numder of reclose delays for this `CurrentRelayInfo`
+        Get the number of reclose delays for this :class:`RelayInfo`
         """
         return nlen(self._reclose_delays)
 
     def get_delay(self, index: int) -> Optional[float]:
+        """
+        Get the reclose delay at the specified index, if it exists. Otherwise, this returns
+
+        :param index: The index of the delay to retrieve.
+        :return: The reclose delay at `index` if it exists, otherwise None.
+        """
         if self._reclose_delays:
             return self._reclose_delays[index] if index in range(len(self._reclose_delays)) else None
         else:
-            return None
+            raise IndexError(index)
 
-    def add_delay(self, delay: float, index: int = None) -> CurrentRelayInfo:
+    def add_delay(self, delay: float, index: int = None) -> RelayInfo:
         """
-        Add a reclose delay
-        `delay` The delay in seconds to add.
-        `index` The index into the list to add the delay at. Defaults to the end of the list.
-        Returns A reference to this `CurrentRelayInfo` to allow fluent use.
+        Add a reclose delay.
+
+        :param delay: The delay in seconds to add.
+        :param index: The index into the list to add the delay at. Defaults to the end of the list.
+        :return: A reference to this :class:`RelayInfo` to allow fluent use.
         """
         if index is None:
             index = self.num_delays()
         require(0 <= index <= self.num_delays(),
                 lambda: f"Unable to add float to {str(self)}. Index number {index} "
                         f"is invalid. Expected a value between 0 and {self.num_delays()}. Make sure you are "
                         f"adding the reclose_delays in the correct order and there are no gaps in the numbering.")
         self._reclose_delays = list() if self._reclose_delays is None else self._reclose_delays
         self._reclose_delays.insert(index, delay)
         return self
 
-    def set_delays(self, delays: List[float]) -> CurrentRelayInfo:
+    def set_delays(self, delays: List[float]) -> RelayInfo:
         """
-        Set the reclose delays for this CurrentRelayInfo
+        Set the reclose delays for this :class:`RelayInfo`.
 
-        `delays` The delays to set. The provided list will be copied.
-        Returns A reference to this `CurrentRelayInfo` to allow fluent use.
+        :param delays: The delays to set. The provided list will be copied.
+        :return: A reference to this :class:`RelayInfo` to allow fluent use.
         """
         self._reclose_delays = delays.copy()
         return self
 
-    def remove_delay_by_delay(self, delay: float) -> CurrentRelayInfo:
+    def remove_delay(self, delay: float) -> RelayInfo:
         """
         Remove a delay from the list.
-        `delay` The delay to remove.
-        Returns A reference to this `CurrentRelayInfo` to allow fluent use.
+
+        :param delay: The delay to remove.
+        :return: A reference to this :class:`RelayInfo` to allow fluent use.
         """
         self._reclose_delays = safe_remove(self._reclose_delays, delay)
         return self
 
-    def remove_delay(self, index: int) -> Optional[float]:
+    def remove_delay_at(self, index: int) -> Optional[float]:
         """
         Remove a delay from the list.
-        `index` The index of the delay to remove.
-        Returns The delay that was removed, or `None` if no delay was present at `index`.
+
+        :param index: The index of the delay to remove.
+        :return: The delay that was removed, or `None` if no delay was present at `index`.
         """
         if self._reclose_delays:
             try:
                 return self._reclose_delays.pop(index)
             except IndexError:
                 return None
         return None
 
-    def clear_delays(self) -> CurrentRelayInfo:
+    def clear_delays(self) -> RelayInfo:
         """
         Clear all reclose delays.
-        Returns A reference to this `CurrentRelayInfo` to allow fluent use.
+
+        :return: A reference to this :class:`RelayInfo` to allow fluent use.
         """
         self._reclose_delays = None
         return self
```

## Comparing `zepben.evolve-0.38.0b7.dist-info/LICENSE` & `zepben.evolve-0.38.0b8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zepben.evolve-0.38.0b7.dist-info/METADATA` & `zepben.evolve-0.38.0b8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zepben.evolve
-Version: 0.38.0b7
+Version: 0.38.0b8
 Summary: Python SDK for interacting with the Evolve platform
 Home-page: https://github.com/zepben/evolve-sdk-python
 Author: Kurt Greaves
 Author-email: kurt.greaves@zepben.com
 License: MPL 2.0
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests <2.27.0,>=2.26.0
 Requires-Dist: zepben.auth ==0.11.0
-Requires-Dist: zepben.protobuf ==0.26.0
+Requires-Dist: zepben.protobuf ==0.27.0b5
 Requires-Dist: dataclassy ==0.6.2
 Requires-Dist: six ==1.16.0
 Provides-Extra: test
 Requires-Dist: pytest ==7.1.2 ; extra == 'test'
 Requires-Dist: pytest-cov ==2.10.1 ; extra == 'test'
 Requires-Dist: pytest-asyncio ==0.19.0 ; extra == 'test'
 Requires-Dist: pytest-timeout ==1.4.2 ; extra == 'test'
```

## Comparing `zepben.evolve-0.38.0b7.dist-info/RECORD` & `zepben.evolve-0.38.0b8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,332 +1,342 @@
-zepben/evolve/__init__.py,sha256=tsViR9H4Vsh0pEvkiQ-wOdoBx7Opvf8_vPwodZu073Y,19009
-zepben/evolve/exceptions.py,sha256=EkNTjvR6UeC8VCAruZGihCdKSh8iXiu0uSqPm9Gvgmw,1387
-zepben/evolve/types.py,sha256=uKIOUunL0LP5CdLENMt7Gyuo6BBC2bf75AQYOPPHzkw,1132
-zepben/evolve/util.py,sha256=aOeCrAjkarUIDU3qOEQ65N-7plt6Kben6yHQkKDJBUg,4576
-zepben/evolve/database/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/database_reader.py,sha256=7eAOET5TRUhIkRWoDPfaimDLNrr47CJhJQQ1AyFmRRw,7148
-zepben/evolve/database/sqlite/database_writer.py,sha256=He0RvIQxzF4gEk6GyAtrRSHea0Ls9Z3QK_Y6w9p6xcs,6108
-zepben/evolve/database/sqlite/readers/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/readers/base_cim_reader.py,sha256=uDpR-OCZ-zp-rlI30yWewuE163D90hGrXrrg8OZKe1Q,5275
-zepben/evolve/database/sqlite/readers/base_service_reader.py,sha256=83i41H1EhiJcp_cSXzr0fXlR1enBwNgShCIiJtS7F7A,2991
-zepben/evolve/database/sqlite/readers/customer_cim_reader.py,sha256=6f46x2HbrR91WR35TQ-kPv0ka11sktAWvoFLrnzrDKE,4510
-zepben/evolve/database/sqlite/readers/customer_service_reader.py,sha256=GriE8_IlirTCeGT1ms6lFeXG16xrntuqE0GgrxtIO9A,1761
-zepben/evolve/database/sqlite/readers/diagram_cim_reader.py,sha256=GTz-BM9J_FDTdrj-iXXnuZVQdp6_tVVZZJ3NvL2wo5I,3245
-zepben/evolve/database/sqlite/readers/diagram_service_reader.py,sha256=PeSrDmYe23_k7TQOT-e2iOqv4JG7YhJ1nvLfKhMqccw,1041
-zepben/evolve/database/sqlite/readers/metadata_collection_reader.py,sha256=0UNBRZQ2QrUp3at5bfWxKn34j2v6dSUjnFUmd6Xce6Q,733
-zepben/evolve/database/sqlite/readers/metadata_entry_reader.py,sha256=dfHFF4QjjuoTOKexHJFT5iEUfiBsWYDPmpYzkmWoM7M,1088
-zepben/evolve/database/sqlite/readers/network_cim_reader.py,sha256=FxNbkoLfyb6JWB3Lty-IPe-9JBV2H19pOpOwhsZSWw0,80182
-zepben/evolve/database/sqlite/readers/network_service_reader.py,sha256=a4ni0F2faRBiICggFHEu0qlr4vi06cqxMZgrCObcPWE,12684
-zepben/evolve/database/sqlite/readers/result_set.py,sha256=JnTHfC-qKhYotRmTGK0Fa7XlktCNleLaQd0XT9wsB2k,6872
-zepben/evolve/database/sqlite/tables/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/tables/column.py,sha256=pFgEpfZ4On3UACTNNyMqzEKavyGCJ1t_2H8dQWwjKj0,1009
-zepben/evolve/database/sqlite/tables/database_tables.py,sha256=KSZg2nCnanRjdncJsjs5bhjTGaiLgaeriyNRJ3iPMH0,12102
-zepben/evolve/database/sqlite/tables/exceptions.py,sha256=fzyiw-vzP1JrTl8m4s_14cu687LccRwE7uoIv1n0c1s,403
-zepben/evolve/database/sqlite/tables/metadata_tables.py,sha256=qeIQCqe77c28ZpN45HQhM_wC-OtRps5wmubsr1MdkJg,1164
-zepben/evolve/database/sqlite/tables/sqlite_table.py,sha256=ZhKJPrCjD9ojKXCwvmHJxyy79bgh0Xv5wMjj8XZNhU0,5820
-zepben/evolve/database/sqlite/tables/associations/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/tables/associations/assetorganisationroles_association_tables.py,sha256=fox6r1gMBY6PlLY8JnjoDPZc_c1YYhsr1TBejnT7a8Q,1484
-zepben/evolve/database/sqlite/tables/associations/circuit_association_tables.py,sha256=XvU47nF-xqcwaiMJRGQYSMUlNk_JnKn-ISZZP76VrsI,2295
-zepben/evolve/database/sqlite/tables/associations/customeragreements_association_tables.py,sha256=SU0Nhd5UGrF1MPQNGQvxyzg2Gz7mrxlFG-q8gh6OGFc,1561
-zepben/evolve/database/sqlite/tables/associations/equipment_association_tables.py,sha256=5mT0RZBUFTMWYh1zeGctE6HeO9ByfPMIzLAG7T4ukjI,3547
-zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py,sha256=XnpDNTu7vWF4yx4qESrcabLzoouHq-5GqNPW5KDzvjg,1696
-zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py,sha256=W-BMoeaIF4otun-39jm6n8MNFuUPtAadsriOiaw-ZQY,1435
-zepben/evolve/database/sqlite/tables/associations/protection_equipment_protected_switches.py,sha256=8cm62CmmC17CvWBX00DgNV6zq8ad_DPk8Esefj3Lhm4,1572
-zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py,sha256=L_plhIn0lrYi3tooEOujaJsZAfLEjtB3mJx3dXoclNc,1409
-zepben/evolve/database/sqlite/tables/iec61968/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py,sha256=4E4Bc0-RBKBKIwIsseJijLXhSgh2rNP46Idkrx3j6to,2240
-zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py,sha256=221mDp5o-nNyDiuTFUy9x4Wc_TYqqiSdv4RrOIaqHwY,9391
-zepben/evolve/database/sqlite/tables/iec61968/common_tables.py,sha256=ReeUvGAQ8N2BkX9jP7X9sAgBWQx7-rWWBcXdzso35pI,5681
-zepben/evolve/database/sqlite/tables/iec61968/customer_tables.py,sha256=Nk0Xg4U1A3IMfbRAD-rCcFvHgBF3Cbq2NVu5BkdFp8g,1705
-zepben/evolve/database/sqlite/tables/iec61968/metering_tables.py,sha256=IbS24zc68_NanfYpHzcJPZwMLIsgV7E9i9Sr6AjtO2Y,1912
-zepben/evolve/database/sqlite/tables/iec61968/operations_tables.py,sha256=hSzTOVvmIHwdxD73svDEnDkiYimLwOk0NkGJsOT-zYQ,494
-zepben/evolve/database/sqlite/tables/iec61968/infiec61968/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py,sha256=i9d7Eq49-FHOyduiOu9B7AlR2R15pobF_HielWvJnmg,5266
-zepben/evolve/database/sqlite/tables/iec61970/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/tables/iec61970/base/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/tables/iec61970/base/auxiliaryequipment_tables.py,sha256=UdtKI9fDF24_sazB7I_eknffti7GN6sHNcyTIcwH9_E,1995
-zepben/evolve/database/sqlite/tables/iec61970/base/core_tables.py,sha256=kz1Rm4ONBVJbwyFQmQE1rYI29A5Df4iPegRp_UZsCf8,8442
-zepben/evolve/database/sqlite/tables/iec61970/base/diagramlayout_tables.py,sha256=Fj-32dWluhWDi5vTs1gSquBouZRkrANIMNllS6Kpd54,3113
-zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py,sha256=ZlEcO89mU7OuKf-bj1iricMkm16Q78DFYKbMday8rxk,2454
-zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py,sha256=WEpRcgCGcX89AFqBl-jrCun36INyHtFgQmL3ClE2s5E,2581
-zepben/evolve/database/sqlite/tables/iec61970/base/protection_tables.py,sha256=pOghLnBK4dqpY03WqRLNnuO-Mram4yK_7TeGDrZbtfM,1900
-zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py,sha256=4dfxpgkRlO5E8YDfswibKC8Hdj4rm1zeo4Pv73e4e08,1205
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/conductor_tables.py,sha256=zkQglBsnFHm9rkvKPahNHVCqAFkq-QxYiLAYrNwkXIk,1226
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/connector_tables.py,sha256=sCM-BulLdiik6eMjVtELD5r_RDDJDP69wnzvpiMvNbM,710
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/container_tables.py,sha256=iGL6w5zcMZJPjLMD4z5rKg9mAbo42YiSJ1qrHytz_L4,458
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/energyconnection_tables.py,sha256=KeiqFD70YhdOX_qZEw2UKAA-n2UWofZlxHgEP4RoU4U,16832
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/perlength_tables.py,sha256=dVh6C2Qh0cEvYuQy9BmDfQdeqbA2ejCbLZ4XWwmZY3w,1845
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py,sha256=00RPMxOOqT7_SHTqeO3awZbep4pznMKmv5pP6Kjlthk,2325
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/transformer_tables.py,sha256=NB3om_k6BCIWmlHXdESQlGRo5lU-mYtkOaEE2uwtvrU,8640
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/production_tables.py,sha256=UKFbbOOONMqkMt1I74j2I6DL4741-fSl2XUBtmqeMvc,2114
-zepben/evolve/database/sqlite/tables/iec61970/infiec61970/__init__.py,sha256=rOE8bsFXgo1wcEQOVSkrtWlhmusQwRThmIXhF2-WvCg,246
-zepben/evolve/database/sqlite/tables/iec61970/infiec61970/feeder_tables.py,sha256=Sp18HftBVu2pcAjIJJLlQiLvxqW1Vxmxs9AZvctoesQ,1515
-zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/__init__.py,sha256=Z43kZuy6PMJMbDL-8XIPllgYW7_oCy9ofZuisQ1ykAA,245
-zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/__init__.py,sha256=Z43kZuy6PMJMbDL-8XIPllgYW7_oCy9ofZuisQ1ykAA,245
-zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/production_tables.py,sha256=5ZPBni1iaVY5Z5aUg9MvQOdtUixUwJJF8gBCCAROv54,454
-zepben/evolve/database/sqlite/writers/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/database/sqlite/writers/base_cim_writer.py,sha256=saoyuBkZ0VVnKvVppEwnKwQKl-Fb_UOJ3pMz0GEsoDs,5263
-zepben/evolve/database/sqlite/writers/base_service_writer.py,sha256=2DN_Sn09tExzI4LVRCYrY_tRId7Q7NwtcIfGzTg-MCg,2995
-zepben/evolve/database/sqlite/writers/customer_cim_writer.py,sha256=Uo2Vcxq7PZ9nSM_BSZ9mDBvv94nqMEAvQNhN0jRiH9Y,4752
-zepben/evolve/database/sqlite/writers/customer_service_writer.py,sha256=neMgC8L-ufkfJiPZmv67KQExTkKjtLQo6dxOyC_UPFU,1393
-zepben/evolve/database/sqlite/writers/diagram_cim_writer.py,sha256=qFoZF2LWs2UIIw-NAMv0jzkjo_o7ktgkl9gUlO-JXXg,2657
-zepben/evolve/database/sqlite/writers/diagram_service_writer.py,sha256=QZidgC3SKeGhlxBuRQev7pixlyuNUcKIXUu0xH8N_cM,1004
-zepben/evolve/database/sqlite/writers/metadata_collection_writer.py,sha256=6YrJCxl2A3JtH3qpme0r6ZAptvEMPcxWmsCWUbKrqv0,904
-zepben/evolve/database/sqlite/writers/metadata_entry_writer.py,sha256=6WF6CEAoA-SerAp8U9O9h_koG711OwxK1a6nWcVpozc,1257
-zepben/evolve/database/sqlite/writers/network_cim_writer.py,sha256=chjK87h7LxFeOH4Vb0uXckyLmRYFuZwKZbg6R-wWlfI,77362
-zepben/evolve/database/sqlite/writers/network_service_writer.py,sha256=wQ2f5LmKEvX1-uTwyiuZjsjEouC_7IYXHzxKa1KDdjw,8548
-zepben/evolve/database/sqlite/writers/utils.py,sha256=X72qUDfmkLhv9qmx9ch186gkEUMG0gAmRjnUNhowUeU,1430
-zepben/evolve/examples/__init__.py,sha256=WvVuw1R-8znfcMkpJ7n46Y9PryD6gX73vzgQDo-Yvyc,302
-zepben/evolve/examples/simple_test_network.py,sha256=BftlT8mvVwowtXjpHqCZk3DN22eQS_zu8r0jec6FsBE,5062
-zepben/evolve/model/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/phases.py,sha256=KLjG017mJC94EQEudotVJgxgMS6nNqICg3qATJL4JUQ,7357
-zepben/evolve/model/resistance_reactance.py,sha256=_JcuS8YYNbn7XSQok0mmCRxN2-zu6v78dzTj0JAGKlM,1502
-zepben/evolve/model/busbranch/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/busbranch/bus_branch.py,sha256=bp7O1yaWJ0IcCJ9pm1rjUdTRLUAZL2kiYOl833DuM5k,47076
-zepben/evolve/model/cim/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61968/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61968/assetinfo/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61968/assetinfo/no_load_test.py,sha256=-1uuB_0OvJL2Sbs2tkFBV4_kfLVHZfkNC9GINUaFQhM,1398
-zepben/evolve/model/cim/iec61968/assetinfo/open_circuit_test.py,sha256=VRBpheu6RXl_KkhSb6MHzQJDJmDTUg-v8aMAWY_2VoA,1445
-zepben/evolve/model/cim/iec61968/assetinfo/power_transformer_info.py,sha256=49bIaUNiblN0rmQgi9sgIbuDDij6UBUQ9iuO6EtVo3U,4220
-zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py,sha256=zVrzIEgWSfqjmNGgDhFYndQYPcPO5d_o_ZbY9J-2kfA,1877
-zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py,sha256=5LZaFycTFvVN8bEZc6Of3PXZhORBdaFIYI5SZYmPI2Y,927
-zepben/evolve/model/cim/iec61968/assetinfo/switch_info.py,sha256=z_Sdq67hg36stoXMuA8RCwqg4js9bBxhF7EL-pcWVg4,550
-zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py,sha256=stDcylZzWrFR2-GJdkDryePbf5buUuSf-Fym96Vx4T4,5904
-zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py,sha256=rHv-1HFDps1c9KcupFd6cjey0RPP-2y7r_VD4r47V28,4395
-zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py,sha256=WYJ21A0BKnNp6GZedydIxNd5B_kl4EPxomOXrVYky8U,860
-zepben/evolve/model/cim/iec61968/assetinfo/wire_info.py,sha256=k5rIKpcRf8hiyuV9m1GC6hMZ6xMjAgk1z50orOjGFPA,1287
-zepben/evolve/model/cim/iec61968/assetinfo/wire_material_kind.py,sha256=GbmPE6KVq0-pjiNXPbCxjXHura8HPJ7SE53GToWcHSc,1015
-zepben/evolve/model/cim/iec61968/assets/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61968/assets/asset.py,sha256=5SEchnyGgnuDtccczwoZUEUorwZjyLk_D-TVa5-BivE,4019
-zepben/evolve/model/cim/iec61968/assets/asset_info.py,sha256=h1NJkXqPShCT4y0XnCTcUen0y_R1RLrtd0S4bFuJb9w,845
-zepben/evolve/model/cim/iec61968/assets/asset_organisation_role.py,sha256=zNhdgiD-rlctproIiIEqhj_7Dwh0O-DWiw326N5NBm8,588
-zepben/evolve/model/cim/iec61968/assets/pole.py,sha256=ySeyAxOYeii0n-ki_E3gYfwCxkPyap3YnOFp4Dp4Pjc,3009
-zepben/evolve/model/cim/iec61968/assets/streetlight.py,sha256=_kvyqvPPvmoMjXF5yrH3Y6-UvjIbG-I0ADM8SaN3Qh4,1157
-zepben/evolve/model/cim/iec61968/assets/structure.py,sha256=H2utfSBpcdjiP3l2REiyl7AfuvzvOiE8OlW-XB_AkDA,635
-zepben/evolve/model/cim/iec61968/common/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61968/common/document.py,sha256=wcCpqmYwpt3Lb0h2pEqJXG65WtKV4fpBqgA6SD9OaBY,1570
-zepben/evolve/model/cim/iec61968/common/location.py,sha256=Yw0MtTpjF4WUYT8Ngs7qVMoMY0TGXtttQa6gcEyR-5E,7841
-zepben/evolve/model/cim/iec61968/common/organisation.py,sha256=opcilE3GP8_IP8HQHPsvcHHhaScpupaHE68P_bMW1mI,531
-zepben/evolve/model/cim/iec61968/common/organisation_role.py,sha256=O4jK0VGpPtYW-H7RUcx0OtYA7-DF0cl9mVGo0L6f8do,838
-zepben/evolve/model/cim/iec61968/customers/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61968/customers/customer.py,sha256=5zvwX_wNieRgFA1DlpHqrqnrqCa21lEMHkE4-k4t0lg,3534
-zepben/evolve/model/cim/iec61968/customers/customer_agreement.py,sha256=KeiIX7e5D_jSfDpaJUi_rdJNDAflnBJsrK2jRTjxubA,4260
-zepben/evolve/model/cim/iec61968/customers/customer_kind.py,sha256=sKjZ4cKnzsd1cPCHxBVfG8jkZcjnxB4NTFZbf2wtGj0,1474
-zepben/evolve/model/cim/iec61968/customers/pricing_structure.py,sha256=3z3U8Wa7ujWFWZ1xXU3f4pemR7EjTgsCN6m0TfGIt_o,3336
-zepben/evolve/model/cim/iec61968/customers/tariff.py,sha256=Unpz6bE_jMqe8DbCBwlZLgVt_mzCUlgL6D6N-VYpXuI,763
-zepben/evolve/model/cim/iec61968/infiec61968/__init__.py,sha256=h12mcI0GTB7_0cBxdlqFSh6GtD6y8qLE7ANyd0YC4uo,244
-zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py,sha256=h12mcI0GTB7_0cBxdlqFSh6GtD6y8qLE7ANyd0YC4uo,244
-zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_relay_info.py,sha256=Jzc4zt23WjoslxMykA_UZ5LsDJjElC5-VNHC-7lVE_E,4000
-zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py,sha256=wqJzbqADT4hNeVRYUl7-zp2PxQGJQygNMlxdblq2eG4,1859
-zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py,sha256=7hAErD71TjNrcC6DvzWb3fBCeorCl1pVR1AG1F1T53Q,1250
-zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py,sha256=8CcKSzi7nVI9Ur4yziFgbQucIAPiy4CbVJmBtK6394Q,993
-zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py,sha256=91_lc1EYCmmoHb4UmzGrdw6E10_gQcynVayzKHbPgO4,1098
-zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61968/infiec61968/infcommon/ratio.py,sha256=HjHbDXbLePYxEbOhu6uMlZGV9t2dWqgtJ0WDZJuoAxo,1202
-zepben/evolve/model/cim/iec61968/metering/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61968/metering/metering.py,sha256=wrsQgx26Ymtdhrfq6J5bKfbJp109kHSTY1hXeDXkuNQ,11269
-zepben/evolve/model/cim/iec61968/operations/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61968/operations/operational_restriction.py,sha256=isJa0ErKPh1iMImENQszx7IRqY-c3hxpSVsadqXJaF0,3889
-zepben/evolve/model/cim/iec61970/__init__.py,sha256=inR0pmZOK5AyDMOklmVvjxq_n_Ds02JPepMeqzeKYIg,248
-zepben/evolve/model/cim/iec61970/base/__init__.py,sha256=6JjWDqh_D9RO5jS5MbNZvQQRYW0gpTKoflzqnTxOOys,249
-zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/auxiliary_equipment.py,sha256=U21TsoyYwPuQG3wY_DFKDEVwJSX8EmDc623kd7T44Kg,1475
-zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/current_transformer.py,sha256=6_jtr1DtTlZ_14rpatxKGIYtBN8jsIe64SbJToB_EVw,1489
-zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer.py,sha256=gDvx8Px6g7JiyS9SEEwyJNDnzg9JAJV3Fsf_6dD7CVk,1753
-zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer_kind.py,sha256=_VI90aG6daFJuAgxu904E-1-wwadLAtbZhHBALdvwNA,811
-zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/sensor.py,sha256=rda3rgD8-ZnVKNVNLQCnxPY4WY_c5dhh3Oa83BU-Ays,588
-zepben/evolve/model/cim/iec61970/base/core/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/core/base_voltage.py,sha256=PAd1pD8FKV300Nn9GQzpO0qJNgDn-2UQ-4HVu6E5HC4,556
-zepben/evolve/model/cim/iec61970/base/core/conducting_equipment.py,sha256=1dAANu5wQEc2k-j70VdfhGfEgE7zaXMDQP7NUGvmDW8,7135
-zepben/evolve/model/cim/iec61970/base/core/connectivity_node.py,sha256=TqyQ1rd1iReh833AUtF5m2W4IeHdq-94lGHYN1vJa0s,3645
-zepben/evolve/model/cim/iec61970/base/core/connectivity_node_container.py,sha256=PbDHlg-oH3t3kqiG536DFr4c4ZDmwzzxf29JHrgTTO8,592
-zepben/evolve/model/cim/iec61970/base/core/equipment.py,sha256=xE8hRqNyct4vqUY1EVZNirWhrt89q_PN5n-btfvZP_8,14195
-zepben/evolve/model/cim/iec61970/base/core/equipment_container.py,sha256=qHT4M_L8eKIx9OA-srqzxU3n1h1mTquCp6d3q_em8gE,15682
-zepben/evolve/model/cim/iec61970/base/core/identified_object.py,sha256=CIaP7hSo2hoSnw0nZOx_kgItRQmAD1n0NYFaw_Xv0zo,8261
-zepben/evolve/model/cim/iec61970/base/core/name.py,sha256=QoAXV0joIosdc-73GRaghN2tUsu0Q22OxGi9MMJsU1A,1095
-zepben/evolve/model/cim/iec61970/base/core/name_type.py,sha256=xiHeXiGGKGGV2f_K_f-zhmKWW1lK9cDWadFgiYomY5w,7475
-zepben/evolve/model/cim/iec61970/base/core/phase_code.py,sha256=nOiffWhNCHQslthzXiHpYyBPFPQgyue9vxT5VJzQDXU,7033
-zepben/evolve/model/cim/iec61970/base/core/power_system_resource.py,sha256=bq2-Nm3YhsCBLDtyeUfGOV0buVHfym794bmdQtFT6-M,1250
-zepben/evolve/model/cim/iec61970/base/core/regions.py,sha256=iEEVe8TwgtewqGarT3xvAlNaaPH7u0I-weEZ9OzctDE,6734
-zepben/evolve/model/cim/iec61970/base/core/substation.py,sha256=VwGe1YnGh1yuXfjr3ux_l92KT_90WYLKag87ZtgBAVQ,10120
-zepben/evolve/model/cim/iec61970/base/core/terminal.py,sha256=MDEeVIpc_3fHpg9UhIpiUSiDYVEctQj1yevrmSssbgM,6717
-zepben/evolve/model/cim/iec61970/base/diagramlayout/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_layout.py,sha256=X2zbmBu7lun58KBKujv0LUox2ILM-MPH5BPX6TNJgXE,10307
-zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_style.py,sha256=j15HRNo7RfcRJQHs4htMbbXHHgPmp2GIrVqvryzYxaA,748
-zepben/evolve/model/cim/iec61970/base/diagramlayout/orientation_kind.py,sha256=LZhGcDRBNb92L7mxDXjH6ME6Dae7eb89iacvDYS_PUk,1024
-zepben/evolve/model/cim/iec61970/base/domain/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/domain/unit_symbol.py,sha256=TbLTwx_V-g5qqLl12L_HZTixxFx-G25-m3H2PlckgPE,17065
-zepben/evolve/model/cim/iec61970/base/equivalents/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_branch.py,sha256=eBBvB-soQ8IPxN6LVCjd7xJhdvD80pTrOe6YpsCgRuI,5374
-zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_equipment.py,sha256=vYjUVM_4Xq1wkccsz9KXDhtC--8bt6khOPNLRbHrFHs,641
-zepben/evolve/model/cim/iec61970/base/meas/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/meas/control.py,sha256=3oWS6qEv8WcWgMxSvUTGbog0bfmGO3eZPyNCLJyX-S8,963
-zepben/evolve/model/cim/iec61970/base/meas/iopoint.py,sha256=vVMdwJ1m6Q-rZZY55aATIdX_qL6asooC_yIYXdD83EM,576
-zepben/evolve/model/cim/iec61970/base/meas/measurement.py,sha256=SPCZT5A3fkfRlkT_n56sV23-Q6c7rSDH4DNbyP5eQeI,4294
-zepben/evolve/model/cim/iec61970/base/meas/value.py,sha256=ke9FK72ma_jg-qbJdVqzpu7ZI0Eon4qHliEg93X8Cy4,1753
-zepben/evolve/model/cim/iec61970/base/protection/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61970/base/protection/current_relay.py,sha256=64KTDP4-uL7fCSDkNgT8ikVcj8CyOw5CBs0xT4fffmU,1465
-zepben/evolve/model/cim/iec61970/base/protection/protection_equipment.py,sha256=I0EIsgOeR5hY9CXYmepU_EUKmPyEzKvKkGoFx1g97jg,4777
-zepben/evolve/model/cim/iec61970/base/scada/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/scada/remote_control.py,sha256=7Wy8_OOvD7T2gcDbM5Z5gBtS0i4Yw-Rd88DfGUDGj9M,737
-zepben/evolve/model/cim/iec61970/base/scada/remote_point.py,sha256=bSiXF5IF7hYRxDYGlvpE3-W-3HONJEPAGeNFRIh6Wts,587
-zepben/evolve/model/cim/iec61970/base/scada/remote_source.py,sha256=6xh4ig08M4BlUJhTSiUcyPWT02BGlzz7b_8BLRp6Q7Y,734
-zepben/evolve/model/cim/iec61970/base/wires/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py,sha256=2oAkY1u3Cb3eQdTBwqWqE89n5qgbc7mSk7cceyDnm5E,2433
-zepben/evolve/model/cim/iec61970/base/wires/breaker.py,sha256=3yIPVniMxi_-gkuXr3sYGSA4Bw5FyNJzZlBXv_CbpL8,1385
-zepben/evolve/model/cim/iec61970/base/wires/connectors.py,sha256=-lkbHQZc11aoiODZa7ihG84N-OqhEqm3YdG_22_cT-I,1413
-zepben/evolve/model/cim/iec61970/base/wires/disconnector.py,sha256=JiLxyuyRwGFAPhkpomXgEdIVOdXo7Vawvbc8pSByOFg,672
-zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py,sha256=IYO4WNaE1FoRU4VNZYmw78VPhtPgwAyM6DZyQOTDcF0,1929
-zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py,sha256=h1M8WNmtkcsMLz4h7Woy6pocjks5wwYjICNwsHP1U8E,7483
-zepben/evolve/model/cim/iec61970/base/wires/energy_source.py,sha256=ENL2etPi37P8KJ_KEPOgz--DuXnlhIUxS8_NBAy7Iyw,6517
-zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py,sha256=kZx5ZX0i8KFVn63rNbOt4YrGWMIy-Ln0TzG3u3oCzus,1977
-zepben/evolve/model/cim/iec61970/base/wires/fuse.py,sha256=SZ_8BLbz4z5vvp4mnSwEbG_iTgfUEgX9sZY3TScATlo,595
-zepben/evolve/model/cim/iec61970/base/wires/jumper.py,sha256=PzxemGQ2YS4h2gnk3lr1qVn-MXCiGH3ZkjF-ytUXyoY,611
-zepben/evolve/model/cim/iec61970/base/wires/line.py,sha256=jEGsf6Uvz2F9FcX_JJnwUbAsl8lkBHXGTm8tZXB4U5E,492
-zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py,sha256=7lB4HR0YqckUkElrPCSOdMVbzp0a7DiIheqB2dnx68U,584
-zepben/evolve/model/cim/iec61970/base/wires/per_length.py,sha256=5DdKxuGutcv-Qwzi0vtw8BSolhWRqZiptUfy-pWmX3w,1904
-zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py,sha256=daImUAzTP3JsuWUPyv5rr_Pauk2tSkRildpxQovgNUs,884
-zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py,sha256=Mg99CD4rXPd2-pIfsMxj5o7ytvZ8lzHX01g20cEZj0c,24976
-zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py,sha256=FVEAaVUsRIMdBgQkVjQchQCyPFrO_ZV4jhljy352nF4,30217
-zepben/evolve/model/cim/iec61970/base/wires/protected_switch.py,sha256=akuR3ejptC1Ewc7NVIAOAbuU9E62DNxPxqoD9MG9cak,4386
-zepben/evolve/model/cim/iec61970/base/wires/recloser.py,sha256=qYsY9KpbSKpRO40ZSQ4B4kE9kpMP4iI0QSdI5O323gs,582
-zepben/evolve/model/cim/iec61970/base/wires/regulating_control.py,sha256=TwwHANHxNycEWkdmwf_r3issofM1Zz0djx2PRpoVeR4,8103
-zepben/evolve/model/cim/iec61970/base/wires/regulating_control_mode_kind.py,sha256=Yund5-IR2AxFVMWaQQCcpi1wnRSmvYijxvcH4yuvjZo,1168
-zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py,sha256=RC7AaxpyXG-oC2UuDuV52fOYiS4jOMB9prus59SOwCM,3658
-zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py,sha256=DK7csdS9Zqoc7xwsnr7Y-L8x1MRwcKMUiA9RzjYXfQM,2944
-zepben/evolve/model/cim/iec61970/base/wires/switch.py,sha256=GFCj6SgwiVSQ8xmdvKOhOGVPOManIgPHOamKBg3sIIU,4955
-zepben/evolve/model/cim/iec61970/base/wires/tap_changer_control.py,sha256=7rtiIWsb2FvcJ6v5mvY71UtHhXz4jMsocLI0eDEh9No,2112
-zepben/evolve/model/cim/iec61970/base/wires/transformer_cooling_type.py,sha256=zDrrLjx98YSykAehBMpw1x6dtM5jxIdjSSdeq-3h-Uk,1045
-zepben/evolve/model/cim/iec61970/base/wires/transformer_star_impedance.py,sha256=4pOjc9GmfcmcZ21LMF1RjV3jwMdly9DTb9SXtEEefIk,2219
-zepben/evolve/model/cim/iec61970/base/wires/vector_group.py,sha256=_6tDBE3Fp87UYCQKMF_X2h2CtCVl_vamXXCYWJ81UYk,1544
-zepben/evolve/model/cim/iec61970/base/wires/winding_connection.py,sha256=eUsiC-GMoLvIQPeiiEWut-_qHhHtmm9OqiSJnxx4H2E,786
-zepben/evolve/model/cim/iec61970/base/wires/generation/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/wires/generation/production/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/base/wires/generation/production/battery_state_kind.py,sha256=9DJKA7ABux_KImljTzxMFt80MJ7e0qkpuEwkFsJ-lFQ,809
-zepben/evolve/model/cim/iec61970/base/wires/generation/production/power_electronics_unit.py,sha256=VvJB1Dz1JqEORn691YgBY8QroRWWg6hgdMXjZOhdvHI,2215
-zepben/evolve/model/cim/iec61970/infiec61970/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61970/infiec61970/feeder/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/model/cim/iec61970/infiec61970/feeder/circuit.py,sha256=a0WB71pItWhWOakOngSTkq8_1_y5N7FpgxjmbAFAup4,5385
-zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py,sha256=99Vksg_o_V9VA-4NyY6JxpTwx46FbChIRwJKsHNVhvs,7542
-zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py,sha256=tDeZ6PzXGnnEQ5XeztS2z6adTfEkvE_9eEFiLPHJQDc,7636
-zepben/evolve/model/cim/iec61970/infiec61970/protection/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61970/infiec61970/protection/power_direction_kind.py,sha256=lQE7HZZkVQUUwAxD8Ygf-pS8areu199k1J7WTPT-y2A,746
-zepben/evolve/model/cim/iec61970/infiec61970/protection/protection_kind.py,sha256=eQEYyQrzT6z-lSmz4vjN_rQy_4Ao7u_da6S-IuCKkYA,768
-zepben/evolve/model/cim/iec61970/infiec61970/wires/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/ev_charging_unit.py,sha256=B4lAk5twTWVIxb4cjvVsqv0Uj_w59fbfVKXadWO4gB0,426
-zepben/evolve/services/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/common/__init__.py,sha256=WlmZaQ2cAGyEzSLdecEoC1xw5gcfl1DqRA48qVhMAQg,960
-zepben/evolve/services/common/base_service.py,sha256=hNHGm0x--ljVaad6bZstvM3PvSJYYV5tkwQqMf5vhOA,18023
-zepben/evolve/services/common/base_service_comparator.py,sha256=bJUubL-pqOnvywtVzCkmMbYF7nFiVrPtQCrsWSqfqto,16620
-zepben/evolve/services/common/difference.py,sha256=GWVzdr5-emaMkaMW8APCnkZ-SAXFYpM9bTx0SFlqgeU,1189
-zepben/evolve/services/common/reference_resolvers.py,sha256=AiRSe09P4I_Uy0tB1Vy8IOOheF9SXWT36G6ywbzdRHI,22895
-zepben/evolve/services/common/resolver.py,sha256=R2EeZAJ6bUNBLAtKDKLwq9raUYcTeb4YxCvsAAcUbC8,20762
-zepben/evolve/services/common/meta/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/services/common/meta/data_source.py,sha256=9v-6XV-bWmdbjwO95SWAwQR6HW5E9vyzCI4eYJpfJA8,461
-zepben/evolve/services/common/meta/metadata_collection.py,sha256=58Rs3oEcwfHaxtkGLEa2Bce048eeWZ5nf_Ry0MvO4gI,804
-zepben/evolve/services/common/meta/metadata_translations.py,sha256=ZDn6FvpnksHzjPGJsFcHOQvZq96RJFNs1x5qlxluQTw,1481
-zepben/evolve/services/common/meta/service_info.py,sha256=ukgCJ3Rit1jWl-V9GjIXNRp4yb4gvNRNfN2ZBZcbE4o,601
-zepben/evolve/services/common/translator/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/common/translator/base_cim2proto.py,sha256=4qPwsDavirJwhYjnX937Z2NJroJU9eUcfIJpDPYsJLg,3420
-zepben/evolve/services/common/translator/base_proto2cim.py,sha256=gOtzwQOWwf3bkX35wrgBTRKVNArmBEmSAMd-l3V1XzU,3938
-zepben/evolve/services/common/translator/service_differences.py,sha256=7N9j4axwN7-LT8jaOP8o4k-Hy016LjaUUcud4dNQeAI,2924
-zepben/evolve/services/common/translator/util.py,sha256=N9K87gbvNfgn4FEeq617zCcLxRT1dsJ4RfeFoWi2s0Q,2410
-zepben/evolve/services/customer/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/customer/customer_service_comparator.py,sha256=CfN3RRFexlKvXHCe1s_GWzGmM_NOhgyVGRFvRHQjs7o,1922
-zepben/evolve/services/customer/customers.py,sha256=4R-S02Zbg93KhK32aY_5fbRWaLoktcYUl3OXJvaOCHA,467
-zepben/evolve/services/customer/translator/__init__.py,sha256=cVIIxKXN0vBY2IQHlH4ljAjSHdbtDrF0amDdsF4cpek,1044
-zepben/evolve/services/customer/translator/customer_cim2proto.py,sha256=G8g0m8Ynn7CJCOV1M88dOQx45Z_ES32sXi5YnbQECZs,2760
-zepben/evolve/services/customer/translator/customer_proto2cim.py,sha256=ODXzCwdZTm_bx9TgmFoI0hFOyPx6zOqJe9M1_I0Nw1k,3379
-zepben/evolve/services/diagram/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/diagram/diagram_service_comparator.py,sha256=Ho74EQyHVd_ZYIiLxkn5mR64RQtkcfPSCnNYr-Lfhpg,1486
-zepben/evolve/services/diagram/diagrams.py,sha256=2f14D-D2kSaBqjbDD_y3bAWp-1lPZ6UIT6s71X2jaQc,4598
-zepben/evolve/services/diagram/translator/__init__.py,sha256=ToEJ9-lp2oHPrP5Ne_AGqKT472cWdV5gh9FC5o6v6Ss,508
-zepben/evolve/services/diagram/translator/diagram_cim2proto.py,sha256=_Kx89U0nSJlW4ZoLlmMMLde_ExZdaWoqp2u3B5Sz4BU,2237
-zepben/evolve/services/diagram/translator/diagram_proto2cim.py,sha256=IUlj2dBkW9LTzY5tU3f1-n59sfmiY8LD0T335BsldfM,2463
-zepben/evolve/services/measurement/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/measurement/measurements.py,sha256=5-YwnbX9UsTGjcfMXjST-syidHuxCsjDa1WfvJsvVs4,1207
-zepben/evolve/services/measurement/translator/__init__.py,sha256=05AusxZLt6CzJ8GKIjCMhiRcEac6Yb3erG4IMSX2YH4,261
-zepben/evolve/services/measurement/translator/measurement_cim2proto.py,sha256=8phEh8aND0W5QgFUt4peWEjB5DmnutrnI7gldav8Kck,1832
-zepben/evolve/services/measurement/translator/measurement_proto2cim.py,sha256=32fUcSJwtyNkf4e_T0cWN0d-gNDppEWgySS4MPrLisY,1951
-zepben/evolve/services/network/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/network/network_extensions.py,sha256=AlEHyEnQB4B8CWdcsxexnsqRycyvRqrCMXGVf73KzyY,6279
-zepben/evolve/services/network/network_service.py,sha256=VxvRkxBbl8MSsSAOlzg0rfUZGfVZ398Lt4bOIx_zr_k,10634
-zepben/evolve/services/network/network_service_comparator.py,sha256=5CxmCjJoUIOjASVoVm2FnSaVAlqbYLJb51nFHZBdklA,42979
-zepben/evolve/services/network/tracing/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/network/tracing/find.py,sha256=buCTiSsxHMTivolhYjeRsmoZyw0Pq1oFOsp0fbcB9qc,3654
-zepben/evolve/services/network/tracing/find_swer_equipment.py,sha256=wbCNP50MaM08JTZhvZbJ1Rs9mSlIG1BI4zETv2H0OYg,5623
-zepben/evolve/services/network/tracing/tracing.py,sha256=HScmuBg5t4KwB0-d_m7xaXGWLjbTbmjUbBaCOW59vcw,16173
-zepben/evolve/services/network/tracing/util.py,sha256=Axed0aycUQhBxGXSYQTjvUlRM3gr-qnJdxye_Z2YUFA,3395
-zepben/evolve/services/network/tracing/connectivity/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step.py,sha256=yMWtVqUP3yIdnxPmt-eVx3EHT85_egauj4FiAIc2-9o,775
-zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step_tracker.py,sha256=RfRTihPCagiUEghubSv7jBzA5AvIFowr9JcTM9O-q6I,2394
-zepben/evolve/services/network/tracing/connectivity/connected_equipment_trace.py,sha256=IcCqoOPjxKXAdTdl1F7KW5yVd6UyTYHujbnwrVbJMDg,8474
-zepben/evolve/services/network/tracing/connectivity/connected_equipment_traversal.py,sha256=ggKagltzUbu6AMkBE-2ARg1sFm8gKIdCE6B3Ci8tCRk,1162
-zepben/evolve/services/network/tracing/connectivity/connectivity_result.py,sha256=aqxTBi483T5xD97fAISZClMFcnBX80kVmIduw0K5Uq0,4223
-zepben/evolve/services/network/tracing/connectivity/connectivity_trace.py,sha256=BoP86cRvdUXv3xDy_ufelikRyJIjzYBi7t-JS6IepaI,2671
-zepben/evolve/services/network/tracing/connectivity/connectivity_tracker.py,sha256=CbiDdd4jBmYgtU3mvBuG-DjMvMrLvcsAJ_mHNhvPBaA,1212
-zepben/evolve/services/network/tracing/connectivity/limited_connected_equipment_trace.py,sha256=rqWU0HoHbM4zPMxrRw7TRf2tR8WOCO5x4YDygJtWtrs,5162
-zepben/evolve/services/network/tracing/connectivity/phase_paths.py,sha256=GngjXnlRNkljIje9wKBwqt3Vn5efEB7ejdb4SOHddhY,3872
-zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_connected.py,sha256=IIazFKdxs7QjAQpsgbAbgL5XW2VRHogdZyT6hTAQ76E,9998
-zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_internal.py,sha256=VnbbKmypW5fK5qOEziONqhkCA5xu5_J7L84Jy1u51K4,2862
-zepben/evolve/services/network/tracing/connectivity/transformer_phase_paths.py,sha256=xAR-NQ-ksQ2860FCnvjuCFmz4_pT1nTPqOfYjZSOGpw,11472
-zepben/evolve/services/network/tracing/connectivity/xy_candidate_phase_paths.py,sha256=-D50G-a5ZIKA1HFue8JKk1b9CSJXju0eDeehZX5V-bI,10412
-zepben/evolve/services/network/tracing/connectivity/xy_phase_step.py,sha256=3QpxfAS6TJZYuu8IHqicBG6yrCaAGoqkDtlGctC-dts,583
-zepben/evolve/services/network/tracing/feeder/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py,sha256=ZzHgBFXidvf2g82UgNisJKS03P6tRFKC5MLS_f0QBiA,5997
-zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py,sha256=4cjE12QB86ZL5YxLQR9mfgcGyZJAcmDoR_dn3D9DqnM,6053
-zepben/evolve/services/network/tracing/feeder/associated_terminal_trace.py,sha256=UtOjhwv9mzIyVO0hRBpDa8R86qGxjgC8mHb-i7PqZc0,3246
-zepben/evolve/services/network/tracing/feeder/associated_terminal_tracker.py,sha256=f4pUFckQ34SlPbHd4sr3UkSIWRKxBEvgylWsA1R9R90,1477
-zepben/evolve/services/network/tracing/feeder/direction_status.py,sha256=fMBCsWE5yC32iRNLrVi5QZz0r4vV2pSdbqw1U0kScDg,3990
-zepben/evolve/services/network/tracing/feeder/feeder_direction.py,sha256=JBvc4bpC810SPfacaKPK8x-DDOyKdTddrBqm0sidbcc,2546
-zepben/evolve/services/network/tracing/feeder/remove_direction.py,sha256=nt7kaNSyEjbGuthSFTQfMDh1T6zG1zscfvLwcNKCKsI,7410
-zepben/evolve/services/network/tracing/feeder/set_direction.py,sha256=eHkt8WtSO7ABcSgJJAv8ObqtqM-wl3QmH8opfUrHZrM,6757
-zepben/evolve/services/network/tracing/phases/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/network/tracing/phases/phase_inferrer.py,sha256=UXrJMUglpUrEmGJhqBQwxsTSlB8qbqLm0ga0Horn3vI,10311
-zepben/evolve/services/network/tracing/phases/phase_status.py,sha256=pNCrygFtnhbl0XqcNhdas_hecCSPVNE1T23xXeUeT20,3428
-zepben/evolve/services/network/tracing/phases/phase_step.py,sha256=1Yjmg2KQM9jJh0XuQ7GHMJ7u_tiZcgw_pLl_PuKrMsY,2628
-zepben/evolve/services/network/tracing/phases/phase_step_tracker.py,sha256=tV9y1mbKogKiTcehvJiCcShNXtbhtSH9rippP5JUix0,2014
-zepben/evolve/services/network/tracing/phases/phase_trace.py,sha256=Vq5U2NdzA5uxZksurFT2zgiASzFzXjeHN4favx2gTy4,6251
-zepben/evolve/services/network/tracing/phases/remove_phases.py,sha256=SCxHT4_zROc-pVr-lTdQbTyJZFafCKY_4N0bEEI9j6A,5510
-zepben/evolve/services/network/tracing/phases/set_phases.py,sha256=2N5CVbeTmGisXeeFjpzIDz6CzHptO2AhL78XYpUQ2Uc,12798
-zepben/evolve/services/network/tracing/traversals/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/services/network/tracing/traversals/basic_tracker.py,sha256=vP1A-QlnxtUTMPDfIw6c8K9g2cdedvlhIFM5ioIGKU4,1642
-zepben/evolve/services/network/tracing/traversals/basic_traversal.py,sha256=o7dxTDGibqDW6AndLf2q9Ejpjhf5k1I5aSwQycze0gA,2944
-zepben/evolve/services/network/tracing/traversals/branch_recursive_tracing.py,sha256=eGTQoycIs5FzVpvyOue88nVq-_JN2jaGYEMqcY88-ls,6585
-zepben/evolve/services/network/tracing/traversals/queue.py,sha256=uQQdGl7_ILnHPlmVmG8so3JmGZsbvYcSZvzeWQiRLBo,5164
-zepben/evolve/services/network/tracing/traversals/tracker.py,sha256=whRdkMJ5XzZjJvRmibvqIDAWlGBoGQlC4xCh-E6qV9o,1775
-zepben/evolve/services/network/tracing/traversals/traversal.py,sha256=F93xr3SiwemUyTCnNadzcxHZ0MWHeS8ZRv8eOsfJyG4,8650
-zepben/evolve/services/network/tracing/tree/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/services/network/tracing/tree/downstream_tree.py,sha256=MoTGhKWGlnG2gxB6PPt6x6z4YeqEosp2MwMG4ZKfGGo,4454
-zepben/evolve/services/network/tracing/tree/tree_node.py,sha256=Ygi78mb0TZ4BkcSccFjl7t2_ZXyIDVz-7zdIm0HIIso,1780
-zepben/evolve/services/network/tracing/tree/tree_node_tracker.py,sha256=7CzIf4-4uCOSwciJ4xix_q373ZrNmlghls7yKssOZgU,1167
-zepben/evolve/services/network/translator/__init__.py,sha256=FP0qNFsI71TPzTlwMCCxrq_QK7fzO_UMOkkzMrJSOTw,22426
-zepben/evolve/services/network/translator/network_cim2proto.py,sha256=-TMyTiSHLXsRZSbgus2cji4crZ-6RSZJF2azFSFbdDA,65188
-zepben/evolve/services/network/translator/network_proto2cim.py,sha256=rXwQMBIbLdNA73qk8pyoOqmFNnEeh-Om20DArbUvhm8,78124
-zepben/evolve/streaming/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/streaming/exceptions.py,sha256=c9zR-HP1_uP4ehuPmRFX6Ld2C4IV1zMwDIlViisy0TM,427
-zepben/evolve/streaming/get/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/streaming/get/consumer.py,sha256=OyEJ9O17O55MCfsZXuygBrXoNKj3GnC-jENHgacY3eA,9348
-zepben/evolve/streaming/get/customer_consumer.py,sha256=uj0Zh7CfP5yH4UPcK7xqHo1uu2KXonGnXe-ObUWyBy8,5425
-zepben/evolve/streaming/get/diagram_consumer.py,sha256=AxzjUrlvurX3dXVWYiAhD_MsTdTf02XgHdTRZJKFGqA,5032
-zepben/evolve/streaming/get/network_consumer.py,sha256=v021aIaVkxCdGLhdOh59UjtDwZoYy7EvAgmT2B1wsC8,38079
-zepben/evolve/streaming/get/hierarchy/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/streaming/get/hierarchy/data.py,sha256=5q-JbObon_H3YLjT0fLQFAt7muOu1fhc-Q6SRy3FQMU,1047
-zepben/evolve/streaming/grpc/__init__.py,sha256=Ld3jvZ9kl6d5PXde5Yo88E7t1wEpClvkJm3VFa3DPSM,246
-zepben/evolve/streaming/grpc/auth_token_plugin.py,sha256=Reuyv3RmaK9CY8Ph_xCsZ9hsbJ0zykt8agPTb3sr-Ro,801
-zepben/evolve/streaming/grpc/connect.py,sha256=dqcKz85VKzk8hLg65YROIB0qaXu0f9ncaopvrGNs5OA,9451
-zepben/evolve/streaming/grpc/grpc.py,sha256=Xf8x1PaDMbJMVLiYiTK2ilsd_PQJFzXwhrYSEtZuO04,4020
-zepben/evolve/streaming/grpc/grpc_channel_builder.py,sha256=6Rr15jw1rbVX9afqX2fbx2NwXiGQ5skvv9S4UdViKTI,7664
-zepben/evolve/testing/__init__.py,sha256=4_VsSq4lh7u0jpJS8U9AECShaepOAFHC1RmELVT1RtI,245
-zepben/evolve/testing/test_network_builder.py,sha256=Grme1QRDLTQBC7kjvcTZcqOOEjTdcgUeZiaExznnxxw,28552
-zepben/evolve/testing/test_traversal.py,sha256=l3sp8jVT_Oq9T10A7k-uhrpfBW50toN7yCgphkVJWZ4,3238
-zepben.evolve-0.38.0b7.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
-zepben.evolve-0.38.0b7.dist-info/METADATA,sha256=NkiX_wTKZfaLvc-x9IKR0-dHBenMfh87PNexSUccioA,2299
-zepben.evolve-0.38.0b7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-zepben.evolve-0.38.0b7.dist-info/top_level.txt,sha256=eVLDJiO6FGjL_Z7KdmFE-R8uf1Q07aaVLGe9Ee4kmBw,7
-zepben.evolve-0.38.0b7.dist-info/RECORD,,
+zepben/evolve/__init__.py,sha256=21x6AXvMC-XgwkFr-tq9Sq0jfzxKvrKUPhvgVVS6t0g,19853
+zepben/evolve/exceptions.py,sha256=3s7x4COYYOAcua3gFwWDq3-MYZv9uiT4b_RIKWakOv8,1387
+zepben/evolve/types.py,sha256=rqsPeqtXqqdiieCDP6vUjiu9qjh3hiXDe747DYKNuGY,1132
+zepben/evolve/util.py,sha256=JMaw66rE5EswnBTizpaJ2QOQixN12VhOvUyVzsjtbhU,4576
+zepben/evolve/database/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/database_reader.py,sha256=_AcuP_fz5d2jB-zvix45Bo6bslSY18a7LOHAXv1uVgA,7148
+zepben/evolve/database/sqlite/database_writer.py,sha256=40YDXGwKVWGHnzEg15vmderfz9X5hQGU6fncLNE88dc,6108
+zepben/evolve/database/sqlite/readers/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/readers/base_cim_reader.py,sha256=soV4XGreYoc8jejfO60eVk4TSnGfVhh6-OyganuYPng,5275
+zepben/evolve/database/sqlite/readers/base_service_reader.py,sha256=VUcfl8_Zb-iOFIc1MPSsFRJfPULFF8NgrmUbgIQ63cg,2991
+zepben/evolve/database/sqlite/readers/customer_cim_reader.py,sha256=C5uIy67HsItBxHmoA5-ZIrM4aJeJ9qzu1KY-2hTJW3Y,4510
+zepben/evolve/database/sqlite/readers/customer_service_reader.py,sha256=0la9LA89LiOny4elkbxYJup81mvptwLSZPojgOhY0Qw,1761
+zepben/evolve/database/sqlite/readers/diagram_cim_reader.py,sha256=vlo3ejS8nuQD3BEQTLsArQIplX5rkhgKxPzl1ipLKlc,3245
+zepben/evolve/database/sqlite/readers/diagram_service_reader.py,sha256=2N9tm31Hm4Q5-dKRatl-Vxui5PWYGMQdlHYmwgTNmwY,1041
+zepben/evolve/database/sqlite/readers/metadata_collection_reader.py,sha256=-5mu1huTQn_CERS56bevBH65vXTc3PFYHylCzLogeis,733
+zepben/evolve/database/sqlite/readers/metadata_entry_reader.py,sha256=5pJ8Yb-lywnbzI8NmCMYOijhZBRXEjBzurfLCIDLUeg,1088
+zepben/evolve/database/sqlite/readers/network_cim_reader.py,sha256=fEufg6F_imTf7hGya3cFBoVcu4ut-mOLFnc0tBHdwNg,88904
+zepben/evolve/database/sqlite/readers/network_service_reader.py,sha256=2wUXc_-_Y8BVU38ODMjSko2PSRLESdyx4EHzbMzH8wI,14696
+zepben/evolve/database/sqlite/readers/result_set.py,sha256=2-_4rc6CFFUI-AFohxpLEmbn3KxuqKRbZFtV4yMokEc,6872
+zepben/evolve/database/sqlite/tables/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/tables/column.py,sha256=22g4N_afso2OApwRXRZAz3JKAnEOQZQBDqjYXik2lvg,1009
+zepben/evolve/database/sqlite/tables/database_tables.py,sha256=-NAIONVdrd2JU5tG489vXJs9puPJD5rZsZ49AZMo3Zo,13135
+zepben/evolve/database/sqlite/tables/exceptions.py,sha256=HvKVYdpfqiKhx4AWH0fjD9vk-Kg39gPVde_CuqnN8K8,403
+zepben/evolve/database/sqlite/tables/metadata_tables.py,sha256=T43BvHhavUnpk18ubGDEJamSXcA1zt2C9MlILguj6wQ,1164
+zepben/evolve/database/sqlite/tables/sqlite_table.py,sha256=2_AhMZhkKzQWWakFuEjVDVGVD_xRrV8FmG1nXC2D7Ks,5820
+zepben/evolve/database/sqlite/tables/associations/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/tables/associations/assetorganisationroles_association_tables.py,sha256=UOrvdXbAmkyoYDqNc6f87blnI-9FfNSsimS-Zc7P7WM,1484
+zepben/evolve/database/sqlite/tables/associations/circuit_association_tables.py,sha256=gYQkQf7i2dEqT4v1-4rgb3fRS49LZ9hz4GRh6jHBfPg,2295
+zepben/evolve/database/sqlite/tables/associations/customeragreements_association_tables.py,sha256=EyY7DtIou1ciWD1HLl5pPpBPDaiTunlYCtpKNEeJXWs,1561
+zepben/evolve/database/sqlite/tables/associations/equipment_association_tables.py,sha256=Ao0oZDJv3RJDESrcVW8yc1upR96N4kCELFYRPKfBJrs,3547
+zepben/evolve/database/sqlite/tables/associations/loop_association_tables.py,sha256=I5VNDmyEKxMxRDNkEwsV03fO9TK19l73oDs2H7DPnGo,1696
+zepben/evolve/database/sqlite/tables/associations/pricingstructure_association_tables.py,sha256=KMvUABDBjRDd91u5lROBpqOxoQzeaUQJK0wB_Vo8AWw,1435
+zepben/evolve/database/sqlite/tables/associations/protection_relay_functions_protected_switches.py,sha256=K1v9Qs7Xoe3VtU1zBrq_gLL831AYykIvSj39Zq8Pi7M,1628
+zepben/evolve/database/sqlite/tables/associations/protection_relay_functions_sensors.py,sha256=OT98JB7PWX8CekNn96kqYddrq6h6PrBrqB5Ar94q_jQ,1426
+zepben/evolve/database/sqlite/tables/associations/protection_relay_schemes_protection_relay_functions.py,sha256=wmuZyVm1MqjbPiqu49V0hXR__iH-c42szWZLMqfEGcg,1602
+zepben/evolve/database/sqlite/tables/associations/usagepoints_association_tables.py,sha256=bwhpMpI8hL_ImtrDBNkU6dodP3sb3zhKwFZsCq64p-A,1409
+zepben/evolve/database/sqlite/tables/iec61968/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/tables/iec61968/asset_tables.py,sha256=y5fdkbo_avUlRg4YxgF5Y-ZDZqnJyMtXlfgPX1-QRUE,2240
+zepben/evolve/database/sqlite/tables/iec61968/assetinfo_tables.py,sha256=lvM_qWRWx5leggNkyPN9K2qGTvcsJbiBu8R1-01dS6o,9391
+zepben/evolve/database/sqlite/tables/iec61968/common_tables.py,sha256=P6VlIIGD4s0Dt8E9lbVGaunmtDZMpjYTpRvz0zbNhMM,5681
+zepben/evolve/database/sqlite/tables/iec61968/customer_tables.py,sha256=mDhGZ99HrTyPWeX4W72NT0mVriWVS_nBWCbnzvo2Sh4,1705
+zepben/evolve/database/sqlite/tables/iec61968/metering_tables.py,sha256=ZsU7OFUwX-34gqHO7f7d0hpgVVySeV6o9HIOBxNtRJo,1912
+zepben/evolve/database/sqlite/tables/iec61968/operations_tables.py,sha256=TJ_2k2P3efYFgbi9gS5beMK_hfb2mzgc6VbqWtnKiXg,494
+zepben/evolve/database/sqlite/tables/iec61968/infiec61968/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/database/sqlite/tables/iec61968/infiec61968/infassetinfo_tables.py,sha256=4HXpIfgDW_F5XUEysDEPY2j817TyKQC2o5-uPU51I0w,5311
+zepben/evolve/database/sqlite/tables/iec61970/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/tables/iec61970/base/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/tables/iec61970/base/auxiliaryequipment_tables.py,sha256=LzSjDnyY4Osksrmrb6tX3WruG8dMfFrlEMVr2DS7P00,1995
+zepben/evolve/database/sqlite/tables/iec61970/base/core_tables.py,sha256=cPNu67oZJx_AxerHFYgYBWQGKRUwJ9WL5BIdXavx2Qg,8442
+zepben/evolve/database/sqlite/tables/iec61970/base/diagramlayout_tables.py,sha256=5yczJ_Z4CCMzU_kmzwlwaiBnUACMvZI-kIrOTGR0iJ4,3113
+zepben/evolve/database/sqlite/tables/iec61970/base/equivalent_tables.py,sha256=e7R9OWUi8xPt-uTpVrfArZf81BEdFJmSYhofGtc74Tg,2454
+zepben/evolve/database/sqlite/tables/iec61970/base/meas_tables.py,sha256=8Vmthd_JugyE54pMxwiHY46t-F1NGaBNP4RcK-zjScc,2581
+zepben/evolve/database/sqlite/tables/iec61970/base/protection_tables.py,sha256=NjIW8nDqzZvwg8-3q8dpwkmcKckbhfGuMxRURTBPH-s,7143
+zepben/evolve/database/sqlite/tables/iec61970/base/scada_tables.py,sha256=g-HCpWml8cOwm2p5_gK6ZONDffrstvbgdqxFNG-a_nk,1205
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/conductor_tables.py,sha256=6pjPoVoGTAGANQjJ1MDmgqEmnRRW1fjpvEEMgNf41os,1226
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/connector_tables.py,sha256=GMvTXbseRAHDumOiBkl67mRtmn3dcu_fx6f0Y1s5N0Y,710
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/container_tables.py,sha256=X0oQMRu9F89fw5LEuFTaqUUDIcOFxLy3vWnOCXgVEwY,458
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/energyconnection_tables.py,sha256=aId6l8kI1AEGTGyTxQsDP1Q70aA4BEl9u-G5rZ70CTo,17861
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/perlength_tables.py,sha256=OBguQWPQQvD2DJbAFmzUEFmGAi9110OPoehIFi2E13s,1845
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/switch_tables.py,sha256=KSFszJVK0fIGia1NkkNYOLnqTZbr-oakGj6MMnCAowI,2775
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/transformer_tables.py,sha256=yra8w5MI-5xsPpCHb0qWHmyr-DOyg1dUo3p0qWpUU1A,8640
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/tables/iec61970/base/wires/generation/production_tables.py,sha256=n6Qlhcqy_zzZgwOsSzb1_W_nICqfWb483tN6es1bIKg,2114
+zepben/evolve/database/sqlite/tables/iec61970/infiec61970/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/tables/iec61970/infiec61970/feeder_tables.py,sha256=e5r62WYlcTpX2PeD1lx3AYKgghquoV9cqrCUzslRhHY,1515
+zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/database/sqlite/tables/iec61970/infiec61970/wires/generation/production_tables.py,sha256=UEHTNf8SRbgXhrajrq39lllamtFlSX9cdEEYiredG58,454
+zepben/evolve/database/sqlite/writers/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/database/sqlite/writers/base_cim_writer.py,sha256=RpgzOJWu43yYM6q4du1Phzzq339F6zUz4mPk8geEx84,5263
+zepben/evolve/database/sqlite/writers/base_service_writer.py,sha256=dRW_yBye19XRtuirRn93hukpfKBjHZNTgXpGohOu0oU,2995
+zepben/evolve/database/sqlite/writers/customer_cim_writer.py,sha256=pm04hfodTkNHoLiHsZqc1zzgju2rJDbD1gYtEA12dBE,4752
+zepben/evolve/database/sqlite/writers/customer_service_writer.py,sha256=9WAnEO9QbRRIWecBypbGMkJLZvNZ3ZIP4_-rI6-yc1M,1393
+zepben/evolve/database/sqlite/writers/diagram_cim_writer.py,sha256=6NykBSso0_QCrpYGeynJv9YK5_udRvOoPRT0OXcbBrQ,2657
+zepben/evolve/database/sqlite/writers/diagram_service_writer.py,sha256=Aup_1FxFQY_pPeF_fN8KfaPs8J9kQeDRHFEQQ2xS8GI,1004
+zepben/evolve/database/sqlite/writers/metadata_collection_writer.py,sha256=MAwkMatj21_RBZyTMpuY6ExN3AMb1nu6Xk9_atferEs,904
+zepben/evolve/database/sqlite/writers/metadata_entry_writer.py,sha256=d4rvmWQ80l_PnR4Q_5JqOjIAxYh5hPV8B1V_3fmvwYs,1257
+zepben/evolve/database/sqlite/writers/network_cim_writer.py,sha256=_T_vY3v8QM7Q9NXt_XaCgOBsbKqfEVDDJtm0sbwLxdY,86260
+zepben/evolve/database/sqlite/writers/network_service_writer.py,sha256=h7B7qZxFfnjHCdRG3dBARDTsFVcPwGm1gV0Ec2CYBog,9809
+zepben/evolve/database/sqlite/writers/utils.py,sha256=vZ4E7TxwhtUgdNL93U5W_7OI8nIXIkGsPNxUw-Y1iv4,1430
+zepben/evolve/examples/__init__.py,sha256=UjPn12pl5OywCml3MIcU6AaHG2GFzyUhYVIrj82tkBw,302
+zepben/evolve/examples/simple_test_network.py,sha256=FGo5LRxdZTSbD4VQCjuN2pzxm6SiqMXt7gP3kyIflRE,5062
+zepben/evolve/model/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/phases.py,sha256=KhUonIpBmcv20ntT9ma0By8yZXeBDZ-LzlLbh-GIgZw,7357
+zepben/evolve/model/resistance_reactance.py,sha256=5ItKZzzIXpHgpsVoFZoweOooBE9cf8oQ1rEb80s_CoQ,1502
+zepben/evolve/model/busbranch/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/busbranch/bus_branch.py,sha256=Sn0cyKoj6ib96ERh_hcbLh0FfXSQNXblGMVKBknpV98,47076
+zepben/evolve/model/cim/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61968/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61968/assetinfo/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61968/assetinfo/no_load_test.py,sha256=gvPtoL_vaJjXtI_fr88wQ7cboCo08QNUdvMjYFoHaa8,1398
+zepben/evolve/model/cim/iec61968/assetinfo/open_circuit_test.py,sha256=jhbG7JPAvtt-_bCmwuUFwTVEO56qcc7MYMSsxhfRmWo,1445
+zepben/evolve/model/cim/iec61968/assetinfo/power_transformer_info.py,sha256=9PlP9uhn8mgzxwZtyQAjh__NfCwdnSSxzG03ZDF6_eU,4220
+zepben/evolve/model/cim/iec61968/assetinfo/short_circuit_test.py,sha256=sX_8pChU7HE3rKSyNd5SXg2QP28979hm-NqdoIlk9UY,1877
+zepben/evolve/model/cim/iec61968/assetinfo/shunt_compensator_info.py,sha256=w1Szr_bAPlPmx1S4Uy3uYPdxjg0H0yEr_6BzMgdoj7U,927
+zepben/evolve/model/cim/iec61968/assetinfo/switch_info.py,sha256=tBPKU65f28jeRaUxhTkTFQ9Aw5D7qwrmBwF8Tm-4ISI,550
+zepben/evolve/model/cim/iec61968/assetinfo/transformer_end_info.py,sha256=Hqvs0I0Uw9VDYRnGvcdp1DLvGEd6y3jStBPZi1Cuc3g,5904
+zepben/evolve/model/cim/iec61968/assetinfo/transformer_tank_info.py,sha256=VaaSCFdZP4h_FlU-9wFSEkJQkCGAr6AOrwKMo0FRhhY,4395
+zepben/evolve/model/cim/iec61968/assetinfo/transformer_test.py,sha256=qBnuwCL_gLrB4PxFZiqzF6Fl_qqeLgxEC_7qABRE8NM,860
+zepben/evolve/model/cim/iec61968/assetinfo/wire_info.py,sha256=0PHsj93sgs0cFlH6Nk4XeuvNCOHGkfRgM2rHGoaF3bw,1287
+zepben/evolve/model/cim/iec61968/assetinfo/wire_material_kind.py,sha256=Zy6_R0mVwAMEpncHG3OQLkIO6IjX4O0Xo56LQc89_gM,1015
+zepben/evolve/model/cim/iec61968/assets/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61968/assets/asset.py,sha256=uoKbK9A63g_6sZV_QCRffgC6ptOxn6zqxrrJbzmpvIE,4019
+zepben/evolve/model/cim/iec61968/assets/asset_info.py,sha256=gf27UduwVDpQ0jmGeEy_Ic5_tGU3TgSKma_N1AWmqwk,845
+zepben/evolve/model/cim/iec61968/assets/asset_organisation_role.py,sha256=LA2GYqw8G84eD7sj7uQaAU0Eih-nO7JBwkLoe5E5dbo,588
+zepben/evolve/model/cim/iec61968/assets/pole.py,sha256=I_4WAzuRCP7_0NEB2MRdroQsHrwz3teF3t3ATbYdIHw,3009
+zepben/evolve/model/cim/iec61968/assets/streetlight.py,sha256=TMxj76KDNy1gYsHQwllY44tG_o-FlIbCwowTPwFyu50,1157
+zepben/evolve/model/cim/iec61968/assets/structure.py,sha256=qupG-grPU_jeJfxdjBiub1Fzg41NxfgcnH9_FYIpeBM,635
+zepben/evolve/model/cim/iec61968/common/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61968/common/document.py,sha256=YEEQoTMFi-3WUoymOHhXbTLZ7-xQbbKpjhApeZ6J2qg,1570
+zepben/evolve/model/cim/iec61968/common/location.py,sha256=dsAogrJt495ftAUfetiOs37bPBQCzlp5SvzC_WH13zs,7841
+zepben/evolve/model/cim/iec61968/common/organisation.py,sha256=jBWBcfDIv8fNKYsV0oPHFF6ZB1YLkVLim7FcJTA4p68,531
+zepben/evolve/model/cim/iec61968/common/organisation_role.py,sha256=o1cKer0fJQfQ4LCHIw5OIH2oDfI3OHBm_6cl_Jldks4,838
+zepben/evolve/model/cim/iec61968/customers/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61968/customers/customer.py,sha256=QEpXBTheNN3xOBpkR5NEXYEIEU9GY2EdHri6FaU8dmg,3534
+zepben/evolve/model/cim/iec61968/customers/customer_agreement.py,sha256=fwxvEgJfH0W-5HLQiMpwnR7FVJGe9kyWymj4osq9sns,4260
+zepben/evolve/model/cim/iec61968/customers/customer_kind.py,sha256=UpbvTjIbnPZw309y8Qp6RF9rHQBKZU1UI2z8kz-rxo0,1474
+zepben/evolve/model/cim/iec61968/customers/pricing_structure.py,sha256=wkzJRQKIxCwYCTGNSk2tffcUsnyWmMXSfjsdu9MBGSQ,3336
+zepben/evolve/model/cim/iec61968/customers/tariff.py,sha256=KDSJnsZS_1yH31bOfvo-Dz7Df188MX6UTc3OfW_KfBo,763
+zepben/evolve/model/cim/iec61968/infiec61968/__init__.py,sha256=RGM0GFHzBSLROtXidZbsY9X1vCCfGVUO7isA-sYW-GY,244
+zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/__init__.py,sha256=RGM0GFHzBSLROtXidZbsY9X1vCCfGVUO7isA-sYW-GY,244
+zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/current_transformer_info.py,sha256=2EdsKrbFTDcVpO0ilGJOXyVn5iFDnWnMCsAoYLnN1xg,1859
+zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/potential_transformer_info.py,sha256=VDDptnrrAn-lcuoagTwU0M8CjvnLj-vx6z42SeynphM,1250
+zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/relay_info.py,sha256=rK0F27mE7_600iVMOsLymlGe_c7Ko9ZFirZl2JEEhxU,4360
+zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_construction_kind.py,sha256=W3sxisiNRXSrnlFB7pqPeSToA51wvInOODXD1b3fy7I,993
+zepben/evolve/model/cim/iec61968/infiec61968/infassetinfo/transformer_function_kind.py,sha256=9e8UD-vadSdEt-Vnm3wIAZstibBWdxRNBORa-ZXRL8g,1098
+zepben/evolve/model/cim/iec61968/infiec61968/infcommon/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61968/infiec61968/infcommon/ratio.py,sha256=EIO7atqY3ZlP_u0Oahh4iL24Jw_5vFfLiB_PmwYouz0,1202
+zepben/evolve/model/cim/iec61968/metering/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61968/metering/metering.py,sha256=ZKvnvrCAdY2Hai9e6Rj2sn_Cj_wpbzosOiKd5MwfFpY,11269
+zepben/evolve/model/cim/iec61968/operations/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61968/operations/operational_restriction.py,sha256=8zSpERQaLaYX4aIR1EVd-ps3R7xrizyvjZByx-8Q-Uk,3889
+zepben/evolve/model/cim/iec61970/__init__.py,sha256=jojtysZVlur9A2vEmq9WMRCEo3l1saGnlMQOtWJ0frw,248
+zepben/evolve/model/cim/iec61970/base/__init__.py,sha256=S_XWWKVOvvudQ4B5lMlhR0RlPmU5PAIkh8MiZpZxVlM,249
+zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/auxiliary_equipment.py,sha256=9j86ck-xBnuWM4IVg8PqR4JW-oUDqvVeRa2ORZMJfCM,1475
+zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/current_transformer.py,sha256=gHqZLz8ULtxJnmGypp9rY-lyZbNLyR_wdV4lhpdYmw0,1489
+zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer.py,sha256=RmNlLalDYIOnN8PLSfNlNFIFocaCKz5k79mibj26xNw,1753
+zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/potential_transformer_kind.py,sha256=I3jVS-40Sg69bLnqaGGG_4OPfsbdUDNB4fXzt2cyBwA,811
+zepben/evolve/model/cim/iec61970/base/auxiliaryequipment/sensor.py,sha256=1qW-cxX5_Qlsel3Q0p0_ZO7Dk9F1juFylym1gk3EbKY,3877
+zepben/evolve/model/cim/iec61970/base/core/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/core/base_voltage.py,sha256=bf-ehTnrgIsyBLgN-Dp-TE4ez6mrQRvVblseDDVKgo0,556
+zepben/evolve/model/cim/iec61970/base/core/conducting_equipment.py,sha256=Te_aCSIUP3ifd4vQu70b15Z8f-Emgja98ZStz3Xe2gg,7135
+zepben/evolve/model/cim/iec61970/base/core/connectivity_node.py,sha256=px7pqa3AvJ002Z31059A4f8mDn3rLtVNLiCGIgl8ts8,3645
+zepben/evolve/model/cim/iec61970/base/core/connectivity_node_container.py,sha256=HgTcCmPS-KAwdJ1i0KxDUZdcB6j29MNR2RmvjCT1dGg,592
+zepben/evolve/model/cim/iec61970/base/core/equipment.py,sha256=x-WG4AMOQIg6-62W0phDtzzE6KwW7tdJpVeYNWMtANo,14195
+zepben/evolve/model/cim/iec61970/base/core/equipment_container.py,sha256=FApNfDNem8QmP-UlM7wi_cv0f6fs6LssHLB2RkkNCqM,15682
+zepben/evolve/model/cim/iec61970/base/core/identified_object.py,sha256=PwXv1xcB20Bq9301mUcqfiNQvoP9TG6DgR989CWXJ-8,8261
+zepben/evolve/model/cim/iec61970/base/core/name.py,sha256=U3MylzCG10Vcusi_xa2hjkRywTQERKRDICBl0pfrVUw,1095
+zepben/evolve/model/cim/iec61970/base/core/name_type.py,sha256=jYaVOSfSwXlaarRd00Be50hdSUpTv5j6OmulZG08YUc,7475
+zepben/evolve/model/cim/iec61970/base/core/phase_code.py,sha256=-3AZlREfaKE7CBc9fC2u8gFIDRIEpCmbhzZzF3v61tA,7033
+zepben/evolve/model/cim/iec61970/base/core/power_system_resource.py,sha256=-k4ccAxqKLUGvuChwNDKdbTpG9Sj81CPZU0PB4hnr3A,1250
+zepben/evolve/model/cim/iec61970/base/core/regions.py,sha256=6wtRtfMku9ZFOA394ab7LUjsunvKuVSobbMIWk9edLc,6734
+zepben/evolve/model/cim/iec61970/base/core/substation.py,sha256=FlihvZ7f7XNkrcAYXmXvhnpwSSIX9YBup6X_vTFKw_E,10120
+zepben/evolve/model/cim/iec61970/base/core/terminal.py,sha256=qhyAeAJukxm5PkSa1nywH21bA-iv0QTZMjm8pf3HaQ8,6717
+zepben/evolve/model/cim/iec61970/base/diagramlayout/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_layout.py,sha256=3d7cVgc6E_0wyAWfrkztQUp6uc2DGVyQKlzbh3uHIpg,10307
+zepben/evolve/model/cim/iec61970/base/diagramlayout/diagram_style.py,sha256=FHVcPUaotDXtphZh02waP6VvQ_CCXUU2OCAEe3IPSbE,748
+zepben/evolve/model/cim/iec61970/base/diagramlayout/orientation_kind.py,sha256=9ohychwmLYoeJRoT-6_lU0jidbqggZMVwtf2TqFFP9U,1024
+zepben/evolve/model/cim/iec61970/base/domain/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/domain/unit_symbol.py,sha256=GQrbOepPIXBwBCal2YIQcfkdAAMpNpVzz3-oWt7eUJs,17065
+zepben/evolve/model/cim/iec61970/base/equivalents/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_branch.py,sha256=KNPRTGavqMYgCp6MBXBr7f-Dmz5rmW5nkitStI9wf6U,5374
+zepben/evolve/model/cim/iec61970/base/equivalents/equivalent_equipment.py,sha256=QjSqU2XaGRPW4N9ceNX74UUVVrxQl7ze-FW-ZD4QVtg,641
+zepben/evolve/model/cim/iec61970/base/meas/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/meas/control.py,sha256=P8ojErHa1nRxlD5wDccBrqIrvDQUTqiUdjUeP6TfjQk,963
+zepben/evolve/model/cim/iec61970/base/meas/iopoint.py,sha256=4GdY9pPfmFBZPIrGtwLkGMOfy4pK4iGE8qiGUpBrABg,576
+zepben/evolve/model/cim/iec61970/base/meas/measurement.py,sha256=erjhHekmEeIvQpfi9kn8lAM0ACb3tpChdI0lKob8P4w,4294
+zepben/evolve/model/cim/iec61970/base/meas/value.py,sha256=jAXzZVKLTqpI0Wj4rqfAunKvcaLc1f9sbZDvbmZaIh0,1753
+zepben/evolve/model/cim/iec61970/base/protection/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61970/base/protection/current_relay.py,sha256=ARjKwbqivyHRl_-0OosJaLhCVDjWzpmeN8NmmtTRcyA,920
+zepben/evolve/model/cim/iec61970/base/protection/distance_relay.py,sha256=ioN-TL181fs8h6As9cC7u0RkCmF8c50Z-JLSzeX-LpA,2561
+zepben/evolve/model/cim/iec61970/base/protection/protection_relay_function.py,sha256=JxXw-fyGIOn58R1-Xg7mUMhzpdvsN7rYikqWKsNdV9k,18678
+zepben/evolve/model/cim/iec61970/base/protection/protection_relay_scheme.py,sha256=kJRyIBSNUsAcAD5jQYX16UldV-MSUnWEWonz8K6Jpok,4228
+zepben/evolve/model/cim/iec61970/base/protection/protection_relay_system.py,sha256=uDqcKbqC5xanqk_IN6D6-9RXDNBl6psKPrldVx-Ps-s,3848
+zepben/evolve/model/cim/iec61970/base/protection/relay_setting.py,sha256=-AKW679suNyzgbiH9a6Ff7dp_qArDFDNJgMvTpcLOnw,963
+zepben/evolve/model/cim/iec61970/base/protection/voltage_relay.py,sha256=NDvBI-MZCTYjMbl7UleJg92rn7VAN4GF8sUNw5Lehkc,696
+zepben/evolve/model/cim/iec61970/base/scada/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/scada/remote_control.py,sha256=WJtnb3oTqr5uq1j4HVrRglZGNXY3hCWzoFQ16R7uhdk,737
+zepben/evolve/model/cim/iec61970/base/scada/remote_point.py,sha256=u3vkTn0591B0OwwgMguOsjYXovrH47EB0wa7O3ogGyk,587
+zepben/evolve/model/cim/iec61970/base/scada/remote_source.py,sha256=2xglEpjir5wuw1JX9waIpZc5zBOLKrlixALWTpJ0tco,734
+zepben/evolve/model/cim/iec61970/base/wires/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/wires/aclinesegment.py,sha256=1ximiz-CyJY4XlHW9JyVqgvkVLKyz3zl0KHIv-yJoXg,2433
+zepben/evolve/model/cim/iec61970/base/wires/breaker.py,sha256=W7KKBw1n1MqXSnp_gewrfgTA9GAVjZ9XsTk2hdbelDc,1385
+zepben/evolve/model/cim/iec61970/base/wires/connectors.py,sha256=sdyPBxtsOePKqxTkSCSYiYLcaxGzBHtMEQKcog3_tsY,1413
+zepben/evolve/model/cim/iec61970/base/wires/disconnector.py,sha256=cT_2ereQy2YVUfl1bwRRB7cplNBY_WE2NxbzLgJj0Bw,672
+zepben/evolve/model/cim/iec61970/base/wires/energy_connection.py,sha256=d5Q_t4M7hIcE43AYyJ8HtvOTt4glpdZ8DJI_88DYeLY,1929
+zepben/evolve/model/cim/iec61970/base/wires/energy_consumer.py,sha256=DW0Gx98qyT_gAqx6JdsOu7_1gDVu4_BwVyA1hHr8G0k,7483
+zepben/evolve/model/cim/iec61970/base/wires/energy_source.py,sha256=5bJHIkDuqVEAjsOiCjvLKsoyBH0lQ6HyqCuM4XQiifQ,6517
+zepben/evolve/model/cim/iec61970/base/wires/energy_source_phase.py,sha256=7ws_joykdhlo-PhyWDSQU4hHbij9DboVbZb5JsN_GN8,1977
+zepben/evolve/model/cim/iec61970/base/wires/fuse.py,sha256=zkiz01TKLnTWmtc4xc1GVVJbuTFobp03JQzq_7SE5aU,831
+zepben/evolve/model/cim/iec61970/base/wires/ground.py,sha256=FMkyVbBPUpTBBIUKfADOj1KPKnD6CLT-7UxvnaRdQZA,573
+zepben/evolve/model/cim/iec61970/base/wires/ground_disconnector.py,sha256=9-o0XGRhBqeW9ZZ2r8EZwuJYoJHC7aT86_MF5g9BgtU,535
+zepben/evolve/model/cim/iec61970/base/wires/jumper.py,sha256=y3SOu_ul5yOTtksu_WMWaE0yMkXdV-j3HvNCBfhRwSA,611
+zepben/evolve/model/cim/iec61970/base/wires/line.py,sha256=9bAYHVRTIrUghqprdHw2ZY33Zq9SD8yCQDLrmOYg6ho,492
+zepben/evolve/model/cim/iec61970/base/wires/load_break_switch.py,sha256=7GkRZMwD1TWJ5FYMuDzDiHlyxHD3XnRKcB9Fn7EzG3I,584
+zepben/evolve/model/cim/iec61970/base/wires/per_length.py,sha256=E_MIPnSxJwTOzed5js4feOBqkLaDJ0ktAtFMkBCVHwE,1904
+zepben/evolve/model/cim/iec61970/base/wires/phase_shunt_connection_kind.py,sha256=2IEt5oWMbe4JUuZduH-3UE329jcopW93L7bfA9Ugjt0,884
+zepben/evolve/model/cim/iec61970/base/wires/power_electronics_connection.py,sha256=mGmzoODLu91_IKhybPzj0B3qOagAWgOZUTt2dfN2eLI,24976
+zepben/evolve/model/cim/iec61970/base/wires/power_transformer.py,sha256=uFv63t26mK5IDzaV3jBXfK0Uhz0rjITuX-OJVeW70vs,31160
+zepben/evolve/model/cim/iec61970/base/wires/protected_switch.py,sha256=ugleMRPh3CunG_2MqFZ7YtKMBIrZoJzKpD1Hb_3Zndg,4181
+zepben/evolve/model/cim/iec61970/base/wires/recloser.py,sha256=rR8ZPnr6IpnkmvqzwU0HAPB4QLCuvj-dDS9t28TAHsE,582
+zepben/evolve/model/cim/iec61970/base/wires/regulating_control.py,sha256=nVx3S7Fa0NHeqM-8KD7LASxVIG8OfZSm2lSiMosh_cE,8338
+zepben/evolve/model/cim/iec61970/base/wires/regulating_control_mode_kind.py,sha256=ALz87FNgfkgak3dmP87rVTavWnLIAQ4hzFjJQd5XDNc,1168
+zepben/evolve/model/cim/iec61970/base/wires/series_compensator.py,sha256=GWZJno4Jfs_-nsRpKyXCepCtHvRbyepGgw_DpUAvu-A,1635
+zepben/evolve/model/cim/iec61970/base/wires/shunt_compensator.py,sha256=6mSerSy0RGQw6nUz7WyjaTu7NF1ppJotawpk8KAZ0Gs,3658
+zepben/evolve/model/cim/iec61970/base/wires/single_phase_kind.py,sha256=4QMnuASkLatpGwK06iX-DNRw-8eUPt7Gd_5f0rutiJY,2944
+zepben/evolve/model/cim/iec61970/base/wires/switch.py,sha256=1CHEeMTdRQ48O01pKjUMr6H1km9_JDSbnNZMNK8oTxs,4955
+zepben/evolve/model/cim/iec61970/base/wires/tap_changer_control.py,sha256=wPXXSN8m-fZkottPmBQ0LE-DbxGJcjci56woiqksJGU,2112
+zepben/evolve/model/cim/iec61970/base/wires/transformer_cooling_type.py,sha256=G_kRSh2gHF10s22FRqV1KmpJthtl4PGY2KuBa2e_-t4,1045
+zepben/evolve/model/cim/iec61970/base/wires/transformer_star_impedance.py,sha256=aKCF74y1leqikKWTVVBXIO7VLEqJRV42teyzPPnvFQk,2219
+zepben/evolve/model/cim/iec61970/base/wires/vector_group.py,sha256=dsICvkrwR3GADbSjt-nIPjc3ZsD0yWhQGoXXOgCTpXY,1544
+zepben/evolve/model/cim/iec61970/base/wires/winding_connection.py,sha256=i_KupPnfA4i_VC3bAHa_svgX20lbaOM-VCM6jIl-24E,786
+zepben/evolve/model/cim/iec61970/base/wires/generation/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/wires/generation/production/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/base/wires/generation/production/battery_state_kind.py,sha256=mg-EueYAMTXlS8LBDT0cREfL5b5_79sQDpoSIL8G5Rw,809
+zepben/evolve/model/cim/iec61970/base/wires/generation/production/power_electronics_unit.py,sha256=yaSPXGqYE4z3Js4tOUG8RZsm0XGg2WlUIJeYkHDAPQQ,2215
+zepben/evolve/model/cim/iec61970/infiec61970/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61970/infiec61970/feeder/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/model/cim/iec61970/infiec61970/feeder/circuit.py,sha256=Yk9JX7pJkPmtgRsZ-XNHYiFGDGRMCrMC33vYmzJJWVQ,5385
+zepben/evolve/model/cim/iec61970/infiec61970/feeder/loop.py,sha256=cApKLVAqp1dGMJisiFMdIwnzh5sht4yvCDDBx7bXByA,7542
+zepben/evolve/model/cim/iec61970/infiec61970/feeder/lv_feeder.py,sha256=Rm2xqnU9mO5aXsUtZSHLXrPette0zuSkBMOSKu2kq1E,7636
+zepben/evolve/model/cim/iec61970/infiec61970/protection/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61970/infiec61970/protection/power_direction_kind.py,sha256=NUrh6_T68mxUXzZWqHGBg-OzJJ-WyVMVX22pKZEnUwQ,746
+zepben/evolve/model/cim/iec61970/infiec61970/protection/protection_kind.py,sha256=R2DJDdkFKkxL6YXSrKEkyWMrwCe7JTDCo-XWTs_ByGY,2711
+zepben/evolve/model/cim/iec61970/infiec61970/wires/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/model/cim/iec61970/infiec61970/wires/generation/production/ev_charging_unit.py,sha256=DhoY1U3dhX64Kiix5n4yTA112qjCrKyT8xZ5RG5u0Jo,426
+zepben/evolve/services/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/common/__init__.py,sha256=8iViIKUj3S3WA9WuhTb5ot5lg7vKWPvhPIa45QAHMHM,960
+zepben/evolve/services/common/base_service.py,sha256=bkAfk8mW8fR9alD8anV7QcFt0cS1q7s5eYy0-vTnHL4,18023
+zepben/evolve/services/common/base_service_comparator.py,sha256=QFwRUYKT1_W39UzAARJCmY3atsI2m-H-voPI7YQZzno,16620
+zepben/evolve/services/common/difference.py,sha256=hL4oIBGOD4YGcKHQ1K09qR4SYDVLX_1_RKuistLtRDs,1189
+zepben/evolve/services/common/reference_resolvers.py,sha256=9m-ewL5omeEGZKZtyHvHBeUwEh1M0Qj8enYQHPfrbuA,24212
+zepben/evolve/services/common/resolver.py,sha256=3uZeThH0_thHbVsSKp46i5NHpT8eOQA4U1_6UPvDtto,22825
+zepben/evolve/services/common/meta/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/services/common/meta/data_source.py,sha256=0OVR85otIjBty7-g-PW9oJSzH3BOtSowZbDCeAciWI0,461
+zepben/evolve/services/common/meta/metadata_collection.py,sha256=_lB4YmqEoKe4NXVKyyJ3Nh5BCw25fnfwjEXfckaUQy8,804
+zepben/evolve/services/common/meta/metadata_translations.py,sha256=n8xKitFqilzuJO3FPmnryBDHsS3ybaCjbpr8yzyemEY,1481
+zepben/evolve/services/common/meta/service_info.py,sha256=oYFY2-U3pr3LwBwxKLXfbKhJOkA3ZRwn5cOrrGqXIMY,601
+zepben/evolve/services/common/translator/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/common/translator/base_cim2proto.py,sha256=Yk7IvFC-Nm3WP-PO_vrPiuk_odUoY2tyryrb56I670c,3420
+zepben/evolve/services/common/translator/base_proto2cim.py,sha256=wLyywkA85K0ydIUhs-eNfxh0zB2uJLk_1sLrLb6QLfU,3938
+zepben/evolve/services/common/translator/service_differences.py,sha256=uf83wTZLOlGCPaC5n0_m8QmLCBectJ3QPDZ60wJRuNI,2924
+zepben/evolve/services/common/translator/util.py,sha256=Sy2c-j3WXaLI1NMPzepF7DMRq0Niic60rnh_gFYHeTM,2410
+zepben/evolve/services/customer/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/customer/customer_service_comparator.py,sha256=DAFHwl3-3DS4Wlz6GPxfsPWVjAELTWyZefzWyTx2whI,1922
+zepben/evolve/services/customer/customers.py,sha256=C7zYbke24Wo5FiMWyDxImTE-Aq_IRvkVAXDyEQcU8V0,467
+zepben/evolve/services/customer/translator/__init__.py,sha256=c8LWHhBeBFnr8Rwp5YwEzp3P8F_SDeGn6BBf9M146mc,1044
+zepben/evolve/services/customer/translator/customer_cim2proto.py,sha256=7Jep0zKme51zC-r_41CqiO5wf-Sl5gJQpfTopbN8FDE,2760
+zepben/evolve/services/customer/translator/customer_proto2cim.py,sha256=sPl93bytD8vSGI3K1MpZp3TQub6Om_XThkFYramicWk,3379
+zepben/evolve/services/diagram/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/diagram/diagram_service_comparator.py,sha256=kav-3j1t1TeLVtXFKtw6lBs5cYicYVylE_RQX9MarAQ,1486
+zepben/evolve/services/diagram/diagrams.py,sha256=umDzukqpPjQxkv9r_Cgn9whdJZPL1iXhMB8c2NDYPyE,4598
+zepben/evolve/services/diagram/translator/__init__.py,sha256=fP-H0TliyeMQTtvvKkbxYgG4C_SFCGxseJohtHRnzWE,508
+zepben/evolve/services/diagram/translator/diagram_cim2proto.py,sha256=-r579-mySrASPs7Ca8M9rTSq1ipquMaRYKQ8vcOJa0w,2237
+zepben/evolve/services/diagram/translator/diagram_proto2cim.py,sha256=LZ_ppqAWznl6sStFevPcA-pQ9kuFYVDq8XZFtXu19B8,2463
+zepben/evolve/services/measurement/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/measurement/measurements.py,sha256=ZWXCJePhK9tXBbGkWizZ4elvKCOaG6JsHcGgI8Q-Nhc,1207
+zepben/evolve/services/measurement/translator/__init__.py,sha256=l3XZvooZ1GPkhrMz-fRv2IvPTUrtjNGNfPj5ySKq82Q,261
+zepben/evolve/services/measurement/translator/measurement_cim2proto.py,sha256=UQLiPnZS2lZiFTxwIxG1FApUHdxIgoSBZB_CPC-Y11k,1832
+zepben/evolve/services/measurement/translator/measurement_proto2cim.py,sha256=SJGDoQZshsRhPYarSuuNauCMrU3Iiu2HQlv5oRzaLFA,1951
+zepben/evolve/services/network/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/network/network_extensions.py,sha256=1no2umm22z4LsC7ia4xepIKLSlT_YyrHJXdKJ2uEMB8,6279
+zepben/evolve/services/network/network_service.py,sha256=8EGMo1g3Mrz4BwBjom24g2VqZnfd48p8eMIfqqQ5tGo,10634
+zepben/evolve/services/network/network_service_comparator.py,sha256=4duItPYWuilcViprMq2WWWNmIUPRuSA4-l9NyV4hc5E,46822
+zepben/evolve/services/network/tracing/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/network/tracing/find.py,sha256=UhmH3fUHCpcKmnTHcNU8nUfdLAamkxwbgGbU1IFgWp0,3654
+zepben/evolve/services/network/tracing/find_swer_equipment.py,sha256=BYLeCfSn4TQFqJsBHjbH55Wv_HuY4su2Bcij24WOG48,5623
+zepben/evolve/services/network/tracing/tracing.py,sha256=if0JicIVSY_QHffeevBoZueVoKtd8KieUDIVc6eJq1c,16173
+zepben/evolve/services/network/tracing/util.py,sha256=tHLCRqvdlpuLBw8n0zmyZTxu7cf3saUoVCb6u3xf7VI,3395
+zepben/evolve/services/network/tracing/connectivity/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step.py,sha256=G3eTlmh0m802RcQORFF8m6P9eNUH5MuOG1G7VZLgzn0,775
+zepben/evolve/services/network/tracing/connectivity/conducting_equipment_step_tracker.py,sha256=9LsjItuh7HhNnmdkZyqFLfZUts5WIdEfsDjG4vwa-ew,2394
+zepben/evolve/services/network/tracing/connectivity/connected_equipment_trace.py,sha256=p5hwdILCrKa3hgznMCjY-NKqBc9OoFO77b5DvaLRRok,8474
+zepben/evolve/services/network/tracing/connectivity/connected_equipment_traversal.py,sha256=nkJBincJmzKyFzUuDOVkDKtO2vFPI_LeQlu0rlGxX2E,1162
+zepben/evolve/services/network/tracing/connectivity/connectivity_result.py,sha256=ntxiH4exeazs6Zf2lgo3dqY3w86gwOB2b6gs0hS9u5M,4223
+zepben/evolve/services/network/tracing/connectivity/connectivity_trace.py,sha256=uICrBkqQB_5O2TGM2RNl2L3MK_OtesdfDd3-aqgfp4c,2671
+zepben/evolve/services/network/tracing/connectivity/connectivity_tracker.py,sha256=FAwd4IkpXiOk3aGkgxa4lCt7CUzf7DO6Ql9eyoB8JPg,1212
+zepben/evolve/services/network/tracing/connectivity/limited_connected_equipment_trace.py,sha256=GW7LC85MMQnZxWBZ3gJ1Zlg986Tx6evpuZ-oM2jJf6M,5162
+zepben/evolve/services/network/tracing/connectivity/phase_paths.py,sha256=uwLww8-KjcFNXb0XqmFXMLnYklee1fZ81FYkU8B-DdM,3872
+zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_connected.py,sha256=hQfKmWB8chYj-WCAsI3Uv_36O5OC0K-82pHbwRnC_qg,9998
+zepben/evolve/services/network/tracing/connectivity/terminal_connectivity_internal.py,sha256=hc_0YRwb08vABwn9xucPF8TstNgNxBugL4-4z372LCQ,2862
+zepben/evolve/services/network/tracing/connectivity/transformer_phase_paths.py,sha256=5pgOCkEC_m6d-oO9nMPns63TNxcZGex1QcNEQtZAusA,11472
+zepben/evolve/services/network/tracing/connectivity/xy_candidate_phase_paths.py,sha256=0ypMn4L01zr_haV9h3WWP26xlLNqSKxX2BkonvH_NiQ,10412
+zepben/evolve/services/network/tracing/connectivity/xy_phase_step.py,sha256=fOiM79VWa4o2OmAa0pdBzovi-f_VKAn4iIn-x2c2VxY,583
+zepben/evolve/services/network/tracing/feeder/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/network/tracing/feeder/assign_to_feeders.py,sha256=-iYQwFTPEj1PM6g9jA6SsvCHBjlPK7G_UPa9e_LUOEU,5997
+zepben/evolve/services/network/tracing/feeder/assign_to_lv_feeders.py,sha256=9GS0H3dZod3GRKJ5wlte1xhX_5tM2Gr_afRr9VS_wys,6053
+zepben/evolve/services/network/tracing/feeder/associated_terminal_trace.py,sha256=f-NqM2QT9RjUHAORoDTOCcB_XIi_2Rg0Y68PcitAEkI,3246
+zepben/evolve/services/network/tracing/feeder/associated_terminal_tracker.py,sha256=-1gLWYmUMGdSSAWp3ukfVJoR-drsTWKB7Plh0sKXEYQ,1477
+zepben/evolve/services/network/tracing/feeder/direction_status.py,sha256=rrvcUYIKHId9Nnh82U1qU21vcIe4lwLvs1SU5EjDRT8,3990
+zepben/evolve/services/network/tracing/feeder/feeder_direction.py,sha256=u0P585ZRwCGoD_fHTv6fHA2lMrybQ4KNIEO10ExG9Jw,2546
+zepben/evolve/services/network/tracing/feeder/remove_direction.py,sha256=FZwHivx22RhRBqPuLXLeAcax56aQ2eDDnECSJGHztOo,7410
+zepben/evolve/services/network/tracing/feeder/set_direction.py,sha256=DPKqY-TGUJpuiURZPGFT3CrBeM-LeCLkN2rnGsamnl4,6757
+zepben/evolve/services/network/tracing/phases/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/network/tracing/phases/phase_inferrer.py,sha256=dOVVO9PoW7Oa40liYFxTOl9q4M7rJOjOrFXUIVfEDJ8,10311
+zepben/evolve/services/network/tracing/phases/phase_status.py,sha256=8OJ7jodAHvVmqmIeRfRWIHZGKoNZiG7KHHCon2KBaAs,3428
+zepben/evolve/services/network/tracing/phases/phase_step.py,sha256=yCVQfvqVXSQgp86stdxUfe9zN7YcH3VI2a-IaNV7xyk,2628
+zepben/evolve/services/network/tracing/phases/phase_step_tracker.py,sha256=yRxjbBJblxZhAChn9KmMUWt7rDEnx5-1PexfGicU_KM,2014
+zepben/evolve/services/network/tracing/phases/phase_trace.py,sha256=BFmhE-iykeMDKFFgrNDkv8pJm7eQ6TKVYZoIJLCecNQ,6251
+zepben/evolve/services/network/tracing/phases/remove_phases.py,sha256=s75cBBYUBIOZR_TsBJFFURUlAcn3ao6cqLuAJaTbXrI,5510
+zepben/evolve/services/network/tracing/phases/set_phases.py,sha256=cs9Qlrl54iNigLQgxMRHRbivUf5tyKviKdTc0_d0jOY,12798
+zepben/evolve/services/network/tracing/traversals/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/services/network/tracing/traversals/basic_tracker.py,sha256=QcwcctmSnl_QHKi195ladJneUl1DpiEwNLYzcFFNdfA,1642
+zepben/evolve/services/network/tracing/traversals/basic_traversal.py,sha256=lIVSMB4JNll05O7_p2do3JqBdpNd9ner3vQCT5L4L8o,2944
+zepben/evolve/services/network/tracing/traversals/branch_recursive_tracing.py,sha256=dEwVrS-Bl2MsvoAcXJ6eqiSJhMin4OD7gTzOeD_sxno,6585
+zepben/evolve/services/network/tracing/traversals/queue.py,sha256=Q-5PuJgYuiSLlNJkWWiLWEMP1T-9RZeFQAh02WACkvY,5164
+zepben/evolve/services/network/tracing/traversals/tracker.py,sha256=rvLwqzXFjGtMxQH0buUR8IsEDH5Tajavs4QZ8G5VJWE,1775
+zepben/evolve/services/network/tracing/traversals/traversal.py,sha256=-GqtFYx8iHei7A_8GHHnwkCEaTk0fd5xZ8LO3JWfyic,8650
+zepben/evolve/services/network/tracing/tree/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/services/network/tracing/tree/downstream_tree.py,sha256=QPLSrQnFax3wBVOquM61gOh0jbAWcqwwOg96cqY6N5E,4454
+zepben/evolve/services/network/tracing/tree/tree_node.py,sha256=RT2UrlWtABNrtLVQcp7xxC3EWewHWX4w9hluENhT9Yo,1780
+zepben/evolve/services/network/tracing/tree/tree_node_tracker.py,sha256=BaCjCNqrsSw2vnXh3zKlL41d3dpo1Ri2_nJdKoYLZ8A,1167
+zepben/evolve/services/network/translator/__init__.py,sha256=cCTBCnuR6F2ThlV3pmtYfmz50D3QAGR01RQXGGYolOE,23636
+zepben/evolve/services/network/translator/network_cim2proto.py,sha256=rEwL9jnk0ey9lXzWZGajTsxbnEWNhPt4oYvwdsZHO9I,70246
+zepben/evolve/services/network/translator/network_proto2cim.py,sha256=19iC5bT6_T4IUx6Yr_DO-tJdhL-TL2wnl6lEzTvQuq0,84542
+zepben/evolve/streaming/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/streaming/exceptions.py,sha256=i-imo3DJFLdQbVkwlxdvNPhXVLhYAjQbB1YV3V1stH4,427
+zepben/evolve/streaming/get/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/streaming/get/consumer.py,sha256=TcB0TtCPPKxAp8OVHUkzGOsPmel6KsNuRFQPJyWZRDM,9348
+zepben/evolve/streaming/get/customer_consumer.py,sha256=UzS45yUn3OWxZD2E-PYEJR9VUV1tRTaZ3Me80ELpseQ,5425
+zepben/evolve/streaming/get/diagram_consumer.py,sha256=pHmV1NrWQCqjSJuTZuACy9o109nzwNLh6gkm8Q1lxIU,5032
+zepben/evolve/streaming/get/network_consumer.py,sha256=2tdrziibqv1DoslcosbFpVUtAxyfpPjfksNFAgLbavM,38507
+zepben/evolve/streaming/get/hierarchy/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/streaming/get/hierarchy/data.py,sha256=pJKAIyeDzKvLZ80SQXtJzof6qLwDWU7mgVfxXVwh_IQ,1047
+zepben/evolve/streaming/grpc/__init__.py,sha256=59wf_CIVET959dk298B1tLbEfEj4DqNFi6uL11q17Qs,246
+zepben/evolve/streaming/grpc/auth_token_plugin.py,sha256=DYFuWbwj0gikHPLIwERDQcvNBna64gn_C16MJrYCgW0,801
+zepben/evolve/streaming/grpc/connect.py,sha256=SFMRhsQkZQJHha39TORCGH6ShMQEjXp2XwAocBIkBg8,9451
+zepben/evolve/streaming/grpc/grpc.py,sha256=pXj4NLBS9fwVRL9GYeEW3fezIXaTrPdZpIJJwxqTo5Q,4020
+zepben/evolve/streaming/grpc/grpc_channel_builder.py,sha256=IJOKNk_R3QAOC8PJ5nkBqyrSyMNFr6_KmnyzCZMyQP0,7664
+zepben/evolve/testing/__init__.py,sha256=UDtxkB3D_0TeZ3Z1YdznJf6xrmgxcNQwMQTyS4lGZK4,245
+zepben/evolve/testing/test_network_builder.py,sha256=uD0_rWK4_33ON8m67vBQlrfE6mzIC_BiAV5Gf88gk40,28552
+zepben/evolve/testing/test_traversal.py,sha256=Iy7ILctdL75M_qp2qmlLjb6FsuWaZ-Npg4NfPj77bME,3238
+zepben.evolve-0.38.0b8.dist-info/LICENSE,sha256=aAHD66h6PQIETpkJDvg5yEObyFvXUED8u7S8dlh6K0Y,16725
+zepben.evolve-0.38.0b8.dist-info/METADATA,sha256=LrEmTPWSFwK3MS1-JvnzoZDzE8_ByZ_X5F99d7uZgP8,2301
+zepben.evolve-0.38.0b8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+zepben.evolve-0.38.0b8.dist-info/top_level.txt,sha256=eVLDJiO6FGjL_Z7KdmFE-R8uf1Q07aaVLGe9Ee4kmBw,7
+zepben.evolve-0.38.0b8.dist-info/RECORD,,
```

