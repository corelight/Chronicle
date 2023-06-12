``datared`` field reference
---------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The time at which Zeek reported this set of statistics.

   * - ``conn_red`` (integer - count)
     - The reduced number of conn log entries.

   * - ``conn_total`` (integer - count)
     - The original number of conn log entries.

   * - ``dns_red`` (integer - count)
     - The reduced number of DNS log entries.

   * - ``dns_total`` (integer - count)
     - The original number of DNS log entries.

   * - ``dns_coal_miss`` (integer - count)
     - The number of times we wanted to store additional DNS log
       entries for coalescence, but exceeded the storage budget.

   * - ``files_red`` (integer - count)
     - The reduced number of files log entries.

   * - ``files_total`` (integer - count)
     - The original number of files log entries.

   * - ``files_coal_miss`` (integer - count)
     - The number of times we wanted to store additional files log
       entries for coalescence, but exceeded the storage budget.

   * - ``http_red`` (integer - count)
     - The reduced number of HTTP log entries.

   * - ``http_total`` (integer - count)
     - The original number of HTTP log entries.

   * - ``ssl_red`` (integer - count)
     - The reduced number of SSL log entries.

   * - ``ssl_total`` (integer - count)
     - The original number of SSL log entries.

   * - ``ssl_coal_miss`` (integer - count)
     - The number of times we wanted to store additional SSL log
       entries for coalescence, but exceeded the storage budget.

   * - ``weird_red`` (integer - count)
     - The reduced number of weird log entries.

   * - ``weird_total`` (integer - count)
     - The original number of weird log entries.

   * - ``x509_red`` (integer - count)
     - The reduced number of X509 log entries.

   * - ``x509_total`` (integer - count)
     - The original number of X509 log entries.

   * - ``x509_coal_miss`` (integer - count)
     - The number of times we wanted to store additional x509 log
       entries for coalescence, but exceeded the storage budget.
