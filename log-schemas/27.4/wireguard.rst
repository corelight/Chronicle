``wireguard`` field reference
-----------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The ts information.

   * - ``uid`` (string)
     - The uid information.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``established`` (boolean - bool)
     - The established information.

   * - ``initiations`` (integer - count)
     - Number of handshake initiation packets encountered during the connection

   * - ``responses`` (integer - count)
     - Number of handshake response packets we have encountered during the connection
