.. _ref_logs_profinet_dce_rpc:

profinet_dce_rpc
----------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - Timestamp for when the event happened.

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
     - The status of the originator's endpoint agent.

   * - ``id.orig_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint unique ID.

   * - ``id.orig_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint Customer ID.

   * - ``id.orig_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint information source.

   * - ``id.resp_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The status of the responder's endpoint agent.

   * - ``id.resp_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint unique ID.

   * - ``id.resp_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint Customer ID.

   * - ``id.resp_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint information source.

   * - ``id.vlan`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The VLAN that the connection is seen on.

   * - ``id.vlan_inner`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The inner VLAN tag for stacked VLAN tags.

   * - ``version`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - The connection's 4-tuple of endpoint addresses/ports.

   * - ``packet_type`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - The packet_type information.

   * - ``object_uuid`` (string)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - The object_uuid information.

   * - ``interface_uuid`` (string)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - The interface_uuid information.

   * - ``activity_uuid`` (string)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - The activity_uuid information.

   * - ``server_boot_time`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - The server_boot_time information.

   * - ``operation`` (string)
     - site/packages/corelight/packages/zeek-plugin-profinet/main.zeek
     - The operation information.
