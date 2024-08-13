.. _ref_logs_ssl_red:

ssl_red
-------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Time when the SSL connection was first detected.

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

   * - ``version`` (string)
     - base
     - SSL/TLS version that the server chose.

   * - ``cipher`` (string)
     - base
     - SSL/TLS cipher suite that the server chose.

   * - ``curve`` (string)
     - base
     - Elliptic curve the server chose when using ECDH/ECDHE.

   * - ``server_name`` (string)
     - base
     - Value of the Server Name Indicator SSL/TLS extension.  It
       indicates the server name that the client was requesting.

   * - ``resumed`` (boolean - bool)
     - base
     - Flag to indicate if the session was resumed reusing
       the key material exchanged in an earlier connection.

   * - ``last_alert`` (string)
     - base
     - Last alert that was seen during the connection.

   * - ``next_protocol`` (string)
     - base
     - Next protocol the server chose using the application layer
       next protocol extension, if present.

   * - ``established`` (boolean - bool)
     - base
     - Flag to indicate if this ssl session has been established
       successfully, or if it was aborted during the handshake.

   * - ``ssl_history`` (string)
     - base
     - SSL history showing which types of packets we received in which order.
       Letters have the following meaning with client-sent letters being capitalized:
       
       A direction flip occurs when the client hello packet is not sent from the originator
       of a connection. This can, e.g., occur when DTLS is used in a connection that was
       set up using STUN.
       
       
       * ^: direction flipped
       * H: hello_request
       * C: client_hello
       * S: server_hello
       * V: hello_verify_request
       * T: NewSessionTicket
       * X: certificate
       * K: server_key_exchange
       * R: certificate_request
       * N: server_hello_done
       * Y: certificate_verify
       * G: client_key_exchange
       * F: finished
       * W: certificate_url
       * U: certificate_status
       * A: supplemental_data
       * Z: unassigned_handshake_type
       * I: change_cipher_spec
       * B: heartbeat
       * D: application_data
       * E: end_of_early_data
       * O: encrypted_extensions
       * P: key_update
       * M: message_hash
       * J: hello_retry_request
       * L: alert
       * Q: unknown_content_type

   * - ``cert_chain_fps`` (array[string] - vector of string)
     - base
     - An ordered vector of all certificate fingerprints for the
       certificates offered by the server.

   * - ``client_cert_chain_fps`` (array[string] - vector of string)
     - base
     - An ordered vector of all certificate fingerprints for the
       certificates offered by the client.

   * - ``sni_matches_cert`` (boolean - bool)
     - base
     - Set to true if the hostname sent in the SNI matches the certificate.
       Set to false if they do not match. Unset if the client did not send
       an SNI.

   * - ``validation_status`` (string)
     - site/packages/corelight/packages/cert-hygiene/validate-certs.zeek
     - Result of certificate validation for this connection.

   * - ``ja3`` (string)
     - site/packages/corelight/packages/ja3/ja3.zeek
     - The ja3 information.

   * - ``ja3s`` (string)
     - site/packages/corelight/packages/ja3/ja3s.zeek
     - The ja3s information.
