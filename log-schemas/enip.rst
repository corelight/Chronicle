``enip`` field reference
------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The ts information.

   * - ``uid`` (string)
     - Timestamp for when the event happened.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``command`` (string)
     - The connection's 4-tuple of endpoint addresses/ports.

   * - ``length`` (integer - count)
     - Name of the sent ENIP command.

   * - ``session_handle`` (string)
     - Length of the ENIP packet.

   * - ``status`` (string)
     - Session number, generated after a register session

   * - ``sender_context`` (string)
     - Status of the command.

   * - ``options`` (string)
     - Context number
