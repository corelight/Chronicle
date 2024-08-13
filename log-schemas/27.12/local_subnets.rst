.. _ref_logs_local_subnets:

local_subnets
-------------
.. list-table::
   :header-rows: 1
   :class: longtable
   :widths: 1 3 3

   * - Field (Type)
     - Source
     - Description

   * - ``round`` (integer - count)
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The round information.

   * - ``ts`` (time)
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The ts information.

   * - ``ip_version`` (integer - count)
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The ip_version information.

   * - ``subnets`` (array[string] - set[subnet])
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The subnets information.

   * - ``component_ids`` (array[integer] - set[count])
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The component_ids information.

   * - ``size_of_component`` (integer - count)
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The size_of_component information.

   * - ``bipartite`` (boolean - bool)
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The bipartite information.

   * - ``inferred_site`` (boolean - bool)
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The inferred_site information.

   * - ``other_ips`` (array[string] - set[addr])
     - site/packages/corelight/packages/local-subnets/inference/graph.zeek
     - The other_ips information.
