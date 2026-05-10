This is the updated and almost final shematic. It containts everything it will need to function except the connector for joining the two boards together.
It was fully reorganized and made to bve way more readable.
I decided to make the flight controller a stack design to minimise signal interference, make assembly easier and simplify routing reducing the risk of a mistake being made.
The components will be split like this:

  - Top board, top layer
    - LoRa radio transmitter module and its antenna connector
    - GPS module and its patch antenna, possibly connected through a UFL connector
    - bms280 barometer module for better airflow
    - 14 pin connector for future expandability - carries SPI signals, power and four GPIO pins connected to the microcontroller
  
  - Top board, bottom layer
    - 14 pin connector for joining the two boards together, has 4 free pins going to the rp2040 GPIO for expandability, 3 chip select pins for the modules, 3 SPI pins (MISO,MOSI,SCL), 2 power and 2 ground pins
  
  - Bottom board, top layer
    -  RP2040 microcontroller
    -  Flash storage for the microcontroller
    -  Accelerometer and gyro module
    -  Micro USB power and data port and its buck converter'
    -  main buck converter for battery power
    -  voltage divider for battery voltage sensing using the ADC pin
    -  pins for connecting the servo (on the bottom so that the battery voltage isnt carried through the connector)
    -  14 pin connector for joining the two boards together
    -  Crystal oscillator for the RP2040

  - Bottom board, bottom layer
    - XT30 battery connector

  
<img width="1420" height="1417" alt="image" src="https://github.com/user-attachments/assets/0d34649b-6533-4bdd-9809-5dc9530ff4f8" />


I also selected the footprints for all of the components except some connectors. I will mostly be utilizing large 1206 capacitors but will also use small 0402 100nF capacitors for filtering near the RP2040 due to space constraints.
The resistors will be mostly 0805.

You can see the full list here:

<img width="2524" height="1721" alt="image" src="https://github.com/user-attachments/assets/040ef8cf-b2b5-4583-b876-514d45b08c24" />

Some component sizes might still be changed but this should be pretty close to final state.
I needed to download a couple of external footprints for some modules such as the LoRa, I will include them in a folder in the folder of this prototype.
