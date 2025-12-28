---
layout: page
title: Medical Semantic QA System
description: Medical question-answering system based on embedding similarity and curated clinical data.
img: assets/img/proj-medical.png
importance: 1
category: software
related_publications: true
---

Medical Semantic QA System is an applied NLP project focused on semantic retrieval.

The system processes medical questions by encoding them into vector representations and retrieving the most semantically relevant answers from a curated clinical dataset. It is built using sentence-transformer models and fine-tuned with a triplet-loss strategy to improve retrieval quality.

The project covers the full pipeline: data parsing and cleaning, exploratory analysis of label imbalance, model fine-tuning, embedding-based similarity search, and deployment through a lightweight Flask API.

    ---
    Tags: Semantic retrieval (NLP), Sentence embeddings, Triplet loss fine-tuning
    ---

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/proj-medical.png" title="" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/proj-medical2.png" title="" class="img-fluid rounded z-depth-1" %}
    </div>
</div>