.. _ref_logs_http2:

http2
-----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Timestamp for when the event happened.

   * - ``uid`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
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

   * - ``stream_id`` (integer - count)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Unique ID for the stream.

   * - ``method`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Verb used in the HTTP request (GET, POST, HEAD, etc.).

   * - ``host`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Value of the HOST header.

   * - ``uri`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - URI used in the request.

   * - ``referrer`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Value of the "referer" header.  The comment is deliberately
       misspelled like the standard declares, but the name used here
       is "referrer" spelled correctly.

   * - ``version`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Value of the version portion of the request.

   * - ``user_agent`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Value of the User-Agent header from the client.

   * - ``request_body_len`` (integer - count)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Actual uncompressed content size of the data transferred from
       the client.

   * - ``response_body_len`` (integer - count)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Actual uncompressed content size of the data transferred from
       the server.

   * - ``status_code`` (integer - count)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Status code returned by the server.

   * - ``status_msg`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Status message returned by the server.

   * - ``info_code`` (integer - count)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Last seen 1xx informational reply code returned by the server.

   * - ``info_msg`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Last seen 1xx informational reply message returned by the server.

   * - ``encoding`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - A set of indicators of various attributes discovered and
       related to a particular request/response pair.
       Encoding Type.

   * - ``username`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Username if basic-auth is performed for the request.

   * - ``password`` (string)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Password if basic-auth is performed for the request.

   * - ``proxied`` (array[string] - set[string])
     - site/packages/corelight/packages/bro-http2/main.zeek
     - All of the headers that may indicate if the request was proxied.

   * - ``push`` (boolean - bool)
     - site/packages/corelight/packages/bro-http2/main.zeek
     - Whether this was a push transaction
