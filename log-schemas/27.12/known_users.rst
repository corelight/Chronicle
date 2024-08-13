.. _ref_logs_known_users:

known_users
-----------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - When user name first seen within the observation interval.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - How long the observations lasted within the interval.

   * - ``kuid`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Address for host for which user name was observed.
       `host_ip` corresponds to `c$id$orig_h` for 3rd party authentication protocols,
       while it is set to `c$id$resp_h` for remote login protocols.

   * - ``host_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Vlan for host for which user name was observed.

   * - ``host_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Inner_vlan for host for which user name was observed.

   * - ``remote_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Peer address for host_ip for connection on which user name was observed.
       Peer will be local or remote depending on the tracking option.

   * - ``remote_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Vlan for remote host.

   * - ``remote_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Inner_vlan for remote host.

   * - ``user`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - User name observed.

   * - ``protocol`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Protocols for which user name was observed.

   * - ``num_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Number of connections for which user name was observed.

   * - ``long_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - Annotation determined during the interval.

   * - ``last_active_session`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - If persistence is enabled, the observation interval
       when the user name was last seen.

   * - ``last_active_interval`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/users.zeek
     - If persistence is enabled, the time duration in the
       past when the user name was last seen.
