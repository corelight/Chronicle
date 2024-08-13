.. _ref_logs_s7comm_upload_download:

s7comm_upload_download
----------------------
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

   * - ``rosctr`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The rosctr information.

   * - ``pdu_reference`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The pdu_reference information.

   * - ``function_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The function_name information.

   * - ``function_status`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The function_status information.

   * - ``session_id`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The session_id information.

   * - ``blocklength`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The blocklength information.

   * - ``filename`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The filename information.

   * - ``block_type`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The block_type information.

   * - ``block_number`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The block_number information.

   * - ``destination_filesystem`` (string)
     - site/packages/corelight/packages/zeek-plugin-s7comm/main.zeek
     - The destination_filesystem information.
