``irc`` UDM Map Reference
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
     - replace with 'GENERIC_EVENT'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

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

   * - ``nick`` (string)
     -
     - Nickname given for the connection.

   * - ``user`` (string)
     -
     - Username given for the connection.

   * - ``command`` (string)
     -
     - Command given by the client.

   * - ``value`` (string)
     -
     - Value for the command given by the client.

   * - ``addl`` (string)
     -
     - Any additional data for the command.

   * - ``dcc_file_name`` (string)
     -
     - DCC filename requested.

   * - ``dcc_file_size`` (integer - count)
     -
     - Size of the DCC transfer as indicated by the sender.

   * - ``dcc_mime_type`` (string)
     -
     - Sniffed mime type of the file.

   * - ``fuid`` (string)
     -
     - File unique ID.
