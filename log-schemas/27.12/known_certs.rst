.. _ref_logs_known_certs:

known_certs
-----------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - Time at which the certificate was first seen within the observation interval.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - How long the observation lasted within the interval.

   * - ``kuid`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - A unique identifier for the observation interval.

   * - ``host_ip`` (string - addr)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - Address for host that offered the certificate.

   * - ``host_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - Vlan for host that offered the certificate.

   * - ``host_inner_vlan`` (integer - int)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - Inner_vlan for host that offered the certificate.

   * - ``hash`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - The SHA1 hash of the certificate under consideration.

   * - ``port_num`` (integer - port)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - If the certificate was handed out by a server, the
       port that the server was listening on.

   * - ``protocol`` (string - enum transport_proto)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - The transport layer protocol of the connection.

   * - ``serial`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - Serial number for the certificate.

   * - ``subject`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - Certificate subject.

   * - ``issuer_subject`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - Certificate issuer subject.

   * - ``num_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - The number of connections for which we observed the certificate.

   * - ``long_conns`` (integer - count)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - Count of long connections tracked in the current interval.

   * - ``annotations`` (array[string] - vector of string)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - The type of annotation determined during the interval.

   * - ``last_active_session`` (string)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - If persistence is enabled, the observation interval
       when the certificate was last seen.

   * - ``last_active_interval`` (number - interval)
     - site/packages/corelight/packages/known-entities/entities/types/certs.zeek
     - If persistence is enabled, the time duration in the
       past when the certificate was last seen.
