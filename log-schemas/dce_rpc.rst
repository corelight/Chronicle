``dce_rpc`` field reference
---------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp for when the event happened.

   * - ``uid`` (string)
     - Unique ID for the connection.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``rtt`` (number - interval)
     - Round trip time from the request to the response.
       If either the request or response wasn't seen,
       this will be null.

   * - ``named_pipe`` (string)
     - Remote pipe name.

   * - ``endpoint`` (string)
     - Endpoint name looked up from the uuid.

   * - ``operation`` (string)
     - Operation seen in the call.
