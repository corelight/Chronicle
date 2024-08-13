.. _ref_logs_known_names:

known_names
-----------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - When the name was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - How long the observations lasted within the interval.

   * - ``kuid`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - Address for host at which the name was observed.

   * - ``host_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - Vlan for host at which the name was observed.

   * - ``host_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - Inner_vlan for host at which the name was observed.

   * - ``hostname`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - The host name observed.

   * - ``protocols`` (array[string] - set[string])
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - Protocols for which the host name was observed.

   * - ``num_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - Number of connections for which the host name was observed.

   * - ``long_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - Annotations determined during the observation interval.

   * - ``last_active_session`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - If persistence is enabled, the observation interval
       when the host name was last seen.

   * - ``last_active_interval`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/names.zeek
     - If persistence is enabled, the time duration in the
       past when the host name was last seen.
