LinkNode D1 / Wemos D1 for Sierra MacOS
=========================================

Latest driver for devices CH340G CH34G CH34X, Mac OS X Sierra compatible.

With old driver I got kernel panic after connecting a CH340G device (Arduino, etc.), this is the latest driver with full support for Mac OS X Sierra.

Installation:

* Remove the old driver: sudo rm -rf /System/Library/Extensions/usb.kext
*  Restart your Mac
*  Click on CH34x_Install_V1.3.pkg
*  Restart your Mac.
*  Plug in your device, mine is now accessible at /dev/cu.wchusbserial1410

If after installation the device is not recognized /or you cannot install the driver/, please disable System Integrity Protection (I had already disabled, because I had the old driver installed):

*  Reboot your Mac into Recovery Mode by restarting your computer and holding down Command+R until the Apple logo appears on your screen.
*  Click Utilities > Terminal.
*  In the Terminal window, type in csrutil enable --without kext (or to fully disable: csrutil disable) and press Enter.
*  Restart your Mac.

Special Thanks to:

Adrian Mihalko  
www.mihalko.eu

p.s:
I **LOVE** coffee! Buy me a coffee at:   
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=adriankoooo%40gmail%2ecom&lc=SK&item_name=Adrian%20Mihalko&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted)
