# Silo Temperature Measurement <!-- omit in toc -->

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Description](#description)
- [Repositories](#repositories)
- [Things done for now](#things-done-for-now)
- [To do's](#to-dos)
- [Additional informations](#additional-informations)
- [Links, references, etc](#links-references-etc)
- [Dependencies](#dependencies)
- [Notes](#notes)

## Description

Purpose of this device is to replace existing devices, used to temperature
measurement inside of grain siloses, as currently used device are >20 years old,
and are not performing well. They are also using old, unsupported communication
protocol, SIC800. New sensors also brings more modern way to cummunicate -
the Modbus RTU protocol. To allow compatibility with old devices, the desired
protocol can be selected during configuration. As the sensors used are one
wire DS18x sensors, device allows to detect connected sensors, and sort them,
by heating one by one. Whole configuration is performed via RS485 serial port.
It can operate with up to 10 sensors on the bus. Device can be powered with
wide range of voltage - -6-55V DC- and -6-40V AC-.

## Repositories

- [Sensor Software](https://github.com/magiczny-kacper/SiloTemp_Software)
- [Sensor Hardware](https://github.com/magiczny-kacper/SiloTemp_PCB)

## Things done for now

- Modbus communication works
- One Wire protocol is supported
- Sensors are detected on the bus
- Sorting sensors by heating one by one works
- Improve code quality

## To do's

- Resolve problems with SIC800 protocol
- Consider moving to STM32 and running application on [zephyr os](https://github.com/zephyrproject-rtos/zephyr)
  - Decide which mcu to use
  - Pros and cons of moving to zephyr:
    - Pros:
      - Easier development and debugging
      - Ready to use 1 wire and DS18B20 driver
      - Easier to develop serial console
      - bootloader
    - Cons:
      - Needs whole rework and pcb redesign
      - SIC800 could be pretty big issue

## Additional informations

## Links, references, etc

## Dependencies

## Notes
