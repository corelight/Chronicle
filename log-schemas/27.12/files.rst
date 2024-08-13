.. _ref_logs_files:

files
-----
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - The time when the file was first seen.

   * - ``fuid`` (string)
     - base
     - An identifier associated with a single file.

   * - ``uid`` (string)
     - base
     - If this file, or parts of it, were transferred over a
       network connection, this is the uid for the connection.

   * - ``id.orig_h`` (string - addr)
     - base
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - base
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - base
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - base
     - The responder's port number.

   * - ``id.orig_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_status information.

   * - ``id.orig_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_uid information.

   * - ``id.orig_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_cid information.

   * - ``id.orig_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.orig_ep_source information.

   * - ``id.resp_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_status information.

   * - ``id.resp_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_uid information.

   * - ``id.resp_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_cid information.

   * - ``id.resp_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The id.resp_ep_source information.

   * - ``id.vlan`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The VLAN that the connection is seen on.

   * - ``id.vlan_inner`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The inner VLAN tag for stacked VLAN tags.

   * - ``source`` (string)
     - base
     - An identification of the source of the file data.  E.g. it
       may be a network protocol over which it was transferred, or a
       local file path which was read, or some other input source.

   * - ``depth`` (integer - count)
     - base
     - A value to represent the depth of this file in relation
       to its source.  In SMTP, it is the depth of the MIME
       attachment on the message.  In HTTP, it is the depth of the
       request within the TCP connection.

   * - ``analyzers`` (array[string] - set[string])
     - base
     - A set of analysis types done during the file analysis.

   * - ``mime_type`` (string)
     - base
     - A mime type provided by the strongest file magic signature
       match against the *bof_buffer* field of `fa_file`,
       or in the cases where no buffering of the beginning of file
       occurs, an initial guess of the mime type based on the first
       data seen.

   * - ``filename`` (string)
     - base
     - A filename for the file if one is available from the source
       for the file.  These will frequently come from
       "Content-Disposition" headers in network protocols.

   * - ``duration`` (number - interval)
     - base
     - The duration the file was analyzed for.

   * - ``local_orig`` (boolean - bool)
     - base
     - If the source of this file is a network connection, this field
       indicates if the data originated from the local network or not as
       determined by the configured `Site::local_nets`.

   * - ``is_orig`` (boolean - bool)
     - base
     - If the source of this file is a network connection, this field
       indicates if the file is being sent by the originator of the
       connection or the responder.

   * - ``seen_bytes`` (integer - count)
     - base
     - Number of bytes provided to the file analysis engine for the file.
       The value refers to the total number of bytes processed for this
       file across all connections seen by the current Zeek instance.

   * - ``total_bytes`` (integer - count)
     - base
     - Total number of bytes that are supposed to comprise the full file.

   * - ``missing_bytes`` (integer - count)
     - base
     - The number of bytes in the file stream that were completely missed
       during the process of analysis e.g. due to dropped packets.
       The value refers to number of bytes missed for this file
       across all connections seen by the current Zeek instance.

   * - ``overflow_bytes`` (integer - count)
     - base
     - The number of bytes in the file stream that were not delivered to
       stream file analyzers.  This could be overlapping bytes or
       bytes that couldn't be reassembled.

   * - ``timedout`` (boolean - bool)
     - base
     - Whether the file analysis timed out at least once for the file.

   * - ``parent_fuid`` (string)
     - base
     - Identifier associated with a container file from which this one was
       extracted as part of the file analysis.

   * - ``md5`` (string)
     - base
     - An MD5 digest of the file contents.

   * - ``sha1`` (string)
     - base
     - A SHA1 digest of the file contents.

   * - ``sha256`` (string)
     - base
     - A SHA256 digest of the file contents.

   * - ``extracted`` (string)
     - base
     - Local filename of extracted file.

   * - ``extracted_cutoff`` (boolean - bool)
     - base
     - Set to true if the file being extracted was cut off
       so the whole file was not logged.

   * - ``extracted_size`` (integer - count)
     - base
     - The number of bytes extracted to disk.

   * - ``tx_hosts`` (array[string] - set[addr])
     - policy/frameworks/files/deprecated-txhosts-rxhosts-connuids.zeek
     - If this file was transferred over a network
       connection this should show the host or hosts that
       the data sourced from.

   * - ``rx_hosts`` (array[string] - set[addr])
     - policy/frameworks/files/deprecated-txhosts-rxhosts-connuids.zeek
     - If this file was transferred over a network
       connection this should show the host or hosts that
       the data traveled to.

   * - ``conn_uids`` (array[string] - set[string])
     - policy/frameworks/files/deprecated-txhosts-rxhosts-connuids.zeek
     - Connection UIDs over which the file was transferred.

   * - ``vlan`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/files.zeek
     - The vlan information.

   * - ``vlan_inner`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/files.zeek
     - The vlan_inner information.
