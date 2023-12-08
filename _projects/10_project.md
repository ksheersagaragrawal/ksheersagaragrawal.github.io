---
layout: page
title: Statistical Language Modelling Using N-grams
description: English Word Prediction Model which predicts the next word in a semi-complete sentence
img: assets/img/next_word.gif
importance: 3
category: AI
giscus_comments: true
repo: ksheersagaragrawal/Next_Word_Prediction_Using_Ngrams
---

## GitHub Repository

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo.html repository=page.repo %}
</div>
{% endif %}

## <span style="font-size: 24px;font-weight: bold;">Keywords </span>
`Next Word Prediction`, `N-gram Model`, `Natural Language Toolkit`, `Probabilistic Models`, `Laplace Smoothing`, `Python`, `Gradio`, `Python`, `Text Processing`, `Hugging Face`.

## <span style="font-size: 24px;font-weight: bold;">Next Word Prediction Using the NGram </span>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/next_word.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>


This project leverages the power of N-gram models for predicting the next word in a given sentence fragment. The core of the project is built using Python and the Natural Language Toolkit (NLTK) for processing and analyzing text data. The model uses trigrams as the basis for predictions, incorporating Laplace Smoothing to deal with rare words. The application is made user-friendly and interactive through a Gradio web interface, facilitating easy testing and demonstration of the model's capabilities.

## <span style="font-size: 24px;font-weight: bold;">Interactive Demo <a href="https://huggingface.co/spaces/Shruhrid/Next_Word_Prediction" title="hugging face"><i class="fas fa-play-circle"></i></a></span>
Explore the model's capabilities through an interactive web application hosted on Hugging Face. Simply input a partial sentence, and the model will predict the next word.

