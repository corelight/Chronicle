.. _ref_logs_sip:

sip
---
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Timestamp for when the request happened.

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

   * - ``trans_depth`` (integer - count)
     - base
     - Represents the pipelined depth into the connection of this
       request/response transaction.

   * - ``method`` (string)
     - base
     - Verb used in the SIP request (INVITE, REGISTER etc.).

   * - ``uri`` (string)
     - base
     - URI used in the request.

   * - ``date`` (string)
     - base
     - Contents of the Date: header from the client

   * - ``request_from`` (string)
     - base
     - Contents of the request From: header
       Note: The tag= value that's usually appended to the sender
       is stripped off and not logged.

   * - ``request_to`` (string)
     - base
     - Contents of the To: header

   * - ``response_from`` (string)
     - base
     - Contents of the response From: header
       Note: The ``tag=`` value that's usually appended to the sender
       is stripped off and not logged.

   * - ``response_to`` (string)
     - base
     - Contents of the response To: header

   * - ``reply_to`` (string)
     - base
     - Contents of the Reply-To: header

   * - ``call_id`` (string)
     - base
     - Contents of the Call-ID: header from the client

   * - ``seq`` (string)
     - base
     - Contents of the CSeq: header from the client

   * - ``subject`` (string)
     - base
     - Contents of the Subject: header from the client

   * - ``request_path`` (array[string] - vector of string)
     - base
     - The client message transmission path, as extracted from the headers.

   * - ``response_path`` (array[string] - vector of string)
     - base
     - The server message transmission path, as extracted from the headers.

   * - ``user_agent`` (string)
     - base
     - Contents of the User-Agent: header from the client

   * - ``status_code`` (integer - count)
     - base
     - Status code returned by the server.

   * - ``status_msg`` (string)
     - base
     - Status message returned by the server.

   * - ``warning`` (string)
     - base
     - Contents of the Warning: header

   * - ``request_body_len`` (integer - count)
     - base
     - Contents of the Content-Length: header from the client

   * - ``response_body_len`` (integer - count)
     - base
     - Contents of the Content-Length: header from the server

   * - ``content_type`` (string)
     - base
     - Contents of the Content-Type: header from the server
