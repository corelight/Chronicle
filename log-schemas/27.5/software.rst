``software`` field reference
----------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The time at which the software was detected.

   * - ``host`` (string - addr)
     - The IP address detected running the software.

   * - ``host_p`` (integer - port)
     - The port on which the software is running. Only sensible for
       server software.

   * - ``software_type`` (string - enum)
     - The type of software detected (e.g. `HTTP::SERVER`).

   * - ``name`` (string)
     - Name of the software (e.g. Apache).

   * - ``version.major`` (integer - count)
     - Major version number.

   * - ``version.minor`` (integer - count)
     - Minor version number.

   * - ``version.minor2`` (integer - count)
     - Minor subversion number.

   * - ``version.minor3`` (integer - count)
     - Minor updates number.

   * - ``version.addl`` (string)
     - Additional version string (e.g. \"beta42\").

   * - ``unparsed_version`` (string)
     - The full unparsed version string found because the version
       parsing doesn't always work reliably in all cases and this
       acts as a fallback in the logs.
