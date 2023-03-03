``ntlm`` field reference
------------------------

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
     - Username given by the client.

   * - ``hostname`` (string)
     - Hostname given by the client.

   * - ``domainname`` (string)
     - Domainname given by the client.

   * - ``server_nb_computer_name`` (string)
     - NetBIOS name given by the server in a CHALLENGE.

   * - ``server_dns_computer_name`` (string)
     - DNS name given by the server in a CHALLENGE.

   * - ``server_tree_name`` (string)
     - Tree name given by the server in a CHALLENGE.

   * - ``success`` (boolean - bool)
     - Indicate whether or not the authentication was successful.
