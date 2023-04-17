``x`` UDM Map Reference
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
     - replace with 'NETWORK_SMTP'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * -
     - ``network_application_protocol``
     - replace with 'SMTP'

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

   * - ``trans_depth`` (integer - count)
     -
     - A count to represent the depth of this message transaction in
       a single connection where multiple messages were transferred.

   * - ``helo`` (string)
     -
     - Contents of the Helo header.

   * - ``mailfrom`` (string)
     - ``network_email.from``
     - Email addresses found in the From header.

   * - ``rcptto`` (array[string] - set[string])
     -
     - Email addresses found in the Rcpt header.

   * - ``date`` (string)
     -
     - Contents of the Date header.

   * - ``from`` (string)
     -
     - Contents of the From header.

   * - ``to`` (array[string] - set[string])
     -
     - Contents of the To header.

   * - ``cc`` (array[string] - set[string])
     -
     - Contents of the CC header.

   * - ``reply_to`` (string)
     - ``network_email.reply_to``
     - Contents of the ReplyTo header.

   * - ``msg_id`` (string)
     -
     - Contents of the MsgID header.

   * - ``in_reply_to`` (string)
     -
     - Contents of the In-Reply-To header.

   * - ``subject`` (string)
     - ``email_subject``
     - Contents of the Subject header.

   * - ``x_originating_ip`` (string - addr)
     -
     - Contents of the X-Originating-IP header.

   * - ``first_received`` (string)
     -
     - Contents of the first Received header.

   * - ``second_received`` (string)
     -
     - Contents of the second Received header.

   * - ``last_reply`` (string)
     -
     - The last message that the server sent to the client.

   * - ``path`` (array[string] - vector of addr)
     -
     - The message transmission path, as extracted from the headers.

   * - ``user_agent`` (string)
     -
     - Value of the User-Agent header from the client.

   * - ``tls`` (boolean - bool)
     - ``event1.idm.read_only_udm.network.tls.established``
     - Indicates that the connection has switched to using TLS.

   * - ``fuids`` (array[string] - vector of string)
     -
     - An ordered vector of file unique IDs seen attached to
       the message.

   * - ``is_webmail`` (boolean - bool)
     -
     - Boolean indicator of if the message was sent through a
       webmail interface.

   * - ``urls`` (array[string] - set[string])
     -
     - The URLs seen in the email.

   * - ``domains`` (array[string] - set[string])
     -
     - The URLs seen in the email.
