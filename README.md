# Hillside View Ergonomic Keyboard

The Hillside View (HSV) is a modified version of the [Hillside 46](https://github.com/mmccoyd/hillside). It is a 
 wireless (or wired) [40%](https://deskthority.net/wiki/40%25) 
 split-[ergonomic](https://deskthority.net/wiki/Ergonomic_keyboard) 
 keyboards with a 
 [column-stagger](https://deskthority.net/wiki/Staggering#Columnar_layout) 3x6+5 or a 3x5+5 layout.

The main features that the HSV adds over the Hillside 46 are:
- [nice!view](https://github.com/getkeops/keops/tree/main) e-paper display for better battery life
- Cleaner outer pinky column cut-off
- Support for a cirque trackpad with an FFC connector on the PCB itself
- Case design with support for large 750-3000 mAh batteries under the PCB
- Under PCB mount for the MCU for a cleaner top display mounting

The HSV has optional factory parts soldering (PCBA) except for the switches, MCU, display, TRRS, LEDs, battery switch, and optional hotswap sockets.

Their common features are:

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

See the board readmes for details, rationales and default keymaps.

*Keycaps*: Hillside View is _only_ suitable for choc v1 switches and keycaps based on an 18 x 17mm switch spacing, such as the [MBK](https://mkultra.click/mbk-choc-keycaps), [Lowprokb LDSA](https://lowprokb.ca/products/ldsa-low-profile-blank-keycaps), [MoErgo MCC](https://mkultra.click/moergo-mcc-pom-1u-keycap/) or [Asymplex Choc](https://www.asymplex.xyz/category/choc). Not MX ones, nor 18 x 18mm ones such as Work Louder, nor Kailh Choc Transparent.

Hillside View includes ZMK Firmware
- [full size](https://github.com/mike1808/zmk-config)
- [five column](https://github.com/wannabecoffeenerd/zmk-config)

QMK firmware can be adapeted from the [Hillside firmware](https://github.com/qmk/qmk_firmware/tree/master/keyboards/handwired/hillside) 


## Key Use

I expect most people will primarily use either the tucked three thumbs or the extended three (not counting the upper thumb). They can choose where the thumb arc suits them best. I find the thumb finger is best for reaching the upper thumb key; clearing the lower thumb requires some care, but it is still very useful. The middle finger also handily reaches the most tucked thumb key, as the open space is a good reference. The keys outside of the primary three thumb keys are convenient for infrequent lock layers, escape, or for use when not actively typing for things such as mute.

## Why

The main reason for this project is to make the keyboard more wireless friendly by adding the e-paper display and allowing experimenting with using a cirque trackpad (once ZMK support for it is more stable)

## Hardware and Build Guide

See the [original Hillside wiki](https://github.com/mmccoyd/hillside/wiki)
 first for PCB ordering, parts links and a build guide with pictures.

See the [HSV wiki](https://github.com/wannabecoffeenerd/hillside/wiki) for HSV specific
 build guide.

## Acknowledgments

Several keyboards have influenced this boards, primarily the
  [Hillside 46](https://github.com/mmccoyd/hillside), but also
  [Atreus](https://shop.keyboard.io/products/keyboardio-atreus),
  [Lily58](https://github.com/kata0510/Lily58),
  [Kyria](https://splitkb.com/collections/keyboard-kits/products/kyria-pcb-kit),
  [Corne](https://github.com/foostan/crkbd) and
  [Ferris](https://github.com/pierrechevalier83/ferris).
