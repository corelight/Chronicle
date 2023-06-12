``corelight_burst`` field reference
-----------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp of when the burst was identified.

   * - ``uid`` (string)
     - Connection unique ID.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``proto`` (string - enum)
     - Protocol of the connection.

   * - ``orig_size`` (integer - count)
     - Amount of data sent by the originator of the connection.

   * - ``resp_size`` (integer - count)
     - Amount of data sent by the responder of the connection.

   * - ``mbps`` (number - double)
     - Speed of the connection when the burst identification occurred.

   * - ``age_of_conn`` (number - interval)
     - How fast the connection was when the burst identication occurred.
