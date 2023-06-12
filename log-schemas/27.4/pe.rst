``pe`` field reference
----------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Current timestamp.

   * - ``id`` (string)
     - File id of this portable executable file.

   * - ``machine`` (string)
     - The target machine that the file was compiled for.

   * - ``compile_ts`` (time)
     - The time that the file was created at.

   * - ``os`` (string)
     - The required operating system.

   * - ``subsystem`` (string)
     - The subsystem that is required to run this file.

   * - ``is_exe`` (boolean - bool)
     - Is the file an executable, or just an object file?

   * - ``is_64bit`` (boolean - bool)
     - Is the file a 64-bit executable?

   * - ``uses_aslr`` (boolean - bool)
     - Does the file support Address Space Layout Randomization?

   * - ``uses_dep`` (boolean - bool)
     - Does the file support Data Execution Prevention?

   * - ``uses_code_integrity`` (boolean - bool)
     - Does the file enforce code integrity checks?

   * - ``uses_seh`` (boolean - bool)
     - Does the file use structured exception handing?

   * - ``has_import_table`` (boolean - bool)
     - Does the file have an import table?

   * - ``has_export_table`` (boolean - bool)
     - Does the file have an export table?

   * - ``has_cert_table`` (boolean - bool)
     - Does the file have an attribute certificate table?

   * - ``has_debug_data`` (boolean - bool)
     - Does the file have a debug table?

   * - ``section_names`` (array[string] - vector of string)
     - The names of the sections, in order.
