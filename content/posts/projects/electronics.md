---
title: "Electronics Projects"
hero: /images/projects/electronics.jpg
date: 2014-12-10T20:08:28-03:00
description: Electronics Projects
theme: Toha
menu:
  sidebar:
    name: Electronics Projects
    identifier: electronics
    parent: projects
    weight: 500
---


TCC Liceu
---------

**Development**

Start: 09/2014.

End: 11/2014.


**Project description**

This work aims at the implementation of electronic concepts for the creation of a project that assists the parking of an automotive vehicle. The circuit used will detect obstacles through the use of an ultrasonic sensor, which will emit sound waves that will be reflected by the object. Their return time will determine the distance between the vehicle and the obstacle. If the distance is short, a sound alert will warn the driver, thus avoiding possible accidents and damage to the vehicle.

**Screenshot**

<div style="display: flex; flex-wrap: wrap; justify-content: center;">
    <img src="/posts/projects/images/electronics/tcc car.png" alt="tcc" style="width: 40%; margin: 10px;">
    <img src="/posts/projects/images/electronics/tcc liceu.png" alt="tcc" style="width: 40%; margin: 10px;">
    <img src="/posts/projects/images/electronics/tcc prototype.png" alt="tcc" style="width: 60%; margin: 10px;">
</div>

**Tools**
- Arduino
- Buzzer
- Ultrasonic sensor SRF04
- LCD Display

<!-- ########################################################################################################### -->
<hr> <!-- Divider line -->

LED Bargraph
------------

**Development**

Start: -/2013.

End: -/2013.

**Project description**

An LED bargraph is a visual display that responds to audio frequencies. It consists of a series of LEDs arranged in a linear configuration. The incoming audio signal from a device, such as a cell phone, is filtered into different frequency ranges using transistors. Each LED is associated with a specific frequency range, and when the audio signal falls within that range, the corresponding LED lights up. The LED signals are amplified and transmitted to a speaker, allowing the LEDs to light up in synchronization with the music being played from the connected device. This creates an engaging visual representation of the audio, where the LEDs illuminate and change intensity in response to the music's frequencies.

**Screenshot**

<div style="display: flex; flex-wrap: wrap; justify-content: center;">
    <img src="/posts/projects/images/electronics/liceu bargraph 3.png" alt="pisca" style="width: 50%; margin: 10px;">
    <img src="/posts/projects/images/electronics/liceu bargraph.png" alt="pisca" style="width: 30%; margin: 10px;">
    <img src="/posts/projects/images/electronics/liceu bargraph 2.png" alt="pisca" style="width: 70%; margin: 10px;">
</div>

**Tools**
- Speaker
- LEDs
- Capacitors
- Homemade board
- Transistors

<!-- ########################################################################################################### -->
<hr> <!-- Divider line -->

Analogic Blinking LEDs
-----------------------

**Development**

Start: -/2012.

End: -/2012.

**Project description**

An analog blink circuit, also known as an astable multivibrator, is an electronic circuit that generates a continuous blinking or oscillating output signal. It typically consists of two transistors, capacitors, resistors, and a power supply.

Here's how it works:

- **Initial State**: The circuit begins in an unstable state where one transistor is in the "ON" state (conducting) and the other is in the "OFF" state (non-conducting).

- **Capacitor Charging**: The capacitor connected to the "ON" transistor starts to charge through a resistor. As the voltage across the capacitor increases, it eventually reaches a threshold level.

- **Switching Transistors**: Once the threshold voltage is reached, it triggers a switch, causing the "ON" transistor to turn off and the "OFF" transistor to turn on.

- **Capacitor Discharging**: The capacitor connected to the "OFF" transistor starts to discharge through another resistor. As the voltage across the capacitor decreases, it eventually drops below a threshold level.

- **Switching Transistors Again**: Once the threshold voltage is reached, it triggers another switch, causing the "OFF" transistor to turn off and the "ON" transistor to turn on again.

- **Repeat Cycle**: The process repeats, with the transistors switching back and forth in an oscillating manner. This results in a continuous blinking or oscillating output signal.

By adjusting the values of the resistors and capacitors in the circuit, you can control the frequency and duty cycle of the blinking signal. Although simple the analog blink circuit is very used in applications such as blinking LEDs, timers, and oscillators.

**Screenshot**

<div style="display: flex; flex-wrap: wrap; justify-content: center;">
    <img src="/posts/projects/images/electronics/pisca 1.jpg" alt="pisca" style="width: 30%; margin: 10px;">
    <img src="/posts/projects/images/electronics/pisca 2.jpg" alt="pisca" style="width: 30%; margin: 10px;">
    <img src="/posts/projects/images/electronics/pisca 3.jpg" alt="pisca" style="width: 30%; margin: 10px;">
</div>


**Tools**
- LEDs
- Homemade board