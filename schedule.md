---
layout: post
title: Schedule
permalink: /schedule/
---

We will split our tutorial into three key parts, with one hour allocated for each speaker, as follows.

### Part I: **Developing** NAR (_Petar Veličković_)

The first part of the tutorial will introduce neural algorithmic reasoning, through the lens of learning to execute classical algorithms. We will clarify why this is a worthwhile pursuit, and how---due to the requirement of generalising _out-of-distribution_---it is challenging enough to warrant its own subfield.

Once the above is ascertained, we will use a series of example tasks, progressively increasing in difficulty, to motivate several (G)NN architectures through the lens of algorithmic alignment. 

Given the tutorial nature of this talk, emphasis will be placed on _key practical takeaways_ from prior work rather than deeply explaining any particular prior paper, however detailed lists of references will be provided whenever necessary, to supplement future study.

Lastly, we will present a **hands-on coding example** to help attendees make immediate interactions with the area. We will show how to train a GNN-based algorithmic reasoner on a standard task from the CLRS-30 benchmark, such as executing the Bellman-Ford algorithm.

### Part II: **Deploying** NAR (_Andreea Deac_)

The second part of the tutorial will discuss how, once a neural algorithmic reasoner is trained, it can be leveraged in a downstream application.

We will focus on the domain of deep reinforcement learning (DRL), for two reasons: first, it is a well-known, high-impact area of deep learning; secondly, indeed, many classical algorithms exist that _provably_ and _perfectly_ solve the RL task, given access to substantial privileged information.

Accordingly, we will show how to incorporate these classical algorithms into a GNN, and then use them to improve data efficiency of DRL agents---since they do not need to relearn such algorithmic principles from sparse rewards. This will lead us to a rederivation of the XLVIN agent.

Besides XLVIN, this tutorial will also cover, as additional examples, the deployment of NAR in self-supervised learning (leading to the RMR model), along with downstream applications to blood vessel segmentation, extensions of XLVIN to continuous action spaces, and more. 

This part will also feature a **hands-on coding example**. The attendees will be able to take the pre-trained CLRS-30 model from the previous part, and deploy it inside a DRL agent that needs to solve path-finding problems (amenable to Bellman-Ford) from noisy observations.

### Part III: **Deepening** NAR (_Andrew Dudzik_)

The third and final part of the tutorial will present the current bleeding edge of understanding algorithmic alignment, through the lens of category theory and abstract algebra.

First, we give an overview of the definition of algorithmic alignment due to Xu et al.  We explain how this definition points to the need for a rigorous and practical definition of the program structures that arise in dynamic programming.

Once we cover the above, we will attempt to distill the essence of the dataflow of both (G)NNs, and the algorithms they are supposed to model. This will lead us to the discovery of polynomial spans, which we will motivate through several guiding examples: representation learning over circles and lines, and the message passing primitive in a GNN. 

We will ground the utility of polynomial spans through a few example derivations, showing how it can be used to re-derive the Bellman-Ford algorithm as well as the equations of a (non-parametric) GNN.

Lastly, using the polynomial span in the category of sets, we can derive a _type checker_ for GNNs, using which we can immediately explain some of the prior publications in the area, as well as propose potent improvements (such as triplet reasoning).
