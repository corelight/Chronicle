.. _ref_logs_opcua_binary_aggregate_filter:

opcua_binary_aggregate_filter
-----------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

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

   * - ``monitored_parameters_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The monitored_parameters_link_id information.

   * - ``start_time`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The start_time information.

   * - ``start_time_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The start_time_str information.

   * - ``aggregate_type_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The aggregate_type_encoding_mask information.

   * - ``aggregate_type_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The aggregate_type_namespace_idx information.

   * - ``aggregate_type_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The aggregate_type_numeric information.

   * - ``aggregate_type_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The aggregate_type_string information.

   * - ``aggregate_type_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The aggregate_type_guid information.

   * - ``aggregate_type_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The aggregate_type_opaque information.

   * - ``processing_interval`` (number - double)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The processing_interval information.

   * - ``use_server_capabilities_default`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The use_server_capabilities_default information.

   * - ``treat_uncertain_as_bad`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The treat_uncertain_as_bad information.

   * - ``percent_data_good`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The percent_data_good information.

   * - ``percent_data_bad`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The percent_data_bad information.

   * - ``use_slopped_extrapolation`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The use_slopped_extrapolation information.

   * - ``revised_start_time`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The revised_start_time information.

   * - ``revised_start_time_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The revised_start_time_str information.

   * - ``revised_processing_interval`` (number - double)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The revised_processing_interval information.

   * - ``revised_use_server_capabilities_default`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The revised_use_server_capabilities_default information.

   * - ``revised_treat_uncertain_as_bad`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The revised_treat_uncertain_as_bad information.

   * - ``revised_percent_data_good`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The revised_percent_data_good information.

   * - ``revised_percent_data_bad`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The revised_percent_data_bad information.

   * - ``revised_use_slopped_extrapolation`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/filter-types.zeek
     - The revised_use_slopped_extrapolation information.
