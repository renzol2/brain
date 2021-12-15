---
tags: mus-305 mus-407 filter
---

# Comb Filter

**Comb filters** are audio signal filters that filter out [[noise]] into discrete [[docs/frequency|frequencies]] and impose [[resonance]].

## Implementation

Comb filters are just **[[digital-delay-line|delay lines]] with [[feedback]]**

- feeding signal into itself with an extremely _short delay time_, to the point of hearing a periodic waveform
- any partial with aligns with the inverse of the delay time (and all the harmonics of that partial) will experience 100% [[wave-interference|constructive interference]]
  - creates peaks in the spectrum
- conversely, any harmonic that has 1.5/2.5/3.5/etc. times the frequency of the original partial will experience 100% [[wave-interference|destructive interference]]
