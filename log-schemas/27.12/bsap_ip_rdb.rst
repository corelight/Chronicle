.. _ref_logs_bsap_ip_rdb:

bsap_ip_rdb
-----------
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

   * - ``header_size`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - Unique ID for the connection.

   * - ``mes_seq`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The connection's 4-tuple of endpoint addresses/ports.

   * - ``res_seq`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The res_seq information.

   * - ``data_len`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The data_len information.

   * - ``sequence`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The sequence information.

   * - ``app_func_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The app_func_code information.

   * - ``node_status`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The node_status information.

   * - ``func_code`` (string)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The func_code information.

   * - ``variable_count`` (integer - count)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The variable_count information.

   * - ``variables`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The variables information.

   * - ``variable_value`` (array[string] - vector of string)
     - site/packages/corelight/packages/zeek-plugin-bsap/main.zeek
     - The variable_value information.
