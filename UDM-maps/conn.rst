``conn`` UDM Map Reference
--------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 1 3

   * - Field (Type)
     - UDM Field (Type)
     - Description

   * -
     - ``metadata_vendor_name``
     - replace with 'Corelight'

   * -
     - ``metadata_event_type``
     - replace with 'NETWORK_CONNECTION'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - This is the time of the first packet.

   * - ``uid`` (string)
     - ``metadata_product_log_id``
     - A unique identifier of the connection.

   * - ``id.orig_h`` (string - addr)
     - ``principal_ip``
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - ``principal_port`` (string)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - ``target_ip``
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - ``target_port`` (string)
     - The responder's port number.

   * - ``proto`` (string - enum)
     - ``network_ip_protocol``
     - The transport layer protocol of the connection.

   * - ``service`` (string)
     - ``network_application_protocol``
     - An identification of an application protocol being sent over
       the connection.

   * - ``duration`` (number - interval)
     -
     - How long the connection lasted.  For 3-way or 4-way connection
       tear-downs, this will not include the final ACK.

   * - ``orig_bytes`` (integer - count)
     - ``network_sent_bytes`` (uinteger)
     - The number of payload bytes the originator sent. For TCP
       this is taken from sequence numbers and might be inaccurate
       (e.g., due to large connections).

   * - ``resp_bytes`` (integer - count)
     - ``network_received_bytes`` (uinteger)
     - The number of payload bytes the responder sent. See
       *orig_bytes*.

   * - ``conn_state`` (string)
     - ``metadata_description``
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
         SYN ACK from the responder (hence the connection was \""half\"" open).

       * SHR: Responder sent a SYN ACK followed by a FIN, we never saw a
         SYN from the originator.

       * OTH: No SYN seen, just midstream traffic (one example of this
         is a \""partial connection\"" that was not later closed).

   * - ``local_orig`` (boolean - bool)
     -
     - If the connection is originated locally, this value will be T.
       If it was originated remotely it will be F.  In the case that
       the `Site::local_nets` variable is undefined, this
       field will be left empty at all times.

   * - ``local_resp`` (boolean - bool)
     -
     - If the connection is responded to locally, this value will be T.
       If it was responded to remotely it will be F.  In the case that
       the `Site::local_nets` variable is undefined, this
       field will be left empty at all times.

   * - ``missed_bytes`` (integer - count)
     -
     - Indicates the number of bytes missed in content gaps, which
       is representative of packet loss.  A value other than zero
       will normally cause protocol analysis to fail but some
       analysis may have been completed prior to the packet loss.

   * - ``history`` (string)
     -
     - Records the state history of connections as a string of
       letters.  The meaning of those letters is:


       * s: a SYN w/o the ACK bit set
       * h: a SYN+ACK (\""handshake\"")
       * a: a pure ACK
       * d: packet with payload (\""data\"")
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
     -
     - Number of packets that the originator sent.
       Only set if `use_conn_size_analyzer` = T.

   * - ``orig_ip_bytes`` (integer - count)
     -
     - Number of IP level bytes that the originator sent (as seen on
       the wire, taken from the IP total_length header field).
       Only set if `use_conn_size_analyzer` = T.

   * - ``resp_pkts`` (integer - count)
     -
     - Number of packets that the responder sent.
       Only set if `use_conn_size_analyzer` = T.

   * - ``resp_ip_bytes`` (integer - count)
     -
     - Number of IP level bytes that the responder sent (as seen on
       the wire, taken from the IP total_length header field).
       Only set if `use_conn_size_analyzer` = T.

   * - ``tunnel_parents`` (array[string] - set[string])
     -
     - If this connection was over a tunnel, indicate the
       *uid* values for any encapsulating parent connections
       used over the lifetime of this inner connection.

   * - ``orig_cc`` (string)
     -
     - The name of the node where this connection was analyzed.
       Country code for GeoIP lookup of the originating IP address.

   * - ``resp_cc`` (string)
     -
     - Country code for GeoIP lookup of the responding IP address.

   * - ``suri_ids`` (array[string] - set[string])
     -
     - The suri_ids information.

   * - ``spcap.url`` (string)
     -
     - The spcap.url information.

   * - ``spcap.rule`` (integer - count)
     -
     - The spcap.rule information.

   * - ``spcap.trigger`` (string)
     -
     - The spcap.trigger information.

   * - ``app`` (array[string] - vector of string)
     -
     - The app information.

   * - ``corelight_shunted`` (boolean - bool)
     -
     - The corelight_shunted information.

   * - ``orig_shunted_pkts`` (integer - count)
     -
     - The orig_shunted_pkts information.

   * - ``orig_shunted_bytes`` (integer - count)
     -
     - The orig_shunted_bytes information.

   * - ``resp_shunted_pkts`` (integer - count)
     -
     - The resp_shunted_pkts information.

   * - ``resp_shunted_bytes`` (integer - count)
     -
     - The resp_shunted_bytes information.

   * - ``orig_l2_addr`` (string)
     -
     - Link-layer address of the originator, if available.

   * - ``resp_l2_addr`` (string)
     -
     - Link-layer address of the responder, if available.

   * - ``id_orig_h_n.src`` (string)
     -
     - How we determined the name/address pair. Either
       ``DNS_A`` representing the DNS_A* family of query types,
       or ``DNS_PTR`` for reverse DNS lookups.

   * - ``id_orig_h_n.vals`` (array[string] - set[string])
     -
     - The set of names we observed for a given address.

   * - ``id_resp_h_n.src`` (string)
     -
     - How we determined the name/address pair. Either
       ``DNS_A`` representing the DNS_A* family of query types,
       or ``DNS_PTR`` for reverse DNS lookups.

   * - ``id_resp_h_n.vals`` (array[string] - set[string])
     -
     - The set of names we observed for a given address.

   * - ``vlan`` (integer - int)
     -
     - The outer VLAN for this connection, if applicable.

   * - ``inner_vlan`` (integer - int)
     -
     - The inner VLAN for this connection, if applicable.

   * - ``community_id`` (string)
     - ``event1.idm.read_only_udm.network.community_id``
     - The community_id information.
