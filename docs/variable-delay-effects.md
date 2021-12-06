---
tags: mus-407 delay delay-line
---

# Variable Delay Effects

**Variable delay effects** are [[digital-delay-line|digital delay effects]] in which delay time changes dynamically.

Imagine a tape loop as an analogy to a [[circular-queue|circular queue]]:

- read/write pointers as play/record heads
- instead of pointers advancing, tape moves underneath heads

Essential behavior of variable delay:

- delay time (distance) between read pointer and write pointer varies
- as delay time _increases_, read pointer _lags behind_ write pointer, reading through samples more _slowly_, causing a _downward_ pitch shift
- as delay time _decreases_, read pointer _catches up_ to write pointer, reading through samples more _quickly_, causing an _upward_ pitch shift
- delay time usually driven by oscillator or noise generator
