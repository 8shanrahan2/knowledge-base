---
type: "Concept"
sources: ["summaries/Serum-2-User-Guide.md"]
description: "Wavetable synthesis in Serum 2 centers on scanning, shaping, unison-stacking, warping, and modulating oscillator frames."
---

# Wavetable Synthesis

Wavetable synthesis is one of the primary sound-generation systems in [[entities/serum-2]]. In Serum 2, a wavetable oscillator is not just a static waveform player. It is a morphable source whose timbre can change through wavetable position, phase behavior, unison, warp modes, stereo spread, level, and modulation.

## Core controls

### Wavetable position

The wavetable position control selects where the oscillator reads within the wavetable. A static position gives a fixed timbre. Modulating position with an envelope, LFO, macro, velocity, or note tracking creates movement.

Use cases:

- Slow LFO movement for evolving pads.
- Envelope movement for plucks, growls, and transient sweeps.
- Macro assignment for performance control.
- Velocity assignment for harder playing producing brighter or more complex timbres.

### Phase

Phase controls where playback begins within the waveform cycle. This matters most for basses, plucks, kicks, and other sounds where transient consistency matters.

Related controls include randomizing phase and phase memory. Lower randomness generally produces more repeatable attacks; higher randomness can reduce sterile repetition and add width or variation.

### Unison

Unison stacks multiple oscillator voices. Detune, width, range, blend, start/span behavior, and stack-style choices determine whether the result feels like a subtle thickener, supersaw, chord stack, noisy spread, or wide stereo layer.

Tradeoff: more unison voices generally means more CPU use. Use unison intentionally instead of reflexively maxing it out.

### Warp

Warp changes the waveform shape before it reaches the rest of the synth path. Warp can be used for sync-like tones, bending, folding, distortion-like harmonics, FM/PM/AM/RM-style movement, and other nonlinear timbral effects.

A useful patch habit is to set the core wavetable first, then add warp, then decide whether the warp depth should be static or modulated.

### Pan and level

Pan and level are basic mix controls, but they matter in layered patches. A wide wavetable oscillator can fight with a mono sub oscillator. A quiet oscillator sent into a driven filter or distortion may behave very differently from a loud one.

## Common workflows

### Evolving wavetable pad

1. Select a wavetable with meaningful frame variation.
2. Set unison to add width.
3. Use a slow LFO to move wavetable position.
4. Add a filter and modulate cutoff subtly.
5. Add reverb/chorus in the [[concepts/fx-modules]] page workflow.

### Consistent bass transient

1. Use a simple wavetable or a harmonically stable frame.
2. Reduce random phase.
3. Keep phase behavior consistent.
4. Add sub oscillator support from [[concepts/filters-routing-and-mixer]].
5. Use controlled distortion rather than excessive stereo unison.

### Growl / talking movement

1. Pick a wavetable with formant-like or uneven harmonic movement.
2. Assign an envelope or LFO to wavetable position.
3. Add warp modulation.
4. Route through filter movement.
5. Add distortion, compression, and EQ in the FX rack.

## Related pages

- [[concepts/modulation-system]] — assigning movement to wavetable position, warp, pan, and level.
- [[concepts/wavetable-editor-and-imports]] — creating and importing the source wavetables.
- [[concepts/fx-modules]] — post-oscillator shaping.
- [[entities/serum-2]]
