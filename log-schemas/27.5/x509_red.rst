``x509_red`` field reference
----------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Current timestamp.

   * - ``fingerprint`` (string)
     - Fingerprint of the certificate - uses chosen algorithm.

   * - ``certificate.version`` (integer - count)
     - Version number.

   * - ``certificate.serial`` (string)
     - Serial number.

   * - ``certificate.subject`` (string)
     - Subject.

   * - ``certificate.issuer`` (string)
     - Issuer.

   * - ``certificate.not_valid_before`` (time)
     - Timestamp before when certificate is not valid.

   * - ``certificate.not_valid_after`` (time)
     - Timestamp after when certificate is not valid.

   * - ``certificate.key_alg`` (string)
     - Name of the key algorithm

   * - ``certificate.sig_alg`` (string)
     - Name of the signature algorithm

   * - ``certificate.key_type`` (string)
     - Key type, if key parseable by openssl (either rsa, dsa or ec)

   * - ``certificate.key_length`` (integer - count)
     - Key length in bits

   * - ``certificate.exponent`` (string)
     - Exponent, if RSA-certificate

   * - ``certificate.curve`` (string)
     - Curve, if EC-certificate

   * - ``san.dns`` (array[string] - vector of string)
     - List of DNS entries in SAN

   * - ``san.uri`` (array[string] - vector of string)
     - List of URI entries in SAN

   * - ``san.email`` (array[string] - vector of string)
     - List of email entries in SAN

   * - ``san.ip`` (array[string] - vector of addr)
     - List of IP entries in SAN

   * - ``basic_constraints.ca`` (boolean - bool)
     - CA flag set?

   * - ``basic_constraints.path_len`` (integer - count)
     - Maximum path length

   * - ``host_cert`` (boolean - bool)
     - Indicates if this certificate was a end-host certificate, or sent as part of a chain

   * - ``client_cert`` (boolean - bool)
     - Indicates if this certificate was sent from the client
