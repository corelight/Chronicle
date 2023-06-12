``smb_files`` field reference
-----------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time when the file was first discovered.

   * - ``uid`` (string)
     - Unique ID of the connection the file was sent over.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``fuid`` (string)
     - Unique ID of the file.

   * - ``action`` (string - enum)
     - Action this log record represents.

   * - ``path`` (string)
     - Path pulled from the tree this file was transferred to or from.

   * - ``name`` (string)
     - Filename if one was seen.

   * - ``size`` (integer - count)
     - Total size of the file.

   * - ``prev_name`` (string)
     - If the rename action was seen, this will be
       the file's previous name.

   * - ``times.modified`` (time)
     - The time when data was last written to the file.

   * - ``times.accessed`` (time)
     - The time when the file was last accessed.

   * - ``times.created`` (time)
     - The time the file was created.

   * - ``times.changed`` (time)
     - The time when the file was last modified.

   * - ``data_offset_req`` (integer - count)
     - The data_offset_req information.

   * - ``data_len_req`` (integer - count)
     - The data_len_req information.

   * - ``data_len_rsp`` (integer - count)
     - The data_len_rsp information.
