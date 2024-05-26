# Reflow Solder Plate Version 1

# WARNING:
### It is not recommended to make this project as there are tons of issues, see the 'Known issues' below

## Features
- 10x10cm hot plate
- EST 100W PCB hot plate
- Soldering with reflow curves
- LCD display with rotary encoder controls
- 3D printed casing
- Case temperature management with fan and temp sensor
- Fused power socket
- Multiple boards, compact assembly

## Guide
### Electronics
Download the provider gerber files and upload to your favorite PCB manufacturer. It is recommended to purchase a stencil too.
Settings for both PCBs:

| Setting | Value |
| --- | --- |
| Base Material | FR-4 |
| Layers: | 2 |
| Dimension: | 100 mm* 100 mm |
| PCB Qty: | 5 |
| Product Type | Industrial/Consumer electronics |
| Different Design | 1 |
| Delivery Format | Single PCB |
| PCB Thickness: | 1.6 |
| Impedance Control | no |
| PCB Color | Green |
| Silkscreen | White |
| Material Type | FR4-Standard TG 135-140 |
| Via Covering | Tented |
| Surface Finish | HASL(with lead) |
| Deburring/Edge rounding | No |
| Outer Copper Weight | 1 oz |
| Gold Fingers | No |
| Flying Probe Test | Fully Test |
| Castellated Holes | no |
| Edge Plating | No	|
| 4-Wire Kelvin Test | No |
| Paper between PCBs | No |
| Appearance Quality | IPC Class 2 Standard	Confirm |
| Silkscreen Technology | Ink-jet/Screen Printing Silkscreen |
| Board Outline Tolerance |±0.2mm(Regular) |

Other manufacturing settings might work too, these are which I used when ordering at JLCPCB

After ordering the PCBs and the parts, which can be found in the BOM, you can start soldering. You can use the BOM to know where each component goes.

### Case
You can now print the casing, files can be found in the repo. For the assebly you will need 6 M2(2 long, 4 short), 8 M3 and 2 M4 screws and inserts.

### Assembly
There is a seperate file in the repo that goes in depth on how to assemble the case
 

## Known issues
Due to the scope and time limitation of the project there are numerous known issues
- Headers used for power delivery for the heating circuitry is not capable of handling the currents
- Pads on the RFR board are too small to solder the wires from the transformer to.
- Annular rings on the mounting holes are too small
- Resistance calculation on the hot plate is wrong, too low resistance -> pulls too much current
- Tolerances on some case parts are too narrow (especially when 3D printing)
- Hole for the LCD display is too small
- Standoffs bend and fold when inserting the threaded inserts
- No support for a second case fan