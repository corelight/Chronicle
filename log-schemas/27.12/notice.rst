.. _ref_logs_notice:

notice
------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - An absolute time indicating when the notice occurred,
       defaults to the current network time.

   * - ``uid`` (string)
     - base
     - A connection UID which uniquely identifies the endpoints
       concerned with the notice.

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

   * - ``fuid`` (string)
     - base
     - A file unique ID if this notice is related to a file.  If
       the *f* field is provided, this will be automatically filled
       out.

   * - ``file_mime_type`` (string)
     - base
     - A mime type if the notice is related to a file.  If the *f*
       field is provided, this will be automatically filled out.

   * - ``file_desc`` (string)
     - base
     - Frequently files can be "described" to give a bit more
       context.  This field will typically be automatically filled
       out from an fa_file record.  For example, if a notice was
       related to a file over HTTP, the URL of the request would
       be shown.

   * - ``proto`` (string - enum transport_proto)
     - base
     - The transport protocol. Filled automatically when either
       *conn*, *iconn* or *p* is specified.

   * - ``note`` (string - enum Notice::Type)
     - base
     - The `Notice::Type` of the notice.

   * - ``msg`` (string)
     - base
     - The human readable message for the notice.

   * - ``sub`` (string)
     - base
     - The human readable sub-message.

   * - ``src`` (string - addr)
     - base
     - Source address, if we don't have a `conn_id`.

   * - ``dst`` (string - addr)
     - base
     - Destination address.

   * - ``p`` (integer - port)
     - base
     - Associated port, if we don't have a `conn_id`.

   * - ``n`` (integer - count)
     - base
     - Associated count, or perhaps a status code.

   * - ``peer_descr`` (string)
     - base
     - Textual description for the peer that raised this notice,
       including name, host address and port.

   * - ``actions`` (array[string] - set[enum Notice::Action])
     - base
     - The actions which have been applied to this notice.

   * - ``suppress_for`` (number - interval)
     - base
     - This field indicates the length of time that this
       unique notice should be suppressed.

   * - ``remote_location.country_code`` (string)
     - base
     - The country code.

   * - ``remote_location.region`` (string)
     - base
     - The region.

   * - ``remote_location.city`` (string)
     - base
     - The city.

   * - ``remote_location.latitude`` (number - double)
     - base
     - Latitude.

   * - ``remote_location.longitude`` (number - double)
     - base
     - Longitude.

   * - ``severity.level`` (integer - count)
     - site/packages/corelight/packages/notice-severity/main.zeek
     - The severity.level information.

   * - ``severity.name`` (string)
     - site/packages/corelight/packages/notice-severity/main.zeek
     - The severity.name information.

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
