.. _ref_logs_s7comm_read_szl:

s7comm_read_szl
---------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
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
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The is_orig information.

   * - ``pdu_reference`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The pdu_reference information.

   * - ``method`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The method information.

   * - ``szl_id`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The szl_id information.

   * - ``szl_id_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The szl_id_name information.

   * - ``szl_index`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The szl_index information.

   * - ``return_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The return_code information.

   * - ``return_code_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The return_code_name information.
