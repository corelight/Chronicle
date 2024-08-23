.. _ref_logs_rdp:

rdp
---
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Timestamp for when the event happened.

   * - ``uid`` (string)
     - base
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

   * - ``cookie`` (string)
     - base
     - Cookie value used by the client machine.
       This is typically a username.

   * - ``result`` (string)
     - base
     - Status result for the connection.  It's a mix between
       RDP negotiation failure messages and GCC server create
       response messages.

   * - ``security_protocol`` (string)
     - base
     - Security protocol chosen by the server.

   * - ``client_channels`` (array[string] - vector of string)
     - base
     - The channels requested by the client

   * - ``keyboard_layout`` (string)
     - base
     - Keyboard layout (language) of the client machine.

   * - ``client_build`` (string)
     - base
     - RDP client version used by the client machine.

   * - ``client_name`` (string)
     - base
     - Name of the client machine.

   * - ``client_dig_product_id`` (string)
     - base
     - Product ID of the client machine.

   * - ``desktop_width`` (integer - count)
     - base
     - Desktop width of the client machine.

   * - ``desktop_height`` (integer - count)
     - base
     - Desktop height of the client machine.

   * - ``requested_color_depth`` (string)
     - base
     - The color depth requested by the client in
       the high_color_depth field.

   * - ``cert_type`` (string)
     - base
     - If the connection is being encrypted with native
       RDP encryption, this is the type of cert
       being used.

   * - ``cert_count`` (integer - count)
     - base
     - The number of certs seen.  X.509 can transfer an
       entire certificate chain.

   * - ``cert_permanent`` (boolean - bool)
     - base
     - Indicates if the provided certificate or certificate
       chain is permanent or temporary.

   * - ``encryption_level`` (string)
     - base
     - Encryption level of the connection.

   * - ``encryption_method`` (string)
     - base
     - Encryption method of the connection.

   * - ``auth_success`` (boolean - bool)
     - site/packages/corelight/packages/rdp-inference/setup.zeek
     - Whether the client successfully authenticated or not

   * - ``channels_joined`` (integer - int)
     - site/packages/corelight/packages/rdp-inference/setup.zeek
     - The number of channels a client joined during the connection sequence

   * - ``inferences`` (array[string] - set[string])
     - site/packages/corelight/packages/rdp-inference/setup.zeek
     - A set of inference "tags" about the connection

   * - ``rdpeudp_uid`` (string)
     - site/packages/corelight/packages/rdp-inference/setup.zeek
     - The connection UID of the UDP connection which assisted this TCP connection. If UDP was not used, this is unset.

   * - ``rdfp_string`` (string)
     - site/packages/corelight/packages/rdp-inference/setup.zeek
     - A fingerprint which represents am RDP client

   * - ``rdfp_hash`` (string)
     - site/packages/corelight/packages/rdp-inference/setup.zeek
     - The rdfp_hash information.
