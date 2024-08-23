.. _ref_logs_smtp:

smtp
----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Time when the message was first seen.

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

   * - ``trans_depth`` (integer - count)
     - base
     - A count to represent the depth of this message transaction in
       a single connection where multiple messages were transferred.

   * - ``helo`` (string)
     - base
     - Contents of the Helo header.

   * - ``mailfrom`` (string)
     - base
     - Email addresses found in the From header.

   * - ``rcptto`` (array[string] - set[string])
     - base
     - Email addresses found in the Rcpt header.

   * - ``date`` (string)
     - base
     - Contents of the Date header.

   * - ``from`` (string)
     - base
     - Contents of the From header.

   * - ``to`` (array[string] - set[string])
     - base
     - Contents of the To header.

   * - ``cc`` (array[string] - set[string])
     - base
     - Contents of the CC header.

   * - ``reply_to`` (string)
     - base
     - Contents of the ReplyTo header.

   * - ``msg_id`` (string)
     - base
     - Contents of the MsgID header.

   * - ``in_reply_to`` (string)
     - base
     - Contents of the In-Reply-To header.

   * - ``subject`` (string)
     - base
     - Contents of the Subject header.

   * - ``x_originating_ip`` (string - addr)
     - base
     - Contents of the X-Originating-IP header.

   * - ``first_received`` (string)
     - base
     - Contents of the first Received header.

   * - ``second_received`` (string)
     - base
     - Contents of the second Received header.

   * - ``last_reply`` (string)
     - base
     - The last message that the server sent to the client.

   * - ``path`` (array[string] - vector of addr)
     - base
     - The message transmission path, as extracted from the headers.

   * - ``user_agent`` (string)
     - base
     - Value of the User-Agent header from the client.

   * - ``tls`` (boolean - bool)
     - base
     - Indicates that the connection has switched to using TLS.

   * - ``fuids`` (array[string] - vector of string)
     - base
     - An ordered vector of file unique IDs seen attached to
       the message.

   * - ``is_webmail`` (boolean - bool)
     - policy/protocols/smtp/software.zeek
     - Boolean indicator of if the message was sent through a
       webmail interface.

   * - ``urls`` (array[string] - set[string])
     - site/packages/corelight/packages/smtp-links/log_urls.zeek
     - The URLs seen in the email.

   * - ``domains`` (array[string] - set[string])
     - site/packages/corelight/packages/smtp-links/log_domains.zeek
     - The URLs seen in the email.
