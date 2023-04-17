``dns`` UDM map reference
-------------------------

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
     - replace with 'NETWORK_DNS'

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

   * - ``trans_id`` (integer - count)
     -
     - A 16-bit identifier assigned by the program that generated
       the DNS query.  Also used in responses to match up replies to
       outstanding queries.

   * - ``rtt`` (number - interval)
     -
     - Round trip time for the query and response. This indicates
       the delay between when the request was seen until the
       answer started.

   * - ``query`` (string)
     - ``dns_question.name``
     - The domain name that is the subject of the DNS query.

   * - ``qclass`` (integer - count)
     - ``dns_question.class`` (uinteger)
     - The QCLASS value specifying the class of the query.

   * - ``qclass_name`` (string)
     - ``metadata_description``
     - A descriptive name for the class of the query.

   * - ``qtype`` (integer - count)
     - ``dns_question.type`` (uinteger)
     - A QTYPE value specifying the type of the query.

   * - ``qtype_name`` (string)
     -
     - A descriptive name for the type of the query.

   * - ``rcode`` (integer - count)
     - ``network_dns_response_code`` (uinteger)
     - The response code value in DNS response messages.

   * - ``rcode_name`` (string)
     -
     - A descriptive name for the response code value.

   * - ``AA`` (boolean - bool)
     - ``dns.authoritative``
     - The Authoritative Answer bit for response messages specifies
       that the responding name server is an authority for the
       domain name in the question section.

   * - ``TC`` (boolean - bool)
     - ``dns.truncated``
     - The Truncation bit specifies that the message was truncated.

   * - ``RD`` (boolean - bool)
     - ``dns.recursion_desired``
     - The Recursion Desired bit in a request message indicates that
       the client wants recursive service for this query.

   * - ``RA`` (boolean - bool)
     - ``dns.recursion_available``
     - The Recursion Available bit in a response message indicates
       that the name server supports recursive queries.

   * - ``Z`` (integer - count)
     -
     - A reserved field that is usually zero in
       queries and responses.

   * - ``answers`` (array[string] - vector of string)
     - ``dns_answer.name`` (vector of string)
     - The set of resource descriptions in the query answer.

   * - ``TTLs`` (array[number] - vector of interval)
     -  (vector of interval)
     - The caching intervals of the associated RRs described by the
       *answers* field.

   * - ``rejected`` (boolean - bool)
     -
     - The DNS query was rejected by the server.

   * - ``is_trusted_domain`` (string)
     -
     - The is_trusted_domain information. Requires the icannTLD package.

   * - ``icann_host_subdomain`` (string)
     -
     - The host or subdomain information based on publicsuffix.org. Requires the icannTLD package.

   * - ``icann_domain`` (string)
     - ``event1.idm.read_only_udm.network.dns_domain``
     - The Domain information based on publicsuffix.org. Requires the icannTLD package.

   * - ``icann_tld`` (string)
     -
     - The Top-level Domain information from publicsuffix.org. Requires the icannTLD package.
