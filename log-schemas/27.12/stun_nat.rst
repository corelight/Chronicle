.. _ref_logs_stun_nat:

stun_nat
--------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-spicy-stun/main.zeek
     - Time the first packet was encountered.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-spicy-stun/main.zeek
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

   * - ``proto`` (string - enum transport_proto)
     - site/packages/corelight/packages/zeek-spicy-stun/main.zeek
     - Associated transport protocol.

   * - ``is_orig`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-stun/main.zeek
     - Whether the packet was sent by the originator.

   * - ``wan_addrs`` (array[string] - vector of addr)
     - site/packages/corelight/packages/zeek-spicy-stun/main.zeek
     - WAN address as reported by STUN.

   * - ``wan_ports`` (array[integer] - vector of count)
     - site/packages/corelight/packages/zeek-spicy-stun/main.zeek
     - Corresponding ports.

   * - ``lan_addrs`` (array[string] - vector of addr)
     - site/packages/corelight/packages/zeek-spicy-stun/main.zeek
     - NAT'd LAN address as reported by STUN.
