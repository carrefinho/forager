# Forager

> why does the large Voyager not simply eat the small Forager?

Forager is a Voyager-inspired 34-key low-profile wireless split keyboard powered by ZMK.

![Forager keyboard in white](/docs/images/forager_white.jpg)

## Design

- Condensed [ZSA Voyager](https://www.zsa.io/voyager) layout without outer pinkie column and number row
- Hot-swap Kailh Choc V1 switches in Choc (18x17mm) spacing with Voyager-esque switch puller grooves

![Switch-plate cutouts](/docs/images/forager_switch.jpg)

- Wireless only with Seeed XIAO nRF52840 running ZMK firmware
- Magnetic tenting legs inspired by Voyager and [Unicorne](https://www.boardsource.xyz/products/unicorne)

![Forager keyboard with magnetic tenting legs attached](/docs/images/forager_tented.jpg)

- Compact silhouette without the usual blank space occupied by the controller board
- Fully enclosed with 3D-printed two-piece case
- Minimal BOM by utilizing XIAO nRF52840's onboard RGB LED and reset button

![Forager keyboard with LED indicator lit up in blue alongside reset button on the bottom](/docs/images/forager_led_reset.jpg)


## Build Guide and Parts List

[Find the build guide here.](/docs/build-guide.md)

## Firmware

[Find the ZMK module here.](https://github.com/carrefinho/forager-zmk-module)

## Credits

- [ZSA Voyager](https://www.zsa.io/voyager): overall layout & aesthetics
- [GEIGEIGEIST/TOTEM](https://github.com/GEIGEIGEIST/TOTEM): XIAO PCB footprint and general placement
- [ebastler/marbastlib](https://github.com/ebastler/marbastlib): symbols and PCB footprints
- [caksoylar/zmk-rgbled-widget](https://github.com/caksoylar/zmk-rgbled-widget): enables the RGB LED to display ZMK relevant info

## Gallery

![Forager keyboard in black and white](/docs/images/forager_bw.jpg)
![Forager keyboard with detached tenting leg](/docs/images/forager_legs.jpg)
![Forager keyboard in black](/docs/images/forager_bob.jpg)