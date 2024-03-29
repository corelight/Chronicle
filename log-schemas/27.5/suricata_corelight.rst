``suricata_corelight`` field reference
--------------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The Suricata alert timestamp

   * - ``uid`` (string)
     - The conn log identifier [from conn.log].

   * - ``id.orig_h`` (string - addr)
     - The id.orig_h information.

   * - ``id.orig_p`` (integer - port)
     - The id.orig_p information.

   * - ``id.resp_h`` (string - addr)
     - The id.resp_h information.

   * - ``id.resp_p`` (integer - port)
     - The id.resp_p information.

   * - ``id.vlan`` (integer - count)
     - The id.vlan information.

   * - ``id.vlan_inner`` (integer - count)
     - The id.vlan_inner information.

   * - ``icmp_type`` (integer - count)
     - The icmp type if this was ICMP.

   * - ``icmp_code`` (integer - count)
     - The icmp code if this was ICMP.

   * - ``suri_id`` (string)
     - The Suricata log id.

   * - ``service`` (string)
     - The service name (e.g., http)

   * - ``flow_id`` (integer - count)
     - The flow id

   * - ``tx_id`` (integer - count)
     - The transaction id

   * - ``pcap_cnt`` (integer - count)
     - The pcap record count

   * - ``alert.action`` (string)
     - The alert.action information.

   * - ``alert.gid`` (integer - count)
     - The alert.gid information.

   * - ``alert.signature_id`` (integer - count)
     - The alert.signature_id information.

   * - ``alert.rev`` (integer - count)
     - The alert.rev information.

   * - ``alert.signature`` (string)
     - The alert.signature information.

   * - ``alert.category`` (string)
     - The alert.category information.

   * - ``alert.severity`` (integer - count)
     - The alert.severity information.

   * - ``alert.metadata`` (array[string] - vector of string)
     - The alert.metadata information.

   * - ``community_id`` (string)
     - The community id

   * - ``payload`` (string)
     - The payload

   * - ``packet`` (string)
     - The packet

   * - ``metadata`` (array[string] - vector of string)
     - Alert metadata, if any

   * - ``orig_cve`` (string)
     - The orig_cve information.

   * - ``resp_cve`` (string)
     - The resp_cve information.
