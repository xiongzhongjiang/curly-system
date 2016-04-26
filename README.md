# curly-system
The patches are selected from the mainline to implement the writeback better.

The patches are divied into four parts. The first part: 
The realization of the function of basic writeback, and change the original 
hierarchy to unified mode.  meanwhile, The corresponding commit information
are acquired from the Merge commit id(e4bc13adfd016fc1036838170288b5680d1a98b0).

The second part minly aims to update the cgroup interface to v2 version.

The three part mainly implement the blkcg interface for the unified hierarchy 
and the weight control based on CFQ scheduler. This patches are Merged into the
mainline. The Merge Id is b0a1ea51bda4c2bcdde460221e1772f3a4f8c44f.

The last part is  mainly bugfix.

Ps: cgroup writeback only support filesystem both ext4 and ext2. so I introdece 
the corresponding patch and bugfix about ext4 and ext2.
