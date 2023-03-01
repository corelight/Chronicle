sip
---
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp for when the request happened.

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

   * - ``trans_depth`` (integer - count)
     - Represents the pipelined depth into the connection of this
       request/response transaction.

   * - ``method`` (string)
     - Verb used in the SIP request (INVITE, REGISTER etc.).

   * - ``uri`` (string)
     - URI used in the request.

   * - ``date`` (string)
     - Contents of the Date: header from the client

   * - ``request_from`` (string)
     - Contents of the request From: header
       Note: The tag= value that's usually appended to the sender
       is stripped off and not logged.

   * - ``request_to`` (string)
     - Contents of the To: header

   * - ``response_from`` (string)
     - Contents of the response From: header
       Note: The ``tag=`` value that's usually appended to the sender
       is stripped off and not logged.

   * - ``response_to`` (string)
     - Contents of the response To: header

   * - ``reply_to`` (string)
     - Contents of the Reply-To: header

   * - ``call_id`` (string)
     - Contents of the Call-ID: header from the client

   * - ``seq`` (string)
     - Contents of the CSeq: header from the client

   * - ``subject`` (string)
     - Contents of the Subject: header from the client

   * - ``request_path`` (array[string] - vector of string)
     - The client message transmission path, as extracted from the headers.

   * - ``response_path`` (array[string] - vector of string)
     - The server message transmission path, as extracted from the headers.

   * - ``user_agent`` (string)
     - Contents of the User-Agent: header from the client

   * - ``status_code`` (integer - count)
     - Status code returned by the server.

   * - ``status_msg`` (string)
     - Status message returned by the server.

   * - ``warning`` (string)
     - Contents of the Warning: header

   * - ``request_body_len`` (integer - count)
     - Contents of the Content-Length: header from the client

   * - ``response_body_len`` (integer - count)
     - Contents of the Content-Length: header from the server

   * - ``content_type`` (string)
     - Contents of the Content-Type: header from the server
