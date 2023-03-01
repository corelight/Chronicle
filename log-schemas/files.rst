files
-----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts`` (time)
     - The time when the file was first seen.

   * - ``fuid`` (string)
     - An identifier associated with a single file.

   * - ``tx_hosts`` (array[string] - set[addr])
     - If this file was transferred over a network
       connection this should show the host or hosts that
       the data sourced from.

   * - ``rx_hosts`` (array[string] - set[addr])
     - If this file was transferred over a network
       connection this should show the host or hosts that
       the data traveled to.

   * - ``conn_uids`` (array[string] - set[string])
     - Connection UIDs over which the file was transferred.

   * - ``source`` (string)
     - An identification of the source of the file data.  E.g. it
       may be a network protocol over which it was transferred, or a
       local file path which was read, or some other input source.

   * - ``depth`` (integer - count)
     - A value to represent the depth of this file in relation
       to its source.  In SMTP, it is the depth of the MIME
       attachment on the message.  In HTTP, it is the depth of the
       request within the TCP connection.

   * - ``analyzers`` (array[string] - set[string])
     - A set of analysis types done during the file analysis.

   * - ``mime_type`` (string)
     - A mime type provided by the strongest file magic signature
       match against the *bof_buffer* field of `fa_file`,
       or in the cases where no buffering of the beginning of file
       occurs, an initial guess of the mime type based on the first
       data seen.

   * - ``filename`` (string)
     - A filename for the file if one is available from the source
       for the file.  These will frequently come from
       \""Content-Disposition\"" headers in network protocols.

   * - ``duration`` (number - interval)
     - The duration the file was analyzed for.

   * - ``local_orig`` (boolean - bool)
     - If the source of this file is a network connection, this field
       indicates if the data originated from the local network or not as
       determined by the configured `Site::local_nets`.

   * - ``is_orig`` (boolean - bool)
     - If the source of this file is a network connection, this field
       indicates if the file is being sent by the originator of the
       connection or the responder.

   * - ``seen_bytes`` (integer - count)
     - Number of bytes provided to the file analysis engine for the file.

   * - ``total_bytes`` (integer - count)
     - Total number of bytes that are supposed to comprise the full file.

   * - ``missing_bytes`` (integer - count)
     - The number of bytes in the file stream that were completely missed
       during the process of analysis e.g. due to dropped packets.

   * - ``overflow_bytes`` (integer - count)
     - The number of bytes in the file stream that were not delivered to
       stream file analyzers.  This could be overlapping bytes or
       bytes that couldn't be reassembled.

   * - ``timedout`` (boolean - bool)
     - Whether the file analysis timed out at least once for the file.

   * - ``parent_fuid`` (string)
     - Identifier associated with a container file from which this one was
       extracted as part of the file analysis.

   * - ``md5`` (string)
     - An MD5 digest of the file contents.

   * - ``sha1`` (string)
     - A SHA1 digest of the file contents.

   * - ``sha256`` (string)
     - A SHA256 digest of the file contents.

   * - ``extracted`` (string)
     - Local filename of extracted file.

   * - ``extracted_cutoff`` (boolean - bool)
     - Set to true if the file being extracted was cut off
       so the whole file was not logged.

   * - ``extracted_size`` (integer - count)
     - The number of bytes extracted to disk.
