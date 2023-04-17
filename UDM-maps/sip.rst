``sip`` UDM map reference
-------------------------

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
     - replace with 'NETWORK_UNCATEGORIZED'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * -
     - ``metadata_description``
     - replace with '%{method}'

   * -
     - ``network_application_protocol``
     - replace with 'SIP'

   * -
     - ``network_session_id``
     - replace with '%{call_id}'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - Timestamp for when the request happened.

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

   * - ``trans_depth`` (integer - count)
     -
     - Represents the pipelined depth into the connection of this
       request/response transaction.

   * - ``method`` (string)
     - ``metadata_description``
     - Verb used in the SIP request (INVITE, REGISTER etc.).

   * - ``uri`` (string)
     - ``about.url``
     - URI used in the request.

   * - ``date`` (string)
     -
     - Contents of the Date: header from the client

   * - ``request_from`` (string)
     -
     - Contents of the request From: header
       Note: The tag= value that's usually appended to the sender
       is stripped off and not logged.

   * - ``request_to`` (string)
     -
     - Contents of the To: header

   * - ``response_from`` (string)
     -
     - Contents of the response From: header
       Note: The ``tag=`` value that's usually appended to the sender
       is stripped off and not logged.

   * - ``response_to`` (string)
     -
     - Contents of the response To: header

   * - ``reply_to`` (string)
     -
     - Contents of the Reply-To: header

   * - ``call_id`` (string)
     -
     - Contents of the Call-ID: header from the client

   * - ``seq`` (string)
     -
     - Contents of the CSeq: header from the client

   * - ``subject`` (string)
     - ``labels_about_subject.value``
     - Contents of the Subject: header from the client

   * - ``request_path`` (array[string] - vector of string)
     -
     - The client message transmission path, as extracted from the headers.

   * - ``response_path`` (array[string] - vector of string)
     -
     - The server message transmission path, as extracted from the headers.

   * - ``user_agent`` (string)
     -
     - Contents of the User-Agent: header from the client

   * - ``status_code`` (integer - count)
     - ``security_result.summary`` (string)
     - Status code returned by the server.

   * - ``status_msg`` (string)
     - ``security_result.description``
     - Status message returned by the server.

   * - ``warning`` (string)
     -
     - Contents of the Warning: header

   * - ``request_body_len`` (integer - count)
     - ``network_sent_bytes`` (uinteger)
     - Contents of the Content-Length: header from the client

   * - ``response_body_len`` (integer - count)
     - ``network_received_bytes`` (uinteger)
     - Contents of the Content-Length: header from the server

   * - ``content_type`` (string)
     -
     - Contents of the Content-Type: header from the server
