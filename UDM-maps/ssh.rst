``ssh`` UDM map reference
-------------------------

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
     - replace with 'NETWORK_UNCATEGORIZED'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * -
     - ``metadata_product_version``
     - replace with 'SSH %{version}'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - This is the time of the first packet.

   * - ``uid`` (string)
     - ``metadata_product_log_id``
     - A unique identifier of the connection.

   * - ``id.orig_h`` (string - addr)
     - ``principal_ip``
     - The originator's IP address.

   * - ``id.orig_p`` (integer - port)
     - ``principal_port`` (string)
     - The originator's port number.

   * - ``id.resp_h`` (string - addr)
     - ``target_ip``
     - The responder's IP address.

   * - ``id.resp_p`` (integer - port)
     - ``target_port`` (string)
     - The responder's port number.

   * - ``version`` (integer - count)
     -
     - SSH major version (1, 2, or unset). The version can be unset if the
       client and server version strings are unset, malformed or incompatible
       so no common version can be extracted. If no version can be extracted
       even though both client and server versions are set a weird
       will be generated.

   * - ``auth_success`` (boolean - bool)
     -
     - Authentication result (T=success, F=failure, unset=unknown)

   * - ``auth_attempts`` (integer - count)
     - (string)
     - The number of authentication attempts we observed. There's always
       at least one, since some servers might support no authentication at all.
       It's important to note that not all of these are failures, since
       some servers require two-factor auth (e.g. password AND publickey)

   * - ``direction`` (string - enum)
     -
     - Direction of the connection. If the client was a local host
       logging into an external host, this would be OUTBOUND. INBOUND
       would be set for the opposite situation.

   * - ``client`` (string)
     - ``principal_platform_version``
     - The client's version string

   * - ``server`` (string)
     - ``target_platform_version``
     - The server's version string

   * - ``cipher_alg`` (string)
     -
     - The encryption algorithm in use

   * - ``mac_alg`` (string)
     -
     - The signing (MAC) algorithm in use

   * - ``compression_alg`` (string)
     -
     - The compression algorithm in use

   * - ``kex_alg`` (string)
     -
     - The key exchange algorithm in use

   * - ``host_key_alg`` (string)
     -
     - The server host key's algorithm

   * - ``host_key`` (string)
     -
     - The server's key fingerprint

   * - ``remote_location.country_code`` (string)
     -
     - The country code.

   * - ``remote_location.region`` (string)
     -
     - The region.

   * - ``remote_location.city`` (string)
     -
     - The city.

   * - ``remote_location.latitude`` (number - double)
     -
     - Latitude.

   * - ``remote_location.longitude`` (number - double)
     -
     - Longitude.

   * - ``hasshVersion`` (string)
     -
     - The hasshVersion information.

   * - ``hassh`` (string)
     - ``principal_process_md5``
     - The hassh information.

   * - ``hasshServer`` (string)
     - ``target_process_md5``
     - The hasshServer information.

   * - ``cshka`` (string)
     -
     - The cshka information.

   * - ``hasshAlgorithms`` (string)
     -
     - The hasshAlgorithms information.

   * - ``sshka`` (string)
     -
     - The sshka information.

   * - ``hasshServerAlgorithms`` (string)
     -
     - The hasshServerAlgorithms information.

   * - ``inferences`` (array[string] - set[string])
     - ``code``
     - Inferences from SOL analysis.


        * if [code] == "ABP"

          * "sr.summary" => "Client Authentication Bypass"
          * "sr.description" => "A client wasn't adhering to expectations of SSH either through server exploit or by the client and server switching to a protocol other than SSH after encryption begins"

        * if [code] == "AFR"

          * "sr.summary" => "SSH Agent Forwarding Requested"
          * "sr.description" => "Agent Forwarding is requested by tge Client"

        * if [code] == "APWA"

          * "sr.summary" => "Automated Password Authentication"
          * "sr.description" => "The client authenticated with an automated password tool (like sshpass)"

        * if [code] == "AUTO"

          * "sr.summary" => "Automated Interaction"
          * "sr.description" => "The client is a script automated utility and not driven by a user"

        * if [code] == "BAN"

          * "sr.summary" => "Server Banner"
          * "sr.description" => "The server sent the client a pre-authentication banner, likely for legal reasons"

        * if [code] == "BF"

          * "sr.summary" => "Client Brute Force Guessing"
          * "sr.description" => "A client made a number of authentication attempts that exceeded some configured, pre-connection threshold"

        * if [code] == "BFS"

          * "sr.summary" => "Client Brute Force Success"
          * "sr.description" => "A client made a number of authentication attempts that exceeded some configured, pre-connection threshold"

        * if [code] == "CTS"

          * "sr.summary" => "Client Trusted Server"
          * "sr.description" => "The client already has an entry in its known_hosts file for this server"

        * if [code] == "CUS"

          * "sr.summary" => "Client Untrusted Server"
          * "sr.description" => "The client did not have an entry in its known_hosts file for this server"

        * if [code] == "IPWA"

          * "sr.summary" => "Interactive Password Authentication"
          * "sr.description" => "The client interactively typed their password to authenticate"

        * if [code] == "KS"

          * "sr.summary" => "Keystrokes"
          * "sr.description" => "An interactive session occurred in which the client set user-driven keystrokes to the server"

        * if [code] == "LFD"

          * "sr.summary" => "Large Client File Download"
          * "sr.description" => "A file transfer occurred in which the server sent a sequence of bytes to the client"

        * if [code] == "LFU"

          * "sr.summary" => "Large Client File Upload"
          * "sr.description" => "A file transfer occurred in which the client sent a sequence of bytes to the server. Large file are identified dynamically based on trains of MTU-sized packets"

        * if [code] == "MFA"

          * "sr.summary" => "Multifactor Authentication"
          * "sr.description" => "The server required a second form of authentication (a code) after password or public key was accepted, and the client successfully provided it"

        * if [code] == "NA"

          * "sr.summary" => "None Authentication"
          * "sr.description" => "The client successfully authenticated using the None method"

        * if [code] == "NRC"

          * "sr.summary" => "No Remote Command"
          * "sr.description" => "The -N flag was used in SSH authentication"

        * if [code] == "PKA"

          * "sr.summary" => "Public Key Authentication"
          * "sr.description" => "The client automatically authenticated using publickey authentication"

        * if [code] == "RSI"

          * "sr.summary" => "Reverse SSH Initiated"
          * "sr.description" => "The Reverse session is initiated from the server back to the client"

        * if [code] == "RSIA"

          * "sr.summary" => "Reverse SSH Initiated Automated"
          * "sr.description" => "The initiation of the Reverse session happened very early in the packet stream, indicating automation"

        * if [code] == "RSK"

          * "sr.summary" => "Reverse SSH Keystrokes"
          * "sr.description" => "Keystrokes are detected within the Reverse tunnel"

        * if [code] == "RSL"

          * "sr.summary" => "Reverse SSH Logged In"
          * "sr.description" => "The Reverse Tunnel login has succeeded"

        * if [code] == "RSP"

          * "sr.summary" => "Reverse SSH Provisioned"
          * "sr.description" => "The client connected with -R flag, which provisions the port to be used for a Reverse Session set up at any future time"

        * if [code] == "SA"

          * "sr.summary" => "Authentication Scanning"
          * "sr.description" => "The client scanned authentication method with the server and then disconnected"

        * if [code] == "SC"

          * "sr.summary" => "Capabilities Scanning"
          * "sr.description" => "The client exchanged capabilities with the server and then disconnected"

        * if [code] == "SFD"

          * "sr.summary" => "Small Client File Download"
          * "sr.description" => "A file transfer occurred in which the server sent a sequence of bytes to the client"

        * if [code] == "SFU"

          * "sr.summary" => "Small Client File Upload"
          * "sr.description" => "A file transfer occurred in which the client sent a sequence of bytes to the server"

        * if [code] == "SP"

          * "sr.summary" => "Other Scanning"
          * "sr.description" => "A client and server didn't exchange encrypted packets but the client wasn't a version or capabilities scanner"

        * if [code] == "SV"

          * "sr.summary" => "Version Scanning"
          * "sr.description" => "A client exchanged version strings with the server and than disconnected"

        * if [code] == "UA"

          * "sr.summary" => "Unknown Authentication"
          * "sr.description" => "The authentication method is not determined or is unknown"
