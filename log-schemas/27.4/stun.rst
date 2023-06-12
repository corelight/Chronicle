``stun`` field reference
------------------------

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

   * - ``proto`` (string - enum)
     - The protocol

   * - ``is_orig`` (boolean - bool)
     - The is_orig information.

   * - ``trans_id`` (string)
     - The transaction ID

   * - ``method`` (string)
     - The STUN method

   * - ``class`` (string)
     - The STUN class

   * - ``attr_types`` (array[string] - vector of string)
     - The attribute type

   * - ``attr_vals`` (array[string] - vector of string)
     - The attribute value
