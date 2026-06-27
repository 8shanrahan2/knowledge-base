---
type: "Concept"
sources: ["summaries/Serum-2-User-Guide.md"]
description: "Serum 2's wavetable editor supports drawing, FFT editing, frame operations, formula generation, morphing, audio import, image import, and embedding."
---

# Wavetable Editor and Imports

The wavetable editor is where Serum 2 becomes a design tool rather than only a preset player. It supports drawing waveforms, editing harmonic content, managing frames, importing audio, importing images, applying formula-generated shapes, exporting wavetables, and embedding wavetables in presets.

## Editor areas

The manual covers:

- Thumbnails.
- Drawing tools.
- FFT area.
- Frame/subtable management.
- Common frame operations.
- Copying and pasting frames.
- Inserting and removing frames.
- Sorting frames.
- Formula parser.
- Menu commands.
- Import and export operations.
- Single, All, and Morph menus.
- Saving wavetables.

## Frame workflow

A wavetable is easiest to reason about as a set of ordered frames. The order matters because modulation through wavetable position moves through that order.

Useful frame operations:

- Copy/paste frames to preserve useful shapes.
- Insert/remove frames to control density of change.
- Sort frames when imported material is disorganized.
- Morph between frames to create smoother motion.
- Export useful tables for reuse.

## Formula parser

The formula parser is an advanced way to generate waveforms mathematically. The manual covers basic functions, binary operators, constants, variables, formula presets, saving formulas, manually managing formula files, and examples.

Use formulas when drawing is too imprecise or when a repeatable mathematical shape is desired.

## Audio imports

Serum 2 supports importing audio as wavetables. The manual covers multi-cycle waveforms, importing multi-cycle waveforms, advanced import settings, text-file overrides, importing single-cycle waveforms, import menu choices, and creating source sounds specifically for Serum import.

Practical rule: clean, intentional source audio imports better than messy audio. If you want a smooth wavetable, feed Serum something with stable pitch or clear cycles. If you want artifacts and motion, use more complex source material intentionally.

## Image imports

The manual also covers importing an image file as a wavetable. This can create unusual harmonic structures and visual-to-audio experiments.

## Embedding

Embedding wavetables when saving a preset helps preserve custom assets. This matters when sharing patches or moving projects between systems.

## Related pages

- [[concepts/wavetable-synthesis]] — using the resulting wavetable in an oscillator.
- [[concepts/modulation-system]] — scanning the wavetable with LFOs, envelopes, macros, velocity, or note tracking.
- [[concepts/presets-global-settings-and-optimization]] — preset and file-management implications.
