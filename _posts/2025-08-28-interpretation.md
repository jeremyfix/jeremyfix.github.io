---
layout: post
title: Rethinking deep vision interpretability
date: 2025-08-28 10:00:00
description: Explainability with attribution is limited to indicate the where. Concept extraction allows to capture the what.
tags: explainability deep vision concept
categories: explanability
featured: true
related_publications: true
---

For his PhD award talk at Gretsi, Thomas Fel gave a talk on explainability of
deep vision models. Among the various approaches, attribution methods (Grad CAM) produce
saliency maps indicating which part of the input is used by the neural network
to build up its response. 

However, these attribution methods are restricted to inform about the where and
not the what. It does not tell you about the nature of the pattern the neural
networks has extracted. In this work, T. Fel developes techniques to extract
concepts from deep neural networks. Concepts are extracted by non-negative
matrix factorization techniques {% cite Gillis2024 %}. A survey on concept based
explainable AI can be found in {% cite Poeta2023 %}. In deep neural networks,
there is nothing like the grand mother cell, the concepts are encoded by
distributed patterns of activations {% cite Elhag2022 %}.


TBC
