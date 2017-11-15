Please refer to the BOM in [Consolidated/BOM](https://github.com/eez-open/psu-hw/tree/master/Consolidated/BOM) folder where **Board Name** (Col F) is *Arduino shield*. Eagle files is available in [Consolidated/Eagle files](https://github.com/eez-open/psu-hw/tree/master/Consolidated/Eagle%20files) folder.
![Shield_top](Arduino%20r5B12%20top%20view.jpg)
![Shield_bottom](Arduino%20r5B12%20bottom%20view.jpg)

**Revision history:**
* 2017-11-04: **r5B13a**
    - Soft start and DOUT2 controls ([#36](https://github.com/eez-open/psu-hw/issues/36))
    - Removed JP5, JP6, JP7 ([#59](https://github.com/eez-open/psu-hw/issues/59))
    - R93 PCB layout spacing ([#60](https://github.com/eez-open/psu-hw/issues/60))
* 2017-09-24: **r5B12**
    - X12, X14 connection improvement on PCB ([#43](https://github.com/eez-open/psu-hw/issues/43))
* 2017-02-23: **r5B12**
    - Encoder with switch mounted directly on the PCB ([#20](https://github.com/eez-open/psu-hw/issues/20))
    - Power relay MCU controlled on the AUX PS module([#23](https://github.com/eez-open/psu-hw/issues/23))
    - Support for 3.5" Riverdi TFT touchscreen display ([#24](https://github.com/eez-open/psu-hw/issues/24))
    - Micro SD card socket ([#30](https://github.com/eez-open/psu-hw/issues/30))
* 2017-01-11: **r4B2**
    - +3.3V for buzzer ([#16](https://github.com/eez-open/psu-hw/issues/16))
    - Reorganized capacitors ([#17](https://github.com/eez-open/psu-hw/issues/17))
    - Wrong positions of DOUT pins on X14 push-in connector ([#18](https://github.com/eez-open/psu-hw/issues/18))
* 2016-12-11: **r4B1**
    - Added isolated output on X14 that is replaced with 8 pin push-in connector ([#8](https://github.com/eez-open/psu-hw/issues/8))
    - D33 is added to isolate RESET signal ([#14](https://github.com/eez-open/psu-hw/issues/14))
    - Space for optional R33 is added and IC31 is replaced with 4 AND gate ([#15](https://github.com/eez-open/psu-hw/issues/15))
* 2016-10-24: **r3B5**
    - Small adjustment of TFT display (holes and offset)
    - Removed header for optional WiFi module
    - Ethernet header (X18) is moved to the right ([#5](https://github.com/eez-open/psu-hw/issues/5))
    - Fixed wrong silkscreen for all red LEDs ([#6](https://github.com/eez-open/psu-hw/issues/6))
    - Arduino output is used to generate master sync for switching regulators ([#7](https://github.com/eez-open/psu-hw/issues/7))
    - Additional Cout is added ([#12](https://github.com/eez-open/psu-hw/issues/12))
* 2016-07-23: **r3B4** ([Version 2.0](https://github.com/eez-open/psu-hw/releases/tag/2.0) on github)
	- Corrected WATCHDOG functionality, added possibility to choose between RESET and Power off if MCU stalled
	- Optimized number of parts size and values, renumbered reference designators
* 2016-06-14: **r3B3**
    - Removed suport for Mega2560 - only 3.3 V board such as Due (and hopefully soon [STAR - OTTO](http://www.arduino.org/products/boards/arduino-star-otto) is supported
    - TFT touch screen rotated (landscape view) for housing in more compact (2U height) enclosure. Tested with both SSD1289 and ILI9341 display controllers
    - Reset supervisor and watchdog (TPS3705-33)
    - Power connector replaced with 10-pin IDC to carry master sync out
    - W5500 Ethernet controller
    - 10-pin IDC for channel's SPI bus replaced with 26-pin IDC that carry output power signals, remote sense, remote programming, temperature sensor and SMPS sync
    - Redesigned wiring of output serial/parallel connection
    - Ethernet RJ-45 connector replaced with 8-pin 0.1" header (see also new AUX PS board)
    - 2x5-pin 0.1" header for optional W5500 Ethernet module (eBay)
    - 2x4-pin 0.1" header for optional NRF24L01 Wifi module (eBay)
    - Added support for incremental encoder
    - 4 mm binding posts for remote sensing inputs replaced with 0.1" push-in connector
    - New numbering in sync with consolidated schematics
* 2016-04-06: **r1B14** ([Version 1.0](https://github.com/eez-open/psu-hw/releases/tag/1.0) on github)
    - Added fan control (FAN_PWM, FAN_SENSE)
    - Power connector replaced with 6-pin IDC as on the AUX PS r4B41
    - Removed optional reset connector
* 2016-03-28: **r1B13a**
    - Change remote sense inputs position on X4
* 2016-03-27: **r1B13**
    - Fixed remote sense wiring
    - Output protection redesigned (TVS moved, SAR and MOVs removed)
    - Smaller footprint
    - Remote sense 4 mm banana binding posts replaced with compact "push-in" connectors
    - Digital trigger input (with buffer and level shifter) added
    - THT LEDs replaced with SMD counterparts (lightpipes are now required)
* 2015-12-07: **r1B12b** - *First public release*

**********************

This product is made available under the terms of the TAPR Open Hardware License. See the LICENSE.TXT file that accompanies this distribution for the full text of the license.

**********************

Repository: [www.github.com/eez-open](https://www.github.com/eez-open)  
Web site: [www.envox.hr/eez](https://www.envox.hr/eez)

**********************

Consult [EEZ PSU Arduino pin mapping r5B12.odt
](https://github.com/eez-open/psu-hw/raw/master/Arduino%20shield/EEZ%20PSU%20Arduino%20pin%20mapping%20r5B12.odt) for Arduino pins assignements and [EEZ PSU Arduino shield+BP TLC5925 codes r3B3.odt](https://github.com/eez-open/psu-hw/raw/master/Arduino%20shield/EEZ%20PSU%20Arduino%20shield%2BBP%20TLC5925%20codes%20r3B3.odt) for binding posts connections and LED indications.
