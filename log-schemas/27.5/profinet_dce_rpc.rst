``profinet_dce_rpc`` field reference
------------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The ts information.

   * - ``uid`` (string)
     - Timestamp for when the event happened.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``version`` (integer - count)
     - The connection's 4-tuple of endpoint addresses/ports.

   * - ``packet_type`` (integer - count)
     - The packet_type information.

   * - ``object_uuid`` (string)
     - The object_uuid information.

   * - ``interface_uuid`` (string)
     - The interface_uuid information.

   * - ``activity_uuid`` (string)
     - The activity_uuid information.

   * - ``server_boot_time`` (integer - count)
     - The server_boot_time information.

   * - ``operation`` (string)
     - The operation information.
