dns_red
-------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The earliest time at which a DNS protocol message over the
       associated connection is observed.

   * - ``uid`` (string)
     - A unique identifier of the connection over which DNS messages
       are being transferred.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``query`` (string)
     - The domain name that is the subject of the DNS query.

   * - ``qtype_name`` (string)
     - A descriptive name for the type of the query.

   * - ``rcode`` (integer - count)
     - The response code value in DNS response messages.

   * - ``answers`` (array[string] - vector of string)
     - The set of resource descriptions in the query answer.

   * - ``num`` (integer - count)
     - How often we've seen this query in this coalescence interval.
