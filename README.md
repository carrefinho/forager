# Forager

> why does the larger Voyager not simply eat the smaller Forager?

Forager is a Voyager-inspired 34-key low-profile wireless split keyboard powered by ZMK.

![Forager keyboard in white](/docs/images/forager_white.jpg)
![Forager keyboard with magnetic tenting legs attached](/docs/images/forager_tented.jpg)

## Design Goals

- Condensed [ZSA Voyager](https://www.zsa.io/voyager) layout without outer pinkie column and number row
- Magnetic tenting legs inspired by Voyager and [Unicorne](https://www.boardsource.xyz/products/unicorne)
- Compact silhouette eliminating the usual blank space occupied by the dev board
- Fully enclosed with 3D-printed two-piece case
- Minimal BOM by making use of XIAO nRF52840's onboard reset button and RGB LED
- Hot-swap Kailh Choc V1 switches in Choc (18x17mm) spacing

## List of Components

| Part Name | Part Number | Count | Notes |
| --------- | ----------- | ----- | -------------- |
| Seeeduino XIAO nRF52840 | - | 2 | Including Sense version; not compatible with other variants of the XIAO including RP2040 and ESP32-C3 |
| Choc V1 hot swap sockets | CPG135001S30 | 34 | |
| Diodes | 1N4148W | 34 | Designed for SOD-123; glass MELF diodes may work too
| Battery Connector | JST BM02B-ACHSS-GAN / MOLEX 781710002 | 2 (OPTIONAL) | Only required for batteries with JST ACH/Molex ezMate Pico connectors. The two types should be compatible in both PCB footprint and physical connector.
| Battery | 301230 / 401230 | 2 | Widely available from many keyboard vendors. [Little Keyboards sell ones with JST ACH connectors](https://www.littlekeyboards.com/collections/new-products/products/battery-w-jst-connector) for use with the connector above.
| SMD M2 Nuts | SMTSO2020MTJ | 10 | https://www.lcsc.com/product-detail/SMD-round-nut_Sinhoo-SMTSO2020MTJ_C2916384.html |
| Countersunk M2 Screws | - | 18 | Total length 4-5mm. https://www.mcmaster.com/91294A002/
| Rubber Bumpers | - | 8+ | Anything not too thick will do. https://www.mcmaster.com/95495K18/

### Tenting Legs Parts

| Part Name | Part Number | Count | Notes |
| --------- | ----------- | ----- | -------------- |
| Locating Pins | McMaster-Carr 97049A206 | 8 | https://www.mcmaster.com/97049A206/ |
| 8mm x 4mm x 2mm rectangular Magnets | Apex Magnets M8x4x2MMBL | 8 | https://www.apexmagnets.com/magnets/8mm-x-4mm-x-2mm-block-neodymium-magnet |
| Rubber Bumpers | - | 4 | 10mm diameter, preferably hemispherical.

## Build Guide


## To-Do

- Detailed Build Guide
- Potential 36 key option

## Credits

- [ZSA Voyager](https://www.zsa.io/voyager): overall layout & aesthetics

- [GEIST TOTEM](https://github.com/GEIGEIGEIST/TOTEM): XIAO PCB footprint and general placement

- [Cem Aksoylar's zmk-rgbled-widget](https://github.com/caksoylar/zmk-rgbled-widget): enabling the RGB LED to display ZMK relevant info.

## Gallery

![Forager keyboard in black and white](/docs/images/forager_bw.jpg)
![Forager keyboard with detached tenting leg](/docs/images/forager_legs.jpg)