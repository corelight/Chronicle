``bacnet`` field reference
--------------------------

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

   * - ``bvlc_function`` (string)
     - The connection's 4-tuple of endpoint addresses/ports.

   * - ``bvlc_len`` (integer - count)
     - The bvlc_len information.

   * - ``apdu_type`` (string)
     - The apdu_type information.

   * - ``service_choice`` (string)
     - The service_choice information.

   * - ``data`` (array[string] - vector of string)
     - The data information.
