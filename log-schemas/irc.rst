``irc`` field reference
-----------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp when the command was seen.

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

   * - ``nick`` (string)
     - Nickname given for the connection.

   * - ``user`` (string)
     - Username given for the connection.

   * - ``command`` (string)
     - Command given by the client.

   * - ``value`` (string)
     - Value for the command given by the client.

   * - ``addl`` (string)
     - Any additional data for the command.

   * - ``dcc_file_name`` (string)
     - DCC filename requested.

   * - ``dcc_file_size`` (integer - count)
     - Size of the DCC transfer as indicated by the sender.

   * - ``dcc_mime_type`` (string)
     - Sniffed mime type of the file.

   * - ``fuid`` (string)
     - File unique ID.
