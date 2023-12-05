---
layout: page
title: Real-Time Object Tracking
description: A real-time object tracking using Gaussian Mixture Models (GMM), focusing on background subtraction and motion analysis in video streams.

img: assets/video/rtod.png
importance: 4
category: AI
giscus_comments: true
repo: ksheersagaragrawal/Real-Time-Object-Tracking-using-GMM
---

## <span style="font-size: 24px;font-weight: bold;">GitHub Repository</span>
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords <a href="{{ site.baseurl }}/assets/pdf/rtod_gmm.pdf" title="IPython Notebook"><i class="fas fa-file-code"></i></a></span>
`Object Tracking`, `Real-Time Analysis`, `Gaussian Mixture Model (GMM)`, `Matrix Algebra`, `Numpy`, `OpenCV`, `Background Subtraction`, `Video Processing`, `Traffic Surveillance`, `Python Programming`.

## <span style="font-size: 24px;font-weight: bold;">Real-Time Object Tracking Demonstration</span>
<div class="row">
    <div class="col-sm mt-3 mt-md-0 mx-auto text-center">
        {% include video.html path="assets/video/object_detection.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
   Segments moving objects from the background - demonstrating effective real-time object detection.
</div>


## <span style="font-size: 24px;font-weight: bold;">Collab File</span>
{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/rtod_gmm.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/rtod_gmm.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
    {% jupyter_notebook jupyter_path %}
{% else %}
    <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
