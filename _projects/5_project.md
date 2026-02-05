---
layout: page
title: Romansh Lemmatizer
description: A basic, dictionary-based lemmatizer for Romansh.
img: assets/img/Lemmatizer.png
category: applications
importance: 3
---

This Python package implements a simple dictionary-based lemmatizer for Romansh. It tokenizes a given text and looks up each word in the Pledari Grond dictionaries, covering the five main Romansh idioms (Sursilvan, Sutsilvan, Surmiran, Puter, Vallader) as well as Rumantsch Grischun. The tool can be used to retrieve possible German glosses and to automatically infer the Romansh variety of a text based on dictionary coverage. A current limitation is that it performs no contextual disambiguation, returning all possible dictionary entries and morphological analyses for ambiguous word forms.

