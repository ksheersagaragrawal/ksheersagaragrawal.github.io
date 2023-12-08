---
layout: page
title: Motion Deblur
description: Removing Motion Blur from Images using Deep Generative Adversarial Network
img: assets/img/motion_blur.png
importance: 2
category: AI
giscus_comments: true
repo: ksheersagaragrawal/DeblurGAN
---

## GitHub Repository

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords </span>
`Generative Adversarial Networks`, `Dense Connections`, `Skip Connections`, `L1 Loss`, `Adversarial Loss`, `Perceptual Loss`, `Differential Augmentation`, `PyTorch Implementation`, `GAN Discriminator`, `GAN Generator`, `Image Quality Metrics`, `PSNR`, `SSIM`, `Motion Deblurring`, `Deep Convolutional Networks`.


## <span style="font-size: 24px;font-weight: bold;">Project Overview</span>
Our project aims to address the common challenge in photography and computer vision: removing motion blur from images. Utilizing the power of Deep Generative Adversarial Networks (GANs), our model successfully restores sharpness and clarity to images that have been distorted by camera shake or subject movement.

## <span style="font-size: 24px;font-weight: bold;">What is a Generative Adversarial Network (GAN)?</span>
GANs are a class of machine learning frameworks designed by opposing two neural networks against each other. A generator network creates images, while a discriminator network evaluates them. Through this adversarial process, the generator learns to produce more realistic images.

## <span style="font-size: 24px;font-weight: bold;">Our Model Architecture</span>
The architecture of our GAN model is specifically tailored to address motion blur. It includes a unique combination of dense and skip connections to efficiently handle varying degrees of blur without explicit blur kernel estimation.

## <span style="font-size: 24px;font-weight: bold;">Results</span>
Our model demonstrates remarkable ability in deblurring images. Below are some before-and-after comparisons showcasing the effectiveness of our approach.

<!-- <div class="row">
    <!-- Add your before-and-after image comparisons here -->
    <!-- Example: -->
    <div class="col-sm-4 mt-3 mt-md-0 text-center">
         {% include figure.html path="assets/img/before_after_example.jpg" title="Before and After Deblurring" class="img-fluid rounded z-depth-1" %}
    </div>
</div> -->

## <span style="font-size: 24px;font-weight: bold;">Conclusion and Future Work</span>
Our project not only enhances the quality of images affected by motion blur but also opens new avenues in real-time image processing applications. Future enhancements may include adapting the model for video deblurring and improving its efficiency for mobile devices.

<!-- ## <span style="font-size: 24px;font-weight: bold;">References and Acknowledgements</span>
We would like to thank [contributors and references], whose insights and resources were invaluable in the success of this project. -->
