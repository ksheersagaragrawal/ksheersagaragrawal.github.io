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

## <span style="font-size: 24px;font-weight: bold;">Keywords <a href="{{ site.baseurl }}/assets/pdf/image_segmentation.pdf" title="CV"><i class="fas fa-file-pdf"></i></a></span>
`Image Segmentation`, `Random Walker Algorithm`, `Graph Theory`, `Digital Image Processing`, `Python`, `Numpy`, `AI in Imaging`, `Computational Techniques`.


## <span style="font-size: 24px;font-weight: bold;">Random Walk Algorithm Formulas </span>
The Random Walk Algorithm for image segmentation is based on the following steps and formulas:

1. **Node Marking**:
   The nodes in the image are marked based on the following criteria:
    - Let `p(i, j)` be the pixel value at position `(i, j)` in the image.
    - Mark the nodes as follows:
        - If `p(i, j) > 110`, then mark as `255` (white).
        - If `p(i, j) < 75`, then mark as `0` (black).

2. **Matrix Operations**:
   All the unmarked nodes will be marked in subsequent steps. The key formula in the Random Walk Algorithm for image segmentation is:

    $$
    L_u \cdot X = (-B)^T \cdot M
    $$

    Where:
    - $$L_u$$ is a submatrix of the L matrix containing information about all the unmarked to unmarked nodes.
    -  $$X$$ is the matrix representing probabilities.
    - $$B^T$$ is a submatrix of the L matrix that contains information about all the unmarked nodes to marked nodes.
    - $$M$$ matrix is defined for zero and 255 class $$M_0$$ and $$M_{255}$$.


3. **Calculating Probabilities**:
   - First, calculate $$X$$ using the formula:
     $$X = L^{-1} \cdot (B^T) \cdot M$$
     where $$L^{-1}$$ is the inverse of matrix $$L$$, $$B^T$$ is the transpose of matrix $$B$$, and $$M$$ is the predefined matrix.
     
   - The probability for pixel $$k$$ taking the value 0 is given by the corresponding element in matrix $$X$$ for $$M_0$$, which can be represented as:
     $$P(k \text{ takes value } 0) = X_k \text{ for } M_0$$
     where $$X_k$$ is the k-th element in the matrix $$X$$.

4. **Image Construction**:
   - Construct a new image from $$X$$ by comparing their probability to determine the final pixel values.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/randomwalk.png" title="example image" class="img-fluid rounded z-depth-1" style="max-width: 50% !important;" %}
    </div>
</div>
<div class="caption">
    Pixels represent nodes with directed, weighted edges.
</div>

## <span style="font-size: 24px;font-weight: bold;">Accuracy Calculation</span>
The accuracy of the segmentation is calculated as follows:

$$
\text{Accuracy} = \frac{|\text{White Pixels in SkitLearn} - \text{White Pixels in New Image}|}{\text{Total White Pixels} + \text{Total Black Pixels}}
$$



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
