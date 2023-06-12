``s7comm`` field reference
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
     - Time when the command was sent.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``rosctr`` (string)
     - The connection's 4-tuple of endpoint addresses/ports.

   * - ``parameter`` (array[string] - vector of string)
     - the s7 message type

   * - ``item_count`` (integer - count)
     - contains header[(error)class, (error)code], (function)type, (function)mode, (function)group, sub(function), (error)code

   * - ``data_info`` (array[string] - vector of string)
     - number of data entries
