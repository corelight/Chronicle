``etc_viz`` field reference
---------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - timestamp of the connection.

   * - ``uid`` (string)
     - The unique identifier of the connection.

   * - ``server_a`` (string - addr)
     - The address of the server in the connection.

   * - ``server_p`` (integer - port)
     - The port of the server in the connection.

   * - ``service`` (array[string] - set[string])
     - The service(s) associated with the connection.

   * - ``viz_stat`` (string)
     - The associated visibility status string.

   * - ``c2s_viz.size`` (integer - count)
     - The total size of the flow.

   * - ``c2s_viz.enc_dev`` (number - double)
     - TBD. of aggregated encrypted blocks.

   * - ``c2s_viz.enc_frac`` (number - double)
     - Proportion of flow (in terms of blocks) consistent
       with encryption.

   * - ``c2s_viz.pdu1_enc`` (boolean - bool)
     - Whether the first PDU (or a proxy for it) was consistent
       with being encrypted.

   * - ``c2s_viz.clr_frac`` (number - double)
     - Proportion of flow (in terms of blocks) consistent
       with clear-text.

   * - ``c2s_viz.clr_ex`` (string)
     - For flows with some clear-text, a snippet.

   * - ``s2c_viz.size`` (integer - count)
     - The total size of the flow.

   * - ``s2c_viz.enc_dev`` (number - double)
     - TBD. of aggregated encrypted blocks.

   * - ``s2c_viz.enc_frac`` (number - double)
     - Proportion of flow (in terms of blocks) consistent
       with encryption.

   * - ``s2c_viz.pdu1_enc`` (boolean - bool)
     - Whether the first PDU (or a proxy for it) was consistent
       with being encrypted.

   * - ``s2c_viz.clr_frac`` (number - double)
     - Proportion of flow (in terms of blocks) consistent
       with clear-text.

   * - ``s2c_viz.clr_ex`` (string)
     - For flows with some clear-text, a snippet.
