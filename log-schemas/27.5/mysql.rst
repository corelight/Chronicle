``mysql`` field reference
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

   * - ``cmd`` (string)
     - The command that was issued

   * - ``arg`` (string)
     - The argument issued to the command

   * - ``success`` (boolean - bool)
     - Did the server tell us that the command succeeded?

   * - ``rows`` (integer - count)
     - The number of affected rows, if any

   * - ``response`` (string)
     - Server message, if any
