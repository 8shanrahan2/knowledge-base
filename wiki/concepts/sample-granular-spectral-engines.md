---
type: "Concept"
sources: ["summaries/Serum-2-User-Guide.md"]
description: "Serum 2 includes sample, granular, and spectral engines for direct playback, grain-based transformation, and frequency-domain resynthesis."
---

# Sample, Granular, and Spectral Engines

Serum 2 expands beyond classic wavetable synthesis by letting audio material become a playable source in three related but different ways: sample playback, granular synthesis, and spectral synthesis.

## Mental model

- **Sample engine**: play and manipulate audio directly.
- **Granular engine**: break audio into grains and reassemble it into textures, stretched movement, clouds, and evolving timbres.
- **Spectral engine**: operate on frequency-domain content, emphasizing scan, cut, filter, and mix controls.

These engines share workflow ideas: load or select audio, define sample start/end, configure loop behavior, set crossfades, control scan/playback, apply unison/warp, then mix with pan and level.

## Sample instruments

Sample mode is the most direct audio-based engine. The manual covers selecting the sampler, setting sample start/end, performing sample operations, slicing samples, loop menus, loop start/end, crossfade, and parameters such as scan, unison, warp, pan, and level.

Use sample mode when you want recognizable audio playback, transients, one-shots, short loops, or sliced material.

## Granular synthesis

Granular mode uses sample material but turns it into grains. The manual covers selecting granular synthesis, sample start/end, granular operations, loop/crossfade controls, window amount, unison, X/Y control, scan, density, length, pan, level, and grain randomization.

Use granular mode when you want:

- Pads from short samples.
- Frozen or stretched textures.
- Swarms/clouds of tiny audio fragments.
- Movement that feels less like an oscillator and more like transformed source material.

Important controls:

- **Scan** — where the engine reads through the source.
- **Density** — how many grains occur.
- **Length** — size/duration of grains.
- **Window amount** — shape/smoothness of grain boundaries.
- **Randomization** — variation in grain behavior.

## Spectral synthesis

Spectral mode treats the sample as frequency material. The manual covers selecting spectral synthesis, sample start/end, high/low frequency ranges, sample operations, loop/crossfade controls, unison, X/Y control, scan, cut, filter, mix, warp, pan, and level.

Use spectral mode when you want frequency-focused transformation rather than straightforward playback. It is useful for glassy, vocal, metallic, resynthesized, filtered, or partially abstracted tones.

## How to choose the engine

| Goal | Best starting engine |
|---|---|
| Play a one-shot or loop | Sample |
| Slice or reposition audio | Sample |
| Make a pad from a tiny sound | Granular |
| Stretch/freeze texture | Granular |
| Reshape frequency content | Spectral |
| Create glassy or formant-like timbres | Spectral |
| Convert sample to oscillator-like material | Consider switching sample to wavetable |

## Cross-links

- [[concepts/wavetable-synthesis]] — oscillator-based alternative.
- [[concepts/modulation-system]] — scan, density, length, cut, filter, mix, and warp become more powerful when modulated.
- [[concepts/filters-routing-and-mixer]] — route these engines into filters and busses.
- [[concepts/fx-modules]] — finish audio-source patches with effects.
