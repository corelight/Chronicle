.. _ref_logs_known_services:

known_services
--------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Time at which service first seen within the observation interval.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - How long the observations lasted within the interval.

   * - ``kuid`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Address for host associated with the service.

   * - ``host_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Vlan for host associated with the service.

   * - ``host_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Inner_vlan for host associated with the service.

   * - ``port_num`` (integer - port)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Associated port.

   * - ``protocol`` (string - enum transport_proto)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Associated transport layer protocol.

   * - ``service`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Same, but as a vector so it can be logged. Only created during logging.

   * - ``software`` (array[string] - set[string])
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Software that offered the service.

   * - ``app`` (array[string] - set[string])
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Apps that offered the service.

   * - ``num_conns_pending`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Number of in-flight connections for which the service was observed.

   * - ``num_conns_complete`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Number of completed connections for which the service was observed.

   * - ``long_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - Annotation determined during the interval.

   * - ``last_active_session`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - If persistence is enabled, the observation interval
       when the service was last seen.

   * - ``last_active_interval`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/services.zeek
     - If persistence is enabled, the time duration in the
       past when the service was last seen.
