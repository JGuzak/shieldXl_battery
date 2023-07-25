# shieldXl-battery

A case and internal battery mod for the [shieldXl](https://github.com/okyeron/shieldXL/blob/main/LICENSE.txt)

![shieldXl_battery 1](images/.jpg)

*DISCLAIMER: This mod is not supported by Denki Oto and they are not responsible for assisting with assembly or troubleshooting.*

| Table of Contents |
| - |
| Use |
| BOM |
| Case |
| Installation |
| Troubleshooting |

![shieldXl_battery 2](images/.jpg)

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

### Development

STL made in reference to the original shieldXl case. shieldXl_battery was made with [Blender](https://www.blender.org/) and [CAD Sketcher](https://www.cadsketcher.com/).

## Installation

*PREFACE: Assemble the mod outside of the case to verify things are working before attempting to install the assembly into the case.*

*NOTE: The original battery header can be left on the pisugar. If being as slim as possible is your jam, the original header can be removed and there is a modified bottom case part that is shallower.*

1. Disconnect the battery from the pisugar pcba.
2. Carefully solder the leads of the JST pigtail to the contacts on the pisugar pcba.

![pig tail power assembly 1](images/.jpg)

![pig tail power assembly 2](images/.jpg)

2. Set the battery into the compartment on the bottom case part and attach the battery arm with 1 M2.5x10mm, 1 M2.5x8mm, and 2 M2.5 nuts.
3. Connect the battery.
4. Rest the pisugar pcba on the bottom case part with the power header side facing down.

![pisugar resting in case](images/.jpg)

5. Start threading 3 M2.5x8mm screws into the pisugar from the bottom of the case

*Thread the screws through the pcba with ~1mm of thread sticking out of the top. To ensure a close fit with the raspberry pi board, the screws shouldn't stick out too much before adding the shieldXl assembly ontop.*

![pisugar mounting screws](images/.jpg)

6. Place the shieldXl ontop of the pisugar, ensure that the spring loaded pins on the pisugar press into the back of the pins on the raspberry pi board. (A good amount of force will be needed to get the pi sugar flush with the raspberry pi board)

![pisugar pin connection](images/.jpg)

7. Finish screwing in the M2.5 screws through the raspberry pi and into the standoffs between the shieldXl pcba and pi board.
8. Align and gentily press the top case part onto the shieldXl.
9. Attach the washers and nuts to the encoders.

![case encoder nuts](images/.jpg)

10. From the bottom of the case, attach the final 2 M2.5x20mm screws

![case final screws](images/.jpg)

## Troubleshooting
