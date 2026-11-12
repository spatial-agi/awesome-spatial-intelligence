# Contributing to Awesome-Spatial-Intelligence

Thanks for helping keep this list of spatial intelligence research up to date. This guide describes how to add a paper so that every entry stays consistent with the handbook and easy to scan.

If anything is unclear, open an issue before submitting a pull request.

---

## Scope

We list work that is **cited in the Handbook of Spatial Intelligence** or that directly extends a topic the handbook covers:

- spatial representations in 2D, 3D, 4D, language, audio, and across modalities
- spatial perception, spatial reasoning, and spatial reconstruction and generation
- spatial intelligence in embodied systems, virtual realities, geo-spatial systems, biomedicine and natural science, and assistance
- benchmarks and datasets that evaluate any of the above

Out-of-scope: work that uses spatial terms only as vocabulary, and general-purpose models without a spatial component.

---

## How to submit

1. **Open an issue first** (recommended) if you are unsure about scope or placement.
2. **Fork** the repository and create a branch from `main`: `add/<short-paper-slug>`.
3. **Add your entry** to the subsection that matches the handbook section; each heading carries its section number in the handbook (see below).
4. **Open a pull request** and fill in the template.

One paper per pull request is preferred, unless the papers form an obvious cluster (a method and its benchmark, for example).

---

## Entry format

```markdown
- [**Paper Title**](paper-url) [![Paper](https://img.shields.io/badge/VENUE-COLOR)](paper-url) [![Star](https://img.shields.io/github/stars/USER/REPO.svg?style=social&label=Star)](https://github.com/USER/REPO) <!-- MM-YY -->
```

Rules:

- **Title** is wrapped in `[**...**]` and links to the paper itself: the arXiv abstract page when there is one, otherwise the publisher page.
- **Venue badge** uses the palette below. A preprint without a venue uses `arXiv-b22222`.
- **Code badge** is included only for the repository released by the authors. Third-party reimplementations are not listed.
- **Trailing comment** `<!-- MM-YY -->` records the month and year of first public release and is used for sorting.

Example:

```markdown
- [**Depth Anything: Unleashing the Power of Large-Scale Unlabeled Data**](https://arxiv.org/abs/2401.10891) [![Paper](https://img.shields.io/badge/CVPR-8A2BE2)](https://arxiv.org/abs/2401.10891) [![Star](https://img.shields.io/github/stars/LiheYoung/Depth-Anything.svg?style=social&label=Star)](https://github.com/LiheYoung/Depth-Anything) <!-- 01-24 -->
```

Entries are grouped by year, newest first, under a bold year label such as `**2025**`. Place a new entry at the top of its year.

---

## Where does my paper go?

| If the paper ... | Add to |
|---|---|
| Introduces a benchmark for spatial reasoning | The matching table under **7.5. Spatial Reasoning Benchmarks** |
| Studies how space was represented in an earlier era | The matching era table under **1.2. Historical Evolution and Milestones** |
| Proposes a representation or an alignment method | The matching section of **Part II · Spatial-aware Representation** |
| Addresses detection, depth, pose, structure, motion, or grounding | The matching section of **6. Spatial Perception** |
| Reasons over space with symbolic, learned, or foundation-model methods | The matching section of **7. Spatial Reasoning** |
| Generates images, 3D content, video, motion, 4D content, or worlds | The matching section of **8. Spatial Reconstruction and Generation** |
| Builds a system for robots, vehicles, cities, hospitals, or homes | The matching section of **Part IV · Applications** |
| Addresses an open question of Part V | The matching section of **Part V · Discussions and Futures** |

---

## Venue colors

Use these badge colors so that the page stays visually consistent. To add a venue, use the conference or journal abbreviation with a reasonable hex color and list it here in the same pull request.

| Venue | Badge | Color |
|---|---|---|
| arXiv | `arXiv-b22222` | `#b22222` |
| CVPR | `CVPR-8A2BE2` | `#8A2BE2` |
| ICCV | `ICCV-00CED1` | `#00CED1` |
| ECCV | `ECCV-1e90ff` | `#1e90ff` |
| WACV | `WACV-6a5acd` | `#6a5acd` |
| NeurIPS | `NeurIPS-CD5C5C` | `#CD5C5C` |
| ICLR | `ICLR-355C7D` | `#355C7D` |
| ICML | `ICML-FF7F50` | `#FF7F50` |
| AAAI | `AAAI-c71585` | `#c71585` |
| IJCAI | `IJCAI-228b22` | `#228b22` |
| ACL | `ACL-191970` | `#191970` |
| EMNLP | `EMNLP-191970` | `#191970` |
| NAACL | `NAACL-191970` | `#191970` |
| TACL | `TACL-191970` | `#191970` |
| ACMMM | `ACMMM-FFD700` | `#FFD700` |
| TMLR | `TMLR-FFA07A` | `#FFA07A` |
| ICASSP | `ICASSP-FFC0CB` | `#FFC0CB` |
| Interspeech | `Interspeech-FFC0CB` | `#FFC0CB` |
| ICRA | `ICRA-3CB371` | `#3CB371` |
| IROS | `IROS-20B2AA` | `#20B2AA` |
| RSS | `RSS-2E8B57` | `#2E8B57` |
| CoRL | `CoRL-4682B4` | `#4682B4` |
| IJRR | `IJRR-6B8E23` | `#6B8E23` |
| TPAMI | `TPAMI-BC8F8F` | `#BC8F8F` |
| IJCV | `IJCV-9370DB` | `#9370DB` |
| TOG | `TOG-DAA520` | `#DAA520` |
| SIGGRAPH | `SIGGRAPH-DAA520` | `#DAA520` |
| TVCG | `TVCG-DAA520` | `#DAA520` |
| 3DV | `3DV-4169E1` | `#4169E1` |
| BMVC | `BMVC-708090` | `#708090` |
| MICCAI | `MICCAI-B22222` | `#B22222` |
| MedIA | `MedIA-B22222` | `#B22222` |
| TMI | `TMI-B22222` | `#B22222` |
| Nature | `Nature-2F4F4F` | `#2F4F4F` |
| TGRS | `TGRS-2E8B57` | `#2E8B57` |
| JSTARS | `JSTARS-2E8B57` | `#2E8B57` |
| Other conferences | `SHORTNAME-2F4F4F` | `#2F4F4F` |
| Other journals | `Journal-808080` | `#808080` |

---

## Checklist before opening a pull request

- [ ] The paper is in scope and not already listed.
- [ ] The entry follows the format above and the badges render correctly.
- [ ] Every link resolves, and the paper link is the paper itself rather than a search page.
- [ ] The year placement and the `<!-- MM-YY -->` comment match the first public release.
- [ ] The code badge links to the authors' own repository.
- [ ] No unrelated parts of the README were changed.

---

## Style

- Use `-` for list bullets.
- Keep entries on a single line and do not break long titles.
- Do not add commentary to an entry. Descriptions belong to the paper.
