.. _ref_logs_telnet:

telnet
------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - Timestamp for when the activity happened.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - Unique ID for the connection.

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

   * - ``tn3270`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - If this Telnet session is also TN3270.

   * - ``tn3270e`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - If this Telnet session is also TN3270E.

   * - ``terminal_type`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - Terminal Type.

   * - ``terminal_speed`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - Terminal Speed.

   * - ``x_display_location`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - X Display Location.

   * - ``environ_value_names`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - Names to environment variables, in order.

   * - ``environ_value_values`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - Values to environment variables, in order.

   * - ``tn3270e_device_type_request`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - The device type provided in a device type request.

   * - ``tn3270e_device_type_request_associate`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - The associate value provided in a device type request.

   * - ``tn3270e_device_type_request_connect`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - The connect value provided in a device type request.

   * - ``tn3270e_device_type_is`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - The device type reply to a request.

   * - ``tn3270e_device_type_is_associate`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - The associate value provided in a device type reply to a request.

   * - ``tn3270e_device_type_is_connect`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - The connect value provided in a device type reply to a request.

   * - ``data`` (string)
     - site/packages/corelight/packages/zeek-spicy-telnet/main.zeek
     - The first few bytes from the connection.
