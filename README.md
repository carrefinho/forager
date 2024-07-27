# Forager

> why does the larger Voyager not simply eat the small Forager?

Forager is a Voyager-inspired 34-key low-profile wireless split keyboard powered by ZMK.

![Forager keyboard in black and white](/docs/images/forager_bw.jpg)

## Design

- Condensed [ZSA Voyager](https://www.zsa.io/voyager) layout without outer pinkie column and number row
- Hot-swap Kailh Choc V1 switches in Choc (18x17mm) spacing
- Wireless only with Seeed XIAO nRF52840 running ZMK firmware
- Magnetic tenting legs inspired by Voyager and [Unicorne](https://www.boardsource.xyz/products/unicorne)

![Forager keyboard with magnetic tenting legs attached](/docs/images/forager_tented.jpg)

- Compact silhouette that eliminates the usual blank space occupied by the controller board
- Fully enclosed with 3D-printed two-piece case
- Minimal BOM by making use of XIAO nRF52840's onboard reset button and RGB LED

![Forager keyboard with LED indicater lit up in blue](/docs/images/forager_led.jpg)


## Build Guide and Parts List

[Read the build guide here.](/docs/build-guide.md)

## Firmware

[ZMK config repository.](https://github.com/carrefinho/forager-zmk-module)

## To-Do

- Detailed Build Guide
- Potential 36-key option

## Credits

- [ZSA Voyager](https://www.zsa.io/voyager): overall layout & aesthetics
- [GEIST TOTEM](https://github.com/GEIGEIGEIST/TOTEM): XIAO PCB footprint and general placement
- [Cem Aksoylar's zmk-rgbled-widget](https://github.com/caksoylar/zmk-rgbled-widget): enables the RGB LED to display ZMK relevant info.

## Gallery

![Forager keyboard in white](/docs/images/forager_white.jpg)
![Forager keyboard with detached tenting leg](/docs/images/forager_legs.jpg)