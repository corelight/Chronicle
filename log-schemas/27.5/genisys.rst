``genisys`` field reference
---------------------------

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

   * - ``proto`` (string)
     - The proto information.

   * - ``header`` (string)
     - The header information.

   * - ``server`` (integer - count)
     - The server information.

   * - ``direction`` (string)
     - The direction information.

   * - ``crc_transmitted`` (string)
     - The crc_transmitted information.

   * - ``crc_calculated`` (string)
     - The crc_calculated information.

   * - ``payload`` (array[string] - vector of string)
     - The payload information.
