---
layout: page
title: Pruning
description: Effects of Structured Pruning on Handling Uncertainty Estimates
img: assets/img/pruning.png
importance: 1
category: AI
giscus_comments: true
repo: ksheersagaragrawal/LotteryTicketPruning
related_publications: frankle2018the, blalock2020state,laves2020wellcalibrated, daxberger2021laplace
---

## <span style="font-size: 24px;font-weight: bold;">Github Repository</span>

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}


## <span style="font-size: 24px;font-weight: bold;">Keywords <a href="{{ site.baseurl }}/assets/pdf/pruning.pdf" title="CV"><i class="fas fa-file-pdf"></i></a></span>
`Neural Network Pruning`, `Lottery Ticket Hypothesis`, `Structured Pruning`, `Overfitting`, `PyTorch`, `CNN`. `FCC`, `Accuracy Metrics`, `Uncertainty Estimation`, `Monte-Carlo Drop Out`, `Reliability Diagram`,`Expected Caliberation Error`,`Out-Of-Distribution Test`.

## <span style="font-size: 24px;font-weight: bold;">Project Overview <a href="{{ site.baseurl }}/assets/pdf/Affects_of_Pruning_Neural_Network.pdf" title="CV"><i class="fas fa-file-pdf"></i></a></span>
Our project focuses on implementing and researching various neural network pruning techniques, particularly extending the lottery ticket hypothesis to structured pruning. 

<div class="row">
    <div class="col-sm-9 mt-md-0 mx-auto text-center">
         {% include figure.html path="assets/img/pruning_strats.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An illustration of various structured pruning strategies.
</div>

## <span style="font-size: 24px;font-weight: bold;">Lottery Ticket Hypothesis</span>
{% raw %}
```html
<div class="lottery-ticket-hypothesis">
  <p>A randomly-initialized, dense neural network contains a subnetwork that is initialized such that—when trained in isolation—it can match the test accuracy of the original network after training for at most the same number of iterations.</p>
</div>
```
{% endraw %}

We aim to reduce model size while maintaining performance, accuracy, and uncertainty, and to decrease training time.

<div class="row">
    <div class="col-sm-12 mt-md-0 mx-auto text-center">
         {% include figure.html path="assets/img/make_moons_acc.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Accuracy vs Pruning Ratio for Different Techniques
</div>

## <span style="font-size: 24px;font-weight: bold;">Uncertainity </span>
 For a better understanding of calibration and the value of ECE, we performed an Out-of-Distribution (OOD) Detection for CIFAR10 trained model on CIFAR100 dataset.

<div class="row">
    <div class="col-sm-4 mt-md-0 mx-auto text-center">
         {% include figure.html path="assets/img/cifar10.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-8 mt-md-0 mx-auto text-center">
         {% include figure.html path="assets/img/ood_cifar100.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Our analysis demonstrates that neural network pruning reallocates confidence intervals, evidenced from the reduced misclassification of <b>man</b> images in the <b>deer</> category after intensive pruning, enhancing the model's reliability and robustness.
</div>