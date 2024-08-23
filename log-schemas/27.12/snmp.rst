.. _ref_logs_snmp:

snmp
----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Timestamp of first packet belonging to the SNMP session.

   * - ``uid`` (string)
     - base
     - The unique ID for the connection.

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

   * - ``duration`` (number - interval)
     - base
     - The amount of time between the first packet belonging to
       the SNMP session and the latest one seen.

   * - ``version`` (string)
     - base
     - The version of SNMP being used.

   * - ``community`` (string)
     - base
     - The community string of the first SNMP packet associated with
       the session.  This is used as part of SNMP's (v1 and v2c)
       administrative/security framework.  See :rfc:`1157` or :rfc:`1901`.

   * - ``get_requests`` (integer - count)
     - base
     - The number of variable bindings in GetRequest/GetNextRequest PDUs
       seen for the session.

   * - ``get_bulk_requests`` (integer - count)
     - base
     - The number of variable bindings in GetBulkRequest PDUs seen for
       the session.

   * - ``get_responses`` (integer - count)
     - base
     - The number of variable bindings in GetResponse/Response PDUs seen
       for the session.

   * - ``set_requests`` (integer - count)
     - base
     - The number of variable bindings in SetRequest PDUs seen for
       the session.

   * - ``display_string`` (string)
     - base
     - A system description of the SNMP responder endpoint.

   * - ``up_since`` (time)
     - base
     - The time at which the SNMP responder endpoint claims it's been
       up since.
