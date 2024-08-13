.. _ref_logs_opcua_binary_diag_info_detail:

opcua_binary_diag_info_detail
-----------------------------
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

   * - ``diag_info_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The diag_info_link_id information.

   * - ``root_object_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The root_object_id information.

   * - ``source`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The source information.

   * - ``source_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The source_str information.

   * - ``inner_diag_level`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The inner_diag_level information.

   * - ``has_symbolic_id`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The has_symbolic_id information.

   * - ``symbolic_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The symbolic_id information.

   * - ``symbolic_id_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The symbolic_id_str information.

   * - ``has_namespace_uri`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The has_namespace_uri information.

   * - ``namespace_uri`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The namespace_uri information.

   * - ``namespace_uri_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The namespace_uri_str information.

   * - ``has_locale`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The has_locale information.

   * - ``locale`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The locale information.

   * - ``locale_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The locale_str information.

   * - ``has_locale_txt`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The has_locale_txt information.

   * - ``locale_txt`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The locale_txt information.

   * - ``locale_txt_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The locale_txt_str information.

   * - ``has_addl_info`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The has_addl_info information.

   * - ``addl_info`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The addl_info information.

   * - ``has_inner_stat_code`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The has_inner_stat_code information.

   * - ``inner_stat_code`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The inner_stat_code information.

   * - ``has_inner_diag_info`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/statuscode-diagnostic-types.zeek
     - The has_inner_diag_info information.
