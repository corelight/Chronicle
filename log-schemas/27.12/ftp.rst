.. _ref_logs_ftp:

ftp
---
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Time when the command was sent.

   * - ``uid`` (string)
     - base
     - Unique ID for the connection.

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

   * - ``user`` (string)
     - base
     - User name for the current FTP session.

   * - ``password`` (string)
     - base
     - Password for the current FTP session if captured.

   * - ``command`` (string)
     - base
     - Command given by the client.

   * - ``arg`` (string)
     - base
     - Argument for the command if one is given.

   * - ``mime_type`` (string)
     - base
     - Sniffed mime type of file.

   * - ``file_size`` (integer - count)
     - base
     - Size of the file if the command indicates a file transfer.

   * - ``reply_code`` (integer - count)
     - base
     - Reply code from the server in response to the command.

   * - ``reply_msg`` (string)
     - base
     - Reply message from the server in response to the command.

   * - ``data_channel.passive`` (boolean - bool)
     - base
     - Whether PASV mode is toggled for control channel.

   * - ``data_channel.orig_h`` (string - addr)
     - base
     - The host that will be initiating the data connection.

   * - ``data_channel.resp_h`` (string - addr)
     - base
     - The host that will be accepting the data connection.

   * - ``data_channel.resp_p`` (integer - port)
     - base
     - The port at which the acceptor is listening for the data
       connection.

   * - ``fuid`` (string)
     - base
     - File unique ID.
