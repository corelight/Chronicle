``known_hosts`` field reference
-------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time when host first seen within the observation interval.

   * - ``duration`` (number - interval)
     - How long the observation lasted within the interval.

   * - ``kuid`` (string)
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - Address for which connections are observed in the interval.

   * - ``conns_opened`` (integer - count)
     - Count of connections opened by host during the interval.

   * - ``conns_closed`` (integer - count)
     - Count of connections closed by host.

   * - ``conns_pending`` (integer - count)
     - Count of pending connections. Such connections were
       opened in an earlier interval, but not yet closed.

   * - ``long_conns`` (integer - count)
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - Annotations determined during the interval.

   * - ``last_active_session`` (string)
     - If persistence is enabled, the observation interval
       when the host was last seen.

   * - ``last_active_interval`` (number - interval)
     - If persistence is enabled, the time duration in the
       past when the host was last seen.
