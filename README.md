# Svg2Shenzhen
Inkscape extension for exporting drawing into Kicad PCB

TODO

![screenshot_125](https://user-images.githubusercontent.com/64752/38157030-170a81a0-34ad-11e8-85df-667a642505d8.png)

## Features

- Draw Any kind of shapes without restriction (unlike svg2mod)
- Support Drill Pad, and custom drill size
- Support Edge Cut (PCB Shape)
- Tested on OSX, and Windows and Linux

## Install

Download latest version of [svg2shenzhen-extension.zip](https://github.com/badgeek/svg2shenzhen-next/releases)

Extract and copy the files into the directory indicated in Edit -> Preferences -> System: User extensions

## How to

    1.Extension > Svg2Shenzhen > Prepare Document
    2.Choose layer (F.Cu.. etc)
    3.Draw PCB 
    4.Extension > Svg2Shenzhen > Export Kicad

Download and open [Example PCB](https://raw.githubusercontent.com/badgeek/svg2shenzhen-next/master/examples/viruspcb.svg)

## Tips

1. For Edge.Cut Layer, polygon or object need to be converted to path without fill and only outline
2. For Drill layer, place Circle object and it will be converted into drill pad in kicad

## Known Bugs

- The port of bitmap2component does not support non square image input, this issue tackled in prepare document by setting the document to square

## Reference

- [Svg2Shenzhen Announcement on Gosh Community Forum](https://forum.openhardware.science/t/svg2shenzhen-save-inkscape-drawing-as-kicad-pcb/989)
- [PCB Art with Inkscape - Developer log](http://wiki.8bitmixtape.cc/#/4_7.1-PCB-Art-with-Kicad-and-Inkscape) on 8BitMixtape Wiki 
- [Practical Guide to Designing PCB Art](https://medium.com/@urish/a-practical-guide-to-designing-pcb-art-b5aa22926a5c)
- [KitSprint ANORG 2018](http://wiki.sgmk-ssam.ch/wiki/KitSprint_ANORG_2018#Kicad_bitmap_import_for_Shenzhen_Ready)


## Buy me a Coffee

- [Buy me Coffee - patreon](https://www.patreon.com/badgeek)

## Credits
* inkscape-export-layers - https://github.com/jespino/inkscape-export-layers
* bitmap2component (kicad) - https://github.com/KiCad/kicad-source-mirror/tree/master/bitmap2component
* csv_output - https://github.com/tbekolay/csv_output
* svg2mod - https://github.com/mtl/svg2mod