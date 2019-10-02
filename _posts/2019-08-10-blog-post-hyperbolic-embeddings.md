---
title: 'Text embeddings in hyperbolic space'
date: 2019-08-10
permalink: /posts/2019/08/blog-post-hyperbolic-embeddings/
tags:
  - representation learning
---

Here I review the idea of representation learning in hyperbolic space following [1-6].  I will focus on the application of these methods towards the generation of word embeddings from natural language in an unsupervised manner.   The standard algorithms for generating word embeddings, such as word2vec or GloVe, generate word representations in a multidimensional Euclidean space.  These have proven to be extremely useful for so called downstream tasks (such as text classification, word similarity and name entity recognition) due to their ability to capture semantic and syntactic relations among words when trained on large text corpora.   


Representation learning in hyperbolic space was studied initially in the context of graphs (see [1] and references therein), finding interesting results. Its extension to derive word embeddings from large corpora in an unsupervised manner is a natural follow-up.  The main motivation for building word embeddings in hyperbolic space is that these embeddings might be able to capture better hierarchical relations present in language, such as hypernym-hyponym relationships, and therefore have the potential to perform better than traditional embeddings on certain tasks.  


There are different realizations of hyperbolic space.   The authors of [3-4] stress that optimization problems can be formulated more efficiently in the hyperboloid model.  It therefore seems conventient to use the hyperboloid model as our realization of the hyperbolic space.  The n-dimensional hyperbolic model is defined by the points lying on the forward sheet (with the zero coordinate positive) of an hyperboloid in (n+1)-dimensional Minkowski space.  


Some works, including [1] have used the Poincaré ball representation of hyperbolic space. At the end, one can map points in a hyperboloid model to a corresponding Poincaré ball representation, so choosing one or the other is matter of convenience.



Implementations of the model presented in [1] can be found in [gensim](https://radimrehurek.com/gensim/models/poincare.html)
and [facebook research](https://github.com/facebookresearch/poincare-embeddings). Implementation of the code used in [3] can be found in [minkowski](https://github.com/lateral/minkowski)



<a href="https://www.codecogs.com/eqnedit.php?latex=x_0^2&space;-&space;x_i&space;x^{i}&space;=&space;-1" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x_0^2&space;-


**References:**

[1] *"Poincaré Embeddings for Learning Hierarchical Representations"* from Maximilian Nickel and Douwe Kiela [arxiv:1705.08039](https://arxiv.org/abs/1705.08039).  

[2] *"Embedding Text in Hyperbolic Spaces"* from Bhuwan Dhingra, Christopher J. Shallue, Mohammad Norouzi, Andrew M. Dai and George E. Dahl [arxiv:1806.04313](https://arxiv.org/abs/1806.04313)

[3] *"Learning Continuous Hierarchies in the Lorentz Model of Hyperbolic Geometry"* from Maximilian Nickel and Douwe Kiela [arxiv:1806.03417](https://arxiv.org/abs/1806.03417)

[4] *"Skip-gram word embeddings in hyperbolic space"* from Matthias Leimeister and Benjamin J. Wilson [arxiv:1809.01498](https://arxiv.org/abs/1809.01498)

[5] *"Poincaré GloVe: Hyperbolic Word Embeddings"* from Alexandru Tifrea, Gary Bécigneul and Octavian-Eugen Ganea [arxiv:1810.06546](https://arxiv.org/abs/1810.06546)

[6] *"Inferring Concept Hierarchies from Text Corpora via Hyperbolic Embeddings"* from Matt Le, Stephen Roller, Laetitia Papaxanthos, Douwe Kiela and Maximilian Nickel [arxiv:1902.00913](https://arxiv.org/abs/1902.00913)
