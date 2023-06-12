``dpd`` field reference
-----------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp for when protocol analysis failed.

   * - ``uid`` (string)
     - Connection unique ID.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``proto`` (string - enum)
     - Transport protocol for the violation.

   * - ``analyzer`` (string)
     - The analyzer that generated the violation.

   * - ``failure_reason`` (string)
     - The textual reason for the analysis failure.
