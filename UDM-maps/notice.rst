``notice`` UDM Map Reference
----------------------------

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
     - An absolute time indicating when the notice occurred,
       defaults to the current network time.

   * - ``uid`` (string)
     - ``metadata_product_log_id``
     - A connection UID which uniquely identifies the endpoints
       concerned with the notice.

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
     - A file unique ID if this notice is related to a file.  If
       the *f* field is provided, this will be automatically filled
       out.

   * - ``file_mime_type`` (string)
     -
     - A mime type if the notice is related to a file.  If the *f*
       field is provided, this will be automatically filled out.

   * - ``file_desc`` (string)
     -
     - Frequently files can be \""described\"" to give a bit more
       context.  This field will typically be automatically filled
       out from an fa_file record.  For example, if a notice was
       related to a file over HTTP, the URL of the request would
       be shown.

   * - ``proto`` (string - enum)
     -
     - The transport protocol. Filled automatically when either
       *conn*, *iconn* or *p* is specified.

   * - ``note`` (string - enum)
     - ``metadata_description``
     - The `Notice::Type` of the notice.

   * - ``note`` (string - enum)
     - ``security_result.description``
     - The `Notice::Type` of the notice.

   * - ``msg`` (string)
     -
     - The human readable message for the notice.

   * - ``sub`` (string)
     -
     - The human readable sub-message.

   * - ``src`` (string - addr)
     -
     - Source address, if we don't have a `conn_id`.

   * - ``dst`` (string - addr)
     -
     - Destination address.

   * - ``p`` (integer - port)
     -
     - Associated port, if we don't have a `conn_id`.

   * - ``n`` (integer - count)
     -
     - Associated count, or perhaps a status code.

   * - ``peer_descr`` (string)
     -
     - Textual description for the peer that raised this notice,
       including name, host address and port.

   * - ``actions`` (array[string] - set[enum])
     -
     - The actions which have been applied to this notice.

   * - ``suppress_for`` (number - interval)
     -
     - This field indicates the length of time that this
       unique notice should be suppressed.

   * - ``remote_location.country_code`` (string)
     -
     - The country code.

   * - ``remote_location.region`` (string)
     -
     - The region.

   * - ``remote_location.city`` (string)
     -
     - The city.

   * - ``remote_location.latitude`` (number - double)
     -
     - Latitude.

   * - ``remote_location.longitude`` (number - double)
     -
     - Longitude.
