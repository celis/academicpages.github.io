---
title: 'Text embeddings in hyperbolic space'
date: 2019-08-10
permalink: /posts/2019/08/blog-post-hyperbolic-embeddings/
tags:
  - representation learning
---

Here I review the idea of embedding text in hyperbolic space.  I follow the following articles:

[1] *"Poincaré Embeddings for Learning Hierarchical Representations"* from Maximilian Nickel and Douwe Kiela [arxiv:1705.08039](https://arxiv.org/abs/1705.08039).  

[2] *"Embedding Text in Hyperbolic Spaces"* from Bhuwan Dhingra, Christopher J. Shallue, Mohammad Norouzi, Andrew M. Dai and George E. Dahl [arxiv:1806.04313](https://arxiv.org/abs/1806.04313)

[3] *"Learning Continuous Hierarchies
in the Lorentz Model of Hyperbolic Geometry" from Maximilian Nickel and
Douwe Kiela [arxiv:1806.03417](https://arxiv.org/abs/1806.03417)

[4] *"Skip-gram word embeddings in hyperbolic space"* from Matthias Leimeister and Benjamin J. Wilson [arxiv:1809.01498](https://arxiv.org/abs/1809.01498)

[5] *"Poincaré GloVe: Hyperbolic Word Embeddings"* from Alexandru Tifrea, Gary Bécigneul and Octavian-Eugen Ganea [arxiv:1810.06546](https://arxiv.org/abs/1810.06546)


[6] *"Inferring Concept Hierarchies from Text Corpora via Hyperbolic Embeddings"* from Matt Le, Stephen Roller, Laetitia Papaxanthos, Douwe Kiela and Maximilian Nickel [arxiv:1902.00913](https://arxiv.org/abs/1902.00913)


I will focus on the application of these methods towards the generation of word embeddings in an unsupervised manner.   The standard algorithms for generating word embeddings, such as word2vec or glove, generate word representations in a multidimensional Euclidean space.  These have proven to be extremely useful for so called downstream tasks due to their ability to capture semantic and syntactic relations among words when trained on large text corpora.   The main idea behind these works is that 


There are different realizations of hyperbolic space. I find it convenient to use the the hyperboloid model of hyperbolic space (see for instance [2-3]) as it is connected to Minkowski space and I can rely on some intuition from the theory of special relativity.   However most of the works above have used the Poincaré ball model of hyperbolic space, likely because of some inertia from the work in [1].  The authors of [2-3] stress that optimization can be formulated more efficiently in the hyperboloid model. 


Implementations of the model presented in [1] can be found in [gensim](https://radimrehurek.com/gensim/models/poincare.html)
and [facebook research](https://github.com/facebookresearch/poincare-embeddings). Implementation of the code used in [3] can be found in [minkowski](https://github.com/lateral/minkowski)






