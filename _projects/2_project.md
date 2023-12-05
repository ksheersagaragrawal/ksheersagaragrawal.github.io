---
layout: page
title: IoT SentryRover
description: STM-32 based IOT Sentry Rover, integrates sensor fusion and robust communication protocol for wide-range controllability.
img: assets/img/robot.jpg
importance: 1
category: Systems
giscus_comments: true
repo: ksheersagaragrawal/surveillancerobot
---


## <span style="font-size: 24px;font-weight: bold;">Github Repository</span>

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords</span>
`Sensor Fusion`,`Computer Vision`, `OpenCV`, `STM-32 Microcontroller`, `NodeMCU`, `Network Communication `, `Embedded Systems`.


IOT Surveillance Robot is a sentry rover designed for wide-range accessibility. It operates on the NodeMCU protocol, enabling seamless communication and control.

The Surveillance Robot can be controlled remotely through a user-friendly web application hosted at [https://ksheersagaragrawal.github.io/surveillancerobot/src/public/](https://ksheersagaragrawal.github.io/surveillancerobot/src/public/). The web interface provides intuitive controls for real-time interaction with the robot.

<div class="row text-center">
    <div class="col-sm mt-3 mt-md-0">
        <embed src="https://ksheersagaragrawal.github.io/surveillancerobot/src/public/" style="width:100%; height: 500px;">
    </div>
</div>

## <span style="font-size: 24px;font-weight: bold;">Operation</span>

**1. Surveillance Robot:** 
- The surveillance robot is designed for unmanned spaces. It has no range constraints and operates on battery power and internet connectivity.
- Team can operate rover using only four keys (A, W, S, D) from anywhere around the globe using a user-friendly web application interface.
- NodeMCU Server facilitates in real time communication between the web application and the sensors.

**2. Data Processing:**
- The NodeMCU reads data from various sensors, including temperature & humidity sensors, Camera Module, GPS Module.
- The NodeMCU connects to the predefined WiFi network and posts the json data on NodeMCU server.
- The Web Application fetches the sensor data from the NodeMCU in real time.
- The Web Application read the movement of operation of the rover and sends the data to the NodeMCU server.
- The NodeMCU reads incoming data and translates it into directional commands to the STM32 microcontroller.
- The STM32 interacts with motor driver, adjusting the robot’s movements based on the interpreted commands.

**2. Real-time Tracking:**
- The surveillance robot features a SIM28ML GPS module that continuously fetches real-time location data.
- The accuracy of location mapping is equivalent to the highest resolution available on Google Maps.
- The robot publishes its location data onto a dedicated website for remote monitoring.
- The web application connects to the live video streaming server using the ESP32 camera module attactched at the fore front of rover.
- ESP32 Cam Module featues Object Detection & Identification with OpenCV. Captured data, including images, can be stored in a database for future reference.

**4. Sensor Data Transmission:**
- The STM32 collects real-time data from temperature and humidity sensors, transmitting this information to the website.
- A safety feature is integrated into the robot, utilizing a proximity sensor at the front.
- In the presence of an unseen barrier, the robot automatically halts its movement, providing a safety mechanism.
- The operator can then redirect the robot in an alternative direction, ensuring safe and obstacle-free operation.


