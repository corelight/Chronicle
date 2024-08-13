.. _ref_logs_ecat_registers:

ecat_registers
--------------
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

   * - ``srcmac`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Timestamp for when the event happened

   * - ``dstmac`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Source Mac Address

   * - ``Command`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Destination Mac Address

   * - ``Slave_Addr`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Ethercat Command

   * - ``Register_Type`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Ethercat Slave Address

   * - ``Register_Addr`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Register Information

   * - ``data`` (string)
     - site/packages/corelight/packages/zeek-plugin-ethercat/main.zeek
     - Memory Address being accessed
