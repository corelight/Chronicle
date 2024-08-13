.. _ref_logs_dnp3_control:

dnp3_control
------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
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

   * - ``block_type`` (string)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The block_type information.

   * - ``function_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The function_code information.

   * - ``index_number`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The index_number information.

   * - ``trip_control_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The trip_control_code information.

   * - ``operation_type`` (string)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The operation_type information.

   * - ``execute_count`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The execute_count information.

   * - ``on_time`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The on_time information.

   * - ``off_time`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The off_time information.

   * - ``status_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-dnp3/main.zeek
     - The status_code information.
