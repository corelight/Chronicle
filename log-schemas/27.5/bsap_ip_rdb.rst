``bsap_ip_rdb`` field reference
-------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The ts information.

   * - ``uid`` (string)
     - Timestamp for when the event happened.

   * - ``header_size`` (integer - count)
     - Unique ID for the connection.

   * - ``mes_seq`` (integer - count)
     - The connection's 4-tuple of endpoint addresses/ports.

   * - ``res_seq`` (integer - count)
     - The res_seq information.

   * - ``data_len`` (integer - count)
     - The data_len information.

   * - ``sequence`` (integer - count)
     - The sequence information.

   * - ``app_func_code`` (string)
     - The app_func_code information.

   * - ``node_status`` (integer - count)
     - The node_status information.

   * - ``func_code`` (string)
     - The func_code information.

   * - ``variable_count`` (integer - count)
     - The variable_count information.

   * - ``variables`` (array[string] - vector of string)
     - The variables information.

   * - ``variable_value`` (array[string] - vector of string)
     - The variable_value information.
