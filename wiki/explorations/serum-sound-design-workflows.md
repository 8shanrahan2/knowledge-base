---
type: "Exploration"
sources: ["summaries/Serum-2-User-Guide.md"]
description: "Practical Serum 2 sound-design workflows combining oscillators, sample engines, modulation, routing, FX, clips, arp, and preset management."
---

# Serum Sound Design Workflows

This exploration turns the wiki concepts into patch-building recipes. It is not a replacement for the manual; it is a working map for deciding what to touch first.

## Workflow 1: Init patch to basic wavetable pluck

1. Start with an initialized preset.
2. Use [[concepts/wavetable-synthesis]] to choose a wavetable and position.
3. Set envelope behavior for a short attack and controlled decay.
4. Route oscillator through a filter in [[concepts/filters-routing-and-mixer]].
5. Assign an envelope to filter cutoff using [[concepts/modulation-system]].
6. Add light distortion or compression in [[concepts/fx-modules]].
7. Save with metadata using [[concepts/presets-global-settings-and-optimization]].

## Workflow 2: Stable bass patch

1. Use a simple wavetable or stable frame.
2. Add sub oscillator support.
3. Keep random phase low for repeatable attack.
4. Keep the sub path clean and centered.
5. Distort mid/high content rather than the whole low end.
6. Use EQ/filter cleanup.
7. Reduce unison if the bass loses focus or wastes CPU.

## Workflow 3: Evolving pad

1. Pick a wavetable with smooth frame variation.
2. Add unison width.
3. Modulate wavetable position slowly with an LFO.
4. Add slow filter movement.
5. Use chorus/hyper/dimension and reverb in the FX rack.
6. Macro-map brightness, width, and reverb mix.

## Workflow 4: Granular texture from a sample

1. Load a sample into the granular engine from [[concepts/sample-granular-spectral-engines]].
2. Set sample start/end and loop behavior.
3. Adjust scan, density, length, and window amount.
4. Add randomization if the texture feels too static.
5. Use filter and FX movement for shape.
6. Save the patch with embedded assets if needed.

## Workflow 5: Built-in motion with arpeggiator or clips

1. Decide whether the motion is a fixed phrase or chord-driven pattern.
2. Use clips for fixed piano-roll note material.
3. Use arpeggiator for held-note pattern behavior.
4. Use velocity and note tracking in the modulation system for expressive changes.
5. Route MIDI out if another instrument should receive the generated notes.

## Patch debugging checklist

- Is the sound source actually enabled?
- Is the source routed to the expected filter, bus, direct output, or main output?
- Is a modulation assignment moving a parameter unexpectedly?
- Is the FX rack bypassed or over-processing the sound?
- Is unison causing CPU or phase problems?
- Are custom assets embedded or available in the expected file location?
- Is the preset browser metadata good enough to find this patch later?

## Related pages

- [[concepts/wavetable-synthesis]]
- [[concepts/sample-granular-spectral-engines]]
- [[concepts/filters-routing-and-mixer]]
- [[concepts/modulation-system]]
- [[concepts/fx-modules]]
- [[concepts/clips-and-arpeggiator]]
- [[concepts/wavetable-editor-and-imports]]
- [[concepts/presets-global-settings-and-optimization]]
