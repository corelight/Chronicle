``x`` UDM map reference
--------------------------

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
     - ``network_ip_protocol``
     - replace with 'TCP'

   * -
     - ``target_resource_type``
     - replace with 'FILE'

   * -
     - ``metadata_description``
     - replace with 'action: %{action} on: %{name}'

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

   * - ``fuid`` (string)
     -
     - Unique ID of the file.

   * - ``action`` (string - enum)
     -
     - Action this log record represents.

   * - ``path`` (string)
     -
     - Path pulled from the tree this file was transferred to or from.

   * - ``name`` (string)
     - ``target_file_full_path``
     - Filename if one was seen.

   * - ``size`` (integer - count)
     - ``target_file_size`` (uinteger)
     - Total size of the file.

   * - ``prev_name`` (string)
     -
     - If the rename action was seen, this will be
       the file's previous name.

   * - ``times.modified`` (time)
     -
     - The time when data was last written to the file.

   * - ``times.accessed`` (time)
     -
     - The time when the file was last accessed.

   * - ``times.created`` (time)
     -
     - The time the file was created.

   * - ``times.changed`` (time)
     -
     - The time when the file was last modified.

   * - ``data_offset_req`` (integer - count)
     -
     - The data_offset_req information.

   * - ``data_len_req`` (integer - count)
     -
     - The data_len_req information.

   * - ``data_len_rsp`` (integer - count)
     -
     - The data_len_rsp information.
