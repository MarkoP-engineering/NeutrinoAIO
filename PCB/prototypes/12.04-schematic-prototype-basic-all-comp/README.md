This is the first schematic prototype with all of the needed components present and connected.
The current component list is:
  - RP2040 microcontroller
  - E22-400M22S LoRa radio transmitter
  - Neo M8M GPS module
  - MPU6000 accelerometer and gyro module
  - Bosch BME280 barometer and temperature sensor
  - Texas Instruments TPS563200 buck converter module
  - W25Q128JVS flash module
Notes for PCB design etc.:
Place decoupling 100nF and 1uF caps close to RP2040, 1uF close to VREG IN and VREG OUT, ground plane under USB traces (?)
E22M - verify reset pin cap and resistor, verify antenna inductor coil - afaik unneeded if correct antenna used
Place barometer near the sides for airflow

I am currently unsure all of the components will fit on a single 56mm diameter PCB. If not I will consider moving the buck converter and possibly other components onto a separate board 
and creating a design similar to an FPV stack.
<img width="2074" height="1639" alt="image" src="https://github.com/user-attachments/assets/d66ac5ef-ab5b-45d6-9343-e991724911a9" />
