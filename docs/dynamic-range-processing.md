---
tags: music mus-407 electroacoustic dynamic-range dynamics
---

# Dynamic Range Processing

**Dynamic Range**: Difference between highest/lowest level (dB) of an audio signal

- difference between _loudest_ and _quietest_ part of a signal
- a big part of orchestral music is _large dynamic range_: the drama between the quietest parts of the piece and the loudest parts
- meanwhile, pop music generally has a small dynamic range to be loud across the whole song: for uniformity of energy, to be heard over background noise, etc.

A _dynamic range process_ (DRP) changes a signal's dynamic range by altering its amplitude.

- measuring signal amplitude
- adjusts signal amplitude based on measured value

Measured & processed signals can be the same or different (i.e. there can be distinct _source_ & _target_ signals. see: [[side-chaining]])

Applications include:

- maintaining a constant signal level
- increasing the overall level of a mix
- creative transient shaping
- noise reduction
- preventing clipping/overloading
- [[side-chaining]] (amplitude following, ducking)

## Key Concepts

All forms of DRP rely on an amplitude **threshold**.

- determines signal level above or below which DRP take effect, depending on the type of effect

DRPs utilize a **detection circuit**or **detection algorithm** for tracking signal amplitude, which can track either _peak_ or _average_ signal level

**Peak**: instantaneous measurement, captures true waveform peaks: "no sample left unchecked"

**Average**: signal values averaged over a time interval, also called _RMS_ (root-mean-squared) tracking

- sculpting the dynamic range of the sound without closely monitoring every single peak

Peak tracking is more applicable for preventing overloading/clipping.

RMS tracking provides a smoother response to a changing input signal.

### Why RMS?

What happens if we average sinusoidal values over a period of time?

- Positive and negative values will cancel, resulting in a zero average

RMS means we take the square _root_ of the _mean_ of a sequence of _squared_ sample values:

$x_{RMS}=\sqrt{\frac{x^2_1+x^2_2+x^2_3+...+x^2_n}{n}}$

This always produces non-negative values, provides more meaningful measurement, and more accurately reflects continuous signal power.

### RMS Tracking

![RMS Tracking](../attachments/rms-tracking.png)

General steps:

- Start with original signal
- Take the square of each value
- Over some time interval, find the average level across that interval
- Take the square root of those means (to reproduce a similar level to original signal)

### Peak Tracking

![Sine Wave RMS Tracking](../attachments/sine-wave-rms-tracking.png)

## Types

- Noise gate ([[noise-gate]])
- Compressor ([[compression]])
- [[Limiter]]
- [[Expander]]
- Envelope shaper ([[envelope-shaper]])

## More Terms & Techniques

### DRP Considerations

DRPs, particularly compressors ([[compression]]) and [[limiter]]s, can smear/distort transients

- like all effects, easy to overuse, generally should be applied in moderation
- can be used in extremes for creative effect

DRPs may involve a "look ahead" time to properly anticipate signal levels

- introduces a small delay into processed audio
- can create synchronization issues, but usually automatically or easily managed in DAW context

DRPs generally have more applications in recording/live sound.

In electroacoustic composition, traditional application of DRP less useful

- composer has complete control over levels during compositional process
- can usually go back and adjust levels as necessary

### Knee

When signal level crosses a threshold, DRP ratio may be applied fully or gradually, depending on _knee curve_

_Hard/soft_ knee refers to the smoothness of the transfer function graph across the threshold

- a hard knee has two straight lines, above and below threshold
- a soft knee curves gently between affected and unaffected amplitude regions
- differences between hard/soft knee tend to be very subtle

### Attack, Hold, Release

Many DRPs include envelope parameters: often _attack/release_, sometimes _hold_

**Attack** determines the amount of time for DRP effect to fully activate. The attack transient begins when signal crosses the threshold.

**Release** determines amount of time for DRP effect to deactivate completely. Release transient begins when level no longer crosses threshold.

**Hold** will force DRP effect to remain active for a time, regardless of threshold.

- can be exploited for creative transient shaping (used explicitly in envelope shapers)
- useful in noise gates to prevent intermittent signal near threshold

### Upward/Downward Compression & Expansion

Typical cases:

- compressors attenuate above a threshold ([[compression]])
- [[expander]]s attenuate below a threshold
- both referred to as _"downward"_ compression/expansion

However, it is sometimes possible to set a threshold and amplify signal below it, considered a form of compression.

Likewise, it is possible to boost signal above a threshold - a form of expansion.

This technique is infrequently used:

- upward compression raises the noise floor
- upward expansion makes peaks even louder

### Side-Chaining

See: [[side-chaining]]

## Transfer Function Examples

TODO: add transfer function examples