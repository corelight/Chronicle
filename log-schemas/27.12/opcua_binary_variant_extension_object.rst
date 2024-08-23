.. _ref_logs_opcua_binary_variant_extension_object:

opcua_binary_variant_extension_object
-------------------------------------
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

   * - ``ext_obj_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_link_id information.

   * - ``ext_obj_node_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_node_id_encoding_mask information.

   * - ``ext_obj_node_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_node_id_namespace_idx information.

   * - ``ext_obj_node_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_node_id_numeric information.

   * - ``ext_obj_node_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_node_id_string information.

   * - ``ext_obj_node_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_node_id_guid information.

   * - ``ext_obj_node_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_node_id_opaque information.

   * - ``ext_obj_type_id_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_type_id_str information.

   * - ``ext_obj_encoding`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/variant-types.zeek
     - The ext_obj_encoding information.
