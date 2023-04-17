``smb_mapping`` UDM Map Reference
---------------------------------

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
     - replace with 'DISK'

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

   * - ``path`` (string)
     -
     - Name of the tree path.

   * - ``service`` (string)
     -
     - The type of resource of the tree (disk share, printer share, named pipe, etc.).

   * - ``native_file_system`` (string)
     -
     - File system of the tree.

   * - ``share_type`` (string)
     -
     - If this is SMB2, a share type will be included.  For SMB1,
       the type of share will be deduced and included as well.
