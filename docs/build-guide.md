# Forager Build Guide

## List of Components

| Part Name | Part Number | Count | Notes |
| --------- | ----------- | ----- | ----- |
| Forager PCB | - | 1 | [Files here.](../forager-pcb/) |
| Seeed XIAO nRF52840 | - | 2 | Including Sense version; not compatible with other variants of the XIAO including RP2040 and ESP32-C3 |
| Choc V1 hot swap sockets | CPG135001S30 | 34 | |
| Diodes | 1N4148W | 34 | SOD-123 | - |
| Battery Connector | JST BM02B-ACHSS-GAN / MOLEX 781710002 | 2 (OPTIONAL) | Only required for batteries with JST ACH/Molex Pico-EZmate connectors. The two types should be compatible in both PCB footprint and physical connector.
| Battery | 301230 / 401230 | 2 | Widely available from many keyboard vendors. [Little Keyboards sell ones with JST ACH connectors](https://www.littlekeyboards.com/collections/new-products/products/battery-w-jst-connector) for use with the connector above.
| SMD M2 Nuts | SMTSO2020MTJ | 10 | https://www.lcsc.com/product-detail/SMD-round-nut_Sinhoo-SMTSO2020MTJ_C2916384.html |

### Case

| Part Name | Part Number | Count | Notes |
| --------- | ----------- | ----- | ----- |
| 3D-printed Case | - | 2 | [Files here.](../case/) Designed for FDM but should print just fine with SLA, MJF, etc..
| Countersunk M2 Screws | - | 18 | Total length 4-5mm. https://www.mcmaster.com/91294A002/
| Rubber Bumpers | - | 8+ | Anything not too thick will do. https://www.mcmaster.com/95495K18/
| LED Light Guide | - | 2 | 1.75mm  transparent filament segment, 6mm length |

### Tenting Legs

| Part Name | Part Number | Count | Notes |
| --------- | ----------- | ----- | ----- |
| Locating Pins | McMaster-Carr 97049A206 | 8 | https://www.mcmaster.com/97049A206/ |
| 8mm x 4mm x 2mm Rectangular Magnets | Apex Magnets M8x4x2MMBL | 8 | https://www.apexmagnets.com/magnets/8mm-x-4mm-x-2mm-block-neodymium-magnet |
| Rubber Bumpers | - | 4 | 10mm diameter, preferably hemispherical.

## PCB

Forager is designed for surface mounting the controller board, therefore it's not compatible with sockets.

This guide assumes that you're using a soldering iron; you can use a hot plate or hot air gun with solder paste. Low temp paste is preferred if you'd like to remove the XIAO later since it's less likely to mess up components on the XIAO itself.

Images shown are of an older revision of the board, without battery pads for direct wiring; everything else still apply.

- Break off the two halves from each other.
   - There will be some leftover bits from the mouse bites; leave them alone as they're not exposed and won't interfere with the case.

- Solder everything.

   ![fully soldered PCB](/docs/images/build_pcb_rear.jpg)

   - Start with the back side of the PCB where all the silkscreen is.
   - XIAO nRF52840
      - Solder two pads on opposite corners first to anchor it in place. Make sure it is lined up with the pads both horizontally and vertically.
      - Solder all remaining pads.
      - Flip the board over and solder the pin marked with a circle; this is the battery+ pin. You might need to stick the iron in the cutout to make sure it bonds with the pad on the XIAO properly. Flip the board back around.
   - Hot-swap sockets and diodes
      - Tin one pad first to anchor the diode/socket in place.
      - Solder the other pad.
      - Make sure the line on the diode package matches the direction of the silkscreen.
   - SMD Nuts
      - Place them in their respective holes; make sure they're fully seated. They should be sticking out towards the back like all other components.
      - Apply solder around the perimeter; flux is recommended.
      - Remove the protective tape.
   - ***OPTIONAL*** - Battery Connector
      - It is recommended to solder these with a hot plate or hot air, since the two mounting pads are difficult to reach with an iron and if not soldered properly, the connector may lift off the board entirely when removing the battery.
      - Tin one of the mounting pads (the wider ones), place the connector, make sure the electrical pads are lined up and reheat that pad again from the opening side.
      - Solder the other mounting pad and the electrical pads.
   - Battery without connector
      - Trim the battery wires to an appropriate length that they reach the circular pads with the battery itself inside the rectangle.
      - Solder the red wire to the pad marked +, and the black wire to the other.

## Case

- Print the four case parts. Pay attention to the print-in-place reset lever button on the base; it might fuse together with the surrounding and get stuck depending on the amount of first layer squish. Adjust z-offset if needed.

![case with reset lever button highlighted](/docs/images/build_case_reset.jpg)

- Cut two 6mm segments of transparent 3D-printing filament (1.75mm diameter).
   - From the inside, insert one into the slot in the case.
   - It might need some convincing; use a small pointy tool like an allen key to push it through the hole and then adjust back until it's flush with the case.

   ![case light guide 1](/docs/images/build_case_lg_1.jpg)
   ![case light guide 2](/docs/images/build_case_lg_2.jpg)
- Place the plate/top part on the front side of the PCB.
   - Install a couple of switches around the corners to align it with the PCB.
   - Then screw it in.
- Flip it around and install the base/bottom part.
   - Go first on the USB-C port side; make sure it's snug inside the cutout.
   - Once everything fits nicely together, screw it in.
   - You may want hold the top and bottom part together along the edges to make sure they're lined up while screwing in.

## Tenting Legs

- Insert two Pins and two Magnets into the tenting leg. It should be a very tight friction fit.
   - Apply the adhesive 10mm rubber bumper to the other end.
- Slot two magnets into the slots inside the case.
- Make sure all magnets are of the same orientation so that tenting legs all have the same polarity.
