---
layout: page
title: EMG Signal Analsis
description: Analzying Zygomaticus Muscle Signal using digital signal processing techniques.
img: assets/img/emg.jpeg
importance: 2
category: Misc
giscus_comments: true
repo: ksheersagaragrawal/EMG-Signal-Analysis
---
## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords</span>
`EMG Signal Analysis`,`Muscle Activation Signal`,`Anomaly Detection` `Raw Signal Processing`, `Time Domain Analysis`,`Filtering`, `Zero Padding`, `Windowing`.

## <span style="font-size: 24px;font-weight: bold;">Components <a href="{{ site.baseurl }}/assets/pdf/emg.pdf" title="CV"><i class="fas fa-file-pdf"></i></a></span>
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
        <iframe width="100%" height="315" src="https://www.youtube.com/watch?v=yzUZTIryukM" frameborder="0" allowfullscreen></iframe>
    </div>
</div>
<div class="caption">
    Learn more about the project by watching out analysis video. It provides a detailed explaination of the data aquisition and pre-processing of the raw signal captured. 
</div>

