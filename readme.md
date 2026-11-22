# ICME 2026 Grand Challenge on Academic Text-to-Music Generation (ATTM)

This repository collects community resources from the **ICME 2026 ATTM Grand Challenge**: the official codebase, information about participating teams, and the audio samples they generated for the test prompts.

All resources from participants are shared **voluntarily**, under the option and license each team chose. Please respect each team's license and cite their work when you use their checkpoints or samples.

---

## Table of Contents

- [ICME 2026 Grand Challenge on Academic Text-to-Music Generation (ATTM)](#icme-2026-grand-challenge-on-academic-text-to-music-generation-attm)
  - [Table of Contents](#table-of-contents)
  - [Codebase](#codebase)
  - [Repository Structure](#repository-structure)
  - [Sharing Options](#sharing-options)
  - [Contributed Submissions](#contributed-submissions)
    - [Summary](#summary)
    - [Team Details](#team-details)
      - [e02 — G-Clef](#e02--g-clef)
      - [e09, p09 — UT-AISTimprt](#e09-p09--ut-aistimprt)
      - [p05 — MAAP Lab, Yonsei University](#p05--maap-lab-yonsei-university)
  - [License](#license)
  - [Citation](#citation)
  - [Contact](#contact)

---

## Codebase

**Official website:** <https://ntu-musicailab.github.io/ICME26-ATTM-Grand-Challenge/>

| Description | Repository |
| --- | --- |
| Evaluation | [ICME26-ATTM-GC-Evaluation](https://github.com/ntu-musicailab/ICME26-ATTM-GC-Evaluation) |
| FluxAudio baseline | [ICME26-ATTM-GC-FluxAudio](https://github.com/ntu-musicailab/ICME26-ATTM-GC-FluxAudio) |
| Audio-language-model captioning | [ICME26-ATTM-GC-ALM-captioning](https://github.com/ntu-musicailab/ICME26-ATTM-GC-ALM-captioning) |
| Data preprocessing | [ICME26-ATTM-GC-Preprocessing](https://github.com/ntu-musicailab/ICME26-ATTM-GC-Preprocessing) |

---

## Repository Structure

Audio samples are stored under `assets/`, with one folder per submission. Each folder is named after the submission ID used in the challenge paper.

```
.
├── readme.md
└── assets/
    ├── e02/    # G-Clef
    ├── e08/    # PurpleMusic
    ├── e09/    # UT-AISTimprt
    ├── e10/    # Zper
    ├── p05/    # Junyoung Koh (MAAP Lab, Yonsei University)
    ├── p09/    # UT-AISTimprt
    └── p10/    # Zper
```

Submission ID prefixes:

- `e**`: Efficient track
- `p**`: Performance track

---

## Sharing Options

Each team chose one of the following options:

| Option | What is shared |
| :---: | --- |
| **Option 1** | Model checkpoint **and** generated samples for the test prompts |
| **Option 2** | Generated samples for the test prompts only |

---

## Contributed Submissions

The following teams kindly agreed to share their resources with the community. This is not a complete list of all participants in the challenge.

### Summary

| ID | Team | Option | Checkpoint | Checkpoint License | Samples License | Paper |
| :---: | --- | :---: | --- | --- | --- | --- |
| [e02](#e02--g-clef) | G-Clef | 1 | [GitHub](https://github.com/yonghyunk1m/TTM-HumanPref/releases/tag/v1.0-icme2026) / [HF](https://huggingface.co/yonghyunk1m/TTM-HumanPref) | Weights: CC BY-NC 4.0; Code: MIT | CC BY 4.0 | [arXiv:2606.21670](https://arxiv.org/abs/2606.21670) |
| [e08](#e08--purplemusic) | PurpleMusic | 1 | [HF](https://huggingface.co/hhhhaura/purplemusic-500k) | MIT | CC BY 4.0 | [arXiv:2606.07387](https://arxiv.org/abs/2606.07387) |
| [e09, p09](#e09-p09--ut-aistimprt) | UT-AISTimprt | 2 | — | — | CC BY 4.0 | [arXiv:2607.01669](https://arxiv.org/abs/2607.01669) |
| [e10, p10](#e10-p10--zper) | Zper | 1 | [HF](https://huggingface.co/xlbhzz/bandtok-model) | MIT | CC BY 4.0 | [arXiv:2605.21433](https://arxiv.org/abs/2605.21433) |
| [p05](#p05--maap-lab-yonsei-university) | MAAP Lab, Yonsei University | 2 | — | — | CC BY 4.0 | [arXiv:2605.21433](https://arxiv.org/abs/2605.21433) |

### Team Details

#### e02 — G-Clef

- **Members:** Yonghyun Kim, Junwon Lee, Haiwen Xia, Yinghao Ma, Chris Donahue
- **Option:** 1 (checkpoint + samples)
- **Checkpoint:** [Github](https://github.com/yonghyunk1m/TTM-HumanPref/releases/tag/v1.0-icme2026), [HF](https://huggingface.co/yonghyunk1m/TTM-HumanPref)
  - Model weights: CC BY-NC 4.0
  - Code: MIT
  <!-- - Both submissions come from this single checkpoint, generated with seeds `42` and `55`. -->
- **Samples:** [`assets/e02/`](assets/e02/) — CC BY 4.0
- **Paper:** [*Improving Text-to-Music Generation with Human Preference Rewards*](https://arxiv.org/abs/2606.21670)
    ```bibtex
  @inproceedings{kim2026improving,
    title     = {Improving Text-to-Music Generation with Human Preference Rewards},
    author    = {Yonghyun Kim, Junwon Lee, Haiwen Xia, Yinghao Ma and Chris Donahue},
    booktitle = {IEEE International Conference on Multimedia and Expo (ICME), Grand Challenge},
    year      = {2026}
  }
  ```

#### e08 — PurpleMusic

- **Members:** Yun-Chen Cheng, Tzu-Hung Huang, Chih-Pin Tan
- **Option:** 1 (checkpoint + samples)
- **Checkpoint:** [HF](https://huggingface.co/hhhhaura/purplemusic-500k)
- **Samples:** [`assets/e08/`](assets/e08/) — CC BY 4.0
- **Paper:** [*Making the Most of Limited Data: Score-Aware Training for Text-to-Music Generation*](https://arxiv.org/abs/2606.07387)
  ```bibtex
  @inproceedings{cheng2026making,
    title     = {Making the Most of Limited Data: Score-Aware Training for Text-to-Music Generation},
    author    = {Yun-Chen Cheng, Tzu-Hung Huang and Chih-Pin Tan},
    booktitle = {IEEE International Conference on Multimedia and Expo (ICME), Grand Challenge},
    year      = {2026}
  }
  ```

#### e09, p09 — UT-AISTimprt

- **Members:** Shunsuke Yoshida, Yu-Hua Chen, Satoru Fukayama
- **Option:** 2 (samples only)
- **Samples:** [`assets/e09/`](assets/e09/), [`assets/p09/`](assets/p09/) — CC BY 4.0
- **Paper:** [*UT-AISTimprt submission for ICME 2026 Grand Challenge on Academic Text-to-Music Generation*](https://arxiv.org/abs/2607.01669)
    ```bibtex
  @inproceedings{yoshida2026ut,
    title     = {UT-AISTimprt submission for ICME 2026 Grand Challenge on Academic Text-to-Music Generation},
    author    = {Shunsuke Yoshida, Yu-Hua Chen and Satoru Fukayama},
    booktitle = {IEEE International Conference on Multimedia and Expo (ICME), Grand Challenge},
    year      = {2026}
  }
  ```

#### e10, p10 — Zper

- **Members:** Yuqing Cheng, Xingyu Ma, Guochen Yu, Xiaotao Gu
- **Option:** 1 (checkpoint + samples)
- **Checkpoint:** [HF](https://huggingface.co/xlbhzz/bandtok-model) — MIT License
- **Samples:** [`assets/e10/`](assets/e10/), [`assets/p10/`](assets/p10/) — CC BY 4.0
- **Paper:** [*Modeling Music as a Time-Frequency Image: A 2D Tokenizer for Music Generation*](https://arxiv.org/abs/2605.15831)

  ```bibtex
  @inproceedings{cheng2026bandtok,
    title     = {Modeling Music as a Time-Frequency Image: A 2D Tokenizer for Music Generation},
    author    = {Cheng, Yuqing and Ma, Xingyu and Yu, Guochen and Gu, Xiaotao},
    booktitle = {IEEE International Conference on Multimedia and Expo (ICME), Grand Challenge},
    year      = {2026}
  }
  ```

#### p05 — MAAP Lab, Yonsei University

- **Members:** Junyoung Koh (MAAP Lab, Yonsei University)
- **Option:** 2 (samples only)
- **Samples:** [`assets/p05/`](assets/p05/) — CC BY 4.0
- **Paper:** [*Instrumental Text-to-Music Generation with Auxiliary Conditioning Branches*](https://arxiv.org/abs/2605.21433)
  ```bibtex
  @inproceedings{koh2026instrumental,
    title     = {Instrumental text-to-music generation with auxiliary conditioning branches},
    author    = {Koh, Junyoung},
    booktitle = {IEEE International Conference on Multimedia and Expo (ICME), Grand Challenge},
    year      = {2026}
  }
  ```

---

## License

- **Codebase:** see the [Codebase](#codebase) link.
- **Checkpoints and samples:** each team's resources are released under the license that team chose, listed in [Contributed Submissions](#contributed-submissions). Model checkpoints are hosted by the teams; their own license terms take precedence.
- Copyright of all shared checkpoints and samples remains with the respective teams.

---

## Citation

If you use any team's checkpoint or samples, please cite that team's paper (see [Team Details](#team-details)) along with the challenge overview paper:

```bibtex
@inproceedings{hsieh2026academic,
  title={Academic text-to-music grand challenge: Datasets, baselines, and evaluation methods},
  author={Hsieh, Fang-Chih and Lee, Wei-Jaw and Wang, Chun-Ping and Lee, Hung-yi and Dong, Hao-Wen and Yang, Yi-Hsuan},
  booktitle = {IEEE International Conference on Multimedia and Expo (ICME), Grand Challenge},
  year={2026}
}
```

---

## Contact

<!-- TODO: add organizer contact -->

Thanks to all participating teams for contributing their checkpoints and samples to the community.
