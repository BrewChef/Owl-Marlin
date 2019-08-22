# Owl Marlin Based 3D Printer Firmware

I use ths version on Production. But Please Use with caution!

Owl takes this popular RepRap an focused on add suport for all problematic addons like MKS_MINI_128864, Fysetc RGB Panels and SKR V1.1, V1.3 and MKS SBASE Boards and enable all broken fucntionality tha the comunity report.

I plan to update this version at least twice a year, including the bugfix and pull request I consider copuld bu important to makes my 3d printers Rock Solid.


## Owl Marlin
This Version borns becuase I need to fix issues with some hardware over SKR boards and there was no way to obtain responsr over my bugfixes. 



## Hardware Abstraction Layer (HAL)

Owl Marlin Based 3D Printer Firmware introduces a layer of abstraction so that all the existing high-level code can be built for 32-bit platforms. The 8 bits support will be removed.

### Code Standars
Owl will maintins the opriginal code andthe sections changed allwayus will be enclosed by the follwong CODE

- //DrDitto
  /*
  The New Code
  */

- //DrDitto
  /*
  The Suppresed code and a little explanation
  */



### Current HALs
The main flocus os this firware will be SKR boards, but the complete set of HAL will stay present in case anodoby ask me for a change

  name|processor|speed|flash|sram|logic|fpu
  ----|---------|-----|-----|----|-----|---
  [Arduino AVR](https://www.arduino.cc/)|ATmega, ATTiny, etc.|16-20MHz|64-256k|2-16k|5V|no
  [Teensy++ 2.0](http://www.microchip.com/wwwproducts/en/AT90USB1286)|[AT90USB1286](http://www.microchip.com/wwwproducts/en/AT90USB1286)|16MHz|128k|8k|5V|no
  [Arduino STM32](https://github.com/rogerclarkmelbourne/Arduino_STM32)|[STM32F1](https://www.st.com/en/microcontrollers-microprocessors/stm32f103.html) ARM-Cortex M3|72MHz|256-512k|48-64k|3.3V|no
  [Due](https://www.arduino.cc/en/Guide/ArduinoDue), [RAMPS-FD](http://www.reprap.org/wiki/RAMPS-FD), etc.|[SAM3X8E ARM-Cortex M3](http://www.microchip.com/wwwproducts/en/ATsam3x8e)|84MHz|512k|64+32k|3.3V|no
  [Re-ARM](https://www.kickstarter.com/projects/1245051645/re-arm-for-ramps-simple-32-bit-upgrade)|[LPC1768 ARM-Cortex M3](http://www.nxp.com/products/microcontrollers-and-processors/arm-based-processors-and-mcus/lpc-cortex-m-mcus/lpc1700-cortex-m3/512kb-flash-64kb-sram-ethernet-usb-lqfp100-package:LPC1768FBD100)|100MHz|512k|32+16+16k|3.3-5V|no
  [MKS SBASE](http://forums.reprap.org/read.php?13,499322)|LPC1768 ARM-Cortex M3|100MHz|512k|32+16+16k|3.3-5V|no
  [Azteeg X5 GT](https://www.panucatt.com/azteeg_X5_GT_reprap_3d_printer_controller_p/ax5gt.htm)|LPC1769 ARM-Cortex M3|120MHz|512k|32+16+16k|3.3-5V|no
  [Selena Compact](https://github.com/Ales2-k/Selena)|LPC1768 ARM-Cortex M3|100MHz|512k|32+16+16k|3.3-5V|no
  [Teensy 3.5](https://www.pjrc.com/store/teensy35.html)|ARM-Cortex M4|120MHz|512k|192k|3.3-5V|yes
  [Teensy 3.6](https://www.pjrc.com/store/teensy36.html)|ARM-Cortex M4|180MHz|1M|256k|3.3V|yes


## Credits
Thanks to the 
current Marlin dev team consists of:

 - Scott Lahteine [[@thinkyhead](https://github.com/thinkyhead)] - USA &nbsp; [![Flattr Scott](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=thinkyhead&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)
 - Roxanne Neufeld [[@Roxy-3D](https://github.com/Roxy-3D)] - USA
 - Bob Kuhn [[@Bob-the-Kuhn](https://github.com/Bob-the-Kuhn)] - USA
 - Chris Pepper [[@p3p](https://github.com/p3p)] - UK
 - João Brazio [[@jbrazio](https://github.com/jbrazio)] - Portugal
 - Erik van der Zalm [[@ErikZalm](https://github.com/ErikZalm)] - Netherlands &nbsp; [![Flattr Erik](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ErikZalm&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)

The current Owl dev team consists of:
- Me 
- My Selft
- My Ego
- My need to have a firmwarte that has an esay config and all features I could Need
- Androiditto@gmail.com

## This Version
This version is dedicated to all non approbed changes that enables the usage of
MKS_MINI_12864
FYSETC RGB Panels
and all SKR BOARD Family


## Tested 3D Printers
- Tevo Flash
- Tevo Tornado
- H3d SKY

This version is dedicated to all non approbed changes that enables the usage of
MKS_MINI_12864
FYSETC RGB Panels
and all SKR BOARD Family

## Recovered Broken Functionality
- Custom Boot Screen
- Fysetc RGG Neopixel auto start backlight
- Mks MINI 12864 all bugs Fixed over SKR V1.1 and V1.3


## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
