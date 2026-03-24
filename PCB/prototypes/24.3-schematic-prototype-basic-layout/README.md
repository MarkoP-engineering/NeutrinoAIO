This is the first schematic prototype that has all the basic necessary sensors featured and connected.
The connections are very non-final, and will be redone to assure everything is connected correctly.
The schematic currently features:
  - RP2040 microprocessor with its necessary surrounding components (capacitors, crystal oscillator, flash chip..)
  - USB-C port providing both data and power, for easy programming without neeeding to worry about the battery
  - Step down converter to bring the 5V USB power to 3.3V required for the RP2040
  - MPU6000 accelerometer and gyroscope for rocket orientation and g-force measurement
  - NEO-M8M GPS module for position and altitude tracking
  - Ebyte E22 400 MM22S LoRa 400Mhz radio transmitter for sending telemetry to the ground station during the launch
  - BME 280 Barometer and humidity sensor for precise altitude measurement
