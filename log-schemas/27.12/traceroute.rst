.. _ref_logs_traceroute:

traceroute
----------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/detect-traceroute/detect-traceroute.zeek
     - Timestamp

   * - ``src`` (string - addr)
     - site/packages/corelight/packages/detect-traceroute/detect-traceroute.zeek
     - Address initiating the traceroute.

   * - ``dst`` (string - addr)
     - site/packages/corelight/packages/detect-traceroute/detect-traceroute.zeek
     - Destination address of the traceroute.

   * - ``proto`` (string)
     - site/packages/corelight/packages/detect-traceroute/detect-traceroute.zeek
     - Protocol used for the traceroute.
