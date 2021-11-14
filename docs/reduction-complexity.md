---
tags: cs-374 computer-science computer science p-vs-np algorithms reduction
---

# Reduction (complexity)

Given two problems A and B (ex. [[decision-problems]]), **reduction** is describing an algorithm to solve problem A under the assumption that an algorithm for problem B already exists.

- Intuitively, if you know some algorithm to solve problem B, and you can convert problem A to problem B, then you can solve problem A using the same algorithm.

This reduction process is often used to prove problems are NP-hard (see: [[p-vs-np]]).

> To prove that problem _A_ is NP-hard, reduce a known NP-hard problem to _A_.
