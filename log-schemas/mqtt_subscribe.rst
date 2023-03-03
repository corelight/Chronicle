``mqtt_subscribe`` field reference
----------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp for when the subscribe or unsubscribe request started

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

   * - ``action`` (string - enum)
     - Indicates if a subscribe or unsubscribe action is taking place

   * - ``topics`` (array[string] - vector of string)
     - The topics (or topic patterns) being subscribed to

   * - ``qos_levels`` (array[integer] - vector of count)
     - QoS levels requested for messages from subscribed topics

   * - ``granted_qos_level`` (integer - count)
     - QoS level the server granted

   * - ``ack`` (boolean - bool)
     - Indicates if the request was acked by the server
