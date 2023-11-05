# Hillside View Ergonomic Keyboard

3x6                       |  3x5
:-------------------------:|:-------------------------:
![](https://github.com/wannabecoffeenerd/HillSideView/blob/main/hillsideview46/doc/image/hsv_3x6_with_plate.jpg)  |  ![](https://github.com/wannabecoffeenerd/HillSideView/blob/main/hillsideview46/doc/image/hsv_3x5_klp_lame.jpg)

The HillSideView (HSV) is a modified version of the [Hillside 46](https://github.com/mmccoyd/hillside). It is a 
 wireless (or wired) [40%](https://deskthority.net/wiki/40%25) 
 split-[ergonomic](https://deskthority.net/wiki/Ergonomic_keyboard) 
 keyboard with a 
 [column-stagger](https://deskthority.net/wiki/Staggering#Columnar_layout) 3x6+5 or a 3x5+5 layout.

The main features that the HSV adds over the Hillside 46 are:
- [nice!view](https://github.com/getkeops/keops/tree/main) e-paper display for better battery life
- Cleaner outer pinky column cut-off
- Support for a cirque trackpad with an FFC connector on the PCB itself
- Case design with support for large 750-3000 mAh batteries under the PCB
- Magnetic tenting stand with the case
- Under PCB mount for the MCU for a cleaner top display mounting

The HSV has optional factory parts soldering (PCBA) except for the switches, MCU, display, TRRS, LEDs, battery switch, and optional hotswap sockets.

Other features of the HSV are:

- Choc-spaced keys, aggressive stagger, five thumb keys
- Break-off outer pinkie column
- Tenting puck support
- QMK and wireless ZMK firmware
- Nice!nano battery power switch
- Encoder support
- Underglow from four or five SK6812-MINI-Es
- Reversible PCB
- Detailed BOM and default keyboard rationale.
- SMT diodes, resistors, capacitors, and reset switch

*Keycaps*: HillSideView is _only_ suitable for choc v1 switches and keycaps based on an 18 x 17mm switch spacing, such as the [MBK](https://mkultra.click/mbk-choc-keycaps), [Lowprokb LDSA](https://lowprokb.ca/products/ldsa-low-profile-blank-keycaps) or [KLP Lamé](https://github.com/braindefender/KLP-Lame-Keycaps/). Not MX ones, nor 18 x 18mm ones such as Work Louder, nor Kailh Choc Transparent.

## Keymap

HillSideView includes ZMK Firmware
- [full size](https://github.com/mike1808/zmk-config)
- [five column](https://github.com/wannabecoffeenerd/zmk-config)

QMK firmware can be adapted from the [Hillside firmware](https://github.com/qmk/qmk_firmware/tree/master/keyboards/handwired/hillside) 

The default keymap for the five column build:
![](https://github.com/wannabecoffeenerd/zmk-config/blob/main/visualization/hsv.svg)

## Key Use

I expect most people will primarily use either the tucked three thumbs or the extended three (not counting the upper thumb). They can choose where the thumb arc suits them best. I find the thumb finger is best for reaching the upper thumb key; clearing the lower thumb requires some care, but it is still very useful. The middle finger also handily reaches the most tucked thumb key, as the open space is a good reference. The keys outside of the primary three thumb keys are convenient for infrequent lock layers, escape, or for use when not actively typing for things such as mute.

## Why

The main reason for this project is to make the keyboard more wireless friendly by adding the e-paper display and allowing experimenting with using a cirque trackpad (once ZMK support for it is more stable)

## Hardware and Build Guide

See the [original Hillside wiki](https://github.com/mmccoyd/hillside/wiki)
 first for PCB ordering, parts links and a build guide with pictures.

See the [HSV wiki](https://github.com/wannabecoffeenerd/HillSideView/wiki) for HSV specific
 build guide.

 ### Bill of Materials (BOM)

| **Component**                          | **Quantity per keeb** | **URL**                                                                                                 | **Source**      | **Price Per SKU** |
|----------------------------------------|-----------------------|---------------------------------------------------------------------------------------------------------|-----------------|-------------------|
| PCB                                    |                     1 | JLCPCB                                                                                                  | JLCPCB          |            10.778 |
| nice!nano                              |                     2 | https://typeractive.xyz/products/nice-nano                                                              | typeractive.xyz |                25 |
| nice!view                              |                     2 | https://typeractive.xyz/products/nice-view                                                              | typeractive.xyz |                20 |
| switches - pro pink or other (10 pack) |                     5 | https://lowprokb.ca/collections/keyboards/products/kailh-choc-low-profile-switches                      | lowprokb.ca     |                 5 |
| mill-max sockets                       |                   100 | https://www.mouser.com/ProductDetail/Mill-Max/0305-2-15-80-47-80-10-0?qs=QtQX4uD3c2Uys0ai6Tr8NQ%3D%3D   | mouser.com      |               0.1 |
| keycaps (10 pack)                      |                     5 | https://typeractive.xyz/products/mbk-keycaps                                                            | typeractive.xyz |               3.5 |
| 2x battery - 750 mAh                   |                     2 | https://typeractive.xyz/products/lithium-battery-750mah                                                 | typeractive.xyz |                 6 |
| MCU sockets - low clearance            |                     2 | https://www.mouser.com/ProductDetail/Mill-Max/310-47-132-41-001000?qs=5aG0NVq1C4z8UdNlP%252Bvotg%3D%3D  | mouser.com      |              2.17 |
| Standoffs                              |                     8 | https://www.mouser.com/ProductDetail/Wurth-Elektronik/970060244?qs=%252BEew9%252B0nqrCEb5Os0atlaA%3D%3D | mouser.com      |              0.43 |
| MCU pins                               |                    64 | https://www.mouser.com/ProductDetail/Mill-Max/3320-0-00-15-00-00-03-0?qs=s8Nb1z4Wn%2FQ16WBIwCPrTw%3D%3D | mouser.com      |              0.05 |
| power switches                         |                     2 | https://www.mouser.com/ProductDetail/CK/JS202011AQN?qs=LgMIjt8LuD%252Bmsz6wAeWWtQ%3D%3D                 | mouser.com      |             0.471 |

Some other optional parts:

| **Component**          | **Quantity per keeb** | **URL**                                              | **Source**    | **Price Per SKU** |
|------------------------|-----------------------|------------------------------------------------------|---------------|-------------------|
| battery - 110 mAh      |                     2 | https://www.aliexpress.us/item/2255800150229489.html | aliexpress.us |              1.36 |
| battery - 2000 mAh     |                     2 | https://www.aliexpress.us/item/3256803882039204.html | aliexpress.us |              5.18 |
| EC11 rotary encoders   |                   0.4 | https://www.aliexpress.us/item/2251832789732148.html | aliexpress.us |              5.08 |
| aluminum knob for EC11 |                     1 | https://www.aliexpress.us/item/3256801125707035.html | aliexpress.us |              6.85 |

 ### 3DP case

 The HSV is designed to be used with a 3D printed case. STLs for the case are [here](https://github.com/wannabecoffeenerd/HillSideView/tree/main/hillsideview46/case)

 To main design principles for the case are:
 - Ability to use a large battery mounted under the PCB and
 - Keep the top of the HSV fairly low profile for portability and ensure nothing sticks up above the keys.

 This is achieved by having an empty cavity under the PCB that allows using up to a 2000 mAh 306070 battery. This also allows for mounting the MCU on the underside of the PCB and having the nice!view display sit fairly low on top of the PCB.
 
 The case supports tenting using a magnetic tenting stand that uses 10x1 magnets in the case and 10x3 magnets in the stand. This also allows the two sides to attach magnetically for travel.

 ![](https://github.com/wannabecoffeenerd/HillSideView/blob/main/hillsideview46/doc/image/hsv_stealth_tented.jpg)

## Acknowledgments

Several keyboards have influenced this boards, primarily the
  [Hillside 46](https://github.com/mmccoyd/hillside), but also
  [Atreus](https://shop.keyboard.io/products/keyboardio-atreus),
  [Lily58](https://github.com/kata0510/Lily58),
  [Kyria](https://splitkb.com/collections/keyboard-kits/products/kyria-pcb-kit),
  [Corne](https://github.com/foostan/crkbd) and
  [Ferris](https://github.com/pierrechevalier83/ferris).
