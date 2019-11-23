---
title: "Cartograph: Unlocking Thematic Cartography Through Semantic Enhancement"
collection: research
type: "Research"
permalink: /research/cartograph
venue: "by National Science Foundation, June 2019 - Present"
location: "Saint Paul, Minnesota"
---

[*Cartograph*](https://cartograph.info) is a visualization system that harnesses the vast amount of world knowledge encoded within Wikipedia to create thematic maps of almost any data. Previous version of *Cartograph* takes a long time for the user to upload their own data and to generate their own map. In the summer of 2019, I helped Prof. Shilad Sen explore new algorithms and upgrade the system.

This research project involves three parts: embedding, clustering, and labeling. We used Latent Semantic Analysis (LSA) to represent Wikipedia articles in vector forms. We captured relationship on latent space, the reduced-dimensionality vector space embeddings, using Uniform Manifold Approximation and Projection (UMAP) over the original t-Distributed Stochastic Neighbor Embedding (t-SNE). The UMAP algorithms preserves global data structure, scales well for large sample sizes, and does not consume a lot of memory compared to t-SNE.

In the previous system, the three algorithms are separate. Here we created a joint loss function to cluster the data so the result is much more homogenous. The functions considers the high-dimensional similarity, low-dimensional (2-D latent space) similarity, and the label space similarity (co-occurrence matrix, you can think of rows are articles, columns are words in the entire corpus. The matrix are filled with 0 or 1).

After embedding and clustering, we labeled the cluster using the network on Wikipedia articles. We collected the categories and links, extracted key phrases using gensim and nltk. We collected over 1700 test results from a user test via Amazon Mechanical Turks to generate the best label that makes sense to humans.

We are finalizing the research process and drafting a paper. Stay tuned!
