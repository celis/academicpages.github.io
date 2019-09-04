---
title: 'Text embeddings in hyperbolic space'
date: 2019-08-10
permalink: /posts/2019/08/blog-post-hyperbolic-embeddings/
tags:
  - representation learning
---

Here I review the idea of embedding text in hyperbolic space.  I follow the following articles:

[1] *"Poincaré Embeddings for Learning Hierarchical Representations"* from Maximilian Nickel and Douwe Kiela [arxiv:1705.08039](https://arxiv.org/abs/1705.08039).  

[2] *"Embedding Text in Hyperbolic Spaces"* from Bhuwan Dhingra, Christopher J. Shallue, Mohammad Norouzi, Andrew M. Dai and George E. Dahl [arxiv::1806.04313](https://arxiv.org/abs/:1806.04313)

[3] *"Poincaré GloVe: Hyperbolic Word Embeddings"* from Alexandru Tifrea, Gary Bécigneul and Octavian-Eugen Ganea [arxiv:1810.06546](https://arxiv.org/abs/1810.06546)

[4] *"Inferring Concept Hierarchies from Text Corpora via Hyperbolic Embeddings"* from Matt Le, Stephen Roller, Laetitia Papaxanthos, Douwe Kiela and Maximilian Nickel [arxiv:1902.00913](https://arxiv.org/abs/1902.00913)

Whats the motivation?




<br/><img src='/files/plot_wn_mammals_converged_crop.png' align="middle" style="width:600px;height:550px;"> 



Implementations of the model presented in [1] can be found in [gensim](https://radimrehurek.com/gensim/models/poincare.html)
and [facebook research](https://github.com/facebookresearch/poincare-embeddings). 





