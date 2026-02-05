---
layout: page
title: Romansh Lemmatizer
description: A basic, dictionary-based lemmatizer for Romansh.
img: assets/img/Lemmatizer.png
category: applications
importance: 3
---
*This Lemmatizer is the main fruit of my work as a student research assistant in the post-Bullinger-project era (autumn semester of 2025 until spring semester of 2026)*

This Python package implements a simple dictionary-based lemmatizer for Romansh ([browser demo](https://huggingface.co/spaces/ZurichNLP/romansh-lemmatizer), [repository](https://github.com/ZurichNLP/romansh_lemmatizer)). It tokenizes a given text and looks up each word in the Pledari Grond dictionaries, covering the five main Romansh idioms (Sursilvan, Sutsilvan, Surmiran, Puter, Vallader) as well as Rumantsch Grischun. The tool can be used to retrieve possible German glosses and to automatically infer the Romansh variety of a text based on dictionary coverage. A current limitation is that it performs no contextual disambiguation, returning all possible dictionary entries and morphological analyses for ambiguous word forms. For more details, please consult the linked repository.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lemm.png" title="Lemmatizer illustration" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Above:** an illustration of the core capabilities of the lemmatizer.<br>
**Below:** an example of how to use the python package. We can see the different possible lemmas assigned to the word form *fomantada*.

```
from romansh_lemmatizer import Lemmatizer

lemmatizer = Lemmatizer()
sent = "La vuolp d'eira darcheu üna jada fomantada."
doc = lemmatizer(sent)

doc.idiom               # >>> <Idiom.VALLADER: 'rm-vallader'>
doc.tokens              # >>> ['La', 'vuolp', "d'", 'eira', 'darcheu', 'üna', 'jada', 'fomantada', '.']
token = doc.tokens[-2]  # >>> fomantada
token.all_lemmas        # # {
                        #   rm-surmiran::fomanto: [PoS=ADJ;Gender=FEM;Number=SG],
                        #   rm-surmiran::fomantar: [PoS=V;VerbForm=PTCP;Tense=PST;Gender=FEM;Number=SG],
                        #   rm-vallader::fomantar: [PoS=V;VerbForm=PTCP;Tense=PST;Gender=FEM;Number=SG]
                        #   ...
                        # }
```
