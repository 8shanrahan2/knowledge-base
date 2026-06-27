---
type: "Concept"
sources: ["summaries/Serum-2-User-Guide.md"]
description: "Serum 2 modulation uses envelopes, LFOs, macros, velocity, note tracking, oscillator/filter sources, and a modulation matrix to animate parameters."
---

# Modulation System

Serum 2's modulation system is the glue between sound sources and musical expression. A static patch becomes a playable instrument when envelopes, LFOs, macros, velocity curves, note tracking, and matrix assignments change parameters over time.

## Main modulation sources

### Envelopes

Envelopes are best for one-shot shapes: attacks, decays, plucks, swells, gated movement, and note-triggered contours. ENV 1 is typically associated with amplitude behavior, while additional envelopes can shape filter cutoff, wavetable position, warp, FX mix, or other parameters.

### LFOs

LFOs are best for repeated or drawn movement. The manual covers configuring LFOs, drawing LFO graphs, modifying LFOs, assigning LFOs to controls, copying wavetable shapes to LFOs, copying LFO shapes to wavetables, and modulating LFO points.

Use LFOs for:

- Rhythmic filter movement.
- Wavetable position scanning.
- Tremolo or pan movement.
- Repeating bass/growl patterns.
- Subtle randomization or humanization.

### Macros

Macros expose important patch controls as performance knobs. One macro can control many destinations. This is useful for turning a patch into an instrument: brightness, intensity, width, movement, grit, space, or growl can each become one knob.

### Velocity and note tracking

Velocity and note settings let MIDI input influence sound. Velocity can make harder notes brighter, louder, more distorted, or more open. Note tracking can make higher notes less bass-heavy, brighter, narrower, or differently filtered.

### Oscillators and filters as modulation sources

The manual also covers using oscillators and filters as modulation sources. This is where audio-rate or quasi-audio-rate relationships become possible, including FM/PM/AM/RM-like behaviors depending on destination.

## Modulation assignment workflow

1. Choose the source: envelope, LFO, macro, velocity, note, or another source.
2. Assign it to a target control.
3. Set depth. Positive and negative depths produce opposite movement.
4. Inspect or refine the assignment in the modulation matrix.
5. Add auxiliary shaping if needed.
6. Rename macros and save the preset.

## Modulation depth

Depth is not an afterthought. Most bad Serum patches are over-modulated. A small amount of movement can make a sound alive; too much movement makes it hard to mix or play.

Good defaults:

- Small LFO depth for pads and atmosphere.
- Medium envelope depth for plucks and bass movement.
- Macro depth wide enough to be useful but not destructive.
- Negative depth when you want a parameter to close or reduce while another opens.

## Modulation Matrix

The modulation matrix is the audit table for the patch. Use it when a patch is confusing, overactive, or hard to debug.

Matrix tasks:

- See all source/destination assignments.
- Move modulations.
- Bypass a modulation.
- Remove a modulation.
- Refine depth and behavior.
- Understand why a knob moves when you did not expect it to.

## Related pages

- [[concepts/wavetable-synthesis]] — common destination: wavetable position and warp.
- [[concepts/filters-routing-and-mixer]] — common destination: cutoff, resonance, mix, drive, pan, and levels.
- [[concepts/fx-modules]] — FX parameters can also be modulated.
- [[concepts/clips-and-arpeggiator]] — note material can drive the modulation system indirectly.
