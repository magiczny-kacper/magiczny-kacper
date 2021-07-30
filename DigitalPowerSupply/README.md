# Digital Power Supply<!-- omit in toc -->

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Description](#description)
- [Repositories](#repositories)
- [Things done for now](#things-done-for-now)
- [To do's](#to-dos)
- [Additional informations](#additional-informations)
- [Links, references, etc.](#links-references-etc)
- [Dependencies](#dependencies)
- [Notes](#notes)

## Description

The idea of this project is to the [H-bridge hardware](../H-Bridge/README.md)
into DC/DC bcuk converter, and then move to custom harware, designed for this
project. The prototype is going to be based fully on the H-bridge hardware.
The same PCB with additional passive elements on output as filter and and voltage
divider for voltage measurement. If the prototype will be successfull, then the
application may be ported to STM32G4 instead of STM32F3 if more performace is
required.

Main goals of this project is to create digitally controlled power supply
providing:
* usable user interface using buttons, led, rotary encoder and OLED display, for
configuring the output parameters of converter
* communication interface for remote configuration (via USB, from PC)
* PID controller for regulation of output in CC and CV modes

## Repositories
* [Power Supply Main Board](https://github.com/magiczny-kacper/DigitalPowerSupply_HW_MB)
* [Power Supply Front Panel](https://github.com/magiczny-kacper/DigitalPowerSupply_HW_FP)
* [Power Supply Software](https://github.com/magiczny-kacper/DigitalPowerSupply_SW_App)

## Things done for now

* None

## To do's

* None

## Additional informations

## Links, references, etc.

## Dependencies

## Notes