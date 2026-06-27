---
type: "Concept"
sources: ["summaries/Serum-2-User-Guide.md"]
description: "Serum 2 FX modules are reorderable rack processors for post-synth shaping, splitter routing, modulation, and rack preset reuse."
---

# FX Modules

Serum 2's FX module is a rack system for processing the synth output. Modules can be loaded, added, reordered, copied, bypassed, removed, modulated, and saved as rack presets.

## FX rack operations

The manual covers:

- Selecting a rack.
- Loading rack presets.
- Adding modules.
- Reordering modules.
- Copying a module.
- Bypassing a module.
- Removing a module.
- Saving a rack as a preset.
- Modulating FX parameters.
- Exploring individual module operations.

## Module inventory

The Serum 2 manual lists these FX module areas:

- **Bode** — frequency-shifting style effect.
- **Chorus** — modulation/thickening effect.
- **Compressor** — dynamics control.
- **Convolve** — convolution/impulse-style processing.
- **Distortion** — harmonic and nonlinear shaping.
- **Equalizer** — frequency balance.
- **Filter** — FX-stage filtering.
- **Flanger** — comb-filter/modulation effect.
- **Hyper/Dimension** — width and thickening.
- **Phaser** — phase-swept movement.
- **Reverb** — space and ambience.
- **Splitter L/H** — low/high split processing.
- **Splitter L/M/H** — low/mid/high split processing.
- **Splitter MS** — mid/side split processing.
- **Utility** — practical gain, phase, balance, or width-style operations.

## Signal-chain thinking

Order matters. Distortion before a filter behaves differently than distortion after a filter. Compression before reverb behaves differently than compression after reverb. Splitter modules let a rack behave less like a simple serial chain and more like a controlled multi-band or mid/side processor.

Common patterns:

### Bass processing

1. Keep sub clean or minimally processed.
2. Distort harmonics on the mid/high layer.
3. Use EQ/filter cleanup.
4. Compress for control.
5. Avoid excessive reverb or stereo width on low frequencies.

### Lead processing

1. Add distortion for presence.
2. Use filter or EQ to remove harshness.
3. Add chorus/hyper/dimension for width.
4. Add reverb carefully.
5. Macro-map intensity or space.

### Pad processing

1. Start with chorus/hyper/dimension for width.
2. Use phaser/flanger subtly for movement.
3. Add reverb for space.
4. Use EQ or filter to keep the patch out of the way.

## Modulating FX

FX parameters can become destinations in the [[concepts/modulation-system]]. This is useful for:

- Increasing distortion only during a macro sweep.
- Opening reverb mix on long notes.
- Moving phaser/flanger depth rhythmically.
- Automating filter cutoff inside the FX rack.
- Changing splitter behavior over time.

## Related pages

- [[concepts/filters-routing-and-mixer]] — pre-FX routing and busses.
- [[concepts/modulation-system]] — animating FX parameters.
- [[concepts/wavetable-synthesis]] — oscillator source material sent into FX.
- [[explorations/serum-sound-design-workflows]] — practical chains.
