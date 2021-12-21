# Kernel patch for workaround MSI-X bug in the Silicon Motion SM2262 SSD Controller
 
* From: Alex Williamson <alex.williamson@redhat.com>

* Bugzilla and discussion https://bugzilla.kernel.org/show_bug.cgi?id=202055

Fix bug when PCI passthrough:

```failed to add PCI capability 0x11[0x50]@0xb0: table & pba overlap, or they don't fit in BARs, or don't align.```
 
Tested on Linux 5.15.10 with Intel 760p (8086:f1a6)

Also believed to be affected are the ADATA XPG SX8200, Mushkin Pilot, HP EX920, and Western Digital Black.
