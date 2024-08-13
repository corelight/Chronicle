.. _ref_logs_opcua_binary:

opcua_binary
------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
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
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The opcua_link_id information.

   * - ``msg_type`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The msg_type information.

   * - ``is_final`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The is_final information.

   * - ``msg_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The msg_size information.

   * - ``error`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The error information.

   * - ``reason`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The reason information.

   * - ``version`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The version information.

   * - ``rcv_buf_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The rcv_buf_size information.

   * - ``snd_buf_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The snd_buf_size information.

   * - ``max_msg_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The max_msg_size information.

   * - ``max_chunk_cnt`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The max_chunk_cnt information.

   * - ``endpoint_url`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The endpoint_url information.

   * - ``sec_channel_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The sec_channel_id information.

   * - ``sec_policy_uri_len`` (integer - int)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The sec_policy_uri_len information.

   * - ``sec_policy_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The sec_policy_uri information.

   * - ``snd_cert_len`` (integer - int)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The snd_cert_len information.

   * - ``snd_cert`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The snd_cert information.

   * - ``rcv_cert_len`` (integer - int)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The rcv_cert_len information.

   * - ``rcv_cert`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The rcv_cert information.

   * - ``seq_number`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The seq_number information.

   * - ``request_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The request_id information.

   * - ``encoding_mask`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The encoding_mask information.

   * - ``namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The namespace_idx information.

   * - ``identifier`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The identifier information.

   * - ``identifier_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The identifier_str information.

   * - ``req_hdr_node_id_type`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_node_id_type information.

   * - ``req_hdr_node_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_node_id_namespace_idx information.

   * - ``req_hdr_node_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_node_id_numeric information.

   * - ``req_hdr_node_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_node_id_string information.

   * - ``req_hdr_node_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_node_id_guid information.

   * - ``req_hdr_node_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_node_id_opaque information.

   * - ``req_hdr_timestamp`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_timestamp information.

   * - ``req_hdr_request_handle`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_request_handle information.

   * - ``req_hdr_return_diag`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_return_diag information.

   * - ``req_hdr_audit_entry_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_audit_entry_id information.

   * - ``req_hdr_timeout_hint`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_timeout_hint information.

   * - ``req_hdr_add_hdr_type_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_add_hdr_type_id information.

   * - ``req_hdr_add_hdr_enc_mask`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The req_hdr_add_hdr_enc_mask information.

   * - ``res_hdr_timestamp`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The res_hdr_timestamp information.

   * - ``res_hdr_request_handle`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The res_hdr_request_handle information.

   * - ``status_code_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The status_code_link_id information.

   * - ``res_hdr_service_diag_encoding`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The res_hdr_service_diag_encoding information.

   * - ``res_hdr_add_hdr_type_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The res_hdr_add_hdr_type_id information.

   * - ``res_hdr_add_hdr_enc_mask`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/types.zeek
     - The res_hdr_add_hdr_enc_mask information.
