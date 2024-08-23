.. _ref_logs_opcua_binary_browse_description:

opcua_binary_browse_description
-------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
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

   * - ``browse_description_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_link_id information.

   * - ``browse_description_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_encoding_mask information.

   * - ``browse_description_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_namespace_idx information.

   * - ``browse_description_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_numeric information.

   * - ``browse_description_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_string information.

   * - ``browse_description_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_guid information.

   * - ``browse_description_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_opaque information.

   * - ``browse_direction`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_direction information.

   * - ``browse_description_ref_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_ref_encoding_mask information.

   * - ``browse_description_ref_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_ref_namespace_idx information.

   * - ``browse_description_ref_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_ref_numeric information.

   * - ``browse_description_ref_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_ref_string information.

   * - ``browse_description_ref_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_ref_guid information.

   * - ``browse_description_ref_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_ref_opaque information.

   * - ``browse_description_include_subtypes`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_include_subtypes information.

   * - ``browse_node_class_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_node_class_mask information.

   * - ``browse_result_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_result_mask information.
