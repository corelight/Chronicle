.. _ref_logs_opcua_binary_create_monitored_items_create_item:

opcua_binary_create_monitored_items_create_item
-----------------------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
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

   * - ``create_item_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The create_item_link_id information.

   * - ``item_to_monitor_node_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_node_id_encoding_mask information.

   * - ``item_to_monitor_node_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_node_id_namespace_idx information.

   * - ``item_to_monitor_node_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_node_id_numeric information.

   * - ``item_to_monitor_node_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_node_id_string information.

   * - ``item_to_monitor_node_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_node_id_guid information.

   * - ``item_to_monitor_node_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_node_id_opaque information.

   * - ``item_to_monitor_attribute_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_attribute_id information.

   * - ``item_to_monitor_index_range`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_index_range information.

   * - ``item_to_monitor_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_namespace_idx information.

   * - ``item_to_monitor_name`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The item_to_monitor_name information.

   * - ``monitoring_mode`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_mode information.

   * - ``monitoring_parameters_client_handle`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_client_handle information.

   * - ``monitoring_parameters_sampling_interval`` (number - double)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_sampling_interval information.

   * - ``monitoring_parameters_queue_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_queue_size information.

   * - ``monitoring_parameters_discard_oldest`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_discard_oldest information.

   * - ``monitoring_parameters_filter_info_type_id_node_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_filter_info_type_id_node_id_encoding_mask information.

   * - ``monitoring_parameters_filter_info_type_id_node_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_filter_info_type_id_node_id_namespace_idx information.

   * - ``monitoring_parameters_filter_info_type_id_node_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_filter_info_type_id_node_id_numeric information.

   * - ``monitoring_parameters_filter_info_type_id_node_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_filter_info_type_id_node_id_string information.

   * - ``monitoring_parameters_filter_info_type_id_node_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_filter_info_type_id_node_id_guid information.

   * - ``monitoring_parameters_filter_info_type_id_node_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_filter_info_type_id_node_id_opaque information.

   * - ``monitoring_parameters_filter_info_type_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_filter_info_type_id_string information.

   * - ``monitoring_parameters_filter_info_type_id_encoding`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_filter_info_type_id_encoding information.

   * - ``filter_info_details_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The filter_info_details_link_id information.

   * - ``monitoring_parameters_status_code_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_status_code_link_id information.

   * - ``monitored_item_index_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitored_item_index_id information.

   * - ``monitoring_parameters_revised_sampling_interval`` (number - double)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_revised_sampling_interval information.

   * - ``monitoring_parameters_revised_queue_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-monitored-items-types.zeek
     - The monitoring_parameters_revised_queue_size information.
