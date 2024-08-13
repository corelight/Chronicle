.. _ref_logs_opcua_binary_event_filter_attribute_operand_browse_paths:

opcua_binary_event_filter_attribute_operand_browse_paths
--------------------------------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
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

   * - ``browse_path_element_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The browse_path_element_link_id information.

   * - ``type_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The type_id_encoding_mask information.

   * - ``type_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The type_id_namespace_idx information.

   * - ``type_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The type_id_numeric information.

   * - ``type_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The type_id_string information.

   * - ``type_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The type_id_guid information.

   * - ``type_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The type_id_opaque information.

   * - ``is_inverse`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The is_inverse information.

   * - ``include_subtypes`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The include_subtypes information.

   * - ``target_name_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The target_name_namespace_idx information.

   * - ``target_name`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The target_name information.
