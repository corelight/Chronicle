.. _ref_logs_encrypted_dns:

encrypted_dns
-------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/encrypted_dns/main.zeek
     - The ts information.

   * - ``uid`` (string)
     - site/packages/corelight/packages/encrypted_dns/main.zeek
     - The uid information.

   * - ``resp_h`` (string - addr)
     - site/packages/corelight/packages/encrypted_dns/main.zeek
     - The resp_h information.

   * - ``cert.cn`` (string)
     - site/packages/corelight/packages/encrypted_dns/main.zeek
     - The cert.cn information.

   * - ``cert.sans`` (array[string] - set[string])
     - site/packages/corelight/packages/encrypted_dns/main.zeek
     - The cert.sans information.

   * - ``sni`` (string)
     - site/packages/corelight/packages/encrypted_dns/main.zeek
     - The sni information.

   * - ``match`` (string)
     - site/packages/corelight/packages/encrypted_dns/main.zeek
     - The match information.
