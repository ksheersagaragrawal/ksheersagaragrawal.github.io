---
layout: page
title: Face Recognition 
description: Effects of Structured Pruning on Handling Uncertainty Estimates
img: assets/img/3.jpg
importance: 5
category: AI
giscus_comments: true
repo: ksheersagaragrawal/surveillancerobot
---

## <span style="font-size: 24px;font-weight: bold;">GitHub Repository</span>
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords <a href="{{ site.baseurl }}/assets/pdf/eigenface.pdf" title="IPython Notebook"><i class="fas fa-file-code"></i></a></span>
`Object Tracking`, `Real-Time Analysis`, `Gaussian Mixture Model (GMM)`, `Matrix Algebra`, `Numpy`, `OpenCV`, `Background Subtraction`, `Video Processing`, `Traffic Surveillance`, `Python Programming`.

## <span style="font-size: 24px;font-weight: bold;">Real-Time Object Tracking Demonstration</span>
<div class="row">
    <div class="col-sm-4 text-center">
        <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/Gr0HpDM8Ki8" frameborder="0" allowfullscreen></iframe>
    </div>
    <div class="col-sm-8 mt-3 text-center">
        {% include video.html path="assets/video/object_detection.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    This video demonstrates our GMM-based object tracking algorithm in action, highlighting its capability to accurately differentiate and track moving objects in real-time video streams.
</div>


## <span style="font-size: 24px;font-weight: bold;">Collab File</span>
{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/eigenface.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/eigenface.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
    {% jupyter_notebook jupyter_path %}
{% else %}
    <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
