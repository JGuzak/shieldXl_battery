# ShieldXl Battery Case

A case and internal battery mod for the [shieldXl](https://github.com/okyeron/shieldXL/)

<img src="images/promo_1.JPG" width=100%>

*DISCLAIMER: This mod is not supported by Denki Oto and they are not responsible for assisting with assembly or troubleshooting.*

## Kits for this case are available of on the [Modbang shop](https://www.modbang.com/modbang-shop/shieldxlbatterykit).

| Table of Contents |
| - |
| Credits |
| Use |
| BOM |
| Case |
| Installation |
| Troubleshooting |

<img src="images/promo_2.JPG" width=60%>

## Credits

Referenced model was designed by CarlosUnch, John Park and Steven Noreyko.

Project inspiration from Peter Kassel

## Use

Toggle the power switch to turn on the battery (Blue light will illuminate and green light should flash)

## BOM

<img src="images/bom.JPG" width=80%>

* 1x assembled shieldxl `*` ([bom](https://github.com/okyeron/shieldXL/tree/main/bom) for the shieldXl is available over on GitHub and kits are available at the [Denki Oto Shop](https://denki-oto.weebly.com/))
* 1x Pisugar S Plus battery assembly (5000mAh 5 volt 3 amp)
* 1x shieldXl_battery case (see Models & Printing)
* 1x pig tail JST-PH 2.0 female header
* M2.5 bolts
  * 2x 20mm
  * 3x 16mm
  * 2x 12mm
  * 2x 10mm
  * 1x 9mm `*`
* 2x M2.5 hex nuts *4x M2.5 hex nuts if using the `bottom with hex nut.stl` file.*
* 2x M2.5 heat set inserts *None if using the `bottom with hex nut.stl` file.*
* 3x M2.5 11mm f-f standoffs `*`
* 3x encoder nuts + washers `*`
* 3x encoder caps

*Items marked with `%!` are included in the shieldXl battery kit on the Modbang shop.*

## Case

<img src="images/bare_case_1.JPG" width=49%>
<img src="images/bare_case_2.JPG" width=49%>

### Models & Printing

STL made in reference to the original shieldXl case. shieldXl_battery design was made with [Blender](https://www.blender.org/) and [CAD Sketcher](https://www.cadsketcher.com/).

gcode and prusa slicer files can be found in `/prints`, stls in `/models`. Tested with PLA on Prusa MK3 and Prusa MK4 printers.

## Assembly

### ShieldXl+piSugar

*!!Assemble the battery and shieldxl outside of the case and boot the device to verify things are working before attempting to install the assembly into the case!!*

1. Assemble the shieldXl
2. Using a guitar pick or similar plastic device, carefully remove the battery from both the li-po battery pack and pi sugar pcba
3. Place the pi sugar pcba against the bottom of the pi, make sure the spring loaded pin contacts are seated correctly.
4. Using the bolts included with the pisugar, attach the pisugar to the pi
5. Connect the battery to the pisugar pcba
6. Ensure the dip switch on the bottom of the pi sugar board is set to `off`
7. Plug in the pi sugar to a charger (both usb-c and usb micro ports will charge the battery)

<img src="images/assembled_no_case_running.JPG" width=49%>
<img src="images/startup_dip_switch.JPG" width=49%>

### Case Installation

*NOTE: The original battery header can be left on the pisugar.*

1. Insert either `2` hex nuts or `2` heat set inserts into the bottom portion of the case.

<img src="images/bottom_case_nuts.JPG" width=49%>
<img src="images/bottom_case_heat_set_inserts.JPG" width=49%>


2. Remove the pi from the shieldxl pcba
3. Remove `all` standoffs from the shieldxl except for the bolt/nut through the upper right corner of the display.
4. Disconnect the battery from the pisugar pcba.
5. Carefully solder the leads of the JST pigtail to the contacts on the pisugar pcba. The original jack does not need to be removed.

*I chose to remove it because I may attempt to create a slightly thinner bottom portion of the case but this may not happen.*

<img src="images/pigtail.JPG" width=49%>

6. Set the battery into the compartment on the bottom case part and attach the battery arm with `2` 10mm bolts and `2` nuts.

<img src="images/battery_in_case.JPG" width=49%>

7. Connect the battery to the pig tail adapter.
8. Set the pisugar pcba on the bottom case with the power header side facing down.
9. Thread `3` 16mm bolts into the pisugar pcba from the bottom of the case. The bolts should be threaded all the way through the case and the pi sugar.

<img src="images/pi_sugar_in_case.JPG" width=49%>

1.  Place the pi on top of the pisugar, ensure that the spring loaded pins on the pisugar press into the back of the gpio pins on the pi board. (A good amount of force will be needed to get the pi sugar flush with the pi)
2.  Thread the `3` standoffs up to the pi. Ensure there are no gaps between the case, pisugar, pi, or standoffs.

<img src="images/pi_in_case.JPG" width=49%>

12. Carefully align and gentily press the shieldXl pcba onto the pi.

<img src="images/shieldXl_in_case.JPG" width=49%>

1.  Thread the 9mm bolt through the bottom right corner of the display and into the standoff.
2.  Carefully align and gentily press the case top onto the shieldXl. First align the left side of the case and push to the right.
3.  Thread the `2` 20mm bolts into the left holes on the top of the case.
4.  Thread the `2` remaining 12mm bolts into the right holes on the top of the case.
5.  Place the `3` washers and nuts onto the encoders and tighten by hand.
6.  Insert the micro sd card into the pi.

<img src="images/assembled_1.JPG" width=49%>

## Troubleshooting

### Battery and red led on pi turns on but norns doesn't boot

Double check that the micro sd card is inserted into the pi correctly.
