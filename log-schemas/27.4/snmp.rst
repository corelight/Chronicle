``snmp`` field reference
------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp of first packet belonging to the SNMP session.

   * - ``uid`` (string)
     - The unique ID for the connection.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``duration`` (number - interval)
     - The amount of time between the first packet beloning to
       the SNMP session and the latest one seen.

   * - ``version`` (string)
     - The version of SNMP being used.

   * - ``community`` (string)
     - The community string of the first SNMP packet associated with
       the session.  This is used as part of SNMP's (v1 and v2c)
       administrative/security framework.  See :rfc:`1157` or :rfc:`1901`.

   * - ``get_requests`` (integer - count)
     - The number of variable bindings in GetRequest/GetNextRequest PDUs
       seen for the session.

   * - ``get_bulk_requests`` (integer - count)
     - The number of variable bindings in GetBulkRequest PDUs seen for
       the session.

   * - ``get_responses`` (integer - count)
     - The number of variable bindings in GetResponse/Response PDUs seen
       for the session.

   * - ``set_requests`` (integer - count)
     - The number of variable bindings in SetRequest PDUs seen for
       the session.

   * - ``display_string`` (string)
     - A system description of the SNMP responder endpoint.

   * - ``up_since`` (time)
     - The time at which the SNMP responder endpoint claims it's been
       up since.
