.. _ref_logs_opcua_binary_browse:

opcua_binary_browse
-------------------
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

   * - ``opcua_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The opcua_link_id information.

   * - ``browse_service_type`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_service_type information.

   * - ``browse_view_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_view_id_encoding_mask information.

   * - ``browse_view_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_view_id_namespace_idx information.

   * - ``browse_view_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_view_id_numeric information.

   * - ``browse_view_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_view_id_string information.

   * - ``browse_view_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_view_id_guid information.

   * - ``browse_view_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_view_id_opaque information.

   * - ``browse_view_description_timestamp`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_view_description_timestamp information.

   * - ``browse_view_description_view_version`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_view_description_view_version information.

   * - ``req_max_ref_nodes`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The req_max_ref_nodes information.

   * - ``browse_description_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_description_link_id information.

   * - ``browse_next_release_continuation_point`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_next_release_continuation_point information.

   * - ``browse_next_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_next_link_id information.

   * - ``browse_response_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_response_link_id information.

   * - ``browse_diag_info_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/browse-types.zeek
     - The browse_diag_info_link_id information.
