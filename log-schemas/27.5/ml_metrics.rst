``ml_metrics`` field reference
------------------------------

.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3

   * - Field (Type)
     - Description

   * - ``ts_start`` (time)
     - Start of measurements.

   * - ``ts_end`` (time)
     - End of measurements

   * - ``domain_total`` (integer - count)
     - Total number of domains seen.

   * - ``filtered_candidate`` (integer - count)
     - Number of domains filtered out as not a candidate/alexa.

   * - ``filtered_past_decisions`` (integer - count)
     - Number of domains filtered out because there was a past decision

   * - ``filtered_seen_full`` (integer - count)
     - Number of domains filtered out because they were already seen (full)

   * - ``filtered_seen_eff`` (integer - count)
     - Number of domains filtered out because they were already seen (effective)

   * - ``num_past_decisions`` (integer - count)
     - Size of past decision table

   * - ``num_seen_full`` (integer - count)
     - Size of seen_full table

   * - ``num_seen_eff`` (integer - count)
     - Size of seen_eff table.

   * - ``domains_sent`` (integer - count)
     - Number of domains sent over broker to the ML container

   * - ``result_received`` (integer - count)
     - Number of results received from the ML container.

   * - ``avg_broker_rtt`` (number - double)
     - Average Broker RTT without ML processing.

   * - ``max_broker_rtt`` (number - double)
     - Maximum Broker RTT without ML processing.

   * - ``avg_zeek_to_python_lag`` (number - double)
     - Average Broker Queue time (Zeek -> Python).

   * - ``max_zeek_to_python_lag`` (number - double)
     - Maximum Broker Queue time (Zeek -> Python).

   * - ``avg_python_to_zeek_lag`` (number - double)
     - Average Broker Queue time (Python -> Zeek).

   * - ``max_python_to_zeek_lag`` (number - double)
     - Maximum Broker Queue time (Python -> Zeek).

   * - ``filtered_python_cache`` (integer - count)
     - Number of domains filtered out by Python cache. 

   * - ``filtered_python_time_budget`` (integer - count)
     - Number of domains filtered out by Python time budget.

   * - ``python_cache_size`` (integer - count)
     - Size of Python domain cache.

   * - ``stream`` (boolean - bool)
     - If we are running in stream mode.

   * - ``batched_record_size`` (integer - count)
     - If stream==F, then this is the batch size.

   * - ``node`` (string)
     - The node reporting
