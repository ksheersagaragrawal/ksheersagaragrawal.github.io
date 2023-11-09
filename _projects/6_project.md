---
layout: page
title: Spirometer
description: A project on Spirometer design and development
img: assets/img/spirometer.png
importance: 2
category: fun
---

## <span style="font-size: 24px;font-weight: bold;">Keywords</span>

## Keywords
`COVID-19`,`respiratory diseases`, `spirometry test`, `oxygen levels`,`spirometer`, `Forced vital capacity (FVC)`, `check restricted breathing`.

## Components Used
Node MCU (ESP 8266): Microcontroller for data processing.
LM393 Speed Measuring Sensor: Detects slotted disk rotations.
Arduino-Compatible Components: Manage data acquisition and processing.
Assembly: Integrate LM393 sensor with the slotted disk, ensuring precise alignment.

## Procedure
1. Initialize the Node MCU and configure it for data acquisition.
2. Establish communication with the LM393 speed measuring sensor.
3. Set up a loop to continuously monitor the sensor output.
4. Upon detecting a change in sensor output (hole detection), record the event.
5. Measure the time between consecutive hole detections to calculate the rotations per minute (rpm).
6. Transmit the rpm data to a connected computer or display unit.
7. Repeat the process to ensure real-time monitoring of spirometry readings.

<div class="row">
    <div class="col-sm">
        <iframe width="100%" height="315" src="https://www.youtube.com/embed/ZahFPBmPCoM" frameborder="0" allowfullscreen></iframe>
    </div>
</div>
<div class="caption">
    Learn more about the project by watching my assembling video. It provides a time lapse of the development process and calculating rotations per minute (rpm) for lung capacity. 
</div>