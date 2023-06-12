``intel`` field reference
-------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Timestamp when the data was discovered.

   * - ``uid`` (string)
     - If a connection was associated with this intelligence hit,
       this is the uid for the connection

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``seen.indicator`` (string)
     - The string if the data is about a string.

   * - ``seen.indicator_type`` (string - enum)
     - The type of data that the indicator represents.

   * - ``seen.where`` (string - enum)
     - Where the data was discovered.

   * - ``matched`` (array[string] - set[enum])
     - Which indicator types matched.

   * - ``sources`` (array[string] - set[string])
     - Sources which supplied data that resulted in this match.

   * - ``fuid`` (string)
     - If a file was associated with this intelligence hit,
       this is the uid for the file.

   * - ``file_mime_type`` (string)
     - A mime type if the intelligence hit is related to a file.
       If the $f field is provided this will be automatically filled
       out.

   * - ``file_desc`` (string)
     - Frequently files can be \"described\" to give a bit more context.
       If the $f field is provided this field will be automatically
       filled out.

   * - ``desc`` (array[string] - set[string])
     - The desc information.

   * - ``url`` (array[string] - set[string])
     - The url information.

   * - ``confidence`` (array[number] - set[double])
     - The confidence information.

   * - ``firstseen`` (array[string] - set[string])
     - The firstseen information.

   * - ``lastseen`` (array[string] - set[string])
     - The lastseen information.

   * - ``associated`` (array[string] - set[string])
     - The associated information.

   * - ``category`` (array[string] - set[string])
     - The category information.

   * - ``campaigns`` (array[string] - set[string])
     - The campaigns information.

   * - ``reports`` (array[string] - set[string])
     - The reports information.
