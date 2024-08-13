.. _ref_logs_etc_viz:

etc_viz
-------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - site/packages/corelight/packages/encryption_detection/main.zeek
     - timestamp of the connection.

   * - ``uid`` (string)
     - site/packages/corelight/packages/encryption_detection/main.zeek
     - The unique identifier of the connection.

   * - ``server_a`` (string - addr)
     - site/packages/corelight/packages/encryption_detection/main.zeek
     - The address of the server in the connection.

   * - ``server_p`` (integer - port)
     - site/packages/corelight/packages/encryption_detection/main.zeek
     - The port of the server in the connection.

   * - ``service`` (array[string] - set[string])
     - site/packages/corelight/packages/encryption_detection/main.zeek
     - The service(s) associated with the connection.

   * - ``viz_stat`` (string)
     - site/packages/corelight/packages/encryption_detection/main.zeek
     - The associated visibility status string.

   * - ``c2s_viz.size`` (integer - count)
     - encryption_detection/scripts/types.zeek
     - The total size of the flow.

   * - ``c2s_viz.enc_dev`` (number - double)
     - encryption_detection/scripts/types.zeek
     - TBD. of aggregated encrypted blocks.

   * - ``c2s_viz.enc_frac`` (number - double)
     - encryption_detection/scripts/types.zeek
     - Proportion of flow (in terms of blocks) consistent
       with encryption.

   * - ``c2s_viz.pdu1_enc`` (boolean - bool)
     - encryption_detection/scripts/types.zeek
     - Whether the first PDU (or a proxy for it) was consistent
       with being encrypted.

   * - ``c2s_viz.clr_frac`` (number - double)
     - encryption_detection/scripts/types.zeek
     - Proportion of flow (in terms of blocks) consistent
       with clear-text.

   * - ``c2s_viz.clr_ex`` (string)
     - encryption_detection/scripts/types.zeek
     - For flows with some clear-text, a snippet.

   * - ``s2c_viz.size`` (integer - count)
     - encryption_detection/scripts/types.zeek
     - The total size of the flow.

   * - ``s2c_viz.enc_dev`` (number - double)
     - encryption_detection/scripts/types.zeek
     - TBD. of aggregated encrypted blocks.

   * - ``s2c_viz.enc_frac`` (number - double)
     - encryption_detection/scripts/types.zeek
     - Proportion of flow (in terms of blocks) consistent
       with encryption.

   * - ``s2c_viz.pdu1_enc`` (boolean - bool)
     - encryption_detection/scripts/types.zeek
     - Whether the first PDU (or a proxy for it) was consistent
       with being encrypted.

   * - ``s2c_viz.clr_frac`` (number - double)
     - encryption_detection/scripts/types.zeek
     - Proportion of flow (in terms of blocks) consistent
       with clear-text.

   * - ``s2c_viz.clr_ex`` (string)
     - encryption_detection/scripts/types.zeek
     - For flows with some clear-text, a snippet.
