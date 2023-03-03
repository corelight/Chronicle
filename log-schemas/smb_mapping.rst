``smb_mapping`` field reference
-------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - Time when the tree was mapped.

   * - ``uid`` (string)
     - Unique ID of the connection the tree was mapped over.

   * - ``id.orig_h`` (string - addr)
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - The responder's port number.

   * - ``path`` (string)
     - Name of the tree path.

   * - ``service`` (string)
     - The type of resource of the tree (disk share, printer share, named pipe, etc.).

   * - ``native_file_system`` (string)
     - File system of the tree.

   * - ``share_type`` (string)
     - If this is SMB2, a share type will be included.  For SMB1,
       the type of share will be deduced and included as well.
