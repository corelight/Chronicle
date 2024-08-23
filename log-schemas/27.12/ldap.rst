.. _ref_logs_ldap:

ldap
----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
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

   * - ``proto`` (string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The proto information.

   * - ``message_id`` (integer - int)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The message_id information.

   * - ``version`` (integer - int)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The version information.

   * - ``opcode`` (array[string] - set[string])
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The opcode information.

   * - ``result`` (array[string] - set[string])
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The result information.

   * - ``diagnostic_message`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The diagnostic_message information.

   * - ``object`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The object information.

   * - ``argument`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The argument information.
