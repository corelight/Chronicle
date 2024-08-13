.. _ref_logs_ldap_search:

ldap_search
-----------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

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

   * - ``proto`` (string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The proto information.

   * - ``message_id`` (integer - int)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The message_id information.

   * - ``scope`` (array[string] - set[string])
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The scope information.

   * - ``deref`` (array[string] - set[string])
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The deref information.

   * - ``base_object`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The base_object information.

   * - ``result_count`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The result_count information.

   * - ``result`` (array[string] - set[string])
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The result information.

   * - ``diagnostic_message`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The diagnostic_message information.

   * - ``filter`` (string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The filter information.

   * - ``attributes`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ldap/main.zeek
     - The attributes information.
