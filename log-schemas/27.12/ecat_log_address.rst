.. _ref_logs_ecat_log_address:

ecat_log_address
----------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - The ts information.

   * - ``srcmac`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Timestamp for when the event happened

   * - ``dstmac`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Source Mac Address

   * - ``Log_Addr`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Destination Mac Address

   * - ``Length`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Address data is being accessed from  

   * - ``Command`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Length of data

   * - ``data`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Ethercat Command
