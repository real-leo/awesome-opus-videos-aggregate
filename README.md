# Opus 5.5 Videos Hub

[中文说明](#中文--chinese) · [Sources](sources.md) · [By category](by-category.md) · [Prompts index](prompts.md) · [Data](data/aggregated.json)

**A bilingual discovery hub** that aggregates and deduplicates four community lists of videos people made with [Claude Opus 5.5](https://www.anthropic.com/) (code-rendered animation, explainers, product films, 3D, games, and more).

> Not affiliated with Anthropic. Original videos and prompts belong to their creators. This repo **summarizes and links out**—it does not republish long prompt transcripts or copyrighted footage.

## Snapshot (2026-09-28, Asia/Singapore)

| Metric | Count |
|---|---:|
| **Unique items after dedupe** | **846** |
| With original post URL | 834 |
| Flagged with a public prompt | 430 |
| Appearing in 2+ source repos | 61 |

### Source repos (credit them!)

| Repo | ★ | Indexed | License | What it’s best for |
|---|---:|---:|---|---|
| [athemeroy/awesome-opus-5-5-videos](https://github.com/athemeroy/awesome-opus-5-5-videos) | 282 | 168 reviewed | CC-BY-4.0 | Research corpus, production paths, evidence frames, stats |
| [joeseesun/opus-video-prompts](https://github.com/joeseesun/opus-video-prompts) | 74 | 54 cases + 18 prompts | — | Copy-ready prompts, CN/EN how-to |
| [yihui-dev/awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos) | 538 | 389 | — | Largest prompt set + [Skillry](https://skillry.dev/ai-videos/opus-5-5) remakes |
| [chuspeeism/awesome-opus-5-5-videos](https://github.com/chuspeeism/awesome-opus-5-5-videos) | 76 | 300 | MIT | CN categorized gallery with in-README playback |

Details: [`sources.md`](sources.md).

## Categories (deduped)

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

Opus 5.5 does **not** emit MP4 bytes. Creators typically ask it to **write rendering code** (Canvas, SVG/GSAP, Three.js, Remotion, Manim, p5.js, Blender scripts, …), then capture frames (Playwright/headless Chrome) and mux with FFmpeg. Some pipelines instead **direct external video models** (Seedance, Runway, Higgsfield, …) or **edit supplied footage**. Frames alone cannot prove the path—see athemeroy’s [seven production paths](https://github.com/athemeroy/awesome-opus-5-5-videos#seven-production-paths-with-frames).

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

- **athemeroy** — methodology, Hypit frame sampling, domain×style atlas, color modes, engagement notes. Best when you care *how* a video was made.
- **joeseesun** — bilingual prompt playbook; 18 paste-ready prompt files + technique tips. Best for *getting started*.
- **yihui-dev** — scale (389 prompts) and side-by-side remakes on Skillry. Best for *browsing & remixing*.
- **chuspeeism** — Chinese categorization + GitHub-hosted playable embeds. Best for *CN readers / in-browser watch*.

## Files in this hub

```
README.md           # this page (EN + ZH)
sources.md          # credits, licenses, overlap stats
by-category.md      # deduped tables by category
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

**Opus 5.5 视频聚合站**：把四个社区仓库里的案例与提示词**去重汇总**，方便中英读者发现作品并回链到原帖/原仓库。

| 指标 | 数量 |
|---|---:|
| 去重后唯一条目 | **846** |
| 有原帖链接 | 834 |
| 标有公开提示词 | 430 |
| 出现在 2 个及以上源仓库 | 61 |

**四个来源（请给他们点星）：**

1. [athemeroy/awesome-opus-5-5-videos](https://github.com/athemeroy/awesome-opus-5-5-videos) — 研究型语料、制作路径与证据帧（168）
2. [joeseesun/opus-video-prompts](https://github.com/joeseesun/opus-video-prompts) — 可复制提示词与上手指南（54 案例 + 18 提示词）
3. [yihui-dev/awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos) — 最大提示词库 + Skillry 复刻（389）
4. [chuspeeism/awesome-opus-5-5-videos](https://github.com/chuspeeism/awesome-opus-5-5-videos) — 中文分类图鉴，README 内可播放（300）

**本站不粘贴长提示词全文或视频字幕**；请在 [`prompts.md`](prompts.md) 看短摘要并跳转到源文件。分类浏览见 [`by-category.md`](by-category.md)。

---

Maintained as a discovery index. Corrections and removals: open an issue. Snapshot built 2026-09-28.
