.. _ref_logs_ocsp:

ocsp
----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Time when the OCSP reply was encountered.

   * - ``id`` (string)
     - base
     - File id of the OCSP reply.

   * - ``hashAlgorithm`` (string)
     - base
     - Hash algorithm used to generate issuerNameHash and issuerKeyHash.

   * - ``issuerNameHash`` (string)
     - base
     - Hash of the issuer's distinguished name.

   * - ``issuerKeyHash`` (string)
     - base
     - Hash of the issuer's public key.

   * - ``serialNumber`` (string)
     - base
     - Serial number of the affected certificate.

   * - ``certStatus`` (string)
     - base
     - Status of the affected certificate.

   * - ``revoketime`` (time)
     - base
     - Time at which the certificate was revoked.

   * - ``revokereason`` (string)
     - base
     - Reason for which the certificate was revoked.

   * - ``thisUpdate`` (time)
     - base
     - The time at which the status being shows is known to have been correct.

   * - ``nextUpdate`` (time)
     - base
     - The latest time at which new information about the status of the certificate will be available.
