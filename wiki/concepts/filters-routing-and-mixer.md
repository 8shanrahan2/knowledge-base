---
type: "Concept"
sources: ["summaries/Serum-2-User-Guide.md"]
description: "Serum 2 routing combines oscillator/filter routing, filter types, filter controls, mixer busses, and main/direct output levels."
---

# Filters, Routing, and Mixer

Serum 2's routing system determines where each sound source goes before it reaches the final output. This includes oscillator routing, filter modules, filter mixing, busses, direct output, main output, pan, level, and send-style decisions.

## Why routing matters

A Serum patch is not only defined by oscillator choice. The same wavetable can sound clean, dark, aggressive, wide, mono, filtered, distorted, or layered depending on routing.

Routing answers these questions:

- Does this source pass through a filter?
- Which filter receives which oscillator?
- Does a source bypass the main filter path?
- Is the source sent to a bus or directly to output?
- Are filters mixed in serial-like or parallel-like ways?
- Which layers should be mono, stereo, quiet, loud, clean, or processed?

## Filter modules

The manual covers enabling filter modules, choosing filter options, routing oscillators or filters, selecting filter types, display options, and setting key parameters.

Common filter parameters:

- **Cutoff** — frequency point or main control for the filter response.
- **Resonance** — emphasis around cutoff.
- **Drive** — input or filter saturation/intensity.
- **Fat / variant controls** — mode-specific behavior.
- **Pan** — stereo placement.
- **Mix** — dry/wet blend.
- **Level** — output amount.

## Mixer and busses

The mixer section covers sending to busses, pan/level controls, mixing filters, routing to busses, bus levels, and main/direct levels.

Useful pattern:

1. Keep sub oscillator clean and centered.
2. Send the main wavetable oscillator through filter and FX.
3. Use noise subtly for transient or air.
4. Use busses to separate clean low-end from processed high-end.
5. Use main/direct levels to avoid unintended loudness jumps.

## Patch architecture examples

### Clean bass routing

- Sub oscillator: direct, mono, stable.
- Oscillator A: filtered and possibly distorted.
- Noise: low level, transient only.
- FX: avoid widening the sub region.

### Wide pad routing

- Oscillator A/B: unison and stereo width.
- Filters: lower cutoff with slow modulation.
- Busses: route layered material into shared reverb/chorus.
- Main output: leave headroom.

### Aggressive lead routing

- Oscillator A: warp and filter drive.
- Oscillator B or noise: layer for edge.
- Filters: resonant movement.
- FX: distortion, compression, EQ, and width.

## Related pages

- [[concepts/wavetable-synthesis]]
- [[concepts/sample-granular-spectral-engines]]
- [[concepts/modulation-system]]
- [[concepts/fx-modules]]
