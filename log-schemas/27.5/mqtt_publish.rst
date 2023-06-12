``mqtt_publish`` field reference
--------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp for when the publish message started

   * - ``uid`` (string)
     - UID for the connection

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``from_client`` (boolean - bool)
     - Indicates if the message was published by the client of
       this connection or published to the client.

   * - ``retain`` (boolean - bool)
     - Indicates if the message was to be retained by the server

   * - ``qos`` (string)
     - QoS level set for the message

   * - ``status`` (string)
     - Status of the published message. This will be set to \"incomplete_qos\"
       if the full back and forth for the requested level of QoS was not seen.
       Otherwise if it's successful the field will be \"ok\".

   * - ``topic`` (string)
     - Topic the message was published to

   * - ``payload`` (string)
     - Payload of the message

   * - ``payload_len`` (integer - count)
     - The actual length of the payload in the case the *payload*
       field's contents were truncated according to
       `MQTT::max_payload_size`.
