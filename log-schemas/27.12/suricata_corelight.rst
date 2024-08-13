.. _ref_logs_suricata_corelight:

suricata_corelight
------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The Suricata alert timestamp

   * - ``uid`` (string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The conn log identifier [from conn.log].

   * - ``id.orig_h`` (string - addr)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The id.orig_h information.

   * - ``id.orig_p`` (integer - port)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The id.orig_p information.

   * - ``id.resp_h`` (string - addr)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The id.resp_h information.

   * - ``id.resp_p`` (integer - port)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The id.resp_p information.

   * - ``id.vlan`` (integer - count)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The id.vlan information.

   * - ``id.vlan_inner`` (integer - count)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The id.vlan_inner information.

   * - ``icmp_type`` (integer - count)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The icmp type if this was ICMP.

   * - ``icmp_code`` (integer - count)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The icmp code if this was ICMP.

   * - ``suri_id`` (string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The Suricata log id.

   * - ``service`` (string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The service name (e.g., http)

   * - ``flow_id`` (integer - count)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The flow id

   * - ``tx_id`` (integer - count)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The transaction id

   * - ``pcap_cnt`` (integer - count)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The pcap record count

   * - ``alert.action`` (string)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.action information.

   * - ``alert.gid`` (integer - count)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.gid information.

   * - ``alert.signature_id`` (integer - count)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.signature_id information.

   * - ``alert.rev`` (integer - count)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.rev information.

   * - ``alert.signature`` (string)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.signature information.

   * - ``alert.category`` (string)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.category information.

   * - ``alert.severity`` (integer - count)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.severity information.

   * - ``alert.metadata`` (array[string] - vector of string)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.metadata information.

   * - ``alert.rule`` (string)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.rule information.

   * - ``alert.references`` (array[string] - vector of string)
     - Corelight_Suricata/scripts/types.zeek
     - The alert.references information.

   * - ``community_id`` (string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The community id

   * - ``payload`` (string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The payload

   * - ``packet`` (string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The packet

   * - ``payload_printable`` (string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - The printable payload

   * - ``metadata`` (array[string] - vector of string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - Alert metadata, if any

   * - ``references`` (array[string] - vector of string)
     - Corelight_Suricata/scripts/Corelight/Suricata/suricata.zeek
     - Alert references, if any

   * - ``orig_vulnerable_host.cve`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The ID of the known CVE on the vulnerable host.

   * - ``orig_vulnerable_host.hostname`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The hostname of the vulnerable host.

   * - ``orig_vulnerable_host.host_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The unique identifier, assigned by the CVE information source, of the vulnerable host.

   * - ``orig_vulnerable_host.machine_domain`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The machine domain of the vulnerable host.

   * - ``orig_vulnerable_host.os_version`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The Operating System version of the vulnerable host.

   * - ``orig_vulnerable_host.source`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The source of the CVE information.

   * - ``orig_vulnerable_host.criticality`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The criticality of the host.

   * - ``resp_vulnerable_host.cve`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The ID of the known CVE on the vulnerable host.

   * - ``resp_vulnerable_host.hostname`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The hostname of the vulnerable host.

   * - ``resp_vulnerable_host.host_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The unique identifier, assigned by the CVE information source, of the vulnerable host.

   * - ``resp_vulnerable_host.machine_domain`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The machine domain of the vulnerable host.

   * - ``resp_vulnerable_host.os_version`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The Operating System version of the vulnerable host.

   * - ``resp_vulnerable_host.source`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The source of the CVE information.

   * - ``resp_vulnerable_host.criticality`` (string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The criticality of the host.

   * - ``meta`` (array[string] - vector of string)
     - site/packages/customer-bundle/packages/Zeek-CVE-Enrichment/enrich.zeek
     - The meta information.
