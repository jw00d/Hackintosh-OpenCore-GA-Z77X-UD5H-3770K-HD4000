# Hackintosh-OpenCore-GA-Z77X-UD5H-3770K-HD4000

OpenCore EFI folder for Gigabyte GA-Z77X-UD5H, i7 3770K, HD4000 graphics

Current OC Version is 0.5.4-DEBUG built with OCBuilder

config.plist was built by following the OpenCore Vanilla Desktop Guide:
https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/

I've found no USB mapping necessary to run my back panel USB and two front panel USB3 ports. If you run more USB ports, you may need to map.

No DDST necessary for this board (thanks Gigabyte), only SDST-EC which will need to be uniquely generated for your CPU if not running a i7 3770K.

Marvell 88SE9172 SATA Controller is not fully functional. If any drives are connected to this controller, OpenCore will stall after "connecting drivers" step and take up to 20 minutes to reach picker menu. The controller appears as "Generic AHCI Controller" in SystemInformation.

The config is currently set to heavy logging on screen and to file. This slows down the boot time signifcantly. I will remove logging commands once I solve a couple of issues.

I'm still not able to boot into Recovery partition. Trying to find a solution. Please let me know if you find bugs or enhancements!
