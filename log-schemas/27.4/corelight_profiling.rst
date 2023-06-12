``corelight_profiling`` field reference
---------------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The ts information.

   * - ``node`` (string)
     - The node information.

   * - ``prof.core_stack`` (string)
     - The prof.core_stack information.

   * - ``prof.script_stack`` (string)
     - Execution state is not always within the script interpreter
       so there won't always be a script stack which forces this to be optional

   * - ``prof.sched_wait_ns`` (integer - count)
     - The prof.sched_wait_ns information.
