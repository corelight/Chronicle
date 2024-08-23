.. _ref_logs_known_devices:

known_devices
-------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - When the MAC was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - How long the observation lasted within the interval.

   * - ``kuid`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Address for host associated with the MAC.

   * - ``host_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Vlan for host associated with the MAC.

   * - ``host_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Inner_vlan for host associated with the MAC.

   * - ``mac`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Normalized MAC address for the host under consideration.
       https://docs.zeek.org/en/master/scripts/base/utils/addrs.zeek.html#id-normalize_mac

   * - ``vendor_mac`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Vendor name for MAC based on OUI lookup.

   * - ``protocols`` (array[string] - set[string])
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Protocols that identified the MAC address (e.g. "RADIUS").

   * - ``num_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Number of connections for which the MAC was observed.

   * - ``long_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - (Sorted) annotations identified during the observation interval.

   * - ``last_active_session`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - If persistence is enabled, indicates observation interval
       when MAC was last seen.

   * - ``last_active_interval`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/devices.zeek
     - If persistence is enabled, time duration in the
       past when MAC was last seen.
