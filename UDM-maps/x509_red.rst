``x509_red`` UDM Map Reference
------------------------------

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
     - replace with 'GENERIC_EVENT'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * -
     - ``event1.idm.read_only_udm.target.application``
     - replace with 'x509'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - Timestamp when the data was discovered.

   * - ``fingerprint`` (string)
     - ``metadata_product_log_id``
     - Fingerprint of the certificate - uses chosen algorithm.

   * - ``certificate.version`` (integer - count)
     - ``event1.idm.read_only_udm.network.tls.server.certificate.version`` (string)
     - Version number.

   * - ``certificate.serial`` (string)
     - ``event1.idm.read_only_udm.network.tls.server.certificate.serial``
     - Serial number.

   * - ``certificate.subject`` (string)
     - ``event1.idm.read_only_udm.network.tls.server.certificate.subject``
     - Subject.

   * - ``certificate.issuer`` (string)
     - ``event1.idm.read_only_udm.network.tls.server.certificate.issuer``
     - Issuer.

   * - ``certificate.not_valid_before`` (time)
     - ``event1.idm.read_only_udm.network.tls.server.certificate.not_before`` (yyyy-MM-dd HH:mm:ss.SSS)
     - Timestamp before when certificate is not valid.

   * - ``certificate.not_valid_after`` (time)
     - ``event1.idm.read_only_udm.network.tls.server.certificate.not_after`` (yyyy-MM-dd HH:mm:ss.SSS)
     - Timestamp after when certificate is not valid.

   * - ``certificate.key_alg`` (string)
     -
     - Name of the key algorithm

   * - ``certificate.sig_alg`` (string)
     -
     - Name of the signature algorithm

   * - ``certificate.key_type`` (string)
     -
     - Key type, if key parseable by openssl (either rsa, dsa or ec)

   * - ``certificate.key_length`` (integer - count)
     -
     - Key length in bits

   * - ``certificate.exponent`` (string)
     -
     - Exponent, if RSA-certificate

   * - ``certificate.curve`` (string)
     -
     - Curve, if EC-certificate

   * - ``san.dns`` (array[string] - vector of string)
     -
     - List of DNS entries in SAN

   * - ``san.uri`` (array[string] - vector of string)
     -
     - List of URI entries in SAN

   * - ``san.email`` (array[string] - vector of string)
     -
     - List of email entries in SAN

   * - ``san.ip`` (array[string] - vector of addr)
     -
     - List of IP entries in SAN

   * - ``basic_constraints.ca`` (boolean - bool)
     -
     - CA flag set?

   * - ``basic_constraints.path_len`` (integer - count)
     -
     - Maximum path length

   * - ``host_cert`` (boolean - bool)
     -
     - Indicates if this certificate was a end-host certificate, or sent as part of a chain

   * - ``client_cert`` (boolean - bool)
     -
     - Indicates if this certificate was sent from the client
