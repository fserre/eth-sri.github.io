---
ref: he20lait
title: "Learning Fast and Precise Numerical Analysis"
authors: Jingxuan He, Gagandeep Singh, Markus Püschel, Martin Vechev
year: 2020
month: 06
venue: PLDI
projects: numerical-analysis, plml
awards:
bibtex:
paper: https://files.sri.inf.ethz.ch/website/papers/pldi20-lait.pdf
talk: https://www.youtube.com/watch?v=ObkjUoA7yho
slides: https://files.sri.inf.ethz.ch/website/slides/pldi2020-lait-slides.pdf
---

Numerical abstract domains are a key component of modern static analyzers. Despite recent advances, precise analysis with highly expressive domains remains too costly for many real-world programs. To address this challenge, we introduce a new data-driven method, called LAIT, that produces a faster and more scalable numerical analysis without significant loss of precision. Our approach is based on the key insight that sequences of abstract elements produced by the analyzer contain redundancy which can be exploited to increase performance without compromising precision significantly. Concretely, we present an iterative learning algorithm that learns a neural policy that identifies and removes redundant constraints at various points in the sequence. We believe that our method is generic and can be applied to various numerical domains.

We instantiate LAIT for the widely used Polyhedra and Octagon domains. Our evaluation of LAIT on a range of real-world applications with both domains shows that while the approach is designed to be generic, it is orders of magnitude faster on the most costly benchmarks than a state-of-the-art numerical library while maintaining close-to-original analysis precision. Further, LAIT outperforms hand-crafted heuristics and a domain-specific learning approach in terms of both precision and speed.that even though the approach is generic, it is orders of magnitudes faster than the state-of-the-art numerical library, while maintaining 98% precision w.r.t to the original analysis.
