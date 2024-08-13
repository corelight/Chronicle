.. _ref_logs_bacnet_property:

bacnet_property
---------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
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

   * - ``is_orig`` (boolean - bool)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The is_orig information.

   * - ``invoke_id`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The invoke_id information.

   * - ``pdu_service`` (string)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The pdu_service information.

   * - ``object_type`` (string)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The object_type information.

   * - ``instance_number`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The instance_number information.

   * - ``property`` (string)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The property information.

   * - ``array_index`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The array_index information.

   * - ``value`` (string)
     - site/packages/corelight/packages/zeek-plugin-bacnet/main.zeek
     - The value information.
