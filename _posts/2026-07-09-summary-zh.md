---
layout: default
title: "Horizon Summary: 2026-07-09 (ZH)"
date: 2026-07-09
lang: zh
---

> From 38 items, 16 important content pieces were selected

---

1. [OpenAI 发布 GPT-5.6，改进意图理解](#item-1) ⭐️ 9.0/10
2. [Meta 发布 Muse Spark 1.1 智能体模型](#item-2) ⭐️ 9.0/10
3. [TypeScript 7.0 正式发布：Go 重写带来最高 12 倍速度提升](#item-3) ⭐️ 9.0/10
4. [欧盟议会通过程序伎俩批准聊天控制 1.0](#item-4) ⭐️ 8.0/10
5. [腾讯 Hy3：紧凑 MoE 模型在 OpenRouter 上免费](#item-5) ⭐️ 8.0/10
6. [GLM 5.2 在记账任务上接近人类准确率](#item-6) ⭐️ 8.0/10
7. [用 Rust 重写 PostgreSQL，100%通过回归测试](#item-7) ⭐️ 8.0/10
8. [大三本科生实现投机解码 7.92 倍加速](#item-8) ⭐️ 8.0/10
9. [蚂蚁灵波开源 LingBot-Video：全球首个 MoE 具身视频基模](#item-9) ⭐️ 8.0/10
10. [国家超算互联网核心节点上线](#item-10) ⭐️ 8.0/10
11. [OpenAI 与美国战争部修订合同，禁止 AI 监控公民](#item-11) ⭐️ 8.0/10
12. [在 32GB 内存笔记本上运行 GLM 5.2 的 Colibrì项目](#item-12) ⭐️ 7.0/10
13. [IERS 确认 2026 年底不增加闰秒](#item-13) ⭐️ 7.0/10
14. [美国陆军脆弱后勤或致未来战争失败](#item-14) ⭐️ 7.0/10
15. [内部服务 TLS：首选 DNS-01 而非 Split-Horizon DNS](#item-15) ⭐️ 7.0/10
16. [大疆 EV50 垂直起降无人机飞越珠峰达 8861 米](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.6，改进意图理解](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI 发布了 GPT-5.6，其意图理解能力得到增强，并在 ARC-AGI-3 基准测试中取得了 7.8%的最新最高分。 这标志着向更具能力、更自主的 AI 代理迈出了重要一步，因为 ARC-AGI-3 测试的是交互式推理和适应能力，超越了静态基准测试。 GPT-5.6 能够推断用户意图而无需明确的逐步指令，并能保持原始图像尺寸，但在 ARC-AGI-3 上的 7.8%分数仍远低于人类表现。

hackernews · logickkk1 · Jul 9, 17:04 · [社区讨论](https://news.ycombinator.com/item?id=48849066)

**背景**: ARC-AGI-3 是一个交互式基准测试，评估 AI 代理在需要探索和规划的新颖抽象环境中的表现，不同于之前的静态基准。GPT-5.6 是首个在此基准上取得分数的已验证前沿模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arcprize.org/leaderboard">ARC-AGI-3 Leaderboard - ARC Prize</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence ARC-AGI-3 Leaderboard - ARC Prize ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence ARC-AGI-3: The New Interactive Reasoning Benchmark - DataCamp GitHub - arcprize/arc-agi-3-benchmarking GPT 5.6 Sol Tops ARC-AGI 3 With 7.8%, Becomes First Model To ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人赞赏关于意图理解的开发者提示，也有人批评较低的 ARC-AGI-3 分数，并指出 OpenAI 在比较中排除了一个竞争对手模型。还有关于选择代码编辑器（如 Claude Code 和 GitHub Copilot）的讨论。

**标签**: `#AI`, `#LLM`, `#GPT`, `#OpenAI`, `#frontier model`

---

<a id="item-2"></a>
## [Meta 发布 Muse Spark 1.1 智能体模型](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 9.0/10

Meta 宣布发布 Muse Spark 1.1，这是一个专为智能体编码设计的多模态 AI 模型，通过按使用付费的 API 提供，并发布了声称在 Terminal-Bench 2.1 上表现优异的评估报告。 此次发布标志着 Meta 直接进入由 OpenAI 和 Anthropic 主导的竞争激烈的智能体 AI 市场，但评估方法论引发了社区重大讨论，可能影响该模型的可信度和采用率。 Muse Spark 1.1 的定价为每百万输入 token 1.25 美元，每百万输出 token 4.5 美元，缓存输入为 0.15 美元。社区批评者指出，评估使用了多达 6 个 CPU 核心和 8GB 内存，这可能超出官方任务限制，从而使结果无效。

hackernews · ot · Jul 9, 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48846184)

**背景**: 智能体 AI 模型是能够自主执行多步任务、使用外部工具并与环境交互的 AI 系统。Meta 的 Muse Spark 系列基于早期的开源权重模型构建，1.1 版本引入了商业 API，旨在与 OpenAI 的 GPT-5 和 Anthropic 的 Claude Opus 等模型竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/09/meta-enters-the-crowded-ai-coding-battle-with-muse-spark-1-1/">Meta enters the crowded AI coding battle with Muse Spark 1.1</a></li>
<li><a href="https://kingy.ai/blog/muse-spark-1-1-benchmarks-specs-evals/">Muse Spark 1.1 Benchmarks, Specs, Evals, Strengths & Weaknesses</a></li>
<li><a href="https://officechai.com/ai/muse-spark-1-1-benchmarks/">Meta Announces Muse Spark 1.1, Beats Claude Opus 4.8 And GPT 5.5 On ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员对评估的严谨性表示担忧：用户 GodelNumbering 指出，Terminal-Bench 2.1 评估中使用的资源限制（6 个 CPU 核心、8GB 内存）超出了官方限制，可能使结果无效。Simonw 分享了实际使用技巧，而 jacobgold 认为 Meta 可以通过将编程模型商品化来扮演“搅局者”角色。Tiberium 批评定价过高。

**标签**: `#Meta AI`, `#Muse Spark`, `#agentic model`, `#AI evaluation`, `#LLM`

---

<a id="item-3"></a>
## [TypeScript 7.0 正式发布：Go 重写带来最高 12 倍速度提升](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软正式发布 TypeScript 7.0，这是用 Go 语言重写的原生版本，完整构建速度可比旧版快 8 到 12 倍，并支持共享内存多线程。用户现可通过 npm 直接安装，主流编辑器亦可通过 LSP 支持新语言服务器。 这一重大性能提升直接影响数百万 TypeScript 开发者，大幅缩短编译时间，实现更快的开发迭代。用 Go 重写还为未来进一步的性能改进和更好的并行性铺平了道路。 新版本引入 `--checkers` 与 `--builders` 参数以自定义并行度，并提供兼容包实现与 TypeScript 6 并存。但 Vue、Svelte 等嵌入式语言工具链因 API 尚未就绪，目前仍需使用旧版本。

telegram · zaihuapd · Jul 9, 04:01

**背景**: TypeScript 是 JavaScript 的类型超集，编译为纯 JavaScript。之前的版本是用 TypeScript 本身编写的，对于大型代码库可能会变慢。用 Go 重写利用了 Go 内置的并发支持来并行化构建过程，显著加快编译速度。语言服务器协议 (LSP) 标准化了编辑器与语言服务器之间的通信，支持自动补全、跳转到定义等功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol - Wikipedia</a></li>
<li><a href="https://microsoft.github.io/language-server-protocol/">Official page for Language Server Protocol</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automatic_parallelization">Automatic parallelization - Wikipedia</a></li>

</ul>
</details>

**标签**: `#TypeScript`, `#Microsoft`, `#Go`, `#compiler`, `#performance`

---

<a id="item-4"></a>
## [欧盟议会通过程序伎俩批准聊天控制 1.0](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

2026 年 7 月 9 日，欧洲议会通过了聊天控制 1.0 法案，允许在 2028 年前无需搜查令大规模扫描私人信息，尽管投票的议员多数反对（314 票反对，276 票赞成）；否决动议未达到所需的 361 票绝对多数。 该法律削弱了 4.5 亿欧盟公民的数字隐私和加密，为大规模监控树立先例，可能侵蚀基本权利和对数字通信的信任。 该法律通过程序性手段通过：投票安排在暑假前的最后一个会议日，需要全体议员的绝对多数才能否决，而不仅仅是出席议员。该法允许扫描 Instagram、Discord、Gmail 和 iCloud 等平台，但公开社交媒体帖子和云存储此前已可扫描。

hackernews · rapnie · Jul 9, 11:03 · [社区讨论](https://news.ycombinator.com/item?id=48843923)

**背景**: 聊天控制是一项拟议的欧盟法规，旨在通过扫描私人消息打击儿童性虐待材料（CSAM）。批评者认为这构成大规模监控，且当前技术无法避免高误报率。第一版聊天控制 1.0 在 2026 年 3 月两次被否决，后通过程序性手段通过。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/">EU Parliament greenlights Chat Control 1.0 – Breyer: "Our children lose out"</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.techtimes.com/articles/320010/20260709/eu-parliament-passes-chat-control-default-314-meps-couldnt-block-scanning-law.htm">EU Parliament Passes Chat Control by Default: 314 MEPs Couldn't Block Scanning Law</a></li>

</ul>
</details>

**社区讨论**: 评论者对不民主的进程表示愤怒，称其为‘愚蠢的议会伎俩’，并指责欧盟走向极权。他们指出该法律在多数人反对的情况下通过，破坏了欧盟项目的合法性。

**标签**: `#privacy`, `#EU`, `#surveillance`, `#encryption`, `#legislation`

---

<a id="item-5"></a>
## [腾讯 Hy3：紧凑 MoE 模型在 OpenRouter 上免费](https://hy.tencent.com/research/hy3) ⭐️ 8.0/10

腾讯的 Hy3 是一款 295B 参数的混合专家（MoE）模型，仅有 21B 活跃参数，现已在 OpenRouter 上免费提供（至 2026 年 7 月 21 日），在性能上超越同类模型，可媲美更大规模的开源模型。 此举让高性能开源模型更易获取，在小中型模型领域挑战 DeepSeek V4 Flash 和 Pro，有助于本地部署和成本敏感型应用场景。 Hy3 采用 MoE 架构，拥有 21B 活跃参数和 3.8B 的 MTP 层参数，在多项基准测试中表现优异。免费服务由 Novita Labs 通过 OpenRouter 提供。

hackernews · andai · Jul 9, 15:27 · [社区讨论](https://news.ycombinator.com/item?id=48847552)

**背景**: 混合专家（MoE）模型每次仅激活一部分参数，从而在保持较大总参数量的同时降低计算成本。Hy3 属于腾讯混元（Hunyuan）模型系列，基于 4 月预览版开发，并融入了来自 50 多个产品的反馈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Tencent-Hunyuan/Hy3">GitHub - Tencent-Hunyuan/Hy3: Hy3 (295B A21B), a leading ...</a></li>
<li><a href="https://www.tencent.com/en-us/articles/2202386.html">Tencent Hunyuan Officially Releases Hy3, Advancing Agent ...</a></li>
<li><a href="https://openrouter.ai/collections/free-models">Free AI Models on OpenRouter</a></li>

</ul>
</details>

**社区讨论**: 社区成员注意到 Hy3 以其规模展现出惊人的能力，并将其与 DeepSeek V4 Flash 相提并论。有人质疑其在 OpenRouter 上的排名可持续性及价格竞争力，另一些人则对本地部署潜力持乐观态度。

**标签**: `#AI`, `#LLM`, `#Tencent`, `#OpenRouter`, `#language model`

---

<a id="item-6"></a>
## [GLM 5.2 在记账任务上接近人类准确率](https://toot-books.pages.dev/blog/glm-5-2-vat-benchmark) ⭐️ 8.0/10

GLM 5.2 在记账基准测试中达到接近人类的准确率，能够执行如匹配发票与银行对账单等任务。 这表明人工智能能够以高可靠性自动化核心财务任务，可能颠覆记账行业并降低企业成本。 基准测试仅评估了记账任务的一个狭窄子集；人类记账员还需处理发票搜索和模糊情况的推理。通过改进对税收法规的获取，模型的错误可以减少。

hackernews · adamkurkiewicz · Jul 9, 18:29 · [社区讨论](https://news.ycombinator.com/item?id=48850414)

**背景**: GLM 5.2 是 Z.AI 开发的开源权重语言模型，专为长周期任务和多模态理解设计。它以极低的成本在设计基准测试中表现出色，性能媲美商业模型。在记账领域，AI 模型正被探索用于自动化重复性的财务数据处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-glm-5-2-open-weight-model">What Is GLM 5.2? The Open-Weight Model Beating GPT 5.5 on Design Benchmarks | MindStudio</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，基准测试的范围比实际记账更窄，且责任问题仍未解决——如果 AI 出错，用户可能承担法律责任。此外，对该初创公司缺乏背景和透明度持怀疑态度。

**标签**: `#AI`, `#GLM`, `#bookkeeping`, `#accuracy`, `#automation`

---

<a id="item-7"></a>
## [用 Rust 重写 PostgreSQL，100%通过回归测试](https://github.com/malisper/pgrust) ⭐️ 8.0/10

一个名为 pgrust 的项目借助大语言模型用 Rust 重写了 PostgreSQL，现已 100%通过 PostgreSQL 的回归测试。 这一成就展示了借助大语言模型重写大型复杂代码库的潜力，但也引发了关于代码审查、可维护性以及开源项目许可证兼容性的重要问题。 该项目从 PostgreSQL 许可证改为 AGPL，其仓库在不到一个月内产生了超过 7100 次提交，大部分由大语言模型生成。作者计划推出新版本，融入更多数据库技术。

hackernews · SweetSoftPillow · Jul 9, 06:18 · [社区讨论](https://news.ycombinator.com/item?id=48841676)

**背景**: PostgreSQL 是一款广泛使用的开源关系型数据库管理系统，已有 30 年历史。用 Rust 重写它可能提升内存安全性和性能，但这是一项艰巨的任务。大语言模型辅助开发是一种新兴方法，AI 模型帮助生成代码，可能加速开发但也带来代码质量和审查方面的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now passing 100% of the Postgres regression tests · GitHub</a></li>
<li><a href="https://malisper.me/pgrust-rebuilding-postgres-in-rust-with-ai/">pgrust: Rebuilding Postgres in Rust with AI - malisper.me</a></li>
<li><a href="https://pgrust.com/">pgrust — postgres, rewritten in rust</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一：作者强调了该项目的实验性质及未来计划，而其他人则对缺乏传统的开发产出（如拉取请求和 Makefile）、审查大语言模型生成的提交的难度，以及许可证从 PostgreSQL 改为 AGPL 可能引发的兼容性问题表示担忧。

**标签**: `#Rust`, `#PostgreSQL`, `#database systems`, `#LLM-assisted development`, `#open source`

---

<a id="item-8"></a>
## [大三本科生实现投机解码 7.92 倍加速](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247902587&idx=3&sn=879066ecce663ab9daba5d73fe2dc27b) ⭐️ 8.0/10

一名大三本科生作为第一作者提出了一种投机解码方法，将大语言模型的推理速度提升了 7.92 倍，并已被 DeepSeek 和阶跃星辰两大 AI 实验室引用。 这一突破显著加速了大语言模型的推理，使其更适用于实时应用。顶级实验室的引用验证了该方法的重要性，并凸显了本科生在 AI 前沿研究中的潜力。 该方法在利用并行草稿生成加速的同时，保持了块内的因果一致性，相比标准自回归解码实现了 7.92 倍加速。它解决了并行草稿的速度优势与块内因果完整性之间的矛盾。

rss · 量子位 · Jul 9, 04:17

**背景**: 投机解码是一种针对自回归大语言模型的推理时优化技术，它使用较小的草稿模型并行生成多个候选 token，再由目标模型并行验证。该技术可以在保持输出质量的同时将延迟降低 2-3 倍。这项新工作通过解决相互等待问题和内部因果一致性，改进了现有方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>
<li><a href="https://arxiv.org/abs/2408.11850">[2408.11850] PEARL: Parallel Speculative Decoding with ...</a></li>

</ul>
</details>

**标签**: `#speculative decoding`, `#LLM inference`, `#acceleration`, `#undergraduate research`, `#AI`

---

<a id="item-9"></a>
## [蚂蚁灵波开源 LingBot-Video：全球首个 MoE 具身视频基模](https://www.qbitai.com/2026/07/446458.html) ⭐️ 8.0/10

蚂蚁灵波开源了 LingBot-Video，这是全球首个基于 MoE 架构的具身视频生成基础模型，总参数 30B，推理时仅激活约 3B。该模型在 RBench 评测基准上取得 0.620 分，超越 Wan2.6、Seedance1.5 Pro 等模型。 这是具身智能和视频生成领域的重要进展，展示了 MoE 在大幅提升效率的同时保持高质量的能力。以 Apache 2.0 许可证开源，使研究者和开发者能够在此基础上用于机器人、仿真和世界模型研究。 该模型在架构（DiT+MoE）、数据（7 万小时具身数据画像引擎，覆盖灵巧操作、机器人移动和第一视角交互）和训练（多维强化学习奖励系统，关注物理合理性和任务完成度）三方面进行了创新。

telegram · zaihuapd · Jul 9, 04:30

**背景**: MoE（混合专家）是一种机器学习技术，将模型分割成多个专门的子网络（专家），由门控网络为每个输入选择激活哪些专家，从而实现更高效的计算。DiT（扩散 Transformer）用 Transformer 主干替代传统扩散模型中的 U-Net，提升了图像和视频生成的可扩展性和质量。具身智能专注于创造能够感知、推理并与物理世界交互的智能体，融合了机器人、计算机视觉和语言等技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2212.09748">[2212.09748] Scalable Diffusion Models with Transformers Diffusion Transformers (DiTs) - GeeksforGeeks Images Scalable Diffusion Models with Transformers Diffusion Transformers Explained: The Beginner’s Guide GitHub - FourierPT/Diffusion-Transformer: Official PyTorch ... Diffusion Transformer (DiT) Models: A Beginner’s Guide</a></li>
<li><a href="https://www.frontiersin.org/journals/robotics-and-ai/articles/10.3389/frobt.2025.1668910/full">Frontiers | A review of embodied intelligence systems: a ...</a></li>

</ul>
</details>

**标签**: `#MoE`, `#具身智能`, `#视频生成`, `#机器人`, `#开源`

---

<a id="item-10"></a>
## [国家超算互联网核心节点上线](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

2026 年 7 月 9 日，国家超算互联网核心节点在郑州正式上线，对外提供超过 10 万卡的国产人工智能算力。 这是国家超算互联网平台接入的最大规模单体国产 AI 算力资源池，将显著增强中国的人工智能发展能力，并减少对外国硬件的依赖。 该核心节点以构建覆盖全国的计算资源统筹调度体系为目标，承担运营管理、资源调度等核心功能，并整合供需对接、产业孵化等综合服务。

telegram · zaihuapd · Jul 9, 07:00

**背景**: 国家超算互联网是由中国科技部主导建设的一体化算力服务平台，连接全国多个超算中心，形成统一的高性能计算网络。该核心节点于 2023 年 10 月在郑州启动建设。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260709A03VDU00">刚刚，国家超算互联网核心节点正式上线_腾讯新闻</a></li>
<li><a href="https://baike.baidu.com/item/国家超算互联网核心节点/63648019">国家超算互联网核心节点_百度百科</a></li>
<li><a href="https://www.jiemian.com/article/14728809.html">国家超算互联网核心节点正式上线|界面新闻 · 快讯</a></li>

</ul>
</details>

**标签**: `#supercomputing`, `#AI`, `#China`, `#computing infrastructure`, `#domestic technology`

---

<a id="item-11"></a>
## [OpenAI 与美国战争部修订合同，禁止 AI 监控公民](https://t.me/zaihuapd/42459) ⭐️ 8.0/10

OpenAI 与美国战争部已同意修订双方的 AI 合作协议，明确禁止将 AI 系统用于对美国公民进行蓄意监控，以及基于商业获取的个人身份信息进行追踪或监测。 此举为政府合同中的 AI 伦理树立了重要先例，回应了公众对大规模监控的担忧，并展示了一家领先 AI 公司的主动措施。它可能影响其他科技公司和政府机构采取类似的限制。 新条款由 OpenAI 首席执行官 Sam Altman 主动提议，以回应 AI 被滥用于监控的担忧。该合同尚未正式签署，而此前 Anthropic 与战争部的类似协议曾因争议而中止。

telegram · zaihuapd · Jul 9, 13:22

**背景**: 美国战争部（又称国防部）负责协调和监督武装力量。OpenAI 以其 GPT 模型闻名，正扩大与政府机构的合作。竞争对手 Anthropic 专注于 AI 安全，此前因其与战争部的合同面临批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/United_States_Department_of_War">United States Department of War - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#government contract`, `#surveillance`, `#OpenAI`, `#policy`

---

<a id="item-12"></a>
## [在 32GB 内存笔记本上运行 GLM 5.2 的 Colibrì项目](https://github.com/JustVugg/colibri) ⭐️ 7.0/10

一位开发者创建了 Colibrì，这是一个轻量级推理引擎，通过 int4 量化和按需从磁盘流式加载专家权重，在仅有 32GB 内存的笔记本电脑上运行了 744B 参数的 GLM 5.2 混合专家模型。 这表明即使是最大的开源 LLM 也可以在消费级硬件上运行，使没有昂贵 GPU 的个人也能使用先进的 AI 能力。这里使用的技术可能为其他 MoE 模型带来类似的优化。 该引擎是一个单一的 C 文件（约 1300 行），无 BLAS、Python 或 GPU 依赖。它通过将约 17B 的密集参数保持在 RAM 中（int4 下约 9.9 GB），并从磁盘流式加载 21,504 个路由专家（约 370 GB）并配有 LRU 缓存，在冷启动时达到 0.1 tok/s。

hackernews · vforno · Jul 9, 08:05 · [社区讨论](https://news.ycombinator.com/item?id=48842459)

**背景**: GLM 5.2 是一个 744B 参数的混合专家（MoE）模型，每个 token 只激活约 40B 参数，因此如果管理得当，可以在有限硬件上运行。Int4 量化将模型权重从 32 位浮点数转换为 4 位整数，大幅降低内存占用，但会牺牲少量精度。帖子中提到的多 token 预测（MTP）和动态稀疏注意力（DSA）是进一步提高吞吐量和长上下文效率的高级技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apxml.com/courses/quantized-llm-deployment/chapter-1-advanced-llm-quantization-fundamentals/low-bit-quantization-techniques">Low-Bit LLM Quantization (INT4, NF4, FP4) - apxml.com</a></li>
<li><a href="https://www.spheron.network/blog/multi-token-prediction-mtp-gpu-cloud-deployment-guide/">Multi-Token Prediction on GPU Cloud: Deploy MTP LLMs for 2-3x ...</a></li>
<li><a href="https://amitray.com/deepseek-sparse-attention-dsa-a-comprehensive-review/">DeepSeek Sparse Attention (DSA): A Comprehensive Review</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了这种黑客精神，但指出 0.1 tok/s 的速度对于交互式使用来说不切实际。一些人提出了替代方案，如基于 mmap 的加载（Cieric）或使用 LRU 卸载到 VRAM（kodablah），还有一位评论者分享了对 GLM 5.2 在昂贵硬件上的类似兴奋，并赞赏了让它在普通机器上运行的努力。

**标签**: `#LLM`, `#quantization`, `#local inference`, `#model optimization`, `#open source`

---

<a id="item-13"></a>
## [IERS 确认 2026 年底不增加闰秒](https://datacenter.iers.org/data/latestVersion/bulletinC.txt) ⭐️ 7.0/10

国际地球自转与参考系统服务（IERS）发布公告 C，确认 2026 年 12 月底不引入闰秒，当前 UTC-TAI 偏移量保持为-37 秒，UTC-GPS 偏移量保持为-18 秒。 这一决定为分布式计算、金融网络和卫星导航等对时间敏感的系统提供了稳定性，否则它们需要精心协调来处理闰秒插入，以往的闰秒曾引发显著的软件问题。 下一个可能引入闰秒的时间是 2027 年 6 月或 12 月，具体取决于地球自转的不可预测性；IERS 监测地球自转，并在 UTC 与 UT1 的差异接近 0.9 秒时宣布闰秒。

hackernews · ChrisArchitect · Jul 9, 14:16 · [社区讨论](https://news.ycombinator.com/item?id=48846281)

**背景**: 协调世界时（UTC）基于国际原子时（TAI），后者利用原子钟提供精确均匀的时间。然而，地球自转（UT1）逐渐减慢，导致原子时与天文时间之间产生漂移。闰秒偶尔被插入，以保持 UTC 与 UT1 的差异在 0.9 秒以内。IERS 是负责决定何时添加闰秒的机构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/International_Earth_Rotation_and_Reference_Systems_Service">International Earth Rotation and Reference Systems Service</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Atomic_Time">International Atomic Time - Wikipedia</a></li>
<li><a href="https://www.timeanddate.com/worldclock/other/tai">Current International Atomic Time — TAI International Atomic Time (TAI) - timeanddate.com International Atomic Time - Wikipedia Glossary - International Atomic Time (TAI) - iers.org International Atomic Time (TAI) | Worldwide Clock TAI Time Calculator - International Atomic Time Converter ... Atomic Time - Navipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对地球自转的不可预测性表示好奇，有人询问地质活动或天气等成因。另一人关注 Unix 时间戳及维护问题。讨论中还包含了幽默评论和技术澄清（如 TAI-GPS 偏移量），体现了既有趣味又有真正技术兴趣的结合。

**标签**: `#leap second`, `#UTC`, `#timekeeping`, `#distributed systems`, `#IERS`

---

<a id="item-14"></a>
## [美国陆军脆弱后勤或致未来战争失败](https://mwi.westpoint.edu/the-glass-backbone-why-the-armys-logistics-will-break-in-the-next-war/) ⭐️ 7.0/10

MWI 发表的一份详细分析认为，美国陆军的后勤系统过度依赖复杂技术，使其成为未来冲突中的关键弱点。 这很重要，因为后勤是军事行动的骨干；如果它崩溃，即使最先进的部队也可能被击败。该分析强调了可能削弱美国军事战备和威慑的系统性风险。 文章指出了全球作战支援系统-陆军（GCSS-Army）和后勤信息仓库（LIW）的单点故障等脆弱性。它警告对手可能利用这些数字依赖来破坏供应链。

hackernews · baud147258 · Jul 9, 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48845442)

**背景**: 美国陆军严重依赖数字后勤系统，如基于 SAP 的 ERP 系统 GCSS-Army 和 LIW 来管理供应链。这些系统容易受到网络攻击，并可能在对抗环境中被打断。诸如费边战略之类的历史例子表明， targeting 后勤可以赢得战争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_Combat_Support_System">Global Combat Support System - Wikipedia</a></li>
<li><a href="https://www.brookings.edu/articles/the-department-of-defenses-digital-logistics-are-under-attack/">The Department of Defense's digital logistics are under ...</a></li>
<li><a href="https://atloa.org/securing-the-backbone-cyber-resilience-in-contested-logistics/">Securing the Backbone: Cyber Resilience in Contested Logistics</a></li>

</ul>
</details>

**社区讨论**: 评论者基本同意该分析，并类比历史上的后勤失败，如对抗汉尼拔的费边战略。一些人讨论了星舰投送等新技术的影响，但另一些人强调遗留系统仍然脆弱。

**标签**: `#logistics`, `#military`, `#defense`, `#technology`, `#analysis`

---

<a id="item-15"></a>
## [内部服务 TLS：首选 DNS-01 而非 Split-Horizon DNS](https://tuxnet.dev/posts/tls-for-internal-services/) ⭐️ 7.0/10

一篇博客文章主张使用 Let's Encrypt 的 DNS-01 ACME 挑战来为内部服务获取 TLS 证书，认为这比 split-horizon DNS 更简单且更易维护。 这一建议可以减少许多管理内部 TLS 的工程师的运维复杂性，避免了维护内部和外部解析的独立 DNS 视图的麻烦。 DNS-01 挑战允许在不将内部服务暴露到互联网的情况下签发证书，并且可以使用通配符证书来缓解对证书透明度日志泄露的担忧。

hackernews · mrl5 · Jul 9, 14:57 · [社区讨论](https://news.ycombinator.com/item?id=48846995)

**背景**: Split-horizon DNS 根据客户端的网络位置（内部与外部）提供不同的 DNS 响应，维护起来可能很复杂。ACME DNS-01 挑战通过放置 TXT 记录来证明域名控制权，从而无需公共 HTTP 访问即可签发证书。Let's Encrypt 是一个广泛使用的证书颁发机构，支持这种挑战类型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://letsencrypt.org/docs/challenge-types/">Challenge Types - Let's Encrypt</a></li>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>

</ul>
</details>

**社区讨论**: 评论者们一致同意 DNS-01 方法，许多人分享了他们使用通配符证书和反向代理的设置。一些人呼应说 split-horizon DNS 带来了不必要的复杂性，而另一些人指出对于家庭实验室，结合 VPN 访问的公共 DNS 已经足够。

**标签**: `#TLS`, `#ACME`, `#DNS`, `#internal services`, `#certificate management`

---

<a id="item-16"></a>
## [大疆 EV50 垂直起降无人机飞越珠峰达 8861 米](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 7.0/10

大疆未发布的 EV50 垂直起降运载无人机在珠峰北坡成功飞至 8861 米，创下全球垂直起降固定翼无人机最高飞行升限纪录。该无人机在北京大学研究人员的 12 天科考任务中搭载了臭氧测量设备。 这一成就展示了大疆在高海拔物流和货物运输方面的能力，可能为极端环境下的无人机运输开辟新应用。同时，它提供了 8000 米以上高海拔区域的大气数据，有助于科学研究。 此次飞行在珠峰北坡进行，EV50 在 12 天内完成 32 次起降，连续爬升 3730 米，返程时剩余 30%电量。大疆表示其研发目标包括百公里级货物运输等低空物流场景。

telegram · zaihuapd · Jul 9, 06:00

**背景**: 大疆 EV50 是一款复合翼垂直起降（VTOL）无人机，它能够像直升机一样垂直起降，然后切换至固定翼模式高效巡航。这类无人机结合了多旋翼和固定翼飞机的优点，适合需要垂直起降和长航程的任务。高海拔飞行因空气稀薄导致升力和电池效率下降而极具挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dronexl.co/2026/07/09/dji-ev50-evtol-delivery-drone-everest/">DJI EV50 Debuts As Company's First EVTOL Delivery Drone With ...</a></li>
<li><a href="https://pandaily.com/dji-ev50-everest-vtol-cargo-drone-jul2026">DJI Unreleased EV50 VTOL Cargo Drone Flies Above Everest ...</a></li>

</ul>
</details>

**标签**: `#drone technology`, `#VTOL`, `#high-altitude`, `#DJI`, `#logistics`

---