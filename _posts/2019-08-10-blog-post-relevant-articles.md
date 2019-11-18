---
title: 'Relevant articles'
date: 2019-11-18
permalink: /posts/2019/08/blog-post-relvant-articles/
tags:
  - representation learning
---

Recently, together with [Jose Eliel Camargo](https://github.com/JoseEliel) I have been exploring a very nice and simple idea.    When writing scientific articles, researchers put a lot of effort collecting relevant references and placing them within their text for different puposes: to give credit, to guide the reader to other points of view, to support some statement, etc.  This means that looking for papers which tend to be cited close to each other in a collection of scientific articles should provide a good way to extract a group of similar or relevant articles.  


With this in mind, we have extracted reference lists from [inspirehep](https://labs.inspirehep.net) using the
[inspirehep python wrapper](https://github.com/celis/inspirehep_api_wrapper).  Each reference list for us is just a list of inspire article ids.   We then trained a Skip-Gram model using the [gensim](https://radimrehurek.com/gensim/) library implementation.   We end up with a dense representation in the space of inspirehep article ids, from where we can extract similar items using cosine similarity.   Very simple!  

Lets look at some of the results, I will start with one of my favourites:

I retrieve the three closest articles by cosine similarity to the following classic article:
* [Regularization and Renormalization of Gauge Fields](https://labs.inspirehep.net/literature/74886)
  Gerard 't Hooft, M.J.G. Veltman
    
I get the following results:

* [A Method of Gauge Invariant Regularization](https://labs.inspirehep.net/literature/74882)
J.F. Ashmore

* [Dimensional Renormalization: The Number of Dimensions as a Regularizing Parameter](https://labs.inspirehep.net/literature/74881)
C.G. Bollini, J.J. Giambiagi

* [Lowest order divergent graphs in nu-dimensional space](https://labs.inspirehep.net/literature/74400)
C.G. Bollini, J.J. Giambiagi

These results are very good, as these articles developed simultaneously with the article by Gerard 't Hooft and M.J.G. Veltman the concept of dimensional regularization.

Lets look at another articles, starting with

* [Broken Symmetries and the Masses of Gauge Bosons](https://labs.inspirehep.net/literature/11883)
Peter W. Higgs

we predict the following three similar articles

* [Broken symmetries, massless particles and gauge fields](https://labs.inspirehep.net/literature/40440)
Peter W. Higgs

* [Spontaneous Symmetry Breakdown without Massless Bosons](https://labs.inspirehep.net/literature/50073)
Peter W. Higgs

* [Broken Symmetry and the Mass of Gauge Vector Mesons](https://labs.inspirehep.net/literature/12291)
F. Englert, R. Brout















