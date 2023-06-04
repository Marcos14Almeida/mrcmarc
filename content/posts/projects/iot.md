---
title: "IoT - Temperature module for Weather Station"
date: 2022-12-10T20:08:28-03:00
hero: /images/projects/iot board.jpg
description: A temperature module for the weather station project of my IoT classes
theme: Toha
menu:
  sidebar:
    name: 22-IoT - Weather Station
    identifier: weather station
    parent: projects
    weight: 500
---

**Development**

Start: 08/2022.

End: 12/2022.


**Project description**
([Github](https://github.com/open-weather-iot/temperature-module))

This project was developed for my IoT class - IE321 - Tópicos em Eletrônica II, teached by prof. Fabiano Fruett. The objective of the course was to develop a meteorological station, where each student was responsible for a sensor. I developed the temperature sensor module and helped to create and standardize the code architecture for easy integration with the Raspberry Pi. In addition I worked with 3D printing to integrate the module in the final version of the weather station adding a support.

The temperature sensor project, has a 4-wire PT100 type sensor, a MAX31865 signal converter module for SPI communication with the Raspberry Pi Pico board and with data visualization on a Nokia 5110 display.

VSCode was used together with MicroPython to program the microcontroller. The `main.py` file executes a loop, which performs the sensor reading, and returns a set of parameters (such as the raw resistance value measured by the PT100 and the calculated temperature). The `src/max31865.py` file contains the conversion of the value read by the module to its respective associated temperature value, in which the number of GPIO pins used is defined as an input parameter.

In addition, the project contains the Altium files for creating the 2-sided PCB of the project and the Gerber and NC Drill files for its fabrication in the "Outputs" folder. Datasheets and reference documents are also attached in the project.


([How to use MAX31865](https://learn.adafruit.com/adafruit-max31865-rtd-pt100-amplifier/pinouts))

([Datasheet MAX31865](https://www.analog.com/media/en/technical-documentation/data-sheets/max31865.pdf))

([TinkerCad Design](https://www.tinkercad.com/login?next=%2Fthings%2F56pSbytFH0f-copy-of-pt100-suporte%2Fedit%3Fsharecode%3D3ICvXV23SPOnYPUSbMTf2dd61epz0CMu_3WBmKMw6yA))


**Screenshot**

<div style="display: flex; flex-wrap: wrap; justify-content: center;">
  <img src="/posts/projects/images/iot/iot1.jpg" alt="iot" style="width: 30%; margin: 10px;">
  <img src="/posts/projects/images/iot/iot2.jpg" alt="iot" style="width: 60%; margin: 10px;">
    <figcaption>Final temperature module in operation</figcaption>
</div>

<br>
<div style="display: flex; flex-direction: column;  align-items: center;">
    <img src="/posts/projects/images/iot/tinkercad.jpg" alt="iot" style="width: 50%; margin: 10px;">
      <figcaption>3D printed support designed with TinkerCad</figcaption>
  <br>
    <img src="/posts/projects/images/iot/iot layout.png" alt="iot" style="width: 50%; margin: 10px;">
      <figcaption>Temperature module diagram</figcaption>
  <br>
    <img src="/posts/projects/images/iot/pcb.jpg" alt="iot" style="width: 50%; margin: 10px;">
      <figcaption>Final IoT project board</figcaption>
  <br>
    <img src="/posts/projects/images/iot/final_module.jpg" alt="iot" style="width: 50%; margin: 10px;">
      <figcaption>Final Weather Station board mounted</figcaption>
  <br>
    <img src="/posts/projects/images/iot/weather_station.jpg" alt="iot" style="width: 50%; margin: 10px;">
      <figcaption>Final Weather Station result</figcaption>
  <br>
    <img src="/posts/projects/images/iot/graph.jpg" alt="iot" style="width: 50%; margin: 10px;">
      <figcaption>Temperature module operating</figcaption>
  <br>
</div>

**Tools**

- Micropython
- Altium
- 3-D Printing (TinkerCad)
- MAX31865 signal converter module
- 4-wire PT100 SENSOR
- Raspberry Pi
- Nokia 5110 display