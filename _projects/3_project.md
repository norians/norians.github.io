---
layout: page
title: Concurrent Producer-Consumer
description: Java concurrency system implementing the producer-consumer pattern with synchronized coodination and safe shared-state access.
img: assets/img/proj-hilos.png
importance: 3
category: software
github: https://github.com/norians/concurrent-producer-consumer
---

This project implements the classic producer–consumer concurrency pattern using a First-In, First-Out (FIFO) buffer.

Multiple producer threads generate data and insert it into a shared buffer, while multiple consumer threads retrieve and process that data. The core goal of the project is to ensure correct synchronization, safe shared-state access, and deterministic behavior in a concurrent environment.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/FIFO.png" title="diagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

