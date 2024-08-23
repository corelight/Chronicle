.. _ref_logs_amqp:

amqp
----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - Time

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - Unique ID for the connection

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
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - Is orig info

   * - ``ver_maj`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - AMQP specific fields

   * - ``ver_min`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The ver_min information.

   * - ``ver_rev`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The ver_rev information.

   * - ``host`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The host information.

   * - ``name`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The name information.

   * - ``product`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The product information.

   * - ``version`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The version information.

   * - ``copyright`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The copyright information.

   * - ``platform`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The platform information.

   * - ``information`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The information information.

   * - ``instance`` (string)
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - The instance information.

   * - ``delivered_exchanges`` (array[string] - set[string])
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - Exchanges seen in basic.publish messages

   * - ``published_exchanges`` (array[string] - set[string])
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - Exchanges seen in basic.deliver messages

   * - ``consumed_queues`` (array[string] - set[string])
     - site/packages/corelight/packages/zeek-spicy-amqp/main.zeek
     - Queues seen in basic.consume messages
