ldap
----
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

   * - ``message_id`` (integer - int)
     - The message_id information.

   * - ``version`` (integer - int)
     - The version information.

   * - ``opcode`` (array[string] - set[string])
     - The opcode information.

   * - ``result`` (array[string] - set[string])
     - The result information.

   * - ``diagnostic_message`` (array[string] - vector of string)
     - The diagnostic_message information.

   * - ``object`` (array[string] - vector of string)
     - The object information.

   * - ``argument`` (array[string] - vector of string)
     - The argument information.
