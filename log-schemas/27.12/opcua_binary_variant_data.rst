.. _ref_logs_opcua_binary_variant_data:

opcua_binary_variant_data
-------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The uid information.

   * - ``id.orig_h`` (string - addr)
     - base
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - base
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - base
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - base
     - The responder's port number.

   * - ``id.orig_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The status of the originator's endpoint agent.

   * - ``id.orig_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint unique ID.

   * - ``id.orig_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint Customer ID.

   * - ``id.orig_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint information source.

   * - ``id.resp_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The status of the responder's endpoint agent.

   * - ``id.resp_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint unique ID.

   * - ``id.resp_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint Customer ID.

   * - ``id.resp_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint information source.

   * - ``id.vlan`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The VLAN that the connection is seen on.

   * - ``id.vlan_inner`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The inner VLAN tag for stacked VLAN tags.

   * - ``variant_data_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_link_id information.

   * - ``variant_data_value_signed_numeric`` (integer - int)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_value_signed_numeric information.

   * - ``variant_data_value_unsigned_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_value_unsigned_numeric information.

   * - ``variant_data_value_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_value_string information.

   * - ``variant_data_node_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_node_id_encoding_mask information.

   * - ``variant_data_node_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_node_id_namespace_idx information.

   * - ``variant_data_node_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_node_id_numeric information.

   * - ``variant_data_node_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_node_id_string information.

   * - ``variant_data_node_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_node_id_guid information.

   * - ``variant_data_node_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_node_id_opaque information.

   * - ``variant_data_node_id_namespace_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_node_id_namespace_uri information.

   * - ``variant_data_node_id_server_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_node_id_server_idx information.

   * - ``variant_data_value_time`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_value_time information.

   * - ``variant_data_encoding_name_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_encoding_name_idx information.

   * - ``variant_data_encoding_name`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_encoding_name information.

   * - ``variant_data_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_mask information.

   * - ``variant_data_locale`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_locale information.

   * - ``variant_data_text`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_text information.

   * - ``variant_data_value_decimal`` (number - double)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_value_decimal information.

   * - ``variant_data_status_code_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_status_code_link_id information.

   * - ``variant_data_diag_info_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_diag_info_link_id information.

   * - ``variant_data_ext_obj_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_ext_obj_link_id information.

   * - ``variant_metadata_data_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_metadata_data_link_id information.

   * - ``variant_data_value_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_value_link_id information.
