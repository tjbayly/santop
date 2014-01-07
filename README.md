santop
======

Top-like utility to monitor blockio devices exported by tcm

There are a few implementation-specific details (logical volumes are being exported as blockio devices, a given logical volume lives on a single pv), but should be extensible for general-purpose use.

Spins through /sys/kernel/config/target/core to get the udev path of all iblock devices and their statistics (num_cmds, read_mbytes, write_mbytes).
