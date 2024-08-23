.. _ref_logs_opcua_binary_read_nodes_to_read:

opcua_binary_read_nodes_to_read
-------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
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

   * - ``nodes_to_read_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The nodes_to_read_link_id information.

   * - ``node_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The node_id_encoding_mask information.

   * - ``node_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The node_id_namespace_idx information.

   * - ``node_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The node_id_numeric information.

   * - ``node_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The node_id_string information.

   * - ``node_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The node_id_guid information.

   * - ``node_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The node_id_opaque information.

   * - ``attribute_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The attribute_id information.

   * - ``attribute_id_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The attribute_id_str information.

   * - ``index_range`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The index_range information.

   * - ``data_encoding_name_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The data_encoding_name_idx information.

   * - ``data_encoding_name`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/read-types.zeek
     - The data_encoding_name information.
