.. _ref_logs_opcua_binary_variant_metadata:

opcua_binary_variant_metadata
-----------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

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
     - The id.orig_ep_status information.

   * - ``id.orig_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_uid information.

   * - ``id.orig_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_cid information.

   * - ``id.orig_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_source information.

   * - ``id.resp_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_status information.

   * - ``id.resp_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_uid information.

   * - ``id.resp_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_cid information.

   * - ``id.resp_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_source information.

   * - ``id.vlan`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The VLAN that the connection is seen on.

   * - ``id.vlan_inner`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The inner VLAN tag for stacked VLAN tags.

   * - ``variant_source_data_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_source_data_link_id information.

   * - ``variant_data_source`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_source information.

   * - ``variant_data_source_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_source_str information.

   * - ``dara_variant_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The dara_variant_encoding_mask information.

   * - ``data_variant_data_type`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The data_variant_data_type information.

   * - ``data_variant_data_type_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The data_variant_data_type_str information.

   * - ``built_in_data_type`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The built_in_data_type information.

   * - ``built_in_data_type_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The built_in_data_type_str information.

   * - ``variant_data_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_link_id information.

   * - ``variant_data_array_dim`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_array_dim information.

   * - ``variant_data_array_multi_dim_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The variant_data_array_multi_dim_link_id information.
