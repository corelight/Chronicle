``files`` UDM map reference
---------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 1 3

   * - Field (Type)
     - UDM Field (Type)
     - Description

   * -
     - ``metadata_vendor_name``
     - replace with 'Corelight'

   * -
     - ``metadata_event_type``
     - replace with 'FILE_UNCATEGORIZED'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * -
     - ``principal_ip``
     - replace with '%{tx_hosts.0}'

   * -
     - ``principal_hostname``
     - replace with '%{tx_hosts.0}'

   * -
     - ``target_ip``
     - replace with '%{rx_hosts.0}'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - The time when the file was first seen.

   * - ``fuid`` (string)
     - ``metadata_product_log_id``
     - An identifier associated with a single file.

   * - ``tx_hosts`` (array[string] - set[addr])
     -
     - If this file was transferred over a network
       connection this should show the host or hosts that
       the data sourced from.

   * - ``rx_hosts`` (array[string] - set[addr])
     -
     - If this file was transferred over a network
       connection this should show the host or hosts that
       the data traveled to.

   * - ``conn_uids`` (array[string] - set[string])
     -
     - Connection UIDs over which the file was transferred.

   * - ``source`` (string)
     -
     - An identification of the source of the file data.  It
       may be the network protocol over which it was transferred, a
       local file path which was read, or some other input source.

   * - ``depth`` (integer - count)
     -
     - A value to represent the depth of this file in relation
       to its source.  In SMTP, it is the depth of the MIME
       attachment on the message.  In HTTP, it is the depth of the
       request within the TCP connection.

   * - ``analyzers`` (array[string] - set[string])
     -
     - A set of analysis types done during the file analysis.

   * - ``mime_type`` (string)
     - ``target_file_mime_type``
     - A mime type provided by the strongest file magic signature
       match against the *bof_buffer* field of ``fa_file``,
       or in the cases where no buffering of the beginning of file
       occurs, an initial guess of the mime type based on the first
       data seen.

   * - ``filename`` (string)
     - ``target_file_full_path``
     - A filename for the file if one is available from the source
       for the file.  These will frequently come from
       \""Content-Disposition\"" headers in network protocols.

   * - ``duration`` (number - interval)
     -
     - The duration the file was analyzed for.

   * - ``local_orig`` (boolean - bool)
     -
     - If the source of this file is a network connection, this field
       indicates if the data originated from the local network or not as
       determined by the configured ``Site::local_nets``.

   * - ``is_orig`` (boolean - bool)
     -
     - If the source of this file is a network connection, this field
       indicates if the file is being sent by the originator of the
       connection or the responder.

   * - ``seen_bytes`` (integer - count)
     - ``target_file_size``
     - Number of bytes provided to the file analysis engine for the file.

   * - ``total_bytes`` (integer - count)
     -
     - Total number of bytes that are supposed to comprise the full file.

   * - ``missing_bytes`` (integer - count)
     -
     - The number of bytes in the file stream that were completely missed
       during the process of analysis, e.g. due to dropped packets.

   * - ``overflow_bytes`` (integer - count)
     -
     - The number of bytes in the file stream that were not delivered to
       stream file analyzers.  This could be overlapping bytes or
       bytes that couldn't be reassembled.

   * - ``timedout`` (boolean - bool)
     -
     - Whether the file analysis timed out at least once for the file.

   * - ``parent_fuid`` (string)
     -
     - Identifier associated with a container file from which this one was
       extracted as part of the file analysis.

   * - ``md5`` (string)
     - ``target_file_md5``
     - An MD5 digest of the file contents.

   * - ``sha1`` (string)
     - ``target_file_sha1``
     - A SHA1 digest of the file contents.

   * - ``sha256`` (string)
     - ``target_file_sha256``
     - A SHA256 digest of the file contents.

   * - ``extracted`` (array[string] - set[string])
     - ``about.file.full_path``
     - Local filename of extracted file.

   * - ``extracted_cutoff`` (boolean - bool)
     -
     - Set to true if the file being extracted was cut off
       so the whole file was not logged.

   * - ``extracted_size`` (integer - count)
     -
     - The number of bytes extracted to disk.
