---
title: "Serum 2 User Guide Knowledge Base"
type: "knowledge_base_index"
source_document: "Serum 2 User Guide, Manual Version 1.0.3"
product: "Serum 2"
vendor: "Xfer Records"
version: "2.0.18"
manual_date: "2025-04-27"
status: "seed"
---

# Serum 2 User Guide Knowledge Base

> OpenKB-style compiled wiki page for the Serum 2 manual. The goal is to convert a long PDF manual into durable, queryable knowledge: summaries, concepts, workflows, cross-links, and open questions instead of repeatedly rereading the whole document.

## What this is

This repo is a lightweight knowledge base for **Serum 2**, an advanced virtual synthesizer plug-in for Windows and macOS. Serum 2 supports **VST3**, **Audio Unit**, and **AAX** hosts and combines multiple synthesis methods inside one workflow.

The uploaded source manual identifies Serum 2 as version **2.0.18**, manual version **1.0.3**, dated **April 27, 2025**.

## Source summary

Serum 2 is a virtual synthesizer that combines:

- **Wavetable synthesis**
- **Subtractive synthesis** through filters and routing
- **Multisampled instruments**
- **Sample playback**
- **Granular synthesis**
- **Spectral synthesis**
- **Modulation** through envelopes, LFOs, macros, velocity, note tracking, and the modulation matrix
- **Integrated sequencing tools** including clips and arpeggiators
- **FX racks** with reorderable modules
- **Wavetable editing and importing**

The manual is organized less like a theory text and more like a full operating guide. It starts with installation and preset basics, then moves through sound engines, modulation, routing, sequencing, editing, global settings, file structure, optimization, and keyboard shortcuts.

## Quick mental model

Think of Serum 2 as four linked layers:

1. **Sound sources** — wavetable oscillators, multisamples, samples, granular, spectral, sub oscillator, and noise oscillator.
2. **Shaping and routing** — filters, mixer, busses, pan, level, routing, and direct/main output controls.
3. **Movement** — envelopes, LFOs, macros, velocity, note tracking, and modulation matrix assignments.
4. **Performance/output** — clips, arpeggiator, keyboard settings, MIDI out, FX racks, preset browser, and export workflows.

## Core concepts

### [[Wavetables]]

A wavetable is a collection of waveform frames that can be scanned or modulated over time. Serum 2 exposes wavetable position, phase, random phase, phase memory, unison, warp, pan, and level controls. The wavetable editor can draw, edit, sort, morph, import, export, and save tables.

Useful questions:

- What makes a good wavetable?
- When should wavetable position be automated versus modulated by an LFO?
- How do phase, random phase, and phase memory change transient consistency?

### [[Samples, Granular, and Spectral Engines]]

Serum 2 goes beyond classic wavetable synthesis. It can use samples directly, split samples into grains for granular synthesis, or analyze frequency content for spectral synthesis. These engines share concepts like sample start/end, loop start/end, crossfade, scan, unison, pan, and level, but each engine emphasizes different sound-design goals.

Use this distinction:

- **Sample mode**: play or slice audio material directly.
- **Granular mode**: transform audio into clouds, textures, pads, and stretched material.
- **Spectral mode**: reshape frequency-domain content using scan, cut, filter, mix, and warp controls.

### [[Filters and Routing]]

Filters are not just tone controls. In Serum 2 they are part of the routing system. Oscillators and sound sources can be routed into filters, filters can be mixed, and busses can be used to structure more complex patches.

Key parameters include cutoff, resonance, drive, fat/variant controls, pan, mix, and level.

### [[Modulation System]]

Serum 2's modulation system is one of the main reasons to use it. Envelopes and LFOs can be assigned to controls, modulation depth can be positive or negative, LFO points can themselves be modulated, and the matrix gives a central view of assignments.

Important modulation sources:

- Envelopes
- LFOs
- Macros
- Velocity
- Note tracking
- Oscillators and filters used as modulation sources

Working rule: use **envelopes** for one-shot contour, **LFOs** for repeated or drawn movement, and **macros** for performance controls you want to expose while playing or automating.

### [[FX Rack]]

The FX module uses racks made of reorderable modules. Effects can be loaded from presets, copied, bypassed, removed, reordered, and saved as racks.

Covered modules include Bode, Chorus, Compressor, Convolve, Distortion, Equalizer, Filter, Flanger, Hyper/Dimension, Phaser, Reverb, Splitters, and Utility.

### [[Clips and Arpeggiator]]

Serum 2 includes internal musical control tools. Clips provide a piano-roll-like workflow for triggering and recording note material. The arpeggiator provides banks, patterns, graph editing, transpose settings, playback settings, retrigger settings, velocity settings, and MIDI output.

Use these when you want Serum to generate or structure musical material before it reaches the host DAW piano roll.

### [[Preset Browser and File Structure]]

The appendices cover preset browsing, metadata, ratings, pack creation/export, preference-file edits, file structure, optimization, and shortcuts. These sections matter because Serum sound design is partly about patch creation and partly about managing reusable assets.

## Entity pages to create next

- [[Serum 2]] — product overview
- [[Xfer Records]] — vendor and registration/support context
- [[Wavetable Editor]] — editing, importing, formula parser, frame operations
- [[Modulation Matrix]] — source/destination/depth routing
- [[FX Rack]] — module list and signal-chain behavior
- [[Preset Browser]] — search, tags, metadata, ratings, packs
- [[CPU Optimization]] — unison and quality tradeoffs

## Suggested folder structure

```text
knowledge-base/
  README.md
  sources/
    Serum 2 User Guide.md
  concepts/
    Wavetables.md
    Modulation System.md
    Filters and Routing.md
    Samples Granular Spectral.md
    FX Rack.md
    Clips and Arpeggiator.md
  entities/
    Serum 2.md
    Xfer Records.md
  explorations/
    sound-design-recipes.md
    fl-studio-serum-workflow.md
```

## Starter queries this wiki should answer

- How do I create a new sound in Serum 2 from an initialized patch?
- What is the difference between wavetable, sample, granular, and spectral modes?
- How do I assign an LFO or envelope to a control?
- How do I use the modulation matrix to audit a patch?
- How do I import audio as a wavetable?
- What are the CPU-heavy parts of Serum 2?
- How do I save presets, racks, formulas, and wavetable assets?
- How do clips and the arpeggiator interact with MIDI out?

## Knowledge gaps / next pass

This seed page is based on the manual outline and visible extracted text. A stronger OpenKB-style pass should split the PDF into section-level pages, preserve screenshots as page references, and generate concept pages from the body text for each major section.

Recommended next step: compile sections from the PDF into individual Markdown pages under `concepts/` and `sources/`, then cross-link them from this index.
