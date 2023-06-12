``radius`` field reference
--------------------------

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

   * - ``username`` (string)
     - The username, if present.

   * - ``mac`` (string)
     - MAC address, if present.

   * - ``framed_addr`` (string - addr)
     - The address given to the network access server, if
       present.  This is only a hint from the RADIUS server
       and the network access server is not required to honor
       the address.

   * - ``tunnel_client`` (string)
     - Address (IPv4, IPv6, or FQDN) of the initiator end of the tunnel,
       if present.  This is collected from the Tunnel-Client-Endpoint
       attribute.

   * - ``connect_info`` (string)
     - Connect info, if present.

   * - ``reply_msg`` (string)
     - Reply message from the server challenge. This is
       frequently shown to the user authenticating.

   * - ``result`` (string)
     - Successful or failed authentication.

   * - ``ttl`` (number - interval)
     - The duration between the first request and
       either the \"Access-Accept\" message or an error.
       If the field is empty, it means that either
       the request or response was not seen.
