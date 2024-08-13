.. _ref_logs_gena:

gena
----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - Time

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
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
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - Is orig side of connection

   * - ``proto`` (string - enum transport_proto)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The protcol.

   * - ``operation`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The operation

   * - ``pub_path`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The publication path

   * - ``status_code`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The status code

   * - ``http_ver`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The HTTP version

   * - ``host`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The host

   * - ``usn`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The USN

   * - ``target`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The target (notification or search)

   * - ``target_sub`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The target sub type

   * - ``sid`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The subscription ID

   * - ``seq`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The sequence

   * - ``callback`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The callback

   * - ``user_agent`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The user agent

   * - ``server`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The server info

   * - ``content_len`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - Content length

   * - ``transfer_encoding`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - Transfer encoding

   * - ``remaining_header_names`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - Remaining header names

   * - ``remaining_header_values`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - Remaining header values

   * - ``payload`` (string)
     - site/packages/corelight/packages/zeek-spicy-gena/main.zeek
     - The Payload
