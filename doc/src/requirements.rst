.. _ssm-requirements:

Requirements
============

Python 2.6 or higher is required to run this tool. System Storage Manager
can only be run as root since most of the commands require root privileges.

There are other requirements listed below, but note that you do not
necessarily need all dependencies for all backends. However if some of the
tools required by a backend are missing, that backend will not work.


Python modules
--------------
* os
* re
* sys
* stat
* argparse
* datetime
* threading
* subprocess

System tools
------------
* tune2fs
* fsck.SUPPORTED_FS
* resize2fs
* xfs_db
* xfs_check
* xfs_growfs
* mkfs.SUPPORTED_FS
* which
* mount
* blkid
* wipefs

Lvm backend
-----------
* lvm2 binaries

Some distributions (e.g. Debian) have thin provisioning tools for LVM as an
optional dependency, while others install it automatically. Thin provisioning
without these tools installed is not supported by SSM.

Btrfs backend
-------------
* btrfs progs

Crypt backend
--------------
* dmsetup
* cryptsetup
