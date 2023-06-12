``known_certs`` field reference
-------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time at which the certificate was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - How long the observation lasted within the interval.

   * - ``kuid`` (string)
     - A unique identifier for the observation interval.

   * - ``host_ip`` (string - addr)
     - The address that offered the certificate.

   * - ``hash`` (string)
     - The SHA1 hash of the certificate under consideration.

   * - ``port_num`` (integer - port)
     - If the certificate was handed out by a server, the
       port that the server was listening on.

   * - ``protocol`` (string - enum)
     - The transport layer protocol of the connection.

   * - ``serial`` (string)
     - Serial number for the certificate.

   * - ``subject`` (string)
     - Certificate subject.

   * - ``issuer_subject`` (string)
     - Certificate issuer subject.

   * - ``num_conns`` (integer - count)
     - The number of connections for which we observed the certificate.

   * - ``annotations`` (array[string] - vector of string)
     - The type of annotation determined during the interval.

   * - ``last_active_session`` (string)
     - If persistence is enabled, the observation interval
       when the certificate was last seen.

   * - ``last_active_interval`` (number - interval)
     - If persistence is enabled, the time duration in the
       past when the certificate was last seen.
