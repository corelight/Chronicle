ssh
---
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time when the SSH connection began.

   * - ``uid`` (string)
     - Unique ID for the connection.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``version`` (integer - count)
     - SSH major version (1, 2, or unset). The version can be unset if the
       client and server version strings are unset, malformed or incompatible
       so no common version can be extracted. If no version can be extracted
       even though both client and server versions are set a weird
       will be generated.

   * - ``auth_success`` (boolean - bool)
     - Authentication result (T=success, F=failure, unset=unknown)

   * - ``auth_attempts`` (integer - count)
     - The number of authentication attemps we observed. There's always
       at least one, since some servers might support no authentication at all.
       It's important to note that not all of these are failures, since
       some servers require two-factor auth (e.g. password AND pubkey)

   * - ``direction`` (string - enum)
     - Direction of the connection. If the client was a local host
       logging into an external host, this would be OUTBOUND. INBOUND
       would be set for the opposite situation.

   * - ``client`` (string)
     - The client's version string

   * - ``server`` (string)
     - The server's version string

   * - ``cipher_alg`` (string)
     - The encryption algorithm in use

   * - ``mac_alg`` (string)
     - The signing (MAC) algorithm in use

   * - ``compression_alg`` (string)
     - The compression algorithm in use

   * - ``kex_alg`` (string)
     - The key exchange algorithm in use

   * - ``host_key_alg`` (string)
     - The server host key's algorithm

   * - ``host_key`` (string)
     - The server's key fingerprint

   * - ``remote_location.country_code`` (string)
     - The country code.

   * - ``remote_location.region`` (string)
     - The region.

   * - ``remote_location.city`` (string)
     - The city.

   * - ``remote_location.latitude`` (number - double)
     - Latitude.

   * - ``remote_location.longitude`` (number - double)
     - Longitude.

   * - ``hasshVersion`` (string)
     - The hasshVersion information.

   * - ``hassh`` (string)
     - The hassh information.

   * - ``hasshServer`` (string)
     - The hasshServer information.

   * - ``cshka`` (string)
     - The cshka information.

   * - ``hasshAlgorithms`` (string)
     - The hasshAlgorithms information.

   * - ``sshka`` (string)
     - The sshka information.

   * - ``hasshServerAlgorithms`` (string)
     - The hasshServerAlgorithms information.

   * - ``inferences`` (array[string] - set[string])
     - Inferences from SOL analysis.
