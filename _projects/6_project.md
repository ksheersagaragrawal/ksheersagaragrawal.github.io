---
layout: page
title: Spirometer
description: Arduino based health monitoring equipment for early detection of respiratory issues, including COVID-19.
img: assets/img/spirometer.png
importance: 4
category: Misc
---

## <span style="font-size: 24px;font-weight: bold;">Keywords</span>
`COVID-19`,`respiratory diseases`, `spirometry test`, `oxygen levels`,`spirometer`, `Forced vital capacity (FVC)`, `check restricted breathing`.

## <span style="font-size: 24px;font-weight: bold;">Components <a href="{{ site.baseurl }}/assets/pdf/spirometer.pdf" title="CV"><i class="fas fa-file-pdf"></i></a></span>
- **Node MCU (ESP 8266):** Microcontroller for data processing.
- **LM393 Speed Measuring Sensor:** Detects slotted disk rotations.
- **Arduino-Compatible Components:** Manage data acquisition and processing.
- **Assembly:** Integrate LM393 sensor with the slotted disk, ensuring precise alignment.


## <span style="font-size: 24px;font-weight: bold;">Procedure</span>
1. **Initialize Node MCU:** Set up for data acquisition.
2. **Establish LM393 Communication:** Connect with the speed measuring sensor.
3. **Continuous Monitoring:** Create a loop to monitor sensor output.
4. **Event Recording:** Record events on detecting changes in sensor output (hole detection).
5. **Calculate RPM:** Measure time between consecutive hole detections for rpm.
6. **Transmit Data:** Send rpm data to a computer or display unit.
7. **Real-time Monitoring:** Repeat the process for continuous spirometry readings.


<div class="row">
    <div class="col-sm">
        <iframe width="100%" height="315" src="https://www.youtube.com/embed/ZahFPBmPCoM" frameborder="0" allowfullscreen></iframe>
    </div>
</div>
<div class="caption">
    Learn more about the project by watching my assembling video. It provides a time lapse of the development process and calculating rotations per minute (rpm) for lung capacity. 
</div>