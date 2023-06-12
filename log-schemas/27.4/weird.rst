``weird`` field reference
-------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The time when the weird occurred.

   * - ``uid`` (string)
     - If a connection is associated with this weird, this will be
       the connection's unique ID.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``name`` (string)
     - The name of the weird that occurred.

   * - ``addl`` (string)
     - Additional information accompanying the weird if any.

   * - ``notice`` (boolean - bool)
     - Indicate if this weird was also turned into a notice.

   * - ``source`` (string)
     - The source of the weird. When reported by an analyzer, this
       should be the name of the analyzer.
