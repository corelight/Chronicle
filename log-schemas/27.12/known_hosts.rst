.. _ref_logs_known_hosts:

known_hosts
-----------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Time when host first seen within the observation interval.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - How long the observation lasted within the interval.

   * - ``kuid`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Address for host for which connections are observed in the interval.

   * - ``host_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Vlan for host for which connections are observed in the interval.

   * - ``host_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Inner_vlan for host for which connections are observed in the interval.

   * - ``conns_opened`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Count of connections opened by host during the interval.

   * - ``conns_closed`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Count of connections closed by host.

   * - ``conns_pending`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Count of pending connections. Such connections were
       opened in an earlier interval, but not yet closed.

   * - ``long_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - Annotations determined during the interval.

   * - ``last_active_session`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - If persistence is enabled, the observation interval
       when the host was last seen.

   * - ``last_active_interval`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/hosts.zeek
     - If persistence is enabled, the time duration in the
       past when the host was last seen.

   * - ``ep.desc`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/main.zeek
     - The description of the endpoint.

   * - ``ep.status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/main.zeek
     - The status of the endpoint host.

   * - ``ep.uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/main.zeek
     - The unique identifier, assigned by the source, of the endpoint host.

   * - ``ep.cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/main.zeek
     - The customer ID the host belongs to.

   * - ``ep.os_version`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/main.zeek
     - The Operating System version of the endpoint host.

   * - ``ep.source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/main.zeek
     - The source of the endpoint information.

   * - ``ep.criticality`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/main.zeek
     - The criticality of the endpoint host.
