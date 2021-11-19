---
tags: music compression mus-407 production dynamics drp dynamic-range-compression
---

# Compression

A **compressor** is an amplifier whose gain is determined by an input signal level

- when signal level > threshold, compression effect becomes active and attenuates a signal

Frequently used to regulate a "peaky" signal during recording ,to provide a more constant and predictable level

- e.g. rock drum set, swaying vocalist
- essentially, automates mixer input faders to avoid manual adjustment

Compression is also used during mixing/mastering to provide a higher overall mix level.

Compressor behavior is modeled using a graph of its **transfer function**.

## Transfer Function

- Standard amplifier: no compression, linear response
- Mild compression, peaks above -6 dBFS are slightly attenuated
- More severe compression, peaks above -6 dBFS are more strongly attenuated

Most DRP transfer functions only display **one quadrant** to avoid redundancy.

Typically, 0 dB input/output in upper right, axes labeled linearly with respect to dB.

## Ratio

The severity of signal attenuation is determined by a _compression ratio_.

- Represents change in input signal (dB) compared to change in output signal (dB)

e.g. compression ratio of 4:1

- above threshold, if input signal increases by 4 dB, output signal is attenuated so that the increase is only 1 dB

Ratios of 8:1 and above are generally considered "extreme" compression

- Can result in a perceptual distortion of transients, noticeable changes in timbre, often described as a "squashed" sound

## Makeup gain

After compression is applied, **makeup gain** is a normal amplification process used to compensate for the loss in overall level

- typically used to restore peaks to their original level
- content below threshold undergoes a net level increases

## Multiband compression

A **multi-band compressor** divides a full spectrum signal into discrete frequency bands and applies compression uniquely to each band.

- allows for more detailed control of dynamic range
- compressed spectral bands are summed after compressions are applied
- often used to affect different parts of a drum set, e.g. compress only the [[kick]] drum if the whole drum set is recorded on a single track