---
layout: page
title: Image Encryption
description: Image Encryption Technique based on Chaos Theory and RK Method for confidentiality and protecting sensitive visual information.
img: assets/img/chaos.png
importance: 4
category: Systems
giscus_comments: true
repo: ksheersagaragrawal/ImageEncryption
# related_publications: einstein1956investigations, einstein1950meaning
---

## <span style="font-size: 24px;font-weight: bold;">GitHub Repository</span>
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords <a href="{{ site.baseurl }}/assets/pdf/image_encryption.pdf" title="IPython Notebook"><i class="fas fa-file-code"></i></a></span>
`Chaos Theory`, `Lorenz Equation`, `Runge Kutta Method`, `Image Encryption`, `Numerical Analysis`, `Python`, `Numpy`, `Matplotlib`, `Cryptography`, `Secure Communication`.


{% raw %}

```html
{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/ImageEncryption.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/ImageEncryption.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
    {% jupyter_notebook jupyter_path %}
{% else %}
    <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
```
{% endraw %}
