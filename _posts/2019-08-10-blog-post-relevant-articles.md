---
title: 'Relevant articles'
date: 2019-11-18
permalink: /posts/2019/08/blog-post-relvant-articles/
tags:
  - representation learning
---

Recently, me and [Jose Eliel Camargo](https://github.com/JoseEliel) have been exploring a very nice and simple idea.    When writing scientific articles, researchers put a lot of effort collecting relevant references and placing them within their text for different puposes: to give credit, to guide the reader to other points of view, to support some statemtents, etc.  This means that looking for papers which tend to be cited close to each other in a collection of scientific articles should provide a good way to extract a group of similar or relevant articles.  


With this in mind, we have extracted reference lists from [inspirehep](https://labs.inspirehep.net) using the
[inspirehep python wrapper](https://github.com/celis/inspirehep_api_wrapper).   With this large amount of data, we trained a Skip-Gram model using the [gensim](https://radimrehurek.com/gensim/) library.  We end up with a dense representation in the space of inspirehep article ids, from where we can extract similar items using cosine similarity.   











