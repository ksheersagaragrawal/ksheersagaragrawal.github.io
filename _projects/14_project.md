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


## <span style="font-size: 24px;font-weight: bold;">Random Walk Algorithm Formulas <a href="{{ site.baseurl }}/assets/pdf/
The Random Walk Algorithm for image segmentation is based on the following steps and formulas:

1. **Node Marking**:
   - Mark nodes based on pixel values.
   - If greater than 110, then mark as 255.
   - If less than 75, then mark as 0.

2. **Unmarked Nodes**:
   - All the unmarked nodes will be marked in subsequent steps.

3. **Matrix Operations**:
   - `Lu . X = (-B)^T . M`
   - For a matrix of size p*q, we will have L of size p*q*8.
   - `(B)^T` is a submatrix of the L matrix that contains information about all the unmarked nodes to marked nodes.
   - `Lu` is a submatrix of the L matrix containing information about all the unmarked to unmarked nodes.
   - `M` matrix is defined for zero and 255 class `M0` and `M255`.

4. **Calculating Probabilities**:
   - Find `L inverse`, `(B)^T`, and `M` matrix to find `X`.
   - `X` for `M0` is the probability for pixel k taking value 0.

5. **Image Construction**:
   - Construct a new image from `X` by comparing their probability to determine the final pixel values.

## Accuracy Calculation

The accuracy of the segmentation is calculated as follows:

Accuracy = (|White Pixels in SkitLearn - White Pixels in New Image|) / (Total White + Black Pixels) 

Overall accuracy achieved in the project: 93.682%

## <span style="font-size: 24px;font-weight: bold;">Collab File</span>
{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/Image_Segmentation.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/Image_Segmentation.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
    {% jupyter_notebook jupyter_path %}
{% else %}
    <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
