``icmp_specific_tunnels`` field reference
-----------------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The ts information.

   * - ``start_time`` (time)
     - The start_time information.

   * - ``duration`` (number - interval)
     - The duration information.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``tunnel`` (string)
     - The tunnel information.

   * - ``seq`` (integer - count)
     - The seq information.

   * - ``icmp_id`` (integer - count)
     - The icmp_id information.

   * - ``payload`` (string)
     - The payload information.
