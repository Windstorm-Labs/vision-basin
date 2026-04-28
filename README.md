# Paper 8: The Vision Basin — Experiments & Code

**Cross-Modal Throughput Measurement Reveals Modality-Specific Information Extraction Rates**

[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.19672827-blue)](https://doi.org/10.5281/zenodo.19672827)
[![License: MIT](https://img.shields.io/badge/Code-MIT-green)](https://opensource.org/licenses/MIT)
[![License: CC BY 4.0](https://img.shields.io/badge/Data-CC_BY_4.0-lightgrey)](https://creativecommons.org/licenses/by/4.0/)

---

## Published Paper

**[Windstorm-Institute/vision-basin](https://github.com/Windstorm-Institute/vision-basin)** — paper PDF, article HTML

**Website article:** [windstorminstitute.org/articles/vision-basin.html](https://windstorminstitute.org/articles/vision-basin.html)

**Zenodo (concept DOI, always-latest):** [10.5281/zenodo.19672827](https://doi.org/10.5281/zenodo.19672827) · **v2.2:** [10.5281/zenodo.19672828](https://doi.org/10.5281/zenodo.19672828)

## Experiments

| Experiment | Directory | Key Result |
|---|---|---|
| MAE generative throughput | `experiments/p8_e1_mae_throughput/` | MAE-Base: 1.33, MAE-Large: 1.36 bits/pixel |
| ViT classification survey | `experiments/exp2_vit_survey/` | 8 models: 0.002–0.03 bits/patch |
| Visual source entropy | `experiments/exp5_visual_entropy/` | STL-10: 4.02 bpp (WebP) |
| Visual shuffling cascade | `experiments/p8a_v2_visual_cascade/` | Structural bonus: 0.69 bpp |
| Patch-size invariance | `experiments/p8_e7_patch_invariance/` | Bits/pixel varies 4× with patch size |
| High-res entropy | `experiments/p8_e8_highres_entropy/` | Resolution-dependent: 3.2 at 224×224 |
| Real LJ Speech audio | `experiments/p8_e4_real_audio/` | Real speech: 1.89 bits/mel_dim |
| 12-model throughput survey | `experiments/p8_f1_throughput_survey/` | 3 modalities, 12 models |
| Cross-modal bonus | `experiments/analysis_cross_modal/` | Language 6.7, vision 0.69, music 2.83 |
| Music vs speech entropy | `experiments/analysis_music_speech/` | Music > speech in throughput |

## Hardware

- **GPU:** NVIDIA RTX 5090 (32 GB VRAM)
- **CPU:** Intel Core Ultra 9 285K (24 cores)
- **RAM:** 256 GB
- **OS:** Ubuntu 24.04, Python 3.12, PyTorch 2.11

## Reproduction

All CSVs in `experiments/*/results/` are the raw outputs. Plots in `plots/`.
Training scripts are in the canonical repo: [Windstorm-Institute/throughput-basin-origin](https://github.com/Windstorm-Institute/throughput-basin-origin) under `paper8/` and `weekend_experiments/p8_*/`.

---

## The Windstorm Series

| # | Paper | DOI |
|---|-------|-----|
| 1 | [The Fons Constraint](https://github.com/Windstorm-Institute/fons-constraint) | [10.5281/zenodo.19274048](https://doi.org/10.5281/zenodo.19274048) |
| 2 | [The Receiver-Limited Floor](https://github.com/Windstorm-Institute/receiver-limited-floor) | [10.5281/zenodo.19322973](https://doi.org/10.5281/zenodo.19322973) |
| 3 | [The Throughput Basin](https://github.com/Windstorm-Institute/throughput-basin) | [10.5281/zenodo.19323194](https://doi.org/10.5281/zenodo.19323194) |
| 4 | [The Serial Decoding Basin τ](https://github.com/Windstorm-Institute/serial-decoding-basin) | [10.5281/zenodo.19323423](https://doi.org/10.5281/zenodo.19323423) |
| 5 | [The Dissipative Decoder](https://github.com/Windstorm-Institute/dissipative-decoder) | [10.5281/zenodo.19433048](https://doi.org/10.5281/zenodo.19433048) |
| 6 | [The Inherited Constraint](https://github.com/Windstorm-Institute/inherited-constraint) | [10.5281/zenodo.19432911](https://doi.org/10.5281/zenodo.19432911) |
| 7 | [The Throughput Basin Origin](https://github.com/Windstorm-Institute/throughput-basin-origin) | [10.5281/zenodo.19498582](https://doi.org/10.5281/zenodo.19498582) |
| 8 | [The Vision Basin](https://github.com/Windstorm-Institute/vision-basin) *(this paper)* | [10.5281/zenodo.19672827](https://doi.org/10.5281/zenodo.19672827) |
| 9 | [The Hardware Basin](https://github.com/Windstorm-Institute/hardware-basin) | [10.5281/zenodo.19672921](https://doi.org/10.5281/zenodo.19672921) |

**Website:** [windstorminstitute.org](https://windstorminstitute.org)

---

*Code: MIT License · Data: CC BY 4.0*
