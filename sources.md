# Sources / 资料来源

This hub **aggregates and summarizes** four community repositories of Claude Opus 5.5 video cases and prompts. It does **not** replace them—always prefer the original repos for full prompts, frames, and methodology.

本仓库**汇总并提炼**四个社区仓库中的 Claude Opus 5.5 视频案例与提示词。它**不能替代**原仓库——完整提示词、帧证据与方法论请回原仓库查看。

## Source repos

Star counts refreshed **2026-10-13** (Asia/Singapore). “At merge” = figures used in the 2026-09-28 dedupe.

| Source | Stars | Items (live) | At merge | License | Specialty |
|---|---:|---|---|---|---|
| [athemeroy/awesome-claude-5-5-videos](https://github.com/athemeroy/awesome-claude-5-5-videos) (renamed from `awesome-opus-5-5-videos`) | 531 | 424 source posts (301 Opus; also Sonnet/Haiku/Fable) | 168 | CC-BY-4.0 | Research-grade corpus: production-path labels, frame evidence, domain×style atlas, color study, statistics. Multi-model since rename. |
| [joeseesun/opus-video-prompts](https://github.com/joeseesun/opus-video-prompts) | 304 | 54 cases + 18 prompt files | 54 + 18 | No license file | Copy-ready prompts + public cases; bilingual CN/EN; practical how-to. |
| [yihui-dev/awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos) | 4750 | 853 files under `prompts/` | 389 | MIT | Largest prompt library with Skillry live remakes; categories: motion, explainers, 3D, games. |
| [chuspeeism/awesome-opus-5-5-videos](https://github.com/chuspeeism/awesome-opus-5-5-videos) | 101 | 300 | 300 | See repo | CN-first categorized gallery with GitHub-hosted playable videos, author/post links, per-case notes. |

### Specialization notes / 各源侧重

#### [athemeroy/awesome-claude-5-5-videos](https://github.com/athemeroy/awesome-claude-5-5-videos)

- **EN:** Research-grade corpus with production-path labels, frame evidence, domain×style atlas, color study, and statistics. Expanded beyond Opus-only after the rename.
- **中文:** 研究型语料：制作路径标注、帧证据、领域×风格图谱、色彩研究与统计。更名后覆盖多模型案例。

#### [joeseesun/opus-video-prompts](https://github.com/joeseesun/opus-video-prompts)

- **EN:** Copy-ready prompts (18 full prompt files) + 54 public cases; bilingual CN/EN; practical how-to and technique routes.
- **中文:** 可直接复制的提示词（18 份完整文件）+ 54 个公开案例；中英双语；偏实操上手与技术路线。

#### [yihui-dev/awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos)

- **EN:** Largest prompt library (853 as of 2026-10-13) with Skillry live remakes; categories: motion, explainers, 3D, games.
- **中文:** 最大提示词库（2026-10-13 约 853 条），配合 Skillry 在线复刻对照；分类：动效、讲解、3D、游戏。

#### [chuspeeism/awesome-opus-5-5-videos](https://github.com/chuspeeism/awesome-opus-5-5-videos)

- **EN:** CN-first categorized gallery (300) with GitHub-hosted playable videos, author/post links, per-case notes.
- **中文:** 中文友好分类图鉴（300），GitHub 内嵌可播放视频、作者与原帖链接、逐案说明。

## Overlap / 去重说明

Deduplication key: X/Twitter `status` ID when present, else normalized URL, else title+author.

| Metric | Count |
|---|---:|
| Unique items after merge (2026-09-28) | 846 |
| Appearing in 2+ sources | 61 |
| With original post URL | 834 |
| Flagged as having a public prompt | 430 |

Raw per-source counts **at merge**: athemeroy 168 + joeseesun 54(+18 prompts) + yihui-dev 389 + chuspeeism 300. Many of the same viral posts appear in multiple lists.

**Not yet re-merged:** growth in yihui-dev (→853) and athemeroy (→424 posts), plus the related repos below. The tables in `by-category.md` / `data/` remain the 2026-09-28 snapshot.

## Related lists, skills & tools (2026-10-13)

Linked from the README for discovery; **not** part of the 846-item dedupe.

### Lists

- [zhuyansen/awesome-opus-5.5-video](https://github.com/zhuyansen/awesome-opus-5.5-video) — 1496 high-view works; 166★
- [opusvideo/awesome-claude-video](https://github.com/opusvideo/awesome-claude-video) — curated + implementation guides; 196★
- [xianyu110/awesome-claude-opus-5.5](https://github.com/xianyu110/awesome-claude-opus-5.5) — 292 selected / 1019 full list; 45★
- [LeaddeOpenLab/awesome-opus-5-5-video-prompts](https://github.com/LeaddeOpenLab/awesome-opus-5-5-video-prompts) — 601 prompts; 27★
- [Li-Evan/awesome-opus-5.5-video-prompts](https://github.com/Li-Evan/awesome-opus-5.5-video-prompts) — 334 verbatim prompts; 14★
- [HiAPIAI/awesome-opus-5-5-video-styles](https://github.com/HiAPIAI/awesome-opus-5-5-video-styles) — 425 prompts × 12 styles; 13★
- [X-RayLuan/awesome-opus-5-5-video-prompts](https://github.com/X-RayLuan/awesome-opus-5-5-video-prompts) — 83 demos; 8★

### Skills / plugins / tools

- [lemomo-ai/lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) — 43 film styles; 2127★
- [Vincentwei1021/mg-styles-15](https://github.com/Vincentwei1021/mg-styles-15) — 15 motion styles; 748★
- [zhuyansen/awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills) — ~180 agent video skills; 589★
- [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) — CN motion/口播 Skill; 270★
- [AbubakrChan/product-launch-motion](https://github.com/AbubakrChan/product-launch-motion) — product launch skill; 206★
- [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) — painted + kinetic skills; 166★
- [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) — music→MG plugin; 151★
- [Kianzzz/xilo-opus-video](https://github.com/Kianzzz/xilo-opus-video) — plan→render skill; 74★
- [JohnHeibel/PDoomVideo](https://github.com/JohnHeibel/PDoomVideo) — P(doom) MV source; 2071★
- [diggerhq/shipvideo](https://github.com/diggerhq/shipvideo) — URL/prompt→MP4 tool; 343★

## Attribution / 署名

- Original videos, prompts, and posts belong to their creators.
- Curated annotations belong to the respective source repositories and their licenses.
- This hub’s original English/Chinese writing and the deduped index are offered for discovery; link out rather than republishing long prompt bodies or transcripts.

Deduped snapshot: 2026-09-28. Related-links + source stats refresh: 2026-10-13 (Asia/Singapore).
