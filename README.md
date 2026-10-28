<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/images/logo-light.png">
  <img src="docs/images/logo-dark.png" alt="Schenktronics" width="320">
</picture>

# ST-02 Levels

A 3HP Eurorack dual passive attenuator from **Schenktronics**. Each channel has an input, an output, and a level knob, and the second input is normalled to the first, so one signal can go out at two different levels. No power needed.

<img src="docs/images/outline-front.svg" alt="Levels front panel" width="120">

## Features

- 3HP, 15 mm deep behind the panel (skiff-friendly), no power needed
- Two channels, each turning a signal down from full level to off
- In 2 is normalled to In 1: one input, two outputs at independent levels
- Works on audio, CV, gates, and bipolar signals
- All through-hole, 22 solder joints: a good first kit

## Documentation

| Document | For | PDF |
|----------|-----|-----|
| [User Manual](docs/manual.md) | Using the module | [PDF](docs/pdf/ST-02_Levels_User_Manual.pdf) |
| [Assembly Guide](docs/assembly-guide.md) | Building the kit | [PDF](docs/pdf/ST-02_Levels_Assembly_Guide.pdf) |
| [Bill of Materials](docs/BOM.md) ([CSV](docs/BOM.csv)) | Parts and sourcing | |

## Repository layout

```
hardware/
  ST-02_Levels.step            3D model of the assembled module
  levels/                      Main PCB (KiCad 5.1 schematic, KiCad 10 PCB)
    Levels.sch                   Schematic
    Levels.kicad_pcb             PCB layout
    Levels.step                  3D model
    BOM.ods                      Original BOM spreadsheet
  panel/                       Faceplate (KiCad 10, made as an aluminum PCB)
    LevelsFaceplate.kicad_pcb    Faceplate layout
    LevelsFaceplate.step         3D model
  jig/                         3D-printable solder jig (see below)
    ST-02_Solder_Jig.stl         Holds the pots and jacks while you solder
docs/                          Manual, assembly guide, BOM, images
  pdf/                           PDF versions of the manual and assembly guide
```

The `.github/` folder holds the automation that builds the PDFs. You can ignore it.

## Fabrication

| Board | Size | Layers | Thickness | Notes |
|-------|------|--------|-----------|-------|
| Main PCB | 15 x 100 mm | 2 | 1.6 mm | Standard green is fine |
| Faceplate | 15 x 128.5 mm | 1 | 1.6 mm | Aluminum PCB, white solder mask, black silkscreen. Only the front copper layer is used, so FR4 works too. |

## Sourcing your own parts

The [BOM](docs/BOM.md) lists every part. The jack pads are oval so the board can also take panel-mount style jacks, which may be easier to source. The CUI MJ-3507 is one example: its sleeve is a solder lug rather than a pin, so each one needs a short wire from that lug to the jack's square pad.

## Solder jig (optional)

[`hardware/jig/ST-02_Solder_Jig.stl`](hardware/jig/ST-02_Solder_Jig.stl) is a 3D-printable jig (27 x 116 x 17.5 mm) that holds the two pots and four jacks square and centered while you solder them. It replaces the faceplate as the alignment guide, so you fit the faceplate after soldering.

1. Print it in PLA, pockets facing up. It needs no supports.
2. Take the nuts off the jacks.
3. Fit the pots and jacks into the front of the PCB, the side with the part outlines, as in the [Assembly Guide](docs/assembly-guide.md). Don't solder anything yet.
4. Lower the jig over the parts, pockets down, with the end engraved "RV1" over RV1. Wiggle it until every pot and jack seats in its pocket, with the pot shafts in the round holes. The pocket mouths are chamfered to guide the parts in.
5. Turn the whole stack over so the jig sits on the bench and the back of the PCB (printed "ST-02 v1.1") faces up. Solder all the joints. The board sits 4 mm above the jig, so the plastic stays well clear of the iron.
6. Lift the board out of the jig and continue from the faceplate step of the [Assembly Guide](docs/assembly-guide.md).

The pockets are a close fit (0.1 mm per side). If your printer makes holes small and the jack threads or pot shafts won't drop in, try a slightly larger horizontal-expansion or hole-compensation setting in your slicer.

## License

This hardware design and its documentation are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). See [LICENSE](LICENSE).

The Schenktronics name and logo are trademarks of Schenktronics LLC and are not covered by the CC BY-NC-SA 4.0 license.

## Links

- Shop: <https://schenktronics.com/product/st-02/>
- Docs page: <https://schenktronics.com/docs/st-02/>
- Website: <https://schenktronics.com>
