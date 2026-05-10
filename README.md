# NeutrinoAIO
Overview
This is a flight controller meant for model rockets with a focus on light and robust design. SMD components are utilised whenever possible to bring down the FC (=flight controller) weight and make it more durable
This design is intended to fit a 60 mm rocket, but it can be expanded to fit larger ones too
The design is focused on expandability and future proofness - a connector/pins are provided for daisy chaining expansion boards to the FC.

Who is this meant for?
This is a high performance piece of electronics meant as an all in one solution for complex rockets, though even using it on simple ones will provide a lot of useful and interesting data.

Features
  - An array of sensors for data collection - gyroscope, accelerometer, barometer, GPS
  - Radio transmitter for broadcasting the location of the rocket for easy recovery
  - Pin interface for expandability using board add-ons

Show below is the schematic for the flight controller:

<img width="1420" height="1417" alt="Screenshot 2026-05-10 220315" src="https://github.com/user-attachments/assets/128b6880-6ac2-49cc-ba4d-d05fc436161d" />

The flight controller will feature a "stack" design utilizing two 4 layer PCBs with one sided assembly to make home assembly possible.
The stacks will be connected with a cable and will also have an extra connection for future/community expansion boards, allowing for up to 4 SPI modules to be connected (4 IO) ports.

The design should be cheap and relatively easy to assemble at home, allowing more rocket enthusiast to get detailed information from their launches.
