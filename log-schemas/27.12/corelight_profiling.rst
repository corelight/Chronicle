.. _ref_logs_corelight_profiling:

corelight_profiling
-------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - Corelight_Profiling/scripts/Corelight/Profiling/main.zeek
     - The ts information.

   * - ``node`` (string)
     - Corelight_Profiling/scripts/Corelight/Profiling/main.zeek
     - The node information.

   * - ``prof.core_stack`` (string)
     - Corelight_Profiling/scripts/Corelight/Profiling/main.zeek
     - The prof.core_stack information.

   * - ``prof.script_stack`` (string)
     - Corelight_Profiling/scripts/Corelight/Profiling/main.zeek
     - Execution state is not always within the script interpreter
       so there won't always be a script stack which forces this to be optional

   * - ``prof.sched_wait_ns`` (integer - count)
     - Corelight_Profiling/scripts/Corelight/Profiling/main.zeek
     - The prof.sched_wait_ns information.
