``enip_list_identity`` field reference
--------------------------------------

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

   * - ``device_type`` (string)
     - The connection's 4-tuple of endpoint addresses/ports.

   * - ``vendor`` (string)
     - 16b use lookup number from description table

   * - ``product_name`` (string)
     - 16b use lookup number from description table

   * - ``serial_number`` (string)
     - variable length based from above

   * - ``product_code`` (integer - count)
     - 32b hex

   * - ``revision`` (number - double)
     - 16b padding

   * - ``status`` (string)
     - 16b revision high and low in hex

   * - ``state`` (string)
     - 16b controller status

   * - ``device_ip`` (string - addr)
     - 8b state of device
