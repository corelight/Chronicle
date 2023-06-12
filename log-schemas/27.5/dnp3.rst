``dnp3`` field reference
------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time of the request.

   * - ``uid`` (string)
     - Unique identifier for the connection.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``fc_request`` (string)
     - The name of the function message in the request.

   * - ``fc_reply`` (string)
     - The name of the function message in the reply.

   * - ``iin`` (integer - count)
     - The response's \"internal indication number\".
