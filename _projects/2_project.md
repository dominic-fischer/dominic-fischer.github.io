---
layout: page
title: Text Tutor
description: A local-first application that helps you understand texts of your choice by providing additional clues!
img: assets/img/texttutorbg.png
importance: 3
category: applications
giscus_comments: true
---
*This is my bachelor thesis, done in the spring semester of 2024.*

[Text-Tutor](https://github.com/dominic-fischer/Text-Tutor) is a **local-first application that helps you better understand any text you choose by showing useful clues and annotations**. It runs entirely on your own machine (no cloud required), using a Flask backend, React frontend, and SQLite database. When you input or paste text, it processes the content and displays word-level grammatical cues like parts of speech or grammatical functions. You can also use context menu actions to get Wordnet definitions and synonyms, OLLaMa rephrasing, or GoogleTranslate translations. For a more detailed overview and explanations, please consult the repository linked above.

**Left:** word-level grammatical clues for the word *code*.<br>
**Right:** sentence-level additional functionalities, such as translation (here into dutch) or simplified rephrasing.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/texttutor.png" title="grammar comparison" class="img-fluid rounded z-depth-1" %}
    </div>
        <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/texttutor2.png" title="grammar comparison" class="img-fluid rounded z-depth-1" %}
    </div>
</div>