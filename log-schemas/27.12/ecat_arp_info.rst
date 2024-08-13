.. _ref_logs_ecat_arp_info:

ecat_arp_info
-------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - The ts information.

   * - ``arp_type`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Timestamp for when the event happened

   * - ``mac_src`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Arp command

   * - ``mac_dst`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Source Mac address

   * - ``SPA`` (string - addr)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Destination Mac address

   * - ``SHA`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Sender protocol address

   * - ``TPA`` (string - addr)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Sender hardware address

   * - ``THA`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Target protocol address
