# Ernest Master Node Schematics
Eagle files for Ernest base node

[Master Project Repo](https://github.com/rschlaikjer/Ernest)

## What is this
Ernest is the next step of the [ArNest](https://github.com/rschlaikjer/ArNest),
and takes it from a single-location thermostat to a many node system consisting
of a base station and one or more smaller nodes that collect and report
atmospheric data to the base. This way the system can monitor multiple rooms, as
well as the outside conditions.

These EAGLE files show the schematic for the master node, which collects data
transmitted by the slaves (as well as from its own onboard sensors) and sends
it to the server. This node also controls the relay for the furnace, if you
are using this as a thermostat.

This board is designed to be run over PoE, using a Silvertel AG9000 or similar
module, as is used on the PoE version of the Arduino ethernet.

For the code to run on the master node,
[see here](https://github.com/rschlaikjer/ernest-master-code).

## Parts list
(All prices per unit and approximate)

- ($2.00) Atmega 328P (with arduino-style bootloader)
- ($3.19) USB FTDI programmer
- ($1.50) (Optional) BMP180 breakout board
- ($13.75) (Optional) HIH-6130 humidity sensor
- ($0.98) nrf24L01 wireless transciever
- ($0.39) LM1117 3.3V regulator
- ($0.07) 16 MHz crystal oscillator
- ($0.03) 22pF capacitors
- ($0.08) Momentary reset switch
- ($0.01) 320 Ohm resistors
- ($0.03) LEDs
- ($2.50) RB1-125BHQ1A PoE RJ45 jack
- ($10.64) Ag-9000S (or newer) PoE module

**Total BOM: Approx. $15 per board** + 13.75 for humidity, as well as the cost
of PCB manufacture.

## Pretty Pictures

![Current Prototype](/master_v0.jpg?raw=true "Current prototype")

![Schematic](/master_sch.png?raw=true "Schematic")

![Board Layout](/master_brd.png?raw=true "Board Layout")
