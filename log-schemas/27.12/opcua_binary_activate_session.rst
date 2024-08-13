.. _ref_logs_opcua_binary_activate_session:

opcua_binary_activate_session
-----------------------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``ts`` (time)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ts information.

   * - ``uid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The uid information.

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

   * - ``opcua_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The opcua_link_id information.

   * - ``client_algorithm`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The client_algorithm information.

   * - ``client_signature`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The client_signature information.

   * - ``client_software_cert_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The client_software_cert_link_id information.

   * - ``opcua_locale_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The opcua_locale_link_id information.

   * - ``ext_obj_type_id_encoding_mask`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_type_id_encoding_mask information.

   * - ``ext_obj_type_id_namespace_idx`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_type_id_namespace_idx information.

   * - ``ext_obj_type_id_numeric`` (integer - count)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_type_id_numeric information.

   * - ``ext_obj_type_id_string`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_type_id_string information.

   * - ``ext_obj_type_id_guid`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_type_id_guid information.

   * - ``ext_obj_type_id_opaque`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_type_id_opaque information.

   * - ``ext_obj_type_id_str`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_type_id_str information.

   * - ``ext_obj_encoding`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_encoding information.

   * - ``ext_obj_policy_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_policy_id information.

   * - ``ext_obj_user_name`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_user_name information.

   * - ``ext_obj_password`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_password information.

   * - ``ext_obj_encryption_algorithom`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_encryption_algorithom information.

   * - ``ext_obj_certificate_data`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_certificate_data information.

   * - ``ext_obj_token_data`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The ext_obj_token_data information.

   * - ``user_token_algorithm`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The user_token_algorithm information.

   * - ``user_token_signature`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The user_token_signature information.

   * - ``server_nonce`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The server_nonce information.

   * - ``status_code_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The status_code_link_id information.

   * - ``activate_session_diag_info_link_id`` (string)
     - packages/zeek-plugin-opcua-binary/scripts/activate-session-types.zeek
     - The activate_session_diag_info_link_id information.
