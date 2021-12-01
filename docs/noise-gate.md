---
tags: music mus-407 noise-gate noise gate production compression dynamics drp dynamic-range-processing
---

# Noise Gate

A **noise gate** (or simply **gate**) is a switch that opens/closes depending on whether signal level is above/below an [[amplitude]] threshold

- when signal $>$ threshold, the gate is "open" and allows signal to pass through
- when signal level $\leq$ threshold, the gate is "closed" silencing the signal

Gates are commonly used for removing low-level background noise.

- assumed that noise level is below signal level
- for basic gates, not possible to remove noise while signal is present
- works best when signal masks noise
- works better on short [[transient]]s (percussion, drums, staccato) than sustained or long-decay sounds (held notes)

Basic noise gates only check amplitude; however, more advanced noise gates have additional features for more flexibility/utility:

- use spectral analysis or frequency tracking to remove noise from _all_ parts of the signal, not just through amplitude thresholds
- allow for specific amount of [[decibel]] reduction, rather than just muting the signal
- allow for an [[envelope]] for the gate: specific attack/release times on signal

## Workflow

- Determine approximate threshold
  - ex. loop through part of sample with noise and check what the general threshold is
- Play sample and adjust threshold so that noise is removed as much as possible