.. _ref_logs_conn_long:

conn_long
---------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - This is the time of the first packet.

   * - ``uid`` (string)
     - base
     - A unique identifier of the connection.

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

   * - ``proto`` (string - enum transport_proto)
     - base
     - The transport layer protocol of the connection.

   * - ``service`` (string)
     - base
     - An identification of an application protocol being sent over
       the connection.

   * - ``duration`` (number - interval)
     - base
     - How long the connection lasted.
       
       .. note:: The duration doesn't cover trailing "non-productive"
          TCP packets (i.e., ones not contributing new stream payload)
          once a direction is closed.  For example, for regular
          3-way/4-way connection tear-downs it doesn't include the
          final ACK.  The reason is largely historic: this approach
          allows more accurate computation of connection data rates.
          Zeek does however reflect such trailing packets in the
          connection history.

   * - ``orig_bytes`` (integer - count)
     - base
     - The number of payload bytes the originator sent. For TCP
       this is taken from sequence numbers and might be inaccurate
       (e.g., due to large connections).

   * - ``resp_bytes`` (integer - count)
     - base
     - The number of payload bytes the responder sent. See
       *orig_bytes*.

   * - ``conn_state`` (string)
     - base
     - Possible *conn_state* values:
       
       * S0: Connection attempt seen, no reply.
       
       * S1: Connection established, not terminated.
       
       * SF: Normal establishment and termination.
         Note that this is the same symbol as for state S1.
         You can tell the two apart because for S1 there will not be any
         byte counts in the summary, while for SF there will be.
       
       * REJ: Connection attempt rejected.
       
       * S2: Connection established and close attempt by originator seen
         (but no reply from responder).
       
       * S3: Connection established and close attempt by responder seen
         (but no reply from originator).
       
       * RSTO: Connection established, originator aborted (sent a RST).
       
       * RSTR: Responder sent a RST.
       
       * RSTOS0: Originator sent a SYN followed by a RST, we never saw a
         SYN-ACK from the responder.
       
       * RSTRH: Responder sent a SYN ACK followed by a RST, we never saw a
         SYN from the (purported) originator.
       
       * SH: Originator sent a SYN followed by a FIN, we never saw a
         SYN ACK from the responder (hence the connection was "half" open).
       
       * SHR: Responder sent a SYN ACK followed by a FIN, we never saw a
         SYN from the originator.
       
       * OTH: No SYN seen, just midstream traffic (one example of this
         is a "partial connection" that was not later closed).

   * - ``local_orig`` (boolean - bool)
     - base
     - If the connection is originated locally, this value will be T.
       If it was originated remotely it will be F.  In the case that
       the `Site::local_nets` variable is undefined, this
       field will be left empty at all times.

   * - ``local_resp`` (boolean - bool)
     - base
     - If the connection is responded to locally, this value will be T.
       If it was responded to remotely it will be F.  In the case that
       the `Site::local_nets` variable is undefined, this
       field will be left empty at all times.

   * - ``missed_bytes`` (integer - count)
     - base
     - Indicates the number of bytes missed in content gaps, which
       is representative of packet loss.  A value other than zero
       will normally cause protocol analysis to fail but some
       analysis may have been completed prior to the packet loss.

   * - ``history`` (string)
     - base
     - Records the state history of connections as a string of
       letters.  The meaning of those letters is:
       
       
       * s: a SYN w/o the ACK bit set
       * h: a SYN+ACK ("handshake")
       * a: a pure ACK
       * d: packet with payload ("data")
       * f: packet with FIN bit set
       * r: packet with RST bit set
       * c: packet with a bad checksum (applies to UDP too)
       * g: a content gap
       * t: packet with retransmitted payload
       * w: packet with a zero window advertisement
       * i: inconsistent packet (e.g. FIN+RST bits set)
       * q: multi-flag packet (SYN+FIN or SYN+RST bits set)
       * ^: connection direction was flipped by Zeek's heuristic
       
       
       If the event comes from the originator, the letter is in
       upper-case; if it comes from the responder, it's in
       lower-case.  The 'a', 'd', 'i' and 'q' flags are
       recorded a maximum of one time in either direction regardless
       of how many are actually seen.  'f', 'h', 'r' and
       's' can be recorded multiple times for either direction
       if the associated sequence number differs from the
       last-seen packet of the same flag type.
       'c', 'g', 't' and 'w' are recorded in a logarithmic fashion:
       the second instance represents that the event was seen
       (at least) 10 times; the third instance, 100 times; etc.

   * - ``orig_pkts`` (integer - count)
     - base
     - Number of packets that the originator sent.
       Only set if `use_conn_size_analyzer` = T.

   * - ``orig_ip_bytes`` (integer - count)
     - base
     - Number of IP level bytes that the originator sent (as seen on
       the wire, taken from the IP total_length header field).
       Only set if `use_conn_size_analyzer` = T.

   * - ``resp_pkts`` (integer - count)
     - base
     - Number of packets that the responder sent.
       Only set if `use_conn_size_analyzer` = T.

   * - ``resp_ip_bytes`` (integer - count)
     - base
     - Number of IP level bytes that the responder sent (as seen on
       the wire, taken from the IP total_length header field).
       Only set if `use_conn_size_analyzer` = T.

   * - ``tunnel_parents`` (array[string] - set[string])
     - base
     - If this connection was over a tunnel, indicate the
       *uid* values for any encapsulating parent connections
       used over the lifetime of this inner connection.

   * - ``orig_cc`` (string)
     - conn-decorate.zeek
     - The name of the node where this connection was analyzed.
       Country code for GeoIP lookup of the originating IP address.

   * - ``resp_cc`` (string)
     - conn-decorate.zeek
     - Country code for GeoIP lookup of the responding IP address.

   * - ``suri_ids`` (array[string] - set[string])
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The suri_ids information.

   * - ``app`` (array[string] - vector of string)
     - site/packages/corelight/packages/application-identification/log_recognizers.zeek
     - The app information.

   * - ``corelight_shunted`` (boolean - bool)
     - site/packages/corelight/packages/corelight-shunting/main.zeek
     - The corelight_shunted information.

   * - ``orig_shunted_pkts`` (integer - count)
     - site/packages/corelight/packages/corelight-shunting/main.zeek
     - The orig_shunted_pkts information.

   * - ``orig_shunted_bytes`` (integer - count)
     - site/packages/corelight/packages/corelight-shunting/main.zeek
     - The orig_shunted_bytes information.

   * - ``resp_shunted_pkts`` (integer - count)
     - site/packages/corelight/packages/corelight-shunting/main.zeek
     - The resp_shunted_pkts information.

   * - ``resp_shunted_bytes`` (integer - count)
     - site/packages/corelight/packages/corelight-shunting/main.zeek
     - The resp_shunted_bytes information.

   * - ``orig_l2_addr`` (string)
     - policy/protocols/conn/mac-logging.zeek
     - Link-layer address of the originator, if available.

   * - ``resp_l2_addr`` (string)
     - policy/protocols/conn/mac-logging.zeek
     - Link-layer address of the responder, if available.

   * - ``id_orig_h_n.src`` (string)
     - site/packages/corelight/packages/namecache/main.zeek
     - How we determined the name/address pair. Either
       ``DNS_A`` representing the DNS_A* family of query types,
       or ``DNS_PTR`` for reverse DNS lookups.

   * - ``id_orig_h_n.vals`` (array[string] - set[string])
     - site/packages/corelight/packages/namecache/main.zeek
     - The set of names we observed for a given address.

   * - ``id_resp_h_n.src`` (string)
     - site/packages/corelight/packages/namecache/main.zeek
     - How we determined the name/address pair. Either
       ``DNS_A`` representing the DNS_A* family of query types,
       or ``DNS_PTR`` for reverse DNS lookups.

   * - ``id_resp_h_n.vals`` (array[string] - set[string])
     - site/packages/corelight/packages/namecache/main.zeek
     - The set of names we observed for a given address.

   * - ``vlan`` (integer - int)
     - policy/protocols/conn/vlan-logging.zeek
     - The outer VLAN for this connection, if applicable.

   * - ``inner_vlan`` (integer - int)
     - policy/protocols/conn/vlan-logging.zeek
     - The inner VLAN for this connection, if applicable.

   * - ``community_id`` (string)
     - site/packages/corelight/packages/zeek-community-id/main.zeek
     - The community_id information.

   * - ``orig_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/conn.zeek
     - The status of the originator's endpoint agent.

   * - ``orig_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/conn.zeek
     - The originator's endpoint unique ID.

   * - ``orig_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/conn.zeek
     - The originator's endpoint Customer ID.

   * - ``orig_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/conn.zeek
     - The originator's endpoint information source.

   * - ``resp_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/conn.zeek
     - The status of the responder's endpoint agent.

   * - ``resp_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/conn.zeek
     - The responder's endpoint unique ID.

   * - ``resp_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/conn.zeek
     - The responder's endpoint Customer ID.

   * - ``resp_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/conn.zeek
     - The responder's endpoint information source.
