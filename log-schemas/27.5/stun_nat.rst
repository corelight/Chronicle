``stun_nat`` field reference
----------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The ts information.

   * - ``uid`` (string)
     - The uid information.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``proto`` (string - enum)
     - The protocol

   * - ``is_orig`` (boolean - bool)
     - The is_orig information.

   * - ``wan_addrs`` (array[string] - vector of addr)
     - The WAN address as reported by STUN

   * - ``wan_ports`` (array[integer] - vector of count)
     - The mapped port

   * - ``lan_addrs`` (array[string] - vector of addr)
     - The NAT'd LAN address as reported by STUN
