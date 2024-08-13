.. _ref_logs_opcua_binary_opensecure_channel:

opcua_binary_opensecure_channel
-------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
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
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The opcua_link_id information.

   * - ``client_proto_ver`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The client_proto_ver information.

   * - ``sec_token_request_type`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The sec_token_request_type information.

   * - ``message_security_mode`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The message_security_mode information.

   * - ``client_nonce`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The client_nonce information.

   * - ``req_lifetime`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The req_lifetime information.

   * - ``server_proto_ver`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The server_proto_ver information.

   * - ``sec_token_sec_channel_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The sec_token_sec_channel_id information.

   * - ``sec_token_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The sec_token_id information.

   * - ``sec_token_created_at`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The sec_token_created_at information.

   * - ``sec_token_revised_time`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The sec_token_revised_time information.

   * - ``server_nonce`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/secure-channel-types.zeek
     - The server_nonce information.
