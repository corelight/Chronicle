``tunnel`` field reference
--------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time at which some tunnel activity occurred.

   * - ``uid`` (string)
     - The unique identifier for the tunnel, which may correspond
       to a `connection`'s *uid* field for non-IP-in-IP tunnels.
       This is optional because there could be numerous connections
       for payload proxies like SOCKS but we should treat it as a
       single tunnel.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``tunnel_type`` (string - enum)
     - The type of tunnel.

   * - ``action`` (string - enum)
     - The type of activity that occurred.
