---
type: "Concept"
sources: ["summaries/Serum-2-User-Guide.md"]
description: "Serum 2's management layer includes preset browser workflows, metadata, packs, global preferences, voice control, tuning, file structure, CPU optimization, and shortcuts."
---

# Presets, Global Settings, and Optimization

Serum 2's manual ends with the systems that make patches maintainable: preset browsing, metadata, pack creation, global preferences, voice control, tuning, file structure, optimization, and keyboard shortcuts.

## Preset browser

The preset browser supports navigating folders, loading presets, previewing presets, searching by name, searching by categories/tags, searching by ratings, managing presets, editing metadata, specifying category, rating presets, standard preset operations, and creating/exporting packs.

Practical preset hygiene:

- Name patches by musical role, not just vibe.
- Add category/tag metadata when saving reusable sounds.
- Rate presets honestly so the browser becomes useful.
- Export packs when moving a coherent group of presets.
- Embed custom assets when needed.

## Global settings

The Global module covers preferences, voice control, randomization, scaling, quality, tuning, concert pitch, tuning files, MTS-ESP tuning, locking tuning configuration, and checking build version/date.

Global settings are the difference between a one-off patch and a stable working environment.

## File structure

The manual includes an appendix on Serum's file structure. This matters for backup, migration, preset organization, pack management, wavetable assets, formula files, and troubleshooting.

## CPU optimization

The optimization appendix specifically calls out CPU optimization and managing unison. The most obvious CPU trap in Serum-style patching is stacking too many voices, then adding FX and modulation on top.

Optimization habits:

- Reduce unison voices when the difference is inaudible in the mix.
- Avoid wide stereo unison on layers that do not need it.
- Use quality settings appropriate to the stage: drafting versus final rendering.
- Bypass unused oscillators, filters, and FX modules.
- Keep sub and low-end routing simple.

## Keyboard shortcuts

The manual includes shortcuts for presets/browser, controls, modules, sample/granular/spectral, audio, FX, matrix, LFOs, modulation, clips, and wavetable editor operations. These shortcuts matter because Serum sound design is often iterative. Faster editing makes experimentation cheaper.

## Related pages

- [[concepts/wavetable-editor-and-imports]]
- [[concepts/fx-modules]]
- [[concepts/clips-and-arpeggiator]]
- [[entities/serum-2]]
