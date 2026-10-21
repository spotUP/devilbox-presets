# devilbox-presets

Synth preset banks for [DEViLBOX](https://github.com/spotUP/DEViLBOX). The banks are large, so they live here
and not in the DEViLBOX history. DEViLBOX keeps only the generated preset indexes; the live server clones
this repo and serves it at `/data/presets/`.

## Layout

One directory per synth:

- `vital/` - Vital presets
- `odin2/` - Odin2 presets: factory (GPL-3.0), Lukas Lundh, PSY-LION
- `surge/` - Surge presets (to come)
- `soundfonts/` - SoundFont banks for the FluidSynth host: GeneralUser GS v2.0.3 by S. Christian Collins
  (General MIDI / GS bank, free for any use incl. commercial; see `soundfonts/LICENSE.txt`,
  https://www.schristiancollins.com/generaluser)

Each pack carries its own licence file inside its folder. Only presets whose licence allows
redistribution are included.

## Use

In a DEViLBOX checkout run `npm run presets:sync`; it clones or pulls this repo into `public/data/presets/`.
