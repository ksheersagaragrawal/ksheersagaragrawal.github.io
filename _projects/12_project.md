---
layout: page
title: Edge Detection
description: Implemtation of FFT and IFT in Python for feature extraction in images.   
img: assets/img/edgedetection.jpg
importance: 1
category: Misc
giscus_comments: true
repo: ksheersagaragrawal/Edge-Detection-Using-Fourier-Transform
---

## <span style="font-size: 24px;font-weight: bold;">GitHub Repository</span>
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords <a href="{{ site.baseurl }}/assets/pdf/ImageSegmentation.pdf" title="CV"><i class="fas fa-file-pdf"></i></a></span>
`Fourier Series`,`Convolution`,`Discrete Fourier Transform` `Fast Fourier Transform`, `Inverse Fourier Transform`,`Windowing`,`Zero Padding`,`Numpy`,`Matplotlib`,`OpenCV`.

## <span style="font-size: 24px;font-weight: bold;">Algorithm</span>

# Importing numpy, cv2 & matplotlib
{% raw %}
```html
import cv2 as cv
import numpy as np
from matplotlib import pyplot as plt
```
{% endraw %}

# Reading image in grayscale
{% raw %}
```html
img = cv.imread('lal_minar.jpg', 0)
```
{% endraw %}

# Frequency transform is a complex array
{% raw %}
```html
f = np.fft.fft2(img)
```
{% endraw %}

# Shifting the zero frequency component to the center
{% raw %}
```html
fshift = np.fft.fftshift(f)
```
{% endraw %}

# Finding the magnitude spectrum
{% raw %}
```html
A1 = 20
magnitude_spectrum = A1 * np.log(np.abs(fshift))
```
{% endraw %}

# Plotting
{% raw %}
```html
plt.subplot(121), plt.imshow(img, cmap='gray')
plt.title('Input Image'), plt.xticks([]), plt.yticks([])
plt.subplot(122), plt.imshow(magnitude_spectrum, cmap='gray')
plt.title('Magnitude Spectrum'), plt.xticks([]), plt.yticks([])
plt.show()
```
{% endraw %}

# Center
{% raw %}
```html
rows, cols = img.shape
crow, ccol = rows // 2, cols // 2
```
{% endraw %}

# HPF masking, center 12X12 grid masked 0, remaining all ones
{% raw %}
```html
mask = 12
fshift[crow - mask:crow + mask, ccol - mask:ccol + mask] = 0
```
{% endraw %}

# Finding the magnitude spectrum of masked Fourier Transform
{% raw %}
```html
A2 = 2000
fshift_mask_mag = A2 * np.log(np.abs(fshift))
```
{% endraw %}

# Restoring the original indexing
{% raw %}
```html
f_ishift = np.fft.ifftshift(fshift)
```
{% endraw %}

# Inverse FFT
{% raw %}
```html
img_back = np.fft.ifft2(f_ishift)
```
{% endraw %}

# Finding the magnitude spectrum
{% raw %}
```html
img_back = np.real(img_back)
```
{% endraw %}

# Plotting
{% raw %}
```html
plt.subplot(131), plt.imshow(img, cmap='gray')
plt.title('Lal Minar'), plt.xticks([]), plt.yticks([])
plt.subplot(132), plt.imshow(fshift_mask_mag, cmap='gray')
plt.title('FFT + Mask'), plt.xticks([]), plt.yticks([])
plt.subplot(133), plt.imshow(img_back, cmap='Reds')
plt.title('Image after HPF'), plt.xticks([]), plt.yticks([])
plt.show()
```
{% endraw %}

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ed_first.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ed_middle.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ed_final.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>


## <span style="font-size: 24px;font-weight: bold;">Procedure</span>
1. **Raw Signal Analysis**
   - Removal of power line interference using a notch filter.
   - Filtering out noise using a 4th order Butterworth Bandpass filter.
   - Full-wave rectification to zero-mean power.




