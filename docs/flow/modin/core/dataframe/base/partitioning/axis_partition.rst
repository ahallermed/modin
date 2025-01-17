BaseDataframeAxisPartition
""""""""""""""""""""""""""

The class is base for any axis partition class and serves as the last level on which
operations that were conveyed from the partition manager are being performed on an entire column or row.

The class provides an API that has to be overridden by the child classes in order to manipulate
on a list of block partitions (making up column or row partition) they store.

The procedures that use this class and its methods assume that they have some global knowledge
about the entire axis. This may require the implementation to use concatenation or append on the
list of block partitions.

Public API
----------

.. autoclass:: modin.core.dataframe.base.partitioning.axis_partition.BaseDataframeAxisPartition
  :members:
