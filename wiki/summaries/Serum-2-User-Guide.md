---
type: "Summary"
description: "Serum 2 User Guide documents the Serum 2 synthesizer plug-in, including sound engines, routing, modulation, FX, clips, arpeggiator, wavetable editing, presets, global settings, file structure, optimization, and shortcuts."
doc_type: long_pdf
source: "Serum 2 User Guide, Manual Version 1.0.3, April 27 2025"
product_version: "2.0.18"
---

# Serum 2 User Guide

Serum 2 is an advanced virtual synthesizer instrument plug-in for Microsoft Windows and Apple macOS. It runs inside VST3, Audio Unit, and AAX hosts and combines wavetable, subtractive, multisampled, sampled, granular, and spectral synthesis into a single workflow.

## High-level purpose

The manual is a complete operating guide. It starts with account, download, installation, preset loading, saving, UI help, knobs, sliders, undo/redo, oscillator/filter enablement, routing, pitch controls, and UI resizing. It then moves into the actual sound-design system.

## Major feature areas

### Sound generation

- **Wavetable oscillators** — core oscillator mode with wavetable position, phase, random phase, phase memory, unison, warp, pan, and level.
- **Multisample instruments** — sampled instrument playback with envelope, velocity tracking, randomization, timbre, unison, warp, pan, and level.
- **Sample instruments** — direct sample playback with start/end, sample operations, slicing, loop controls, crossfade, scan, unison, warp, pan, and level.
- **Granular synthesis** — sample-based grain engine with loop/crossfade controls, windowing, unison, X/Y control, scan, density, length, pan, level, and randomization.
- **Spectral synthesis** — frequency-domain engine with sample range, high/low frequency range, loop/crossfade controls, unison, X/Y control, scan, cut, filter, mix, warp, pan, and level.
- **Sub oscillator** — simple low-frequency support oscillator with pitch, waveform, phase, pan, and level.
- **Noise oscillator** — noise/sample source with preset loading, sample loading, one-shot/looping, start, random, pitch, fine, pan, and level.

### Routing and mixing

The guide covers filter modules, oscillator routing, filter type selection, filter parameter controls, mixer busses, filter mixing, bus mixing, and main/direct output levels. This makes Serum 2 more like a compact modular synth than a fixed subtractive synth.

### Modulation

The manual dedicates a large section to envelopes, LFOs, drag-and-drop assignments, modulation depth, negative modulation depth, copying shapes between wavetables and LFOs, modulating LFO points, context menus, velocity, note modulation, macros, oscillator/filter modulation sources, and the modulation matrix.

### Effects

Serum 2 includes an FX module with racks, rack presets, add/reorder/copy/bypass/remove workflows, rack saving, modulation of FX parameters, and detailed documentation for individual FX modules.

### Composition and performance

The guide documents clips, an internal piano-roll-like system, plus the arpeggiator. These sections cover clip banks, global settings, piano roll editing, grid/zoom/fold/length, triggering, recording, MIDI out, arpeggiator banks, pattern editing, transpose/playback/retrigger/velocity settings, and MIDI routing.

### Editing and asset management

The wavetable editor supports thumbnails, drawing tools, FFT editing, frame/subtable operations, copying/pasting/inserting/removing/sorting frames, formula parser workflows, wavetable importing/exporting, morph operations, audio import, image import, and embedding custom wavetables in presets.

### Administration and optimization

Appendices cover the main menu, preset browser, preset metadata, pack creation/export, preference-file editing, file structure, wavetable creation advice, CPU optimization, and keyboard shortcuts.

## Practical workflow

1. Load Serum 2 on a DAW track.
2. Start from an initialized preset or an existing preset.
3. Choose sound sources: wavetable, sample, granular, spectral, multisample, sub, and/or noise.
4. Route sources through filters and the mixer.
5. Add motion with envelopes, LFOs, macros, velocity, note tracking, and matrix assignments.
6. Shape the patch with FX modules and splitter routing.
7. Use clips or arpeggiator when Serum should generate internal note movement.
8. Save the preset, rack, wavetable, formula, or pack with useful metadata.

## Related concepts

- [[concepts/wavetable-synthesis]]
- [[concepts/sample-granular-spectral-engines]]
- [[concepts/filters-routing-and-mixer]]
- [[concepts/modulation-system]]
- [[concepts/fx-modules]]
- [[concepts/clips-and-arpeggiator]]
- [[concepts/wavetable-editor-and-imports]]
- [[concepts/presets-global-settings-and-optimization]]

## Entities

- [[entities/serum-2]]
- [[entities/xfer-records]]
- [[entities/steve-duda]]
