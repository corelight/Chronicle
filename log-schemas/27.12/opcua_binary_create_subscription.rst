.. _ref_logs_opcua_binary_create_subscription:

opcua_binary_create_subscription
--------------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
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

   * - ``opcua_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The opcua_link_id information.

   * - ``requested_publishing_interval`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The requested_publishing_interval information.

   * - ``requested_lifetime_count`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The requested_lifetime_count information.

   * - ``requested_max_keep_alive_count`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The requested_max_keep_alive_count information.

   * - ``max_notifications_per_publish`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The max_notifications_per_publish information.

   * - ``publishing_enabled`` (boolean - bool)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The publishing_enabled information.

   * - ``priority`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The priority information.

   * - ``subscription_id`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The subscription_id information.

   * - ``revised_publishing_interval`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The revised_publishing_interval information.

   * - ``revised_lifetime_count`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The revised_lifetime_count information.

   * - ``revised_max_keep_alive_count`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/create-subscription-types.zeek
     - The revised_max_keep_alive_count information.
