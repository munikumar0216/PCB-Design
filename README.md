# PCB-Design

# 5 V → 3.3 V Buck Converter

A compact DC-DC buck converter designed in **KiCad** to convert a 5 V input supply to a regulated 3.3 V output.

This project demonstrates the complete PCB design workflow, including component selection, datasheet-based circuit design, schematic capture, footprint assignment, PCB placement, routing, ground-plane implementation, ERC/DRC validation, 3D inspection, and manufacturing-file generation.


## Project Overview 

The objective of this project was to design a practical switching power-supply PCB suitable for powering 3.3 V digital and embedded-system circuits.

### Key Specifications

|        Parameter     |      Value       |
|----------------------|----------------- |
| Input Voltage        |    5 V DC        |
| Output Voltage       |    3.3 V DC      |
| Converter Type       | Synchronous Buck Converter |
| Regulator IC         |    AP63200WU     |
| Switching Frequency  |Datasheet-defined |
| Inductor             |      6.8 µH      |
| PCB Design Tool      |       KiCad      |
| PCB Type             |      2-Layer     |
| Input Connector      |  2-pin, 2.54 mm  |
| Output Connector     |  2-pin, 2.54 mm  |



### Main Components

| Reference |        Component          |   Value / Part | Package     |
|-----------|---------------------------|-----------------|------------|
|     U1    |        Buck Regulator     |     AP63200WU   | TSOT-23-6  |
|     L1    |       Power Inductor      |    6.8 µH | SMD |            |
|     C1    |       Input Capacitor     |    10 µF | 1206 |            | 
|     C2    |     Bootstrap Capacitor   |   100 nF | 0805 |            |
|     C3    |    Feed-forward Capacitor |   100 pF | 0805 |            |
|     C4    |      Output Capacitor     |    22 µF | 1206 |            |
|     C5    |      Output Capacitor     |22 µF| 0805/1206*|            |
|     R1    |     Feedback Resistor     |   196 kΩ | 0805 |            |
|     R2    |     Feedback Resistor     |    62 kΩ | 0805 |            |
|     J1    |      Input Connector      |  2-pin, 2.54 mm |     THT    |
|     J2    |      Output Connector     |  2-pin, 2.54 mm |     THT    | 


> *Verify the final footprint/value combination against the actual BOM before manufacturing.
