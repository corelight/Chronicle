.. _ref_logs_opcua_binary_create_session_user_token:

opcua_binary_create_session_user_token
--------------------------------------
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

   * - ``user_token_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The user_token_link_id information.

   * - ``user_token_policy_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The user_token_policy_id information.

   * - ``user_token_type`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The user_token_type information.

   * - ``user_token_issued_type`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The user_token_issued_type information.

   * - ``user_token_endpoint_url`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The user_token_endpoint_url information.

   * - ``user_token_sec_policy_uri`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-session-types.zeek
     - The user_token_sec_policy_uri information.
