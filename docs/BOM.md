# Bill of Materials: ST-02 Levels v1.1

A machine-readable copy is in [BOM.csv](BOM.csv). The original spreadsheet is [hardware/levels/BOM.ods](../hardware/levels/BOM.ods).

| Qty | Reference | Part | Manufacturer / Part No. | Notes |
|----:|-----------|------|--------------------------|-------|
| 4 | J1-J4 | 3.5 mm mono switched jack, vertical PCB mount, with nut | QingPu WQP-PJ398SM or WQP518MA, or equivalent. Either one works. | [Datasheet / product page](http://www.qingpu-electronics.com/en/products/WQP-PJ398SM-362.html). The switched (normalling) contact is used on J3 (In 2) only, so J3 must be a switched jack. The pads are oval so the board can also take panel-mount style jacks such as the CUI MJ-3507 ([datasheet](https://www.cuidevices.com/product/resource/mj-3507.pdf)), which may be easier to source. Its sleeve is a solder lug rather than a pin, so it needs a short wire from the lug to the square pad. |
| 2 | RV1, RV2 | Potentiometer, 100 kΩ linear, 9 mm, vertical PCB mount with board-lock lugs, 6 mm D shaft (20 mm long), bushingless | Bourns PTV09A-4020F-B104, or equivalent | [Mouser product page](https://www.mouser.com/en/ProductDetail/Bourns/PTV09A-4020F-B104?qs=Qzws7J6gxqwTQanrz88HwA%3D%3D), [datasheet (PTV09 series)](https://www.bourns.com/docs/Product-Datasheets/PTV09.pdf). No center detent. No threaded bushing or nut: it's held by the PCB's two mounting lugs (the same mounting style as the Attenuverter's pots). An equivalent must fit the 9 mm footprint (3 pins in a row, 2 mounting lugs) and have a 6 mm shaft that fits the knob. |
| 2 | | Knob, 12 mm | Davies Molding 1221-J, or equivalent | [Mouser 5164-1221-J](https://www.mouser.com/en/ProductDetail/Davies-Molding/1221-J?qs=AaRlLUpeMsymqGRd5ndiLA%3D%3D). Pushes directly onto the pot's shaft. The pot has no nut, so this knob has no skirt (unlike the earlier 1227-J). An equivalent must fit the pot shaft. |
| 1 | | Main PCB, 15 x 100 mm, 2-layer, 1.6 mm FR4 | Schenktronics | |
| 1 | | Faceplate, 3HP (15 x 128.5 mm), 1.6 mm aluminum PCB | Schenktronics | Single-sided, so it can also be made in FR4. |

## Not included

| Qty | Part | Notes |
|----:|------|-------|
| 2 | M3 rack screws | Supplied with most Eurorack cases. |

No power cable is needed. The module is passive.
