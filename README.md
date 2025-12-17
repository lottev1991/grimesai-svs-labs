# GrimesAI HTK-style SVS Labels
This repository contains HTK-style .lab files, to be used on dry stems from the GrimesAI dataset. This to facilitate them for training SVS (singing voice synthesis) AI models.

~~You can download the audio dataset on [elf.tech](https://elf.tech) (you need to make an account first).~~ **EDIT 2025/12/17:** The elf.tech website seems to currently be experiencing issues, _however_ the stems themselves are still online. They can be downloaded [here](https://grimes.wetransfer.com/downloads/4cf76171fc91733062eb277d9402b13620230430211631/6b2a23). This is the official download link, if anyone is concerned.

## License note
The license included in this repository applies *ONLY* to the .lab files, *NOT* the original audio dataset, which was released under Grimes' own terms of use (more information can be found [here](https://createsafe.notion.site/Elf-Tech-GrimesAI-1-Voiceprint-610d81fcf2844419afafab493c6ec4b4)).

## General information
Canadian singer-songwriter Grimes has authorized her voice and music to be used for the training of AI models. The dataset that she released includes both wet and dry vocal stems, as well as instrument tracks; a selection of the dry vocal stems have been labeled with phonetic transcriptions and phoneme duration information by yours truly. Stems that were deemed unsuitable were left out. The filenames of the labels correspond to the audio files found in the original dataset. Stems from the songs "IDORU" and "Delicate Weapon" have been used.


## Phonetic system
The phonemes are based on [ARPABET](https://en.wikipedia.org/wiki/ARPABET), including the following extended phonemes:
- `ax` (schwa);
- `dx` (tap);
- `em` (syllabic `m`);
- `en` (syllabic `n`).

It also incorporates the following non-ARPABET phonemes:
- `GS` (glottal stop); 
- `EP` (exhale);
- `vf` (vocal fry/creaky voice).

The labels use `SP` as its pause phoneme, and `AP` as its breath (inhale) phoneme. These are considered global/required.

### Notes on phonemes
- I am aware that the extended ARPABET uses `q` for its glottal stop phoneme. However, `GS` was used instead, in order to prevent conflicts with phonetic transcription systems used in other languages that may use `q` for a different sound (e.g. Mandarin Chinese, Arabic).
- Some phonemes are not present in the labels, since they were also not present in the audio data. One example is the phoneme `oy`. **Therefore it is *HIGHLY ADVISED* to train the data in parallel with another public dataset!** An example of a public English corpus you could use for this purpose is my own [Project AI❤dol Public English Dataset](https://github.com/lottev1991/Project-AIdol-Public-English-Dataset), which has a full phonetic inventory.

## A note on commercial use
Any commercial use of models that incorporate these labels requires a 50/50 split of royalties between you and Grimes. This is in accordance with her original terms (see above, under "License note").
