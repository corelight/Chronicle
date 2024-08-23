.. _ref_logs_smb_files:

smb_files
---------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - base
     - Time when the file was first discovered.

   * - ``uid`` (string)
     - base
     - Unique ID of the connection the file was sent over.

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
     - The status of the originator's endpoint agent.

   * - ``id.orig_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint unique ID.

   * - ``id.orig_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint Customer ID.

   * - ``id.orig_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The originator's endpoint information source.

   * - ``id.resp_ep_status`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The status of the responder's endpoint agent.

   * - ``id.resp_ep_uid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint unique ID.

   * - ``id.resp_ep_cid`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint Customer ID.

   * - ``id.resp_ep_source`` (string)
     - site/packages/customer-bundle/packages/Zeek-Endpoint-Enrichment/id-logs.zeek
     - The responder's endpoint information source.

   * - ``id.vlan`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The VLAN that the connection is seen on.

   * - ``id.vlan_inner`` (integer - int)
     - site/packages/customer-bundle/packages/log-add-vlan-everywhere/main.zeek
     - The inner VLAN tag for stacked VLAN tags.

   * - ``fuid`` (string)
     - base
     - Unique ID of the file.

   * - ``action`` (string - enum SMB::Action)
     - base
     - Action this log record represents.

   * - ``path`` (string)
     - base
     - Path pulled from the tree this file was transferred to or from.

   * - ``name`` (string)
     - base
     - Filename if one was seen.

   * - ``size`` (integer - count)
     - base
     - Total size of the file.

   * - ``prev_name`` (string)
     - base
     - If the rename action was seen, this will be
       the file's previous name.

   * - ``times.modified`` (time)
     - base
     - The time when data was last written to the file.

   * - ``times.accessed`` (time)
     - base
     - The time when the file was last accessed.

   * - ``times.created`` (time)
     - base
     - The time the file was created.

   * - ``times.changed`` (time)
     - base
     - The time when the file was last modified.

   * - ``data_offset_req`` (integer - count)
     - site/packages/corelight/packages/bzar/bzar_smb.zeek
     - The data_offset_req information.

   * - ``data_len_req`` (integer - count)
     - site/packages/corelight/packages/bzar/bzar_smb.zeek
     - The data_len_req information.

   * - ``data_len_rsp`` (integer - count)
     - site/packages/corelight/packages/bzar/bzar_smb.zeek
     - The data_len_rsp information.
