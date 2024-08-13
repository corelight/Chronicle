.. _ref_logs_opcua_binary_get_endpoints_description:

opcua_binary_get_endpoints_description
--------------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
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

   * - ``endpoint_description_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The endpoint_description_link_id information.

   * - ``endpoint_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The endpoint_uri information.

   * - ``application_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The application_uri information.

   * - ``product_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The product_uri information.

   * - ``encoding_mask`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The encoding_mask information.

   * - ``locale`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The locale information.

   * - ``text`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The text information.

   * - ``application_type`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The application_type information.

   * - ``gateway_server_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The gateway_server_uri information.

   * - ``discovery_profile_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The discovery_profile_uri information.

   * - ``discovery_profile_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The discovery_profile_link_id information.

   * - ``cert_size`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The cert_size information.

   * - ``server_cert`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The server_cert information.

   * - ``message_security_mode`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The message_security_mode information.

   * - ``security_policy_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The security_policy_uri information.

   * - ``user_token_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The user_token_link_id information.

   * - ``transport_profile_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The transport_profile_uri information.

   * - ``security_level`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/get-endpoints-types.zeek
     - The security_level information.
