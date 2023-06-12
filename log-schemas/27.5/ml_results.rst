``ml_results`` field reference
------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - When the analysis happened.

   * - ``uid`` (string)
     - Associated connection identifier.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``domain`` (string)
     - Domain that was analyzed.

   * - ``path`` (string)
     - The path information.

   * - ``predicted_tag_name`` (string)
     - Name describing a positive detection by an ML model.

   * - ``predicted_probability`` (number - double)
     - Confidence associated with prediction.
