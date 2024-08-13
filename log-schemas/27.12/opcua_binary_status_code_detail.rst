.. _ref_logs_opcua_binary_status_code_detail:

opcua_binary_status_code_detail
-------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
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

   * - ``status_code_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The status_code_link_id information.

   * - ``source`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The source information.

   * - ``source_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The source_str information.

   * - ``source_level`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The source_level information.

   * - ``status_code`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The status_code information.

   * - ``severity`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The severity information.

   * - ``severity_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The severity_str information.

   * - ``sub_code`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The sub_code information.

   * - ``sub_code_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The sub_code_str information.

   * - ``structure_changed`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The structure_changed information.

   * - ``semantics_changed`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The semantics_changed information.

   * - ``info_type`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The info_type information.

   * - ``info_type_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The info_type_str information.

   * - ``limit_bits`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The limit_bits information.

   * - ``limit_bits_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The limit_bits_str information.

   * - ``overflow`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The overflow information.

   * - ``historian_bits`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The historian_bits information.

   * - ``historian_bits_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The historian_bits_str information.

   * - ``historianPartial`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The historianPartial information.

   * - ``historianExtraData`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The historianExtraData information.

   * - ``historianMultiValue`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The historianMultiValue information.
