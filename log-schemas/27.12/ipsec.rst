.. _ref_logs_ipsec:

ipsec
-----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - The uid information.

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

   * - ``is_orig`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - The is_orig information.

   * - ``initiator_spi`` (string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Initiator security parameters index

   * - ``responder_spi`` (string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Responder security parameters index

   * - ``maj_ver`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Major Version

   * - ``min_ver`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Minor Version

   * - ``exchange_type`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Exchange Type

   * - ``flag_e`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Flag E

   * - ``flag_c`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Flag C

   * - ``flag_a`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Flag A

   * - ``flag_i`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Flag I

   * - ``flag_v`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Flag V

   * - ``flag_r`` (boolean - bool)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Flag R

   * - ``message_id`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Message ID

   * - ``vendor_ids`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Vendor IDs

   * - ``notify_messages`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Notify Message Types

   * - ``transforms`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Transforms

   * - ``ke_dh_groups`` (array[integer] - vector of count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - KE DH Group number

   * - ``proposals`` (array[integer] - vector of count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Proposals

   * - ``protocol_id`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Protocol ID

   * - ``certificates`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Certificate hashes

   * - ``transform_attributes`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Transform Attributes

   * - ``length`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Length of headers plus payload

   * - ``hash`` (string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Cipher hash of this IPSec transaction info:
       vendor_ids, notify_messages, transforms, ke_dh_groups, and proposals

   * - ``doi`` (integer - count)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - DOI value

   * - ``situation`` (string)
     - site/packages/corelight/packages/zeek-spicy-ipsec/main.zeek
     - Situation value
