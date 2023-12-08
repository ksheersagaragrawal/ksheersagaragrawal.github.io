---
layout: page
title: Motion Deblur
description: Removing Motion Blur from Images using Deep Generative Adversarial Network
img: assets/img/motion_blur.png
importance: 2
category: AI
giscus_comments: true
repo: ksheersagaragrawal/DeblurGAN
related_publications: ramakrishnan2017deep
---

<span style="font-size: 24px;font-weight: bold;">GitHub Repository</span>
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords <a href="{{ site.baseurl }}/assets/pdf/Deblur_Poster.pdf" title="CV"><i class="fas fa-file-pdf"></i></a></span>
`Generative Adversarial Networks`, `Dense Connections`, `Skip Connections`, `L1 Loss`, `Adversarial Loss`, `Perceptual Loss`, `Differential Augmentation`, `PyTorch Implementation`, `GAN Discriminator`, `GAN Generator`, `Image Quality Metrics`, `PSNR`, `SSIM`, `Motion Deblurring`, `Deep Convolutional Networks`.

## <span style="font-size: 24px;font-weight: bold;">Project Overview</span>
Our research project aims to address the common challenge in photography and computer vision: removing motion blur from images using the Deep Generative Adversarial Networks (GANs). Our model successfully restores sharpness and clarity to images that have been distorted by camera shake or subject movement.

## <span style="font-size: 24px;font-weight: bold;">What is a Generative Adversarial Network (GAN)?</span>
GAN model consists of two neural networks: a generator and a discriminator.The generator network generates synthetic data samples that resemble the training data, while the discriminator network tries to differentiate between the synthetic data and the real data. The generator is trained to produce realistic data while the discriminator is trained to distinguish between real and synthetic data. The networks work together in an adversarial manner to improve the generator's ability to generate realistic data.

<div class="row">
    <div class="col-sm-12 mt-md-0 mx-auto text-center">
         {% include figure.html path="assets/img/gan.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of GAN Structure: The generator output is connected directly to the discriminator input. Through backpropagation, the discriminator's classification provides a signal that the generator uses to update its weights.
</div>
