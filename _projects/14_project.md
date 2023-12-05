---
layout: page
title: Image Segmentation
description: A Scikit-based implementation of the Random Walker Algorithm for image segmentation - distinuishing various features in digital images.
img: assets/img/imagesegmentation.png
importance: 6
category: AI
giscus_comments: true
repo: ksheersagaragrawal/Image-Segmentation-using-Random-Walker-Algorithm
---

## <span style="font-size: 24px;font-weight: bold;">GitHub Repository</span>
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords <a href="{{ site.baseurl }}/assets/pdf/image_segmentation.pdf" title="IPython Notebook"><i class="fas fa-file-code"></i></a></span>
`Image Segmentation`, `Random Walker Algorithm`, `Graph Theory`, `Digital Image Processing`, `Python`, `Numpy`, `AI in Imaging`, `Computational Techniques`.

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/Image_Segmentation.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/Image_Segmentation.ipynb%}{% endcapture %}
{% if notebook_exists == "true" %}
    {% jupyter_notebook jupyter_path %}
{% else %}
    <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
