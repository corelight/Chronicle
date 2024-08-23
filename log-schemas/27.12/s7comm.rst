.. _ref_logs_s7comm:

s7comm
------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

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
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The is_orig information.

   * - ``rosctr_code`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The rosctr_code information.

   * - ``rosctr_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The rosctr_name information.

   * - ``pdu_reference`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The pdu_reference information.

   * - ``function_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The function_code information.

   * - ``function_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The function_name information.

   * - ``subfunction_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The subfunction_code information.

   * - ``subfunction_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The subfunction_name information.

   * - ``error_class`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The error_class information.

   * - ``error_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The error_code information.
