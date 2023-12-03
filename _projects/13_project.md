---
layout: page
title: EMG Signal Analsis
description: Analzying Zygomaticus Muscle Signal in MATLAB using Digital Signal Processing techniques.
img: assets/img/emg.jpeg
importance: 3
category: Misc
giscus_comments: true
repo: ksheersagaragrawal/EMG-Signal-Analysis
---

## <span style="font-size: 24px;font-weight: bold;">GitHub Repository</span>
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords<a href="{{ site.baseurl }}/assets/pdf/emg.pdf" title="CV"><i class="fas fa-file-pdf"></i></a></span>
`EMG Signal Analysis`,`Muscle Activation Signal`,`Anomaly Detection` `Raw Signal Processing`, `Time Domain Analysis`,`Filtering`, `Zero Padding`, `Windowing`.


## <span style="font-size: 24px;font-weight: bold;">Procedure</span>
1. **Raw Signal Analysis**
   - Removal of power line interference using a notch filter.
   - Filtering out noise using a 4th order Butterworth Bandpass filter.
   - Full-wave rectification to zero-mean power.

2. **Time Domain Analysis**
   - Calculation of Mean Absolute Value (MAV) and Root Mean Square (RMS).

3. **Frequency Domain Analysis**
   - Fast Fourier Transform (FFT) to analyze frequency components.
   - Application of bandpass filters for specific frequency ranges.
   - Zero-padding to enhance frequency resolution.
   - Windowing to mitigate spectral leakage effects.

4. **Pattern Recognition**
   - Recognition of sustained smiling patterns.


<div class="row">
    <div class="col-sm">
        <iframe width="100%" height="315" src="https://www.youtube.com/watch?v=yzUZTIryukM" frameborder="0" allowfullscreen></iframe>
    </div>
</div>
<div class="caption">
    Learn more about the project by watching our analysis video. It provides a detailed explaination of the data aquisition and pre-processing of the raw signal captured. 
</div>

