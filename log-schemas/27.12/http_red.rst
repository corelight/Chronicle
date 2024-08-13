.. _ref_logs_http_red:

http_red
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

   * - ``trans_depth`` (integer - count)
     - base
     - Represents the pipelined depth into the connection of this
       request/response transaction.

   * - ``method`` (string)
     - base
     - Verb used in the HTTP request (GET, POST, HEAD, etc.).

   * - ``host`` (string)
     - base
     - Value of the HOST header.

   * - ``uri`` (string)
     - base
     - URI used in the request.

   * - ``referrer`` (string)
     - base
     - Value of the "referer" header.  The comment is deliberately
       misspelled like the standard declares, but the name used here
       is "referrer", spelled correctly.

   * - ``version`` (string)
     - base
     - Value of the version portion of the reply. If you require
       message-level detail, consider the `http_request` and
       `http_reply` events, which report each message's
       version string.

   * - ``user_agent`` (string)
     - base
     - Value of the User-Agent header from the client.

   * - ``origin`` (string)
     - base
     - Value of the Origin header from the client.

   * - ``request_body_len`` (integer - count)
     - base
     - Actual uncompressed content size of the data transferred from
       the client.

   * - ``response_body_len`` (integer - count)
     - base
     - Actual uncompressed content size of the data transferred from
       the server.

   * - ``status_code`` (integer - count)
     - base
     - Status code returned by the server.

   * - ``status_msg`` (string)
     - base
     - Status message returned by the server.

   * - ``info_code`` (integer - count)
     - base
     - Last seen 1xx informational reply code returned by the server.

   * - ``info_msg`` (string)
     - base
     - Last seen 1xx informational reply message returned by the server.

   * - ``tags`` (array[string] - set[enum HTTP::Tags])
     - base
     - A set of indicators of various attributes discovered and
       related to a particular request/response pair.

   * - ``username`` (string)
     - base
     - Username if basic-auth is performed for the request.

   * - ``password`` (string)
     - base
     - Password if basic-auth is performed for the request.

   * - ``proxied`` (array[string] - set[string])
     - base
     - All of the headers that may indicate if the request was proxied.

   * - ``orig_fuids`` (array[string] - vector of string)
     - base
     - An ordered vector of file unique IDs.
       Limited to `HTTP::max_files_orig` entries.

   * - ``orig_filenames`` (array[string] - vector of string)
     - base
     - An ordered vector of filenames from the client.
       Limited to `HTTP::max_files_orig` entries.

   * - ``orig_mime_types`` (array[string] - vector of string)
     - base
     - An ordered vector of mime types.
       Limited to `HTTP::max_files_orig` entries.

   * - ``resp_fuids`` (array[string] - vector of string)
     - base
     - An ordered vector of file unique IDs.
       Limited to `HTTP::max_files_resp` entries.

   * - ``resp_filenames`` (array[string] - vector of string)
     - base
     - An ordered vector of filenames from the server.
       Limited to `HTTP::max_files_resp` entries.

   * - ``resp_mime_types`` (array[string] - vector of string)
     - base
     - An ordered vector of mime types.
       Limited to `HTTP::max_files_resp` entries.

   * - ``post_body`` (string)
     - site/packages/corelight/packages/log-add-http-post-bodies/main.zeek
     - The post_body information.
