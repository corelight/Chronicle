``ftp`` field reference
-----------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time when the command was sent.

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

   * - ``user`` (string)
     - User name for the current FTP session.

   * - ``password`` (string)
     - Password for the current FTP session if captured.

   * - ``command`` (string)
     - Command given by the client.

   * - ``arg`` (string)
     - Argument for the command if one is given.

   * - ``mime_type`` (string)
     - Sniffed mime type of file.

   * - ``file_size`` (integer - count)
     - Size of the file if the command indicates a file transfer.

   * - ``reply_code`` (integer - count)
     - Reply code from the server in response to the command.

   * - ``reply_msg`` (string)
     - Reply message from the server in response to the command.

   * - ``data_channel.passive`` (boolean - bool)
     - Whether PASV mode is toggled for control channel.

   * - ``data_channel.orig_h`` (string - addr)
     - The host that will be initiating the data connection.

   * - ``data_channel.resp_h`` (string - addr)
     - The host that will be accepting the data connection.

   * - ``data_channel.resp_p`` (integer - port)
     - The port at which the acceptor is listening for the data
       connection.

   * - ``fuid`` (string)
     - File unique ID.
