.. _ref_logs_known_domains:

known_domains
-------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - When the domain was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - How long the observation lasted within the interval.

   * - ``kuid`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Address for host for which domain was observed.

   * - ``host_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Vlan for host for which domain was observed.

   * - ``host_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Inner_vlan for host for which domain was observed.

   * - ``domain`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Name observed.

   * - ``protocols`` (array[string] - set[string])
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Protocols for which name was observed.

   * - ``num_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Number of connections for which domain was observed.

   * - ``long_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - Annotations determined during the observation interval.

   * - ``last_active_session`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - If persistence is enabled, indicates the observation interval
       when the host was last seen.

   * - ``last_active_interval`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/domains.zeek
     - If persistence is enabled, indicates the time duration
       when the host was last seen.
