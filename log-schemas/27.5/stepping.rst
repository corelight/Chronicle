``stepping`` field reference
----------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Start time of first connection.

   * - ``dt`` (number - interval)
     - Time elapsed until start of second connection.

   * - ``uid1`` (string)
     - Connection identifier of first connection.

   * - ``uid2`` (string)
     - Connection identifier of second connection.

   * - ``direct`` (boolean - bool)
     - Whether this is a direct client1->server1->server2 stepping stone,
       or an indirect client1->server1->...client2->server2 stepping stone.

   * - ``client1_h`` (string - addr)
     - First connection client address.

   * - ``client1_p`` (integer - port)
     - First connection client port.

   * - ``server1_h`` (string - addr)
     - First connection server address.

   * - ``server1_p`` (integer - port)
     - First connection server port.

   * - ``client2_h`` (string - addr)
     - Second connection client address.

   * - ``client2_p`` (integer - port)
     - Second connection client port.

   * - ``server2_h`` (string - addr)
     - Second connection server address.

   * - ``server2_p`` (integer - port)
     - Second connection server port.
