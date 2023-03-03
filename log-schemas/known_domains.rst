``known_domains`` field reference
---------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - When the domain was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - How long the observation lasted within the interval.

   * - ``kuid`` (string)
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - Address for which domain was observed.

   * - ``domain`` (string)
     - Name observed.

   * - ``protocols`` (array[string] - set[string])
     - Protocols for which name was observed.

   * - ``num_conns`` (integer - count)
     - Number of connections for which domain was observed.

   * - ``annotations`` (array[string] - vector of string)
     - Annotations determined during the observation interval.

   * - ``last_active_session`` (string)
     - If persistence is enabled, indicates the observation interval
       when the host was last seen.

   * - ``last_active_interval`` (number - interval)
     - If persistence is enabled, indicates the time duration
       when the host was last seen.
