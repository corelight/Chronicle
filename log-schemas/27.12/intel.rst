.. _ref_logs_intel:

intel
-----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Timestamp when the data was discovered.

   * - ``uid`` (string)
     - base
     - If a connection was associated with this intelligence hit,
       this is the uid for the connection

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

   * - ``seen.indicator`` (string)
     - base
     - The string if the data is about a string.

   * - ``seen.indicator_type`` (string - enum Intel::Type)
     - base
     - The type of data that the indicator represents.

   * - ``seen.where`` (string - enum Intel::Where)
     - base
     - Where the data was discovered.

   * - ``matched`` (array[string] - set[enum Intel::Type])
     - base
     - Which indicator types matched.

   * - ``sources`` (array[string] - set[string])
     - base
     - Sources which supplied data that resulted in this match.

   * - ``fuid`` (string)
     - base
     - If a file was associated with this intelligence hit,
       this is the uid for the file.

   * - ``file_mime_type`` (string)
     - base
     - A mime type if the intelligence hit is related to a file.
       If the $f field is provided this will be automatically filled
       out.

   * - ``file_desc`` (string)
     - base
     - Frequently files can be "described" to give a bit more context.
       If the $f field is provided this field will be automatically
       filled out.

   * - ``desc`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - The description or source of the intel.

   * - ``url`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - The URL to find more information about the indicator.

   * - ``confidence`` (array[number] - set[double])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - IC-Score: A 0-100 rating, representing the source of the intel's confidence that a particular indicator represents malicious activity.

   * - ``threat_score`` (array[number] - set[double])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - Theat Score is an analytical score from 0-100 that reflects the likelihood of a threat being malicious to an organization.  It is based on Intelligence factors such as threat severity and confidence.

   * - ``verdict`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - The verdict tells you if the determination was malicious or benign.

   * - ``verdict_source`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - The verdict tells you if the verdict was determined by machine learning or an analyst.

   * - ``firstseen`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - The first time this indicator was observed by any of the listed sources.

   * - ``lastseen`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - The most recent time this indicator was observed by any of the listed sources.

   * - ``associated`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - A list of actors associated with this indicator.

   * - ``category`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - A list of categories, as defined by the source, for this indicator.

   * - ``campaigns`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - A list of any known campaigns related to the indicator.

   * - ``reports`` (array[string] - set[string])
     - site/packages/customer-bundle/packages/ExtendIntel/main.zeek
     - A list of any reports relavent to the indicator.
