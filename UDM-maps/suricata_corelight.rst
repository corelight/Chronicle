``suricata_corelight`` UDM Map Reference
----------------------------------------

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
     - replace with 'SCAN_NETWORK'

   * -
     - ``metadata_product_name``
     - replace with 'Suricata'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - The Suricata alert timestamp.

   * - ``uid`` (string)
     - ``metadata_product_log_id``
     - The conn log identifier [from conn.log].

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

   * - ``id.vlan`` (integer - count)
     -
     - The id.vlan information.

   * - ``id.vlan_inner`` (integer - count)
     -
     - The id.vlan_inner information.

   * - ``icmp_type`` (integer - count)
     -
     - The icmp type if this was ICMP.

   * - ``icmp_code`` (integer - count)
     -
     - The icmp code if this was ICMP.

   * - ``suri_id`` (string)
     -
     - The Suricata log id.

   * - ``service`` (string)
     -
     - The service name (e.g., http)

   * - ``flow_id`` (integer - count)
     -
     - The flow id

   * - ``tx_id`` (integer - count)
     -
     - The transaction id

   * - ``pcap_cnt`` (integer - count)
     -
     - The pcap record count

   * - ``alert.action`` (string)
     -
     - The alert.action information.

   * - ``alert.gid`` (integer - count)
     -
     - The alert.gid information.

   * - ``alert.signature_id`` (integer - count)
     - ``security_result.rule_id`` (string)
     - The alert.signature_id information.

   * - ``alert.rev`` (integer - count)
     -
     - The alert.rev information.

   * - ``alert.signature`` (string)
     - ``metadata_product_event_type``
     - The alert.signature information.

   * - ``alert.signature`` (string)
     - ``security_result.summary``
     - The alert.signature information.

   * - ``alert.signature`` (string)
     - ``security_result.threat_name``
     - The alert.signature information.

   * - ``alert.category`` (string)
     - ``sr_category``
     - The alert.category information.

   * - ``alert.severity`` (integer - count)
     - ``security_result.severity_details`` (string)
     - The alert.severity information.

   * - ``alert.metadata`` (array[string] - vector of string)
     -
     - The alert.metadata information.

   * - ``community_id`` (string)
     -
     - The community id

   * - ``payload`` (string)
     -
     - The payload

   * - ``packet`` (string)
     -
     - The packet

   * - ``metadata`` (array[string] - vector of string)
     -
     - Alert metadata, if any

   * - ``orig_cve`` (string)
     -
     - The orig_cve information. Requires the zeek_suricata_cve_enrichment package.

   * - ``resp_cve`` (string)
     -
     - The resp_cve information. Requires the zeek_suricata_cve_enrichment package.
