---
tags: music mus-407 signal-processing sampling
---

# Nyquist Frequency

The sampling theorem's primary consequence of digital audio:

- the highest frequency that can be represented in a digital system is equal to half the sampling rate
- this frequency is called the **Nyquist Frequency**:

$N = \frac{SR}{2}$

If a frequency $> N$ is sampled, the frequency of its digital representation will appear between 0 and $N$ Hz. This phenomenon is called [[aliasing]] or **foldover**.
