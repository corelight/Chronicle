.. _ref_logs_pe:

pe
--
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Current timestamp.

   * - ``id`` (string)
     - base
     - File id of this portable executable file.

   * - ``machine`` (string)
     - base
     - The target machine that the file was compiled for.

   * - ``compile_ts`` (time)
     - base
     - The time that the file was created at.

   * - ``os`` (string)
     - base
     - The required operating system.

   * - ``subsystem`` (string)
     - base
     - The subsystem that is required to run this file.

   * - ``is_exe`` (boolean - bool)
     - base
     - Is the file an executable, or just an object file?

   * - ``is_64bit`` (boolean - bool)
     - base
     - Is the file a 64-bit executable?

   * - ``uses_aslr`` (boolean - bool)
     - base
     - Does the file support Address Space Layout Randomization?

   * - ``uses_dep`` (boolean - bool)
     - base
     - Does the file support Data Execution Prevention?

   * - ``uses_code_integrity`` (boolean - bool)
     - base
     - Does the file enforce code integrity checks?

   * - ``uses_seh`` (boolean - bool)
     - base
     - Does the file use structured exception handing?

   * - ``has_import_table`` (boolean - bool)
     - base
     - Does the file have an import table?

   * - ``has_export_table`` (boolean - bool)
     - base
     - Does the file have an export table?

   * - ``has_cert_table`` (boolean - bool)
     - base
     - Does the file have an attribute certificate table?

   * - ``has_debug_data`` (boolean - bool)
     - base
     - Does the file have a debug table?

   * - ``section_names`` (array[string] - vector of string)
     - base
     - The names of the sections, in order.
