``known_remotes`` field reference
---------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time at which remote was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - How long the observations lasted within the interval.

   * - ``kuid`` (string)
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - The remote host address.

   * - ``num_conns`` (integer - count)
     - Number of connections for which remote was observed.

   * - ``annotations`` (array[string] - vector of string)
     - Annotation determined during the interval.
