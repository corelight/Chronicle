.. _ref_logs_kerberos:

kerberos
--------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Timestamp for when the event happened.

   * - ``uid`` (string)
     - base
     - Unique ID for the connection.

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

   * - ``request_type`` (string)
     - base
     - Request type - Authentication Service ("AS") or
       Ticket Granting Service ("TGS")

   * - ``client`` (string)
     - base
     - Client

   * - ``service`` (string)
     - base
     - Service

   * - ``success`` (boolean - bool)
     - base
     - Request result

   * - ``error_msg`` (string)
     - base
     - Error message

   * - ``from`` (time)
     - base
     - Ticket valid from

   * - ``till`` (time)
     - base
     - Ticket valid till

   * - ``cipher`` (string)
     - base
     - Ticket encryption type

   * - ``forwardable`` (boolean - bool)
     - base
     - Forwardable ticket requested

   * - ``renewable`` (boolean - bool)
     - base
     - Renewable ticket requested

   * - ``client_cert_subject`` (string)
     - base
     - Subject of client certificate, if any

   * - ``client_cert_fuid`` (string)
     - base
     - File unique ID of client cert, if any

   * - ``server_cert_subject`` (string)
     - base
     - Subject of server certificate, if any

   * - ``server_cert_fuid`` (string)
     - base
     - File unique ID of server cert, if any
