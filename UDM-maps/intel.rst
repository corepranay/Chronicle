``intel`` UDM Map Reference
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
     - replace with 'SCAN_NETWORK'

   * -
     - ``metadata_product_name``
     - replace with 'Zeek'

   * - ``_path`` (string)
     - ``metadata_product_event_type``
     - The name of the log

   * - ``system_name`` (string)
     - ``observer_hostname``
     - The name of the sensor that observed the traffic.

   * - ``ts`` (time)
     - ``date``
     - Timestamp when the data was discovered.

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

   * - ``seen.indicator`` (string)
     -
     - The string if the data is about a string.

   * - ``seen.indicator_type`` (string - enum)
     -
     - The type of data that the indicator represents.

   * - ``seen.where`` (string - enum)
     -
     - Where the data was discovered.

   * - ``matched`` (array[string] - set[enum])
     -
     - Which indicator types matched.

   * - ``sources`` (array[string] - set[string])
     -
     - Sources which supplied data that resulted in this match.

   * - ``fuid`` (string)
     -
     - If a file was associated with this intelligence hit,
       this is the uid for the file.

   * - ``file_mime_type`` (string)
     -
     - A mime type if the intelligence hit is related to a file.
       If the $f field is provided this will be automatically filled
       out.

   * - ``file_desc`` (string)
     -
     - Frequently files can be \""described\"" to give a bit more context.
       If the $f field is provided this field will be automatically
       filled out.

   * - ``desc`` (array[string] - set[string])
     -
     - The description information for the indicator. Requires the ExtendIntel package.

   * - ``url`` (array[string] - set[string])
     -
     - The URL with more information about the indicator. Requires the ExtendIntel package.

   * - ``confidence`` (array[number] - set[double])
     -
     - The confidence information for the indicator. Requires the ExtendIntel package.

   * - ``firstseen`` (array[string] - set[string])
     -
     - When the indicator was first seen by one of the sources. Requires the ExtendIntel package.

   * - ``lastseen`` (array[string] - set[string])
     -
     - When the indicator was last seen by one of the sources. Requires the ExtendIntel package.

   * - ``associated`` (array[string] - set[string])
     -
     - Any associated information to the indicator. Requires the ExtendIntel package.

   * - ``category`` (array[string] - set[string])
     -
     - The category of the indicator. Requires the ExtendIntel package.

   * - ``campaigns`` (array[string] - set[string])
     -
     - Any campaigns related to the indicator. Requires the ExtendIntel package.

   * - ``reports`` (array[string] - set[string])
     -
     - Any reports related to the indicator. Requires the ExtendIntel package.
