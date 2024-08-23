.. _ref_logs_enip:

enip
----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The uid information.

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

   * - ``is_orig`` (boolean - bool)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The is_orig information.

   * - ``enip_command_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The enip_command_code information.

   * - ``enip_command`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The enip_command information.

   * - ``length`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The length information.

   * - ``session_handle`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The session_handle information.

   * - ``enip_status`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The enip_status information.

   * - ``sender_context`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The sender_context information.

   * - ``options`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The options information.
