.. _ref_logs_reporter:

reporter
--------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - The network time at which the reporter event was generated.

   * - ``level`` (string - enum Reporter::Level)
     - base
     - The severity of the reporter message. Levels are INFO for informational
       messages, not needing specific attention; WARNING for warning of a potential
       problem, and ERROR for a non-fatal error that should be addressed, but doesn't
       terminate program execution.

   * - ``message`` (string)
     - base
     - An info/warning/error message that could have either been
       generated from the internal Zeek core or at the scripting-layer.

   * - ``location`` (string)
     - base
     - This is the location in a Zeek script where the message originated.
       Not all reporter messages will have locations in them though.
