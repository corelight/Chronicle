``known_devices`` field reference
---------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - When the MAC was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - How long the observation lasted within the interval.

   * - ``kuid`` (string)
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - The address associated with the MAC.

   * - ``mac`` (string)
     - Normalized MAC address for the host under consideration.
       https://docs.zeek.org/en/master/scripts/base/utils/addrs.zeek.html#id-normalize_mac

   * - ``vendor_mac`` (string)
     - Vendor name for MAC based on OUI lookup.

   * - ``protocols`` (array[string] - set[string])
     - Protocols that identified the MAC address (e.g. "RADIUS").

   * - ``num_conns`` (integer - count)
     - Number of connections for which the MAC was observed.

   * - ``annotations`` (array[string] - vector of string)
     - (Sorted) annotations identified during the observation interval.

   * - ``last_active_session`` (string)
     - If persistence is enabled, indicates observation interval
       when MAC was last seen.

   * - ``last_active_interval`` (number - interval)
     - If persistence is enabled, time duration in the
       past when MAC was last seen.
