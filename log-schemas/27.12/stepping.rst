.. _ref_logs_stepping:

stepping
--------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Start time of first connection.

   * - ``dt`` (number - interval)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Time elapsed until start of second connection.

   * - ``uid1`` (string)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Connection identifier of first connection.

   * - ``uid2`` (string)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Connection identifier of second connection.

   * - ``direct`` (boolean - bool)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Whether this is a direct client1->server1->server2 stepping stone,
       or an indirect client1->server1->...client2->server2 stepping stone.

   * - ``client1_h`` (string - addr)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - First connection client address.

   * - ``client1_p`` (integer - port)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - First connection client port.

   * - ``server1_h`` (string - addr)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - First connection server address.

   * - ``server1_p`` (integer - port)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - First connection server port.

   * - ``client2_h`` (string - addr)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Second connection client address.

   * - ``client2_p`` (integer - port)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Second connection client port.

   * - ``server2_h`` (string - addr)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Second connection server address.

   * - ``server2_p`` (integer - port)
     - site/packages/corelight/packages/stepping-stones/main.zeek
     - Second connection server port.
