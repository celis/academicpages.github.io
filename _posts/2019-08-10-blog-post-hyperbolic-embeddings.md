---
title: 'Text embeddings in hyperbolic space'
date: 2019-08-10
permalink: /posts/2019/08/blog-post-hyperbolic-embeddings/
tags:
  - representation learning
---

Here I review the idea of embedding text in hyperbolic space.  I will focus on the application of these methods towards the generation of word embeddings in an unsupervised manner.   The standard algorithms for generating word embeddings, such as word2vec or glove, generate word representations in a multidimensional Euclidean space.  These have proven to be extremely useful for so called downstream tasks due to their ability to capture semantic and syntactic relations among words when trained on large text corpora.   The main idea behind these works is that 


There are different realizations of hyperbolic space.   The authors of [3-4] stress optimization problems can be formulated more efficiently in the hyperboloid model.  The n-dimensional hyperbolic model is defined by the points lying on the forward sheet (with the zero coordinate positive) of an hyperboloid in (n+1)-dimensional Minkowski space.   A nice connection with the special theory of relativity can be drawn as the relativistic momentum of a (unit mass) massive particle defines a 3-dimensional hyperbolic model

<img src="https://latex.codecogs.com/svg.latex?\Large&space;E^2-|\vec~p|^2c^2=m^2c^4" title="\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" />




Implementations of the model presented in [1] can be found in [gensim](https://radimrehurek.com/gensim/models/poincare.html)
and [facebook research](https://github.com/facebookresearch/poincare-embeddings). Implementation of the code used in [3] can be found in [minkowski](https://github.com/lateral/minkowski)






**References:**

[1] *"Poincaré Embeddings for Learning Hierarchical Representations"* from Maximilian Nickel and Douwe Kiela [arxiv:1705.08039](https://arxiv.org/abs/1705.08039).  

[2] *"Embedding Text in Hyperbolic Spaces"* from Bhuwan Dhingra, Christopher J. Shallue, Mohammad Norouzi, Andrew M. Dai and George E. Dahl [arxiv:1806.04313](https://arxiv.org/abs/1806.04313)

[3] *"Learning Continuous Hierarchies in the Lorentz Model of Hyperbolic Geometry"* from Maximilian Nickel and Douwe Kiela [arxiv:1806.03417](https://arxiv.org/abs/1806.03417)

[4] *"Skip-gram word embeddings in hyperbolic space"* from Matthias Leimeister and Benjamin J. Wilson [arxiv:1809.01498](https://arxiv.org/abs/1809.01498)

[5] *"Poincaré GloVe: Hyperbolic Word Embeddings"* from Alexandru Tifrea, Gary Bécigneul and Octavian-Eugen Ganea [arxiv:1810.06546](https://arxiv.org/abs/1810.06546)

[6] *"Inferring Concept Hierarchies from Text Corpora via Hyperbolic Embeddings"* from Matt Le, Stephen Roller, Laetitia Papaxanthos, Douwe Kiela and Maximilian Nickel [arxiv:1902.00913](https://arxiv.org/abs/1902.00913)
