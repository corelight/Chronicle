.. _ref_logs_known_remotes:

known_remotes
-------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - Time at which remote was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - How long the observations lasted within the interval.

   * - ``kuid`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - Remote host address.

   * - ``host_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - Vlan for remote host.

   * - ``host_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - Inner_vlan for remote host.

   * - ``num_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - Number of connections for which remote was observed.

   * - ``long_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/remotes.zeek
     - Annotation determined during the interval.
