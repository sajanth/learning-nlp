# A Hands-On Introduction to Language Modeling

In this repository we are going to dive into the basics of language modeling! If you are looking for the latest and greatest in AI, you have to look somewhere else though - here we will focus on fundamental concepts of statistical modeling and try to derive as much as possible from first principles :) In return, it should be easy to follow even without any background in neural networks!

Our goal will be to build a model that generates fake street names for Zurich. We'll do this by looking at a list containing all the real street names of Zurich and trying to model the probability that two letters appear next to each other. This way, we can generate new street names by randomly selecting letters according to their probability of appearing together.

In fact, we will actually build two models using two different approaches. In the first model, we'll simply count the number of times each pair of letters appears in the data set. In the second model, we'll use matrix multiplication and optimization methods - essentially a simple neural network. Even though we will use two totally different starting points, we will see that we will arrive at the same model!

Note: The general idea and flow of this notebook is heavily adapted from Karpathy's excellent [lecture series](https://www.youtube.com/watch?v=PaCmpygFfXo&list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ&index=2) on language modeling. 

Let's get started!

## Overview
* [Part 1: Exact modeling - Count, count, count!](./notebooks/part1.ipynb)
* [Interlude: What is a model anyway?](./notebooks/interlude.ipynb)
* [Part 2: Approximate modeling - Differentiate, differentiate, differentiate!](./notebooks/part2.ipynb)

### Supplementary material
* [Generalization to n-grams](./notebooks/ngrams.ipynb)

### References
* [Karpathy's lectures on NLP](https://www.youtube.com/watch?v=PaCmpygFfXo&list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ&index=2)
* [A Neural Probabilistic Language Model, Bengio et al. (2003)](https://www.jmlr.org/papers/volume3/bengio03a/bengio03a.pdf)
* https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/