``known_users`` field reference
-------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - When user name first seen within the observation interval.

   * - ``duration`` (number - interval)
     - How long the observations lasted within the interval.

   * - ``kuid`` (string)
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - Address for which user name was observed.
       `host_ip` corresponds to `c$id$orig_h` for 3rd party authentication protocols,
       while it is set to `c$id$resp_h` for remote login protocols.

   * - ``remote_ip`` (string - addr)
     - Peer address for host_ip for connection on which user name was observed.
       Peer will be local or remote depending on the tracking option.

   * - ``user`` (string)
     - User name observed.

   * - ``protocol`` (string)
     - Protocols for which user name was observed.

   * - ``num_conns`` (integer - count)
     - Number of connections for which user name was observed.

   * - ``annotations`` (array[string] - vector of string)
     - Annotation determined during the interval.

   * - ``last_active_session`` (string)
     - If persistence is enabled, the observation interval
       when the user name was last seen.

   * - ``last_active_interval`` (number - interval)
     - If persistence is enabled, the time duration in the
       past when the user name was last seen.
