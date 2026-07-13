A universal I2C hub for fischertechnik systems, designed to connect a variety of controllers to Grove/Seeed modules

More project info on https://www.whizzbizz.com/nl/i2c-hub

## Overview

This repository documents a hardware concept for a compact I2C distribution board with:

- Connectors for multiple fischertechnik controller families
- Six Grove/Seeed-compatible I2C ports
- Both 5V and 3.3V power feed for Grove modules
- Shared I2C bus with proper power and level handling

The goal is to make it easy to connect sensors and I2C devices to fischertechnik robotics controllers while maintaining signal compatibility and clean wiring.

## Features

- Universal I2C hub for fischertechnik controller compatibility
- Six Grove/Seeed I2C connectors
- 5V / 3.3V power for Grove modules
- Common I2C SDA / SCL bus routing
- Power distribution for Grove modules from controller supply
- Pull-up resistor configuration for I2C bus
- I2C bus level shifting and voltage distribution

## Compatibility

This hub is intended to work with a wide range of fischertechnik controllers, including but not limited to:

- Classic TX Controller
- TXT Controller
- TXT4.0 Controller
- RX Controller
- ftDuino & FtDuino32
- Any other I2C device with I2C with 3.3 or 5 volt DC power and I2C levels

## Connector Layout

The board includes:

- Voltage regulators to generate 3.3V from 5V from 9 volt, from the fischertechnik controller or external supply via 2.5mm fischertechnik plug
- 3 flatcable connectors for I2C bus and ground (no DC voltage is passed!) from fischertechnik controllers
- 3 Grove/Seeed I2C connectors (4-pin: VCC, GND, SDA, SCL) providing 3.3 volt DC power
- 3 Grove/Seeed I2C connectors (4-pin: VCC, GND, SDA, SCL) providing 5 volt DC power

### Grove/Seeed Port Pinout

Each Grove connector uses the following pin order:

- SCL
- SDA
- VCC
- GND

## Power Options

Board features:

- 9V input from the fischertechnik controller or external supply
- 3.3V regulator output for modules that require 3.3V
- 5V regulator output for modules that require 5V
