# shieldXl_battery

A case and internal battery mod for the [shieldXl](https://github.com/okyeron/shieldXL/blob/main/LICENSE.txt)

![shieldXl_battery 1](images/.jpg)

*DISCLAIMER: This mod is not supported by Denki Oto and they are not responsible for assisting with assembly or troubleshooting.*

| Table of Contents |
| - |
| Credits |
| Use |
| BOM |
| Case |
| Installation |
| Troubleshooting |

![shieldXl_battery 2](images/.jpg)

## Credits

Referenced model was designed by CarlosUnch, John Park and Steven Noreyko.

Project inspiration from Peter Kassel

## Use

1. Toggle the power switch to turn on the battery `-> *` (Blue light will illuminate)
2. Press and hold the power button `0` (When the green light is stable, release the button)

## BOM

* 1x assembled shieldxl ([The BOM](https://github.com/okyeron/shieldXL/tree/main/bom) is available on the shieldXl GitHub and kits are sometimes available at the [Denki Oto Shop](https://denki-oto.weebly.com/))
* 1x Pisugar S Plus battery assembly (5000mAh 5 volt 3 amp)
* 1x pig tail JST-PH 2.0 female header
* 4x M2.5 hex nuts
* 2x 20mm M2.5 screws

## Case

![assembled mod 1](images/.jpg)

![assembled mod 1](images/.jpg)

Internals

![case internals 1](images/.jpg)

![case internals 2](images/.jpg)

### Models & Printing

STL made in reference to the original shieldXl case. shieldXl_battery design was made with [Blender](https://www.blender.org/) and [CAD Sketcher](https://www.cadsketcher.com/).

Tested with PLA on a Prusa MK3 and Prusa MK4.

There are two flavors of the case; `plus` and `plusplus`.

* The `plus` case has a rectangle cutout on the side for all of the IO and can accomodate a stock pi/shieldxl kit with no modifications.
* The `plusplus` case has only TRS midi, usb charging, and a power switch on the side but requires permiently removing some IO on the pi. *DO THIS AT YOUR OWN RISK, DENKI OTO and I ARE NOT LIABLE IF YOUR PI BREAKS DURING OR AFTER THIS MODIFICATION.*

## Installation

*!!Assemble the battery and shieldxl outside of the case and boot the device to verify things are working before attempting to install the assembly into the case!!*

If video instructions are more your speed, check out the assembly video over on my youtube channel [here]().

*NOTE: The original battery header can be left on the pisugar.*

1. Remove the pi from the shieldxl pcba
2. Remove all standoffs from the shieldxl except for the lower middle standoff that is under the lower right corner of the display.

![removed standoffs](images/.jpg)

3. Disconnect the battery from the pisugar pcba.
4. Carefully solder the leads of the JST pigtail to the contacts on the pisugar pcba.

![pig tail power assembly 1](images/.jpg)

![pig tail power assembly 2](images/.jpg)

5. Set the battery into the compartment on the bottom case part and attach the battery arm with 2 `M2.5x10mm`, and 2 `M2.5` nuts.
6. Connect the battery to the pig tail adapter.
7. Set the pisugar pcba on the bottom case with the power header side facing down.

![pisugar in case](images/.jpg)

8. Thread 2 M2.5x8mm screws into the two right most  from the bottom of the case. The right two screws can be threaded all the way through the pi sugar but the screw nearest the battery should be threaded flush with the top of the pi sugar standoff.

*Thread the screws through the pcba with ~1mm of thread sticking out of the top. To ensure a close fit with the raspberry pi board, the screws shouldn't stick out too much before adding the shieldXl assembly ontop.*

![pisugar mounting screws](images/.jpg)

9. Place the shieldXl on top of the pisugar, ensure that the spring loaded pins on the pisugar press into the back of the gpio pins on the pi board. (A good amount of force will be needed to get the pi sugar flush with the pi)

![pisugar pin connection](images/.jpg)

10. Finish screwing in the M2.5 screws through the pi and into the standoffs between the shieldXl pcba and pi board.
11. Align and gentily press the top case part onto the shieldXl.
12. Attach the washers and nuts to the encoders.

![case encoder nuts](images/.jpg)

13. From the bottom of the case, attach the final 2 M2.5x20mm screws

![case final screws](images/.jpg)

## Troubleshooting