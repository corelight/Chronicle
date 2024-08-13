.. _ref_logs_opcua_binary_browse_response_references:

opcua_binary_browse_response_references
---------------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

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

   * - ``browse_reference_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_reference_link_id information.

   * - ``browse_response_ref_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_encoding_mask information.

   * - ``browse_response_ref_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_namespace_idx information.

   * - ``browse_response_ref_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_numeric information.

   * - ``browse_response_ref_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_string information.

   * - ``browse_response_ref_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_guid information.

   * - ``browse_response_ref_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_opaque information.

   * - ``browse_response_is_forward`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_is_forward information.

   * - ``browse_response_ref_type_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_type_encoding_mask information.

   * - ``browse_response_ref_type_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_type_namespace_idx information.

   * - ``browse_response_ref_type_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_type_numeric information.

   * - ``browse_response_ref_type_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_type_string information.

   * - ``browse_response_ref_type_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_type_guid information.

   * - ``browse_response_ref_type_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_type_opaque information.

   * - ``browse_response_ref_type_namespace_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_type_namespace_uri information.

   * - ``browse_response_ref_type_server_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_type_server_idx information.

   * - ``browse_response_ref_name_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_name_idx information.

   * - ``browse_response_ref_name`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_ref_name information.

   * - ``browse_response_display_name_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_display_name_mask information.

   * - ``browse_response_display_name_locale`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_display_name_locale information.

   * - ``browse_response_display_name_text`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_display_name_text information.

   * - ``browse_response_node_class`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_node_class information.

   * - ``browse_response_type_def_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_type_def_encoding_mask information.

   * - ``browse_response_type_def_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_type_def_namespace_idx information.

   * - ``browse_response_type_def_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_type_def_numeric information.

   * - ``browse_response_type_def_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_type_def_string information.

   * - ``browse_response_type_def_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_type_def_guid information.

   * - ``browse_response_type_def_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_type_def_opaque information.

   * - ``browse_response_type_def_namespace_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_type_def_namespace_uri information.

   * - ``browse_response_type_def_server_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_type_def_server_idx information.
