``vpn`` field reference
-----------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time the vpn was encountered

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

   * - ``proto`` (string - enum)
     - The protcol.

   * - ``vpn_type`` (string - enum)
     - The VPN type.

   * - ``service`` (string)
     - The vpn type

   * - ``inferences`` (array[string] - set[string])
     - VPN inferences
       Legend:
       	NSP	- Non Standard Port.
       	FW	- Using a port to subvert a firewall (i.e. 53/udp).
       	RW	- Road warrior configuration detected (i.e. Cisco Anyconnect).
       	COM	- Commercial VPN service.
       	SK      - Static Key
            TLS     - TLS Auth

   * - ``server_name`` (string)
     - The server_name from SSL log, host from HTTP, if appropriate.

   * - ``client_info`` (string)
     - Client info.  HTTP user agent is an example of client info.

   * - ``duration`` (number - interval)
     - How long the connection lasted.

   * - ``orig_bytes`` (integer - count)
     - The orig bytes

   * - ``resp_bytes`` (integer - count)
     - The resp bytes

   * - ``orig_cc`` (string)
     - The orig  country_code

   * - ``orig_region`` (string)
     - The orig  region

   * - ``orig_city`` (string)
     - The orig  city

   * - ``resp_cc`` (string)
     - The resp country_code

   * - ``resp_region`` (string)
     - The resp region

   * - ``resp_city`` (string)
     - The resp city

   * - ``subject`` (string)
     - SSL subject string

   * - ``issuer`` (string)
     - SSL issuer string

   * - ``ja3`` (string)
     - SSL ja3

   * - ``ja3s`` (string)
     - SSL ja3s
