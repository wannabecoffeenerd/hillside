# Alternative Case for HillSideView

This is an alternative case for HillSideView, sporting the same nice!view display and Cirque devices. The primary design goal was to create a case that's compatible with the current HillSideView build, while hiding the top screws and minimizing any visible gaps from the top.

<img src="./images/complete.jpg" width="640">

## BOM

The following BOM assumes you've already built the keyboard itself, and focuses on the items you'll need to integrate it with this case.


| **Component**                         | **Quantity**  | **Purpose**                                            | **URL**                                                                                                |
|---------------------------------------|---------------|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| M2 3mm screws                         |             3 | Attaching the Cirque's case to the top right side      |[URL](https://www.amazon.com/gp/product/B081GL2Y7Z/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)|
| M2 4mm screws                         |             4 | Attaching the PCBs to the top cases                    |↑                                                                                                  |
| M2 5mm screws                         |            22 | Attaching the cases and battery covers                 |↑                                                                                                  |
| M2 7mm standoffs                      |            16 | Spacing the PCBs from the bottom cases                 |[URL](https://www.amazon.com/dp/B07H3PRQF5?psc=1&ref=ppx_yo2ov_dt_b_product_details)               |
| Loctite Blue 242                      |             1 | Gluing the screws going into the top of the standoffs  |[URL](https://www.amazon.com/dp/B000I1RSNS?ref=ppx_yo2ov_dt_b_product_details&th=1)                |
| 0.04" (~1mm) thick plexiglass/acrylic | 16 mm x 38 mm | Protective cover for the display                       |[URL](https://www.amazon.com/dp/B09XF19CKB?ref=ppx_yo2ov_dt_b_product_details&th=1)                |
| Flex (12 pin, 0.5mm pitch)            |             1 | Connecting the Cirque to the PCB                       |[URL](https://www.amazon.com/dp/B09R9JLWK2?psc=1&ref=ppx_yo2ov_dt_b_product_details)               |

## Printing Instructions

Tested printer configuration:
* Prusa MK4, 0.4mm nozzle
* Overture white matte PLA

| **Component**                    | **Layer height** | **Orientation** | **Supports**                                            |
|----------------------------------|------------------|-----------------|---------------------------------------------------------|
| BatteryCover.stl                 |              0.2 | Upside down     | No                                                      |
| CirqueCaseBottom.stl             |              0.1 | Right side up   | Yes (only under where the keyboard's power switch goes) |
| CirqueCaseTop.stl                |              0.1 | Upside down     | No                                                      |
| HillSideViewCaseBottom.stl       |              0.2 | Right side up   | No                                                      |
| HillSideViewCaseBottomRight.stl  |              0.2 | Right side up   | No                                                      |
| HillSideViewCaseTop.stl          |              0.2 | Upside down     | No                                                      |
| HillSideViewCaseTopRight.stl     |              0.2 | Upside down     | No                                                      |
| HillSideViewDisplayCover.stl     |              0.2 | Upside down     | Yes                                                     |

## Assembly

### Left Half

Use 5mm screws to attach 8 standoffs to the PCB. See the picture below (ignore the case for now). Note that while there are 10 screw holes in total, we're only using 8 of them for standoffs.

Optionally, add a drop of Loctite to the screws during this process and let it fully set. This will help keep these screws and standoffs fixed, as screws will get attached to the other side of the standoffs later in the assembly process (and potentially detached for PCB/battery maintenance later in the keyboard's life).

<img src="./images/pcb_bottom.jpg" width="640">

Glue a piece of plexiglass to the inside of the display cover's view port. This piece of plexiglass will give the display a bit of protection during travel.

<img src="./images/display_cover_plexiglass.jpg" width="640">

Optionally, remove the nice!view's protective film. Lay the display cover on top of the display. Note the correct orientation in the picture below.

<img src="./images/display_cover_in_place.jpg" width="640">

Insert the PCB into the top of the case, with the display cover poking through it. The top of the case should keep the display cover fixed in the XY plane and sandwitched against the PCB.

<img src="./images/display_cover_in_place_with_top.jpg" width="640">

Use two 4mm screws to attach the top of the PCB to the top of the case. These screws aren't really load bearing, they're just a convenient way to keep the PCB and the top of the case fixed as a single unit during the rest of the assebmly. Don't overtighten these screws to avoid having them poke through the top of the case.

<img src="./images/pcb_bottom_annotated.jpg" width="640">

Place the battery in the battery compartment.

<img src="./images/battery_case.jpg" width="640">

Attach the battery and its compatment to the bottom of the case using three 5mm screws.

<img src="./images/battery_wired.jpg" width="640">

Close up the case and use eight 5mm screws to attach the bottom of the case to the standoffs.

<img src="./images/bottom.jpg" width="640">

Pop in your favorite key switches.

<img src="./images/left_top.jpg" width="640">

Here's the final result:

<img src="./images/left.jpg" width="640">

### Right Half

Assembling the right half is very similar to the left. Repeat the same process, up to placing the PCB in the top of the case and securing it with two screws.

<img src="./images/right_before_cirque.jpg" width="640">

Open the flex socket's flap, insert the flex, and close the flap.

<img src="./images/right_with_flex.jpg" width="640">

Insert the flex through the Cirque's bottom case and attach the Cirque's bottom case to the keyboard's top case using three 3mm screws. Don't be afraid to bend the stiff part of the flex.

<img src="./images/right_with_flex_2.jpg" width="640">

Attach the flex to the Cirque.

<img src="./images/right_with_flex_3.jpg" width="640">

Here's where you'll need to get a bit creative: flatten the flex underneath the Cirque, while pushing the Cirque's flex connector through the Cirque's bottom case.

<img src="./images/right_with_cirque.jpg" width="640">

Screw the Cirque's case cap around the Cirque. It should hold the Cirque firmly in place, while also sitting flush with the Cirque's bottom case.

Here it is from the bottom:

<img src="./images/right_with_cirque_bottom.jpg" width="640">

The rest of the assembly process is just like the left half. Here's the final result:

<img src="./images/right.jpg" width="640">