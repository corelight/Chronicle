``kerberos`` field reference
----------------------------

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

   * - ``request_type`` (string)
     - Request type - Authentication Service ("AS") or
       Ticket Granting Service ("TGS")

   * - ``client`` (string)
     - Client

   * - ``service`` (string)
     - Service

   * - ``success`` (boolean - bool)
     - Request result

   * - ``error_msg`` (string)
     - Error message

   * - ``from`` (time)
     - Ticket valid from

   * - ``till`` (time)
     - Ticket valid till

   * - ``cipher`` (string)
     - Ticket encryption type

   * - ``forwardable`` (boolean - bool)
     - Forwardable ticket requested

   * - ``renewable`` (boolean - bool)
     - Renewable ticket requested

   * - ``client_cert_subject`` (string)
     - Subject of client certificate, if any

   * - ``client_cert_fuid`` (string)
     - File unique ID of client cert, if any

   * - ``server_cert_subject`` (string)
     - Subject of server certificate, if any

   * - ``server_cert_fuid`` (string)
     - File unique ID of server cert, if any
