.. _ref_logs_vpn:

vpn
---
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - Time the vpn was encountered

   * - ``uid`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - Unique ID for the connection

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

   * - ``proto`` (string - enum transport_proto)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The protcol.

   * - ``vpn_type`` (string - enum VPNInsights::VPN_Type)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The VPN type.

   * - ``service`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The vpn type

   * - ``inferences`` (array[string] - set[string])
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - VPN inferences
       Legend:
       	NSP	- Non Standard Port.
       	FW	- Using a port to subvert a firewall (i.e. 53/udp).
       	RW	- Road warrior configuration detected (i.e. Cisco Anyconnect).
       	COM	- Commercial VPN service.
       	SK      - Static Key
            TLS     - TLS Auth

   * - ``server_name`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The server_name from SSL log, host from HTTP, if appropriate.

   * - ``client_info`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - Client info.  HTTP user agent is an example of client info.

   * - ``duration`` (number - interval)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - How long the connection lasted.

   * - ``orig_bytes`` (integer - count)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The orig bytes

   * - ``resp_bytes`` (integer - count)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The resp bytes

   * - ``orig_cc`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The orig  country_code

   * - ``orig_region`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The orig  region

   * - ``orig_city`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The orig  city

   * - ``resp_cc`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The resp country_code

   * - ``resp_region`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The resp region

   * - ``resp_city`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - The resp city

   * - ``subject`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - SSL subject string

   * - ``issuer`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - SSL issuer string

   * - ``ja3`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - SSL ja3

   * - ``ja3s`` (string)
     - site/packages/corelight/packages/vpn-insights/vpn.zeek
     - SSL ja3s
