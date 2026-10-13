# Opus 5.5 Videos Hub

[中文说明](#中文--chinese) · [Sources](sources.md) · [By category](by-category.md) · [Prompts index](prompts.md) · [Data](data/aggregated.json)

**A bilingual discovery hub** that aggregates and deduplicates four community lists of videos people made with [Claude Opus 5.5](https://www.anthropic.com/) (code-rendered animation, explainers, product films, 3D, games, and more). This page also points to **newer related lists, skills, and tools** found after the initial merge.

> Not affiliated with Anthropic. Original videos and prompts belong to their creators. This repo **summarizes and links out**—it does not republish long prompt transcripts or copyrighted footage.

## Snapshot

| Metric | Count | As of |
|---|---:|---|
| **Unique items after dedupe** (four original sources) | **846** | 2026-09-28 |
| With original post URL | 834 | 2026-09-28 |
| Flagged with a public prompt | 430 | 2026-09-28 |
| Appearing in 2+ source repos | 61 | 2026-09-28 |
| Related lists / skills / tools linked below | 14 | **2026-10-13** |

The deduped tables in [`by-category.md`](by-category.md) and [`data/`](data/) are still the **2026-09-28** merge. Primary sources (especially yihui-dev and athemeroy) have grown since then; re-merge is tracked separately. Star counts and “indexed” figures in the source table were refreshed on 2026-10-13.

### Source repos (credit them!)

| Repo | ★ | Indexed (live / at merge) | License | What it’s best for |
|---|---:|---|---|---|
| [athemeroy/awesome-claude-5-5-videos](https://github.com/athemeroy/awesome-claude-5-5-videos) (was `awesome-opus-5-5-videos`) | 531 | **424** source posts (301 Opus) / 168 at merge | CC-BY-4.0 | Research corpus, production paths, evidence frames, multi-model (Opus/Sonnet/Haiku/Fable) |
| [joeseesun/opus-video-prompts](https://github.com/joeseesun/opus-video-prompts) | 304 | 54 cases + 18 prompts | — | Copy-ready prompts, CN/EN how-to |
| [yihui-dev/awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos) | **4750** | **853** prompts / 389 at merge | MIT | Largest prompt set + [Skillry](https://skillry.dev/ai-videos/opus-5-5) remakes |
| [chuspeeism/awesome-opus-5-5-videos](https://github.com/chuspeeism/awesome-opus-5-5-videos) | 101 | 300 | — | CN categorized gallery with in-README playback |

Details: [`sources.md`](sources.md).

## Categories (deduped, 2026-09-28)

| Category | Items |
|---|---:|
| [Motion graphics](by-category.md#motion-graphics) | 326 |
| [Brand / Product](by-category.md#brand-product) | 84 |
| [Education / Explainer](by-category.md#education-explainer) | 119 |
| [Story / Music](by-category.md#story-music) | 85 |
| [3D / Art](by-category.md#3d-art) | 90 |
| [Games / Interactive](by-category.md#games-interactive) | 81 |
| [Source transform](by-category.md#source-transform) | 33 |
| [External video model](by-category.md#external-video-model) | 10 |
| [Other / Collections](by-category.md#other-collections) | 18 |

Browse the full tables in [`by-category.md`](by-category.md). Machine-readable: [`data/aggregated.csv`](data/aggregated.csv).

## How Opus 5.5 “makes video”

Opus 5.5 does **not** emit MP4 bytes. Creators typically ask it to **write rendering code** (Canvas, SVG/GSAP, Three.js, Remotion, Manim, p5.js, Blender scripts, …), then capture frames (Playwright/headless Chrome) and mux with FFmpeg. Some pipelines instead **direct external video models** (Seedance, Runway, Higgsfield, …) or **edit supplied footage**. Frames alone cannot prove the path—see athemeroy’s [seven production paths](https://github.com/athemeroy/awesome-claude-5-5-videos#seven-production-paths-with-frames) (path may move as that repo evolves).

## Quick start

1. Open a case you like in [`by-category.md`](by-category.md) → jump to the **original post**.
2. If a prompt is available, open the linked file in [prompts.md](prompts.md) (or the source repo) and copy from there.
3. Paste into Claude Opus 5.5 (Claude Code / Claude app). Ask for a single HTML (or Remotion) deliverable, then record/export.

Short smoke-test prompts (from joeseesun; full text there):

```text
make a modern slick and punchy video for a modern startup that works on inference
```

```text
做一个动画，快速回顾中华五千年的历史。风格轻松有趣，动画格式为线稿，添加合适的音乐，请务必做到引人入胜
```

## Cross-listed highlights (in 2+ sources)

These posts showed up in multiple curated lists (good signal they’re widely referenced):

| Author | Post | Sources |
|---|---|---|
| @Ror_Fly | [@Ror_Fly Negroni recipe](https://x.com/Ror_Fly/status/2102853258582880547) | athemeroy, chuspeeism, joeseesun, yihui-dev |
| @akokoi1 | [@akokoi1 history](https://x.com/akokoi1/status/2102583898865873225) | athemeroy, chuspeeism, joeseesun |
| @LinearUncle | [@LinearUncle](https://x.com/LinearUncle/status/2103128559174971663) | athemeroy, chuspeeism, yihui-dev |
| @gavinpurcell | [@gavinpurcell Runway MCP 纪录片](https://x.com/gavinpurcell/status/2103304514329854102) | athemeroy, chuspeeism, joeseesun |
| @ajith_io | [@ajith_io 15 秒 motion-design showreel](https://x.com/ajith_io/status/2103449416325890146) | athemeroy, chuspeeism, yihui-dev |
| @kevin_t_ngo | [@kevin_t_ngo](https://x.com/kevin_t_ngo/status/2102437977435893771) | athemeroy, chuspeeism, joeseesun |
| @Michaelzsguo | [@Michaelzsguo](https://x.com/Michaelzsguo/status/2102592355165782312) | athemeroy, chuspeeism, yihui-dev |
| @shfred0 | [@shfred0](https://x.com/shfred0/status/2102495989194236158) | athemeroy, chuspeeism, joeseesun |
| @stephanlivera | [@stephanlivera 15 秒 motion-design showreel](https://x.com/stephanlivera/status/2103315922098470926) | athemeroy, joeseesun, yihui-dev |
| @Voxyz_ai | [@Voxyz_ai](https://x.com/Voxyz_ai/status/2102531681450119426) | athemeroy, chuspeeism, joeseesun |
| @deedydas | [@deedydas](https://x.com/deedydas/status/2102787937482252537) | athemeroy, joeseesun, yihui-dev |
| @donaldjewkes | [@donaldjewkes](https://x.com/donaldjewkes/status/2102801274173587569) | athemeroy, chuspeeism, joeseesun |
| @twoclipping | [@twoclipping Hooklab 广告](https://x.com/twoclipping/status/2102554209166000267) | athemeroy, chuspeeism, yihui-dev |
| @alexalbert__ | [alexalbert-274839](https://x.com/alexalbert__/status/2102466523164274839) | chuspeeism, yihui-dev |
| @Ann Nguyen | [丙烯画风新西兰游记](https://x.com/ann_nnng/status/2102573127192727704) | chuspeeism, joeseesun |
| @AxtonLiu | [@AxtonLiu 鹈鹕骑车剧场版](https://x.com/AxtonLiu/status/2103119648271290566) | athemeroy, yihui-dev |
| @gandamu_ml | [@gandamu_ml 90 年代风 demoscene](https://x.com/gandamu_ml/status/2102919394775220530) | athemeroy, yihui-dev |
| @Stefan_3D_AI | [@Stefan_3D_AI Blender 双模型对照](https://x.com/Stefan_3D_AI/status/2102471841046786153) | athemeroy, joeseesun |
| @superalesha | [@superalesha LHC](https://x.com/superalesha/status/2102779758408774104) | athemeroy, chuspeeism |
| @Alex Prompter | [30 秒企业讲解片模板](https://x.com/alex_prompter/status/2103499977632997524) | joeseesun, yihui-dev |

## What each source specializes in

- **athemeroy** — methodology, frame sampling, domain×style atlas, color modes, engagement notes; now multi-model (Opus/Sonnet/Haiku/Fable). Best when you care *how* a video was made.
- **joeseesun** — bilingual prompt playbook; 18 paste-ready prompt files + 54 public cases. Best for *getting started*.
- **yihui-dev** — scale (853 prompts as of 2026-10-13) and side-by-side remakes on Skillry. Best for *browsing & remixing*.
- **chuspeeism** — Chinese categorization + GitHub-hosted playable embeds. Best for *CN readers / in-browser watch*.

## Related lists, skills & tools (added 2026-10-13)

Not yet folded into the 846-item dedupe. Star counts as of 2026-10-13 (Asia/Singapore). Descriptions paraphrased from each project’s own README.

### More community lists

| Repo | ★ | Notes |
|---|---:|---|
| [zhuyansen/awesome-opus-5.5-video](https://github.com/zhuyansen/awesome-opus-5.5-video) | 166 | **1496** high-view works (Opus/Sonnet/Haiku/Fable); 381 with a prompt; EN/ZH + [online browser](https://jasonzhu.ai/en/prompts/claude-opus-5-5) |
| [opusvideo/awesome-claude-video](https://github.com/opusvideo/awesome-claude-video) | 196 | Curated demos with posts, prompts, workflows; 59 cases in `cases.json`; implementation guides |
| [xianyu110/awesome-claude-opus-5.5](https://github.com/xianyu110/awesome-claude-opus-5.5) | 45 | **292** hand-picked from **1019** X posts; [Skilloop](https://skilloop.dev/zh/ai-video/opus-5-5) gallery |
| [LeaddeOpenLab/awesome-opus-5-5-video-prompts](https://github.com/LeaddeOpenLab/awesome-opus-5-5-video-prompts) | 27 | **601** prompts by use case; previews + [site](https://leaddeopenlab.github.io/awesome-opus-5-5-video-prompts/) |
| [Li-Evan/awesome-opus-5.5-video-prompts](https://github.com/Li-Evan/awesome-opus-5.5-video-prompts) | 14 | **334** verbatim creator prompts; EN/ZH; CC-BY-4.0 |
| [HiAPIAI/awesome-opus-5-5-video-styles](https://github.com/HiAPIAI/awesome-opus-5-5-video-styles) | 13 | **425** prompts sorted into **12** visual styles + style recipes; CC-BY-4.0 |
| [X-RayLuan/awesome-opus-5-5-video-prompts](https://github.com/X-RayLuan/awesome-opus-5-5-video-prompts) | 8 | **83** demos with verbatim prompts (EN+ZH); MIT |

### Skills & plugins (make video with Claude Code / agents)

| Repo | ★ | Notes |
|---|---:|---|
| [lemomo-ai/lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) | 2127 | Claude Code skill: **43** film styles, each with a code-only demo film (incl. OPUSCAR 98); MIT |
| [Vincentwei1021/mg-styles-15](https://github.com/Vincentwei1021/mg-styles-15) | 748 | **15** motion-design styles: watch films, copy prompts, read full source; MIT |
| [zhuyansen/awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills) | 589 | Meta-list of **~180** open video skills/toolkits for coding agents, security-graded; EN/ZH |
| [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | 270 | CN motion/口播 templates + Skill for Codex / Claude Code; MIT |
| [AbubakrChan/product-launch-motion](https://github.com/AbubakrChan/product-launch-motion) | 206 | Claude Code skill for continuous-shot product launch reels (60 fps motion blur); MIT |
| [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) | 166 | Skills for painted animation + kinetic-typography reels (code-only frames/music) |
| [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) | 151 | Plugin: motion-graphics video from a music track + prompt; MIT |
| [Kianzzz/xilo-opus-video](https://github.com/Kianzzz/xilo-opus-video) | 74 | Skill: propose 3 plans → preview → frame render (Canvas/WebGL/Three.js/Remotion/HyperFrames); MIT |

### Notable demos & tools

| Repo | ★ | Notes |
|---|---:|---|
| [JohnHeibel/PDoomVideo](https://github.com/JohnHeibel/PDoomVideo) | 2071 | Source for the viral *I’m Upping My P(doom)* Claude Opus 5.5 music video |
| [diggerhq/shipvideo](https://github.com/diggerhq/shipvideo) | 343 | Paste a URL or prompt → Opus 5.5 writes HTML → OpenComputer agent renders MP4 ([launchvideo.io](https://launchvideo.io)) |

## Files in this hub

```
README.md           # this page (EN + ZH)
sources.md          # credits, licenses, overlap stats, related links
by-category.md      # deduped tables by category (2026-09-28 snapshot)
prompts.md          # short excerpts + links (no long transcripts)
data/aggregated.json
data/aggregated.csv
LICENSE
```

## License & copyright

- **This hub’s original text and deduped index:** [CC BY 4.0](LICENSE) (attribution appreciated: link back here and to the four sources).
- **Videos, music, prompts, and posts:** remain with their creators / platforms. Do not treat this repo as a rights clearance.
- **Source-repo annotations:** follow each source’s own license (athemeroy is CC BY 4.0; check the others before reuse).

## 中文 / Chinese

**Opus 5.5 视频聚合站**：把四个社区仓库里的案例与提示词**去重汇总**，方便中英读者发现作品并回链到原帖/原仓库。2026-10-13 起额外收录一批**相关列表 / Skill / 工具**链接（尚未并入下方 846 条去重表）。

| 指标 | 数量 | 时间 |
|---|---:|---|
| 去重后唯一条目（四源合并） | **846** | 2026-09-28 |
| 有原帖链接 | 834 | 2026-09-28 |
| 标有公开提示词 | 430 | 2026-09-28 |
| 出现在 2 个及以上源仓库 | 61 | 2026-09-28 |
| 下方相关仓库链接 | 14 | **2026-10-13** |

**四个来源（请给他们点星；★ 与规模为 2026-10-13 刷新）：**

1. [athemeroy/awesome-claude-5-5-videos](https://github.com/athemeroy/awesome-claude-5-5-videos)（原名 `awesome-opus-5-5-videos`）— 研究型语料、制作路径与证据帧（现约 424 帖 / 合并时 168）
2. [joeseesun/opus-video-prompts](https://github.com/joeseesun/opus-video-prompts) — 可复制提示词与上手指南（54 案例 + 18 提示词）
3. [yihui-dev/awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos) — 最大提示词库（现约 **853**）+ Skillry 复刻
4. [chuspeeism/awesome-opus-5-5-videos](https://github.com/chuspeeism/awesome-opus-5-5-videos) — 中文分类图鉴，README 内可播放（300）

**值得一看的新列表 / Skill（详见英文 Related 表格）：** [zhuyansen/awesome-opus-5.5-video](https://github.com/zhuyansen/awesome-opus-5.5-video)、[lemomo-ai/lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar)、[Vincentwei1021/mg-styles-15](https://github.com/Vincentwei1021/mg-styles-15)、[zhuyansen/awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills)、[diggerhq/shipvideo](https://github.com/diggerhq/shipvideo)、[JohnHeibel/PDoomVideo](https://github.com/JohnHeibel/PDoomVideo) 等。

**本站不粘贴长提示词全文或视频字幕**；请在 [`prompts.md`](prompts.md) 看短摘要并跳转到源文件。分类浏览见 [`by-category.md`](by-category.md)。

---

Maintained as a discovery index. Corrections and removals: open an issue. Deduped snapshot built 2026-09-28; related-links pass 2026-10-13 (Asia/Singapore).
