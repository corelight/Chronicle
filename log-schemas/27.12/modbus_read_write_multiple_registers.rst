.. _ref_logs_modbus_read_write_multiple_registers:

modbus_read_write_multiple_registers
------------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
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
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The is_orig information.

   * - ``tid`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The tid information.

   * - ``unit`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The unit information.

   * - ``func`` (string)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The func information.

   * - ``request_response`` (string)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The request_response information.

   * - ``write_start_address`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The write_start_address information.

   * - ``write_registers`` (array[integer] - vector of count)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The write_registers information.

   * - ``read_start_address`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The read_start_address information.

   * - ``read_quantity`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The read_quantity information.

   * - ``read_registers`` (array[integer] - vector of count)
     - site/packages/corelight/packages/zeek-plugin-modbus/main.zeek
     - The read_registers information.
