# Solax-X3-MIC-G2-Virtual-Smart-Meter
Smart meter emulator

Using Node Red modbus server I was able to sumulate a smart meter wirking with Solax X3 MIC G2 inverter.
It uses Shelly 3em and bunch of Home Assistant helpers to get the necessary data for the inverter.

A Modbus RTU to TCP relay is also needed. Pesonally I am using USR-W610.
Mode selection: Modbus TCP <=> Modbus RTU
Application settings: Socket B set to on, TCP, port - port of the modbus server, address - RPI 4 where Home Assistant and Node Red are installed, timeout 30 (probably does not matter)
**** note, add more screenshots******

The inverter asks for that data which is stored in modbus server in Node Red. Server replies with stored data and inverter seems happy with it.

Statistics in Solax Cloud seem to show correct values, export limiting feature works as well
