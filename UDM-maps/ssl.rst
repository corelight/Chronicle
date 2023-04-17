``ssl`` UDM Map Reference
-------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 1 3

   * - Field (Type)
     - UDM Field (Type)
     - Description

   * -
     - ``metadata_vendor_name``
     - replace with 'Corelight'

   * -
     - ``metadata_event_type``
     - replace with 'NETWORK_CONNECTION'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * -
     - ``network_application_protocol``
     - replace with 'HTTPS'

   * -
     - ``network_ip_protocol``
     - replace with 'TCP'

   * -
     - ``security_result.severity``
     - replace with 'INFORMATIONAL'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - This is the time of the first packet.

   * - ``uid`` (string)
     - ``metadata_product_log_id``
     - A unique identifier of the connection.

   * - ``id.orig_h`` (string - addr)
     - ``principal_ip``
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - ``principal_port`` (string)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - ``target_ip``
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - ``target_port`` (string)
     - The responder's port number.

   * - ``version`` (string)
     - ``event1.idm.read_only_udm.network.tls.version``
     - SSL/TLS version that the server chose.

   * - ``cipher`` (string)
     - ``event1.idm.read_only_udm.network.tls.cipher``
     - SSL/TLS cipher suite that the server chose.

   * - ``curve`` (string)
     -
     - Elliptic curve the server chose when using ECDH/ECDHE.

   * - ``server_name`` (string)
     - ``event1.idm.read_only_udm.target.hostname``
     - Value of the Server Name Indicator SSL/TLS extension.  It
       indicates the server name that the client was requesting.

   * - ``server_name`` (string)
     - ``event1.idm.read_only_udm.network.tls.client.server_name``
     - Value of the Server Name Indicator SSL/TLS extension.  It
       indicates the server name that the client was requesting.

   * - ``resumed`` (boolean - bool)
     - ``event1.idm.read_only_udm.network.tls.resumed``
     - Flag to indicate if the session was resumed reusing
       the key material exchanged in an earlier connection.

   * - ``last_alert`` (string)
     -
     - Last alert that was seen during the connection.

   * - ``next_protocol`` (string)
     - ``event1.idm.read_only_udm.network.tls.next_protocol``
     - Next protocol the server chose using the application layer
       next protocol extension, if present.

   * - ``established`` (boolean - bool)
     - ``event1.idm.read_only_udm.network.tls.established``
     - Flag to indicate if this ssl session has been established
       successfully, or if it was aborted during the handshake.

   * - ``ssl_history`` (string)
     -
     - SSL history showing which types of packets we received in which order.
       Letters have the following meaning with client-sent letters being capitalized:


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
     -
     - An ordered vector of all certificate fingerprints for the
       certificates offered by the server.

   * - ``client_cert_chain_fps`` (array[string] - vector of string)
     -
     - An ordered vector of all certificate fingerprints for the
       certificates offered by the client.

   * - ``sni_matches_cert`` (boolean - bool)
     -
     - Set to true if the hostname sent in the SNI matches the certificate.
       Set to false if they do not match. Unset if the client did not send
       an SNI.

   * - ``validation_status`` (string)
     -
     - Result of certificate validation for this connection.

   * - ``ja3`` (string)
     - ``event1.idm.read_only_udm.network.tls.client.ja3``
     - The ja3 information.

   * - ``ja3s`` (string)
     - ``event1.idm.read_only_udm.network.tls.server.ja3s``
     - The ja3s information.
