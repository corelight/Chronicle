``rdp`` field reference
-----------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp for when the event happened.

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

   * - ``cookie`` (string)
     - Cookie value used by the client machine.
       This is typically a username.

   * - ``result`` (string)
     - Status result for the connection.  It's a mix between
       RDP negotation failure messages and GCC server create
       response messages.

   * - ``security_protocol`` (string)
     - Security protocol chosen by the server.

   * - ``client_channels`` (array[string] - vector of string)
     - The channels requested by the client

   * - ``keyboard_layout`` (string)
     - Keyboard layout (language) of the client machine.

   * - ``client_build`` (string)
     - RDP client version used by the client machine.

   * - ``client_name`` (string)
     - Name of the client machine.

   * - ``client_dig_product_id`` (string)
     - Product ID of the client machine.

   * - ``desktop_width`` (integer - count)
     - Desktop width of the client machine.

   * - ``desktop_height`` (integer - count)
     - Desktop height of the client machine.

   * - ``requested_color_depth`` (string)
     - The color depth requested by the client in
       the high_color_depth field.

   * - ``cert_type`` (string)
     - If the connection is being encrypted with native
       RDP encryption, this is the type of cert
       being used.

   * - ``cert_count`` (integer - count)
     - The number of certs seen.  X.509 can transfer an
       entire certificate chain.

   * - ``cert_permanent`` (boolean - bool)
     - Indicates if the provided certificate or certificate
       chain is permanent or temporary.

   * - ``encryption_level`` (string)
     - Encryption level of the connection.

   * - ``encryption_method`` (string)
     - Encryption method of the connection.

   * - ``auth_success`` (boolean - bool)
     - Whether the client successfully authenticated or not

   * - ``channels_joined`` (integer - int)
     - The number of channels a client joined during the connection sequence

   * - ``inferences`` (array[string] - set[string])
     - A set of inference \"tags\" about the connection

   * - ``rdpeudp_uid`` (string)
     - The connection UID of the UDP connection which assisted this TCP connection. If UDP was not used, this is unset.

   * - ``rdfp_string`` (string)
     - A fingerprint which represents am RDP client

   * - ``rdfp_hash`` (string)
     - The rdfp_hash information.
