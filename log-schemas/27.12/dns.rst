.. _ref_logs_dns:

dns
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
     - The earliest time at which a DNS protocol message over the
       associated connection is observed.

   * - ``uid`` (string)
     - base
     - A unique identifier of the connection over which DNS messages
       are being transferred.

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

   * - ``trans_id`` (integer - count)
     - base
     - A 16-bit identifier assigned by the program that generated
       the DNS query.  Also used in responses to match up replies to
       outstanding queries.

   * - ``rtt`` (number - interval)
     - base
     - Round trip time for the query and response. This indicates
       the delay between when the request was seen until the
       answer started.

   * - ``query`` (string)
     - base
     - The domain name that is the subject of the DNS query.

   * - ``qclass`` (integer - count)
     - base
     - The QCLASS value specifying the class of the query.

   * - ``qclass_name`` (string)
     - base
     - A descriptive name for the class of the query.

   * - ``qtype`` (integer - count)
     - base
     - A QTYPE value specifying the type of the query.

   * - ``qtype_name`` (string)
     - base
     - A descriptive name for the type of the query.

   * - ``rcode`` (integer - count)
     - base
     - The response code value in DNS response messages.

   * - ``rcode_name`` (string)
     - base
     - A descriptive name for the response code value.

   * - ``AA`` (boolean - bool)
     - base
     - The Authoritative Answer bit for response messages specifies
       that the responding name server is an authority for the
       domain name in the question section.

   * - ``TC`` (boolean - bool)
     - base
     - The Truncation bit specifies that the message was truncated.

   * - ``RD`` (boolean - bool)
     - base
     - The Recursion Desired bit in a request message indicates that
       the client wants recursive service for this query.

   * - ``RA`` (boolean - bool)
     - base
     - The Recursion Available bit in a response message indicates
       that the name server supports recursive queries.

   * - ``Z`` (integer - count)
     - base
     - A reserved field that is zero in queries and responses unless
       using DNSSEC. This field represents the 3-bit Z field using
       the specification from RFC 1035.

   * - ``answers`` (array[string] - vector of string)
     - base
     - The set of resource descriptions in the query answer.

   * - ``TTLs`` (array[number] - vector of interval)
     - base
     - The caching intervals of the associated RRs described by the
       *answers* field.

   * - ``rejected`` (boolean - bool)
     - base
     - The DNS query was rejected by the server.

   * - ``is_trusted_domain`` (string)
     - site/packages/customer-bundle/packages/icannTLD/main.zeek
     - Is the domain trusted based on a list of domains created manually.

   * - ``icann_host_subdomain`` (string)
     - site/packages/customer-bundle/packages/icannTLD/main.zeek
     - Based on the publicsuffix.org top level domain database, the remainder of the FQDN after the domain.
       This could be a hostname, or a subdomain with a hostname.

   * - ``icann_domain`` (string)
     - site/packages/customer-bundle/packages/icannTLD/main.zeek
     - The domain, based on the publicsuffix.org top level domain database.

   * - ``icann_tld`` (string)
     - site/packages/customer-bundle/packages/icannTLD/main.zeek
     - The top level domain, based on publicsuffix.org top level domain database.
