``ipsec`` field reference
-------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The ts information.

   * - ``uid`` (string)
     - The uid information.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``is_orig`` (boolean - bool)
     - The is_orig information.

   * - ``initiator_spi`` (string)
     - Initiator security parameters index

   * - ``responder_spi`` (string)
     - Responder security parameters index

   * - ``maj_ver`` (integer - count)
     - Major Version

   * - ``min_ver`` (integer - count)
     - Minor Version

   * - ``exchange_type`` (integer - count)
     - Exchange Type

   * - ``flag_e`` (boolean - bool)
     - Flag E

   * - ``flag_c`` (boolean - bool)
     - Flag C

   * - ``flag_a`` (boolean - bool)
     - Flag A

   * - ``flag_i`` (boolean - bool)
     - Flag I

   * - ``flag_v`` (boolean - bool)
     - Flag V

   * - ``flag_r`` (boolean - bool)
     - Flag R

   * - ``message_id`` (integer - count)
     - Message ID

   * - ``vendor_ids`` (array[string] - vector of string)
     - Vendor IDs

   * - ``notify_messages`` (array[string] - vector of string)
     - Notify Message Types

   * - ``transforms`` (array[string] - vector of string)
     - Transforms

   * - ``ke_dh_groups`` (array[integer] - vector of count)
     - KE DH Group number

   * - ``proposals`` (array[integer] - vector of count)
     - Proposals

   * - ``protocol_id`` (integer - count)
     - Protocol ID

   * - ``certificates`` (array[string] - vector of string)
     - Certificate hashes

   * - ``transform_attributes`` (array[string] - vector of string)
     - Transform Attributes

   * - ``length`` (integer - count)
     - Length of headers plus payload

   * - ``hash`` (string)
     - Cipher hash of this IPSec transaction info:
       vendor_ids, notify_messages, transforms, ke_dh_groups, and proposals

   * - ``doi`` (integer - count)
     - DOI value

   * - ``situation`` (string)
     - Situation value
