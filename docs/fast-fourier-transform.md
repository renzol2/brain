---
tags: ece-402 dsp
---

# Fast Fourier Transform

A **fast Fourier transform (FFT)** is an [[algorithm]] that computes the [[discrete-fourier-transform|discrete Fourier transform]] of a sequence, as well as its [[fourier-inversion-theorem|inverse]] (IDFT).

- rapidly computes transformations by factorizing the DFT matrix into a product of mostly zero factors
- reduces [[runtime]] complexity from $O(n^2)$ to $O(n\text{log}n)$

## Applications

FFTs are important in many applications since it makes working in the [[frequency-domain|frequency domain]] as easy as working in the [[time-domain|time domain]]. This has numerous applications in mathematics, science, music and other fields.

For music:

- digital recording and [[sampling-signal-processing|sampling]]
- [[additive-synthesis|additive synthesis]]
- [[spectral-analysis|spectral analysis]]
- pitch correction software

## Sources

- <https://en.wikipedia.org/wiki/Fast_Fourier_transform>
- <https://download.ni.com/evaluation/pxi/Understanding%20FFTs%20and%20Windowing.pdf>
