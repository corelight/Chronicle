.. _ref_logs_cip:

cip
---
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
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The is_orig information.

   * - ``cip_sequence_count`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The cip_sequence_count information.

   * - ``direction`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The direction information.

   * - ``cip_service_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The cip_service_code information.

   * - ``cip_service`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The cip_service information.

   * - ``cip_status_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The cip_status_code information.

   * - ``cip_status`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The cip_status information.

   * - ``cip_extended_status_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The cip_extended_status_code information.

   * - ``cip_extended_status`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The cip_extended_status information.

   * - ``class_id`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The class_id information.

   * - ``class_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The class_name information.

   * - ``instance_id`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The instance_id information.

   * - ``attribute_id`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The attribute_id information.
