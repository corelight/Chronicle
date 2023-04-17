``http2`` UDM Map Reference
------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 1 3

   * - Field (Type)
     - UDM Field (Type)
     - Description

   * -
     - ``metadata_vendor_name``
     - replace with 'Corelight'

   * -
     - ``metadata_event_type``
     - replace with 'NETWORK_HTTP'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * -
     - ``about.file.mime_type``
     - replace with '%{resp_mime_types.0}'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - This is the time of the first packet.

   * - ``uid`` (string)
     - ``metadata_product_log_id``
     - A unique identifier of the connection.

   * - ``id.orig_h`` (string - addr)
     - ``principal_ip``
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - ``principal_port`` (string)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - ``target_ip``
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - ``target_port`` (string)
     - The responder's port number.

   * - ``stream_id`` (integer - count)
     -
     - Unique ID for the stream.

   * - ``method`` (string)
     - ``network_http_method``
     - Verb used in the HTTP request (GET, POST, HEAD, etc.).

   * - ``host`` (string)
     - ``target_hostname``
     - Value of the HOST header.

   * - ``uri`` (string)
     - ``target_url``
     - URI used in the request.

   * - ``referrer`` (string)
     -
     - Value of the \""referer\"" header.  The comment is deliberately
       misspelled like the standard declares, but the name used here
       is \""referrer\"", spelled correctly.

   * - ``version`` (string)
     -
     - Value of the version portion of the reply. If you require
       message-level detail, consider the `http_request` and
       `http_reply` events, which report each message's
       version string.

   * - ``user_agent`` (string)
     - ``network_http_user_agent``
     - Value of the User-Agent header from the client.

   * - ``request_body_len`` (integer - count)
     - ``network_sent_bytes`` (uinteger)
     - Actual uncompressed content size of the data transferred from
       the client.

   * - ``response_body_len`` (integer - count)
     - ``network_received_bytes`` (uinteger)
     - Actual uncompressed content size of the data transferred from
       the server.

   * - ``status_code`` (integer - count)
     - ``network_http_response_code`` (integer)
     - Status code returned by the server.

   * - ``status_msg`` (string)
     -
     - Status message returned by the server.

   * - ``info_code`` (integer - count)
     -
     - Last seen 1xx informational reply code returned by the server.

   * - ``info_msg`` (string)
     -
     - Last seen 1xx informational reply message returned by the server.

   * - ``encoding`` (string)
     -
     - A set of indicators of various attributes discovered and
       related to a particular request/response pair.
       Encoding Type.

   * - ``username`` (string)
     -
     - Username if basic-auth is performed for the request.

   * - ``password`` (string)
     -
     - Password if basic-auth is performed for the request.

   * - ``proxied`` (array[string] - set[string])
     -
     - All of the headers that may indicate if the request was proxied.

   * - ``push`` (boolean - bool)
     -
     - Whether this was a push transaction
