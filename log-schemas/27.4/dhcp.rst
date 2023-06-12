``dhcp`` field reference
------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The earliest time at which a DHCP message over the
       associated connection is observed.

   * - ``uids`` (array[string] - set[string])
     - A series of unique identifiers of the connections over which
       DHCP is occurring.  This behavior with multiple connections is
       unique to DHCP because of the way it uses broadcast packets
       on local networks.

   * - ``client_addr`` (string - addr)
     - IP address of the client.  If a transaction
       is only a client sending INFORM messages then
       there is no lease information exchanged so this
       is helpful to know who sent the messages.
       Getting an address in this field does require
       that the client sources at least one DHCP message
       using a non-broadcast address.

   * - ``server_addr`` (string - addr)
     - IP address of the server involved in actually
       handing out the lease.  There could be other
       servers replying with OFFER messages which won't
       be represented here.  Getting an address in this
       field also requires that the server handing out
       the lease also sources packets from a non-broadcast
       IP address.

   * - ``mac`` (string)
     - Client's hardware address.

   * - ``host_name`` (string)
     - Name given by client in Hostname option 12.

   * - ``client_fqdn`` (string)
     - FQDN given by client in Client FQDN option 81.

   * - ``domain`` (string)
     - Domain given by the server in option 15.

   * - ``requested_addr`` (string - addr)
     - IP address requested by the client.

   * - ``assigned_addr`` (string - addr)
     - IP address assigned by the server.

   * - ``lease_time`` (number - interval)
     - IP address lease interval.

   * - ``client_message`` (string)
     - Message typically accompanied with a DHCP_DECLINE
       so the client can tell the server why it rejected
       an address.

   * - ``server_message`` (string)
     - Message typically accompanied with a DHCP_NAK to let
       the client know why it rejected the request.

   * - ``msg_types`` (array[string] - vector of string)
     - The DHCP message types seen by this DHCP transaction

   * - ``duration`` (number - interval)
     - Duration of the DHCP "session" representing the
       time from the first message to the last.
