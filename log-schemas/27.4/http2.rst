``http2`` field reference
-------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp for when the event happened.

   * - ``uid`` (string)
     - Unique ID for the connection.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``stream_id`` (integer - count)
     - Unique ID for the stream.

   * - ``method`` (string)
     - Verb used in the HTTP request (GET, POST, HEAD, etc.).

   * - ``host`` (string)
     - Value of the HOST header.

   * - ``uri`` (string)
     - URI used in the request.

   * - ``referrer`` (string)
     - Value of the \""referer\"" header.  The comment is deliberately
       misspelled like the standard declares, but the name used here
       is \""referrer\"" spelled correctly.

   * - ``version`` (string)
     - Value of the version portion of the request.

   * - ``user_agent`` (string)
     - Value of the User-Agent header from the client.

   * - ``request_body_len`` (integer - count)
     - Actual uncompressed content size of the data transferred from
       the client.

   * - ``response_body_len`` (integer - count)
     - Actual uncompressed content size of the data transferred from
       the server.

   * - ``status_code`` (integer - count)
     - Status code returned by the server.

   * - ``status_msg`` (string)
     - Status message returned by the server.

   * - ``info_code`` (integer - count)
     - Last seen 1xx informational reply code returned by the server.

   * - ``info_msg`` (string)
     - Last seen 1xx informational reply message returned by the server.

   * - ``encoding`` (string)
     - A set of indicators of various attributes discovered and
       related to a particular request/response pair.
       Encoding Type.

   * - ``username`` (string)
     - Username if basic-auth is performed for the request.

   * - ``password`` (string)
     - Password if basic-auth is performed for the request.

   * - ``proxied`` (array[string] - set[string])
     - All of the headers that may indicate if the request was proxied.

   * - ``push`` (boolean - bool)
     - Whether this was a push transaction
