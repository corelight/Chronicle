``dce_rpc`` UDM Map Reference
-----------------------------

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
     - ``metadata_description``
     - replace with 'operation %{operation} on %{endpoint} at named pipe [%{named_pipe}]'

   * -
     - ``target_resource_type``
     - replace with 'PIPE'

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

   * - ``rtt`` (number - interval)
     -
     - Round trip time from the request to the response.
       If either the request or response wasn't seen,
       this will be null.

   * - ``named_pipe`` (string)
     -
     - Remote pipe name.

   * - ``endpoint`` (string)
     -
     - Endpoint name looked up from the uuid.

   * - ``operation`` (string)
     -
     - Operation seen in the call.
