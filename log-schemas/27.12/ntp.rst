.. _ref_logs_ntp:

ntp
---
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Timestamp for when the event happened.

   * - ``uid`` (string)
     - base
     - Unique ID for the connection.

   * - ``id.orig_h`` (string - addr)
     - base
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - base
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - base
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - base
     - The responder's port number.

   * - ``id.orig_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_status information.

   * - ``id.orig_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_uid information.

   * - ``id.orig_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_cid information.

   * - ``id.orig_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_source information.

   * - ``id.resp_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_status information.

   * - ``id.resp_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_uid information.

   * - ``id.resp_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_cid information.

   * - ``id.resp_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_source information.

   * - ``id.vlan`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The VLAN that the connection is seen on.

   * - ``id.vlan_inner`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The inner VLAN tag for stacked VLAN tags.

   * - ``version`` (integer - count)
     - base
     - The NTP version number (1, 2, 3, 4).

   * - ``mode`` (integer - count)
     - base
     - The NTP mode being used.

   * - ``stratum`` (integer - count)
     - base
     - The stratum (primary server, secondary server, etc.).

   * - ``poll`` (number - interval)
     - base
     - The maximum interval between successive messages.

   * - ``precision`` (number - interval)
     - base
     - The precision of the system clock.

   * - ``root_delay`` (number - interval)
     - base
     - Total round-trip delay to the reference clock.

   * - ``root_disp`` (number - interval)
     - base
     - Total dispersion to the reference clock.

   * - ``ref_id`` (string)
     - base
     - For stratum 0, 4 character string used for debugging.
       For stratum 1, ID assigned to the reference clock by IANA.
       Above stratum 1, when using IPv4, the IP address of the reference
       clock.  Note that the NTP protocol did not originally specify a
       large enough field to represent IPv6 addresses, so they use
       the first four bytes of the MD5 hash of the reference clock's
       IPv6 address (i.e. an IPv4 address here is not necessarily IPv4).

   * - ``ref_time`` (time)
     - base
     - Time when the system clock was last set or correct.

   * - ``org_time`` (time)
     - base
     - Time at the client when the request departed for the NTP server.

   * - ``rec_time`` (time)
     - base
     - Time at the server when the request arrived from the NTP client.

   * - ``xmt_time`` (time)
     - base
     - Time at the server when the response departed for the NTP client.

   * - ``num_exts`` (integer - count)
     - base
     - Number of extension fields (which are not currently parsed).
