``ntp`` field reference
-----------------------

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

   * - ``version`` (integer - count)
     - The NTP version number (1, 2, 3, 4).

   * - ``mode`` (integer - count)
     - The NTP mode being used.

   * - ``stratum`` (integer - count)
     - The stratum (primary server, secondary server, etc.).

   * - ``poll`` (number - interval)
     - The maximum interval between successive messages.

   * - ``precision`` (number - interval)
     - The precision of the system clock.

   * - ``root_delay`` (number - interval)
     - Total round-trip delay to the reference clock.

   * - ``root_disp`` (number - interval)
     - Total dispersion to the reference clock.

   * - ``ref_id`` (string)
     - For stratum 0, 4 character string used for debugging.
       For stratum 1, ID assigned to the reference clock by IANA.
       Above stratum 1, when using IPv4, the IP address of the reference
       clock.  Note that the NTP protocol did not originally specify a
       large enough field to represent IPv6 addresses, so they use
       the first four bytes of the MD5 hash of the reference clock's
       IPv6 address (i.e. an IPv4 address here is not necessarily IPv4).

   * - ``ref_time`` (time)
     - Time when the system clock was last set or correct.

   * - ``org_time`` (time)
     - Time at the client when the request departed for the NTP server.

   * - ``rec_time`` (time)
     - Time at the server when the request arrived from the NTP client.

   * - ``xmt_time`` (time)
     - Time at the server when the response departed for the NTP client.

   * - ``num_exts`` (integer - count)
     - Number of extension fields (which are not currently parsed).
