.. _ref_logs_cip_identity:

cip_identity
------------
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

   * - ``encapsulation_version`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The encapsulation_version information.

   * - ``socket_address`` (string - addr)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The socket_address information.

   * - ``socket_port`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The socket_port information.

   * - ``vendor_id`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The vendor_id information.

   * - ``vendor_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The vendor_name information.

   * - ``device_type_id`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The device_type_id information.

   * - ``device_type_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The device_type_name information.

   * - ``product_code`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The product_code information.

   * - ``revision`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The revision information.

   * - ``device_status`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The device_status information.

   * - ``serial_number`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The serial_number information.

   * - ``product_name`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The product_name information.

   * - ``device_state`` (string)
     - site/packages/corelight/packages/zeek-plugin-enip/main.zeek
     - The device_state information.
