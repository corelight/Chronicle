``mqtt_connect`` field reference
--------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp for when the event happened

   * - ``uid`` (string)
     - Unique ID for the connection

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``proto_name`` (string)
     - Indicates the protocol name

   * - ``proto_version`` (string)
     - The version of the protocol in use

   * - ``client_id`` (string)
     - Unique identifier for the client

   * - ``connect_status`` (string)
     - Status message from the server in response to the connect request

   * - ``will_topic`` (string)
     - Topic to publish a "last will and testament" message to

   * - ``will_payload`` (string)
     - Payload to publish as a "last will and testament"
