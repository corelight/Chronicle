.. _ref_logs_opcua_binary_create_session_endpoints:

opcua_binary_create_session_endpoints
-------------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

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

   * - ``endpoint_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The endpoint_link_id information.

   * - ``endpoint_url`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The endpoint_url information.

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

   * - ``cert_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The cert_size information.

   * - ``server_cert`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The server_cert information.

   * - ``message_security_mode`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The message_security_mode information.

   * - ``security_policy_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The security_policy_uri information.

   * - ``user_token_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The user_token_link_id information.

   * - ``transport_profile_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The transport_profile_uri information.

   * - ``security_level`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The security_level information.
