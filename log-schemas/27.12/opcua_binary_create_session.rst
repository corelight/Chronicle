.. _ref_logs_opcua_binary_create_session:

opcua_binary_create_session
---------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
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
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The opcua_link_id information.

   * - ``application_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The application_uri information.

   * - ``product_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The product_uri information.

   * - ``encoding_mask`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The encoding_mask information.

   * - ``locale`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The locale information.

   * - ``text`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The text information.

   * - ``application_type`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The application_type information.

   * - ``gateway_server_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The gateway_server_uri information.

   * - ``discovery_profile_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The discovery_profile_uri information.

   * - ``discovery_profile_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The discovery_profile_link_id information.

   * - ``server_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The server_uri information.

   * - ``endpoint_url`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The endpoint_url information.

   * - ``session_name`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The session_name information.

   * - ``client_nonce`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The client_nonce information.

   * - ``client_cert_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The client_cert_size information.

   * - ``client_cert`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The client_cert information.

   * - ``req_session_timeout`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The req_session_timeout information.

   * - ``max_res_msg_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The max_res_msg_size information.

   * - ``session_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The session_id_encoding_mask information.

   * - ``session_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The session_id_namespace_idx information.

   * - ``session_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The session_id_numeric information.

   * - ``session_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The session_id_string information.

   * - ``session_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The session_id_guid information.

   * - ``session_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The session_id_opaque information.

   * - ``auth_token_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The auth_token_encoding_mask information.

   * - ``auth_token_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The auth_token_namespace_idx information.

   * - ``auth_token_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The auth_token_numeric information.

   * - ``auth_token_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The auth_token_string information.

   * - ``auth_token_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The auth_token_guid information.

   * - ``auth_token_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The auth_token_opaque information.

   * - ``revised_session_timeout`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The revised_session_timeout information.

   * - ``server_nonce`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The server_nonce information.

   * - ``server_cert_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The server_cert_size information.

   * - ``server_cert`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The server_cert information.

   * - ``endpoint_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The endpoint_link_id information.

   * - ``algorithm`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The algorithm information.

   * - ``signature`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The signature information.

   * - ``max_req_msg_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The max_req_msg_size information.
