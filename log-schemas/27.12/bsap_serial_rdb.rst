.. _ref_logs_bsap_serial_rdb:

bsap_serial_rdb
---------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - Timestamp for when the event happened.

   * - ``func_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - Unique ID for the connection.

   * - ``variable_count`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The variable_count information.

   * - ``variables`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The variables information.

   * - ``variable_value`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The variable_value information.
