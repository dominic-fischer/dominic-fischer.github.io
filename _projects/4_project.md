---
layout: page
title: Bullinger's Network Visualised
description: A dynamic and interactive visualisation illustrating social Networks in Swiss Reformer Heinrich Bullinger's letter exchange.
img: assets/img/Bullinger.png
category: applications
importance: 3
---
*I began this project while working as a student research assistant at the Institute of Computational Linguistics and later completed and refined it independently (spring semester of 2025 until spring semester of 2026)*

A leading reformer in Zurich and successor to Huldrych Zwingli, **Heinrich Bullinger** played a central role in spreading Reformation ideas across Switzerland and Europe. His vast correspondence, around 12,000 letters, is of exceptional historical value, offering rich insights into contemporary events, political dynamics, and theological debates, as well as the personal lives and economic conditions of people in the early modern era.

In an effort to preserve this letter corpus, the **Bullinger Digital** project ([website](https://www.bullinger-digital.ch/index.html), [repo](https://github.com/bullinger-digital)) aimed to digitise, annotate and enrich these letters. The **visualisation** ([application](https://dominic-fischer.github.io/dynamic-graph/), [repo](https://github.com/dominic-fischer/dynamic-graph)) is based on marked greeting formulas in the letter, which are used to infer the **social networks around Heinrich Bullinger**.

Note: The visualisation and its documentation are still under development.

**Below**: Undirected greetings between the 20 most prolific writers in our corpus in the year 1540.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/saluta.png" title="Greeting network" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
