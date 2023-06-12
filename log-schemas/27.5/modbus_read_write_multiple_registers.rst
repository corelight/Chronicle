``modbus_read_write_multiple_registers`` field reference
--------------------------------------------------------

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

   * - ``unit_id`` (integer - count)
     - The unit_id information.

   * - ``func`` (string)
     - The func information.

   * - ``network_direction`` (string)
     - The network_direction information.

   * - ``write_start_address`` (integer - count)
     - The write_start_address information.

   * - ``write_registers`` (array[integer] - vector of count)
     - The write_registers information.

   * - ``read_start_address`` (integer - count)
     - The read_start_address information.

   * - ``read_quantity`` (integer - count)
     - The read_quantity information.

   * - ``read_registers`` (array[integer] - vector of count)
     - The read_registers information.
