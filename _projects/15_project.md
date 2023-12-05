---
layout: page
title: Real-Time Object Tracking
description: Effects of Structured Pruning on Handling Uncertainty Estimates
img: assets/video/object_detection.mp4
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
`Chaos Theory`, `Lorenz Equation`, `Runge Kutta Method`, `Image Encryption`, `Numerical Analysis`, `Python`, `Numpy`, `Matplotlib`, `Cryptography`, `Secure Communication`.

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
