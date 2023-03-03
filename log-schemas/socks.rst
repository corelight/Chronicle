``socks`` field reference
-------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time when the proxy connection was first detected.

   * - ``uid`` (string)
     - Unique ID for the tunnel - may correspond to connection uid
       or be non-existent.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``version`` (integer - count)
     - Protocol version of SOCKS.

   * - ``user`` (string)
     - Username used to request a login to the proxy.

   * - ``password`` (string)
     - Password used to request a login to the proxy.

   * - ``status`` (string)
     - Server status for the attempt at using the proxy.

   * - ``request.host`` (string - addr)
     - The request.host information.

   * - ``request.name`` (string)
     - The request.name information.

   * - ``request_p`` (integer - port)
     - Client requested port.

   * - ``bound.host`` (string - addr)
     - The bound.host information.

   * - ``bound.name`` (string)
     - The bound.name information.

   * - ``bound_p`` (integer - port)
     - Server bound port.
