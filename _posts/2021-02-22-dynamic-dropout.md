---
title: Dynamic Dropout
layout: default
img_path: assets/images/dd.png
authors: Đorđe Miladinović & Joachim M. Buhmann
conference: arXiv'21
paper: https://openreview.net/forum?id=I4c4K9vBNny
code: https://gitlab.ethz.ch/djordjem/dynamic-dropout
category: ml
---

It is by now well known that MLE-trained autoregressive variational models lead to degenerate learning with uninformative latent variables.
We argue that teacher forcing is a major cause of this issue and propose a dynamic variant of dropout as a novel form of regularization.