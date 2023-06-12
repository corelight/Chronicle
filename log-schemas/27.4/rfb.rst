``rfb`` field reference
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

   * - ``client_major_version`` (string)
     - Major version of the client.

   * - ``client_minor_version`` (string)
     - Minor version of the client.

   * - ``server_major_version`` (string)
     - Major version of the server.

   * - ``server_minor_version`` (string)
     - Minor version of the server.

   * - ``authentication_method`` (string)
     - Identifier of authentication method used.

   * - ``auth`` (boolean - bool)
     - Whether or not authentication was successful.

   * - ``share_flag`` (boolean - bool)
     - Whether the client has an exclusive or a shared session.

   * - ``desktop_name`` (string)
     - Name of the screen that is being shared.

   * - ``width`` (integer - count)
     - Width of the screen that is being shared.

   * - ``height`` (integer - count)
     - Height of the screen that is being shared.
