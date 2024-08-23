.. _ref_logs_files_red:

files_red
---------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (array[time] - vector of time)
     - site/packages/corelight/packages/datared/files.zeek
     - The time(s) when the file was seen.

   * - ``fuid`` (string)
     - site/packages/corelight/packages/datared/files.zeek
     - An identifier associated with one of the highly similar entries.
       We use the first fuid seen within the window for this.

   * - ``tx_hosts`` (array[string] - set[addr])
     - site/packages/corelight/packages/datared/files.zeek
     - The originating hosts involved in the transfers.

   * - ``rx_hosts`` (array[string] - set[addr])
     - site/packages/corelight/packages/datared/files.zeek
     - The responding hosts involved in the transfers.

   * - ``conn_uids`` (array[string] - set[string])
     - site/packages/corelight/packages/datared/files.zeek
     - Connection UIDs over which the file was transferred.

   * - ``source`` (string)
     - site/packages/corelight/packages/datared/files.zeek
     - An identification of the source of the file data.  It
       may be the network protocol over which it was transferred, a
       local file path which was read, or some other input source.

   * - ``depth`` (integer - count)
     - site/packages/corelight/packages/datared/files.zeek
     - A value to represent the depth of this file in relation
       to its source.  In SMTP, it is the depth of the MIME
       attachment on the message.  In HTTP, it is the depth of the
       request within the TCP connection.

   * - ``analyzers`` (array[string] - set[string])
     - site/packages/corelight/packages/datared/files.zeek
     - A set of analysis types done during the file analysis.

   * - ``mime_type`` (string)
     - site/packages/corelight/packages/datared/files.zeek
     - A mime type provided by the strongest file magic signature
       match against the *bof_buffer* field of ``fa_file``,
       or in the cases where no buffering of the beginning of file
       occurs, an initial guess of the mime type based on the first
       data seen.

   * - ``filename`` (string)
     - site/packages/corelight/packages/datared/files.zeek
     - A filename for the file if one is available from the source
       for the file.  These will frequently come from
       "Content-Disposition" headers in network protocols.

   * - ``local_orig`` (boolean - bool)
     - site/packages/corelight/packages/datared/files.zeek
     - If the source of this file is a network connection, this field
       indicates if the data originated from the local network or not as
       determined by the configured ``Site::local_nets``.

   * - ``is_orig`` (boolean - bool)
     - site/packages/corelight/packages/datared/files.zeek
     - If the source of this file is a network connection, this field
       indicates if the file is being sent by the originator of the
       connection or the responder.

   * - ``seen_bytes`` (integer - count)
     - site/packages/corelight/packages/datared/files.zeek
     - Number of bytes provided to the file analysis engine for the file.

   * - ``total_bytes`` (integer - count)
     - site/packages/corelight/packages/datared/files.zeek
     - Total number of bytes that are supposed to comprise the full file.

   * - ``missing_bytes`` (integer - count)
     - site/packages/corelight/packages/datared/files.zeek
     - The number of bytes in the file stream that were completely missed
       during the process of analysis, e.g. due to dropped packets.

   * - ``overflow_bytes`` (integer - count)
     - site/packages/corelight/packages/datared/files.zeek
     - The number of bytes in the file stream that were not delivered to
       stream file analyzers.  This could be overlapping bytes or
       bytes that couldn't be reassembled.

   * - ``timedout`` (boolean - bool)
     - site/packages/corelight/packages/datared/files.zeek
     - Whether the file analysis timed out at least once for the file.

   * - ``parent_fuid`` (string)
     - site/packages/corelight/packages/datared/files.zeek
     - Identifier associated with a container file from which this one was
       extracted as part of the file analysis.

   * - ``extracted`` (array[string] - set[string])
     - site/packages/corelight/packages/datared/files.zeek
     - Local filename of extracted file.

   * - ``extracted_cutoff`` (boolean - bool)
     - site/packages/corelight/packages/datared/files.zeek
     - Set to true if the file being extracted was cut off
       so the whole file was not logged.

   * - ``extracted_size`` (integer - count)
     - site/packages/corelight/packages/datared/files.zeek
     - The number of bytes extracted to disk.

   * - ``md5`` (string)
     - site/packages/corelight/packages/datared/files.zeek
     - An MD5 digest of the file contents.

   * - ``sha1`` (string)
     - site/packages/corelight/packages/datared/files.zeek
     - A SHA1 digest of the file contents.

   * - ``sha256`` (string)
     - site/packages/corelight/packages/datared/files.zeek
     - A SHA256 digest of the file contents.

   * - ``num`` (integer - count)
     - site/packages/corelight/packages/datared/files.zeek
     - Number of times we've seen this file.
