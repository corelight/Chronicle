``known_services`` field reference
----------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time at which service first seen within the observation interval.

   * - ``duration`` (number - interval)
     - How long the observations lasted within the interval.

   * - ``kuid`` (string)
     - Unique identifier for the interval.

   * - ``host_ip`` (string - addr)
     - Associated address.

   * - ``port_num`` (integer - port)
     - Associated port.

   * - ``protocol`` (string - enum)
     - Associated transport layer protocol.

   * - ``service`` (array[string] - vector of string)
     - Same, but as a vector so it can be logged. Only created during logging.

   * - ``software`` (array[string] - set[string])
     - Software that offered the service.

   * - ``app`` (array[string] - set[string])
     - Apps that offered the service.

   * - ``num_conns`` (integer - count)
     - Number of connections for which the service was observed.

   * - ``annotations`` (array[string] - vector of string)
     - Annotation determined during the interval.

   * - ``last_active_session`` (string)
     - If persistence is enabled, the observation interval
       when the service was last seen.

   * - ``last_active_interval`` (number - interval)
     - If persistence is enabled, the time duration in the
       past when the service was last seen.
