``known_names`` field reference
-------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - When the name was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - How long the observations lasted within the interval.

   * - ``kuid`` (string)
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - Address at which the name was observed.

   * - ``hostname`` (string)
     - The host name observed.

   * - ``protocols`` (array[string] - set[string])
     - Protocols for which the host name was observed.

   * - ``num_conns`` (integer - count)
     - Number of connections for which the host name was observed.

   * - ``annotations`` (array[string] - vector of string)
     - Annotations determined during the observation interval.

   * - ``last_active_session`` (string)
     - If persistence is enabled, the observation interval
       when the host name was last seen.

   * - ``last_active_interval`` (number - interval)
     - If persistence is enabled, the time duration in the
       past when the host name was last seen.
