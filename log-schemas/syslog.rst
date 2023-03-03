``syslog`` field reference
--------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp when the syslog message was seen.

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

   * - ``proto`` (string - enum)
     - Protocol over which the message was seen.

   * - ``facility`` (string)
     - Syslog facility for the message.

   * - ``severity`` (string)
     - Syslog severity for the message.

   * - ``message`` (string)
     - The plain text message.
