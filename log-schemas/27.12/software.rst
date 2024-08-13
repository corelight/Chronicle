.. _ref_logs_software:

software
--------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - The time at which the software was detected.

   * - ``host`` (string - addr)
     - base
     - The IP address detected running the software.

   * - ``host_p`` (integer - port)
     - base
     - The port on which the software is running. Only sensible for
       server software.

   * - ``software_type`` (string - enum Software::Type)
     - base
     - The type of software detected (e.g. `HTTP::SERVER`).

   * - ``name`` (string)
     - base
     - Name of the software (e.g. Apache).

   * - ``version.major`` (integer - count)
     - base
     - Major version number.

   * - ``version.minor`` (integer - count)
     - base
     - Minor version number.

   * - ``version.minor2`` (integer - count)
     - base
     - Minor subversion number.

   * - ``version.minor3`` (integer - count)
     - base
     - Minor updates number.

   * - ``version.addl`` (string)
     - base
     - Additional version string (e.g. "beta42").

   * - ``unparsed_version`` (string)
     - base
     - The full unparsed version string found because the version
       parsing doesn't always work reliably in all cases and this
       acts as a fallback in the logs.
