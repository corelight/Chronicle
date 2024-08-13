.. _ref_logs_ssh:

ssh
---
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Time when the SSH connection began.

   * - ``uid`` (string)
     - base
     - Unique ID for the connection.

   * - ``id.orig_h`` (string - addr)
     - base
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - base
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - base
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - base
     - The responder's port number.

   * - ``id.orig_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_status information.

   * - ``id.orig_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_uid information.

   * - ``id.orig_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_cid information.

   * - ``id.orig_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_source information.

   * - ``id.resp_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_status information.

   * - ``id.resp_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_uid information.

   * - ``id.resp_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_cid information.

   * - ``id.resp_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_source information.

   * - ``id.vlan`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The VLAN that the connection is seen on.

   * - ``id.vlan_inner`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The inner VLAN tag for stacked VLAN tags.

   * - ``version`` (integer - count)
     - base
     - SSH major version (1, 2, or unset). The version can be unset if the
       client and server version strings are unset, malformed or incompatible
       so no common version can be extracted. If no version can be extracted
       even though both client and server versions are set a weird
       will be generated.

   * - ``auth_success`` (boolean - bool)
     - base
     - Authentication result (T=success, F=failure, unset=unknown)

   * - ``auth_attempts`` (integer - count)
     - base
     - The number of authentication attempts we observed. There's always
       at least one, since some servers might support no authentication at all.
       It's important to note that not all of these are failures, since
       some servers require two-factor auth (e.g. password AND pubkey)

   * - ``direction`` (string - enum Direction)
     - base
     - Direction of the connection. If the client was a local host
       logging into an external host, this would be OUTBOUND. INBOUND
       would be set for the opposite situation.

   * - ``client`` (string)
     - base
     - The client's version string

   * - ``server`` (string)
     - base
     - The server's version string

   * - ``cipher_alg`` (string)
     - base
     - The encryption algorithm in use

   * - ``mac_alg`` (string)
     - base
     - The signing (MAC) algorithm in use

   * - ``compression_alg`` (string)
     - base
     - The compression algorithm in use

   * - ``kex_alg`` (string)
     - base
     - The key exchange algorithm in use

   * - ``host_key_alg`` (string)
     - base
     - The server host key's algorithm

   * - ``host_key`` (string)
     - base
     - The server's key fingerprint

   * - ``remote_location.country_code`` (string)
     - base
     - The country code.

   * - ``remote_location.region`` (string)
     - base
     - The region.

   * - ``remote_location.city`` (string)
     - base
     - The city.

   * - ``remote_location.latitude`` (number - double)
     - base
     - Latitude.

   * - ``remote_location.longitude`` (number - double)
     - base
     - Longitude.

   * - ``hasshVersion`` (string)
     - site/packages/corelight/packages/hassh/hassh.zeek
     - The hasshVersion information.

   * - ``hassh`` (string)
     - site/packages/corelight/packages/hassh/hassh.zeek
     - The hassh information.

   * - ``hasshServer`` (string)
     - site/packages/corelight/packages/hassh/hassh.zeek
     - The hasshServer information.

   * - ``cshka`` (string)
     - site/packages/corelight/packages/hassh/hassh.zeek
     - The cshka information.

   * - ``hasshAlgorithms`` (string)
     - site/packages/corelight/packages/hassh/hassh.zeek
     - The hasshAlgorithms information.

   * - ``sshka`` (string)
     - site/packages/corelight/packages/hassh/hassh.zeek
     - The sshka information.

   * - ``hasshServerAlgorithms`` (string)
     - site/packages/corelight/packages/hassh/hassh.zeek
     - The hasshServerAlgorithms information.

   * - ``inferences`` (array[string] - set[string])
     - site/packages/corelight/packages/ssh-inference/config.zeek
     - Inferences from SOL analysis.
