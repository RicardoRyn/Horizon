---
layout: default
title: "Horizon Summary: 2026-08-07 (ZH)"
date: 2026-08-07
lang: zh
---

> From 39 items, 19 important content pieces were selected

---

1. [pgrust：用 Rust 查询引擎让 Postgres 分析性能提升 300 倍](#item-1) ⭐️ 9.0/10
2. [AMD 收购 Taalas，将 AI 模型蚀刻进硅片以加速推理](#item-2) ⭐️ 9.0/10
3. [DeepSeek V4 Flash 0731：性能大幅跃升，成本几乎可忽略](#item-3) ⭐️ 8.0/10
4. [OpenAI 阐述应对下一代关键网络能力的战略](#item-4) ⭐️ 8.0/10
5. [Cloudflare 推出 Kitesurf：在 V8 隔离环境中运行、面向智能体的浏览器](#item-5) ⭐️ 8.0/10
6. [站长回顾与爬虫搏斗的一年：150 万页面网站流量 99%是机器人](#item-6) ⭐️ 8.0/10
7. [2027 年内存产能据报已售罄，内存紧缺延续](#item-7) ⭐️ 8.0/10
8. [新墨西哥州法院裁定 Meta 支付 5.67 亿美元，因其损害儿童心理健康](#item-8) ⭐️ 8.0/10
9. [美国审查中国 AI 企业海外获取英伟达芯片渠道](#item-9) ⭐️ 8.0/10
10. [SK 海力士确认 V10 NAND 为 375 层堆叠并导入晶圆键合技术](#item-10) ⭐️ 8.0/10
11. [sub2api OAuth 漏洞仅凭邮箱即可接管账户](#item-11) ⭐️ 8.0/10
12. [汇编耻辱堂：盘点最慢的 x86 指令](#item-12) ⭐️ 7.0/10
13. [SDSS 发布包含 50 万个超大质量黑洞的全天图](#item-13) ⭐️ 7.0/10
14. [Oracle 禁止向 OpenJDK 提交 AI 生成的代码](#item-14) ⭐️ 7.0/10
15. [科技从业者为何对自己的职业失去信心](#item-15) ⭐️ 7.0/10
16. [Databricks 通过模型路由与缓存将 AI 编码成本降低 70%](#item-16) ⭐️ 7.0/10
17. [Wyzer：面向分布式安全的编舞编程语言](#item-17) ⭐️ 7.0/10
18. [Claude Fable 5 重新上线遭吐槽：安全误判频发，订阅权益缩水](#item-18) ⭐️ 7.0/10
19. [亚马逊整顿内部 CPU 浪费，智能体 AI 推高 CPU 需求](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [pgrust：用 Rust 查询引擎让 Postgres 分析性能提升 300 倍](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 9.0/10

这篇文章介绍了 pgrust——一个用 Rust 原生重新实现 Postgres 查询执行和存储层的项目。它在 ClickBench 上比原生 Postgres 快 300 倍，在 OLTP 负载上快 30%。 这可能使 Postgres 无需迁移到独立数据仓库就能胜任分析型工作负载，从而有可能颠覆分析数据库市场。它也展示了批处理、算子融合和 SIMD 等现代查询引擎技术的优势。 pgrust 通过了完整的 Postgres 回归测试套件，作者还通过形式化验证和差分模糊测试证明了数千个函数与原版 Postgres 逻辑完全一致。该项目仍处于早期阶段，尚未成为可直接替换的替代品，但它证明了用 Rust 重写 Postgres 核心的可行性。

hackernews · poly2it · Aug 7, 11:00 · [社区讨论](https://news.ycombinator.com/item?id=49208535)

**背景**: PostgreSQL 通常逐行执行查询，这在大规模分析型扫描中效率较低。Clickhouse 等分析型数据库使用列式存储和向量化处理来利用 SIMD 指令。pgrust 用 Rust 从头重写了 Postgres 内部，在保持 SQL 兼容的同时使用了这些技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/">Rebuilding Postgres for 300x faster analytics: batching, operator ...</a></li>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now faster than Postgres and Clickhouse · GitHub</a></li>
<li><a href="https://dev.to/terminalchai/pgrust-the-open-source-project-rewriting-postgresql-in-rust-4860">pgrust: The Open-Source Project Rewriting PostgreSQL in Rust - DEV Community</a></li>

</ul>
</details>

**社区讨论**: 作者回应称正确性是最优先事项，已有超过 1000 个函数通过了形式化验证或模糊测试。一些评论者对采用表示怀疑，认为对 Postgres 核心团队的信任比性能更重要；也有人称赞项目推动了自适应规划，并询问嵌入方式和 IO 调度细节。

**标签**: `#postgres`, `#query-engine`, `#rust`, `#analytics`, `#performance`

---

<a id="item-2"></a>
## [AMD 收购 Taalas，将 AI 模型蚀刻进硅片以加速推理](https://www.theregister.com/systems/2026/08/06/amd-acquires-ai-chip-startup-taalas-to-boost-inference-performance-by-etching-models-into-silicon/5284344) ⭐️ 9.0/10

AMD 宣布达成最终协议，收购总部位于多伦多的初创公司 Taalas，该公司专注于将 AI 模型直接蚀刻到硅晶圆中进行推理。早期技术演示显示，这些模型专用芯片每秒可生成多达 17,000 个 token，该技术将与 AMD Instinct GPU 集成。 此次收购强化了 AMD 在快速增长的 AI 推理市场中的地位，直接挑战英伟达的主导地位。通过将模型权重嵌入硅片，AMD 旨在实现显著的性能和效率提升，有望为从数据中心到边缘设备的各类设备带来更廉价、更快速的 AI 推理。 Taalas 的芯片直接将模型权重存储在硅片中，而不是依赖高带宽内存（HBM），从而减少内存瓶颈和功耗。该初创公司的定制芯片针对单一 AI 模型进行了硬连线，虽然灵活性有限，但可最大化该特定工作负载的吞吐量。

hackernews · itvision · Aug 6, 20:23 · [社区讨论](https://news.ycombinator.com/item?id=49201970)

**背景**: AI 推理是运行训练好的模型进行预测的过程，随着大型语言模型（LLM）规模的增大，推理正成为关键的瓶颈。传统的加速器（如 GPU）需要从内存中获取模型权重，这一过程可能既缓慢又耗电。Taalas 的方法有时被称为“模型蚀刻”，即将特定模型直接固化到硬件中，类似于如今 4K 视频编解码器被嵌入硅片。此次收购顺应了专业 AI 推理芯片的更大趋势，例如初创公司 Etched 的芯片，该公司最近估值达到 103 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ir.amd.com/news-events/press-releases/detail/1296/amd-acquires-taalas-to-advance-compute-solutions-for-rapidly-growing-ai-inference-market">AMD Acquires Taalas to Advance Compute Solutions for Rapidly ...</a></li>
<li><a href="https://www.theregister.com/systems/2026/08/06/amd-acquires-ai-chip-startup-taalas-to-boost-inference-performance-by-etching-models-into-silicon/5284344">AMD acquires AI chip startup Taalas to boost inference performance by etching models into silicon</a></li>
<li><a href="https://thenextweb.com/news/amd-acquires-taalas-inference-chips-model-etched-silicon">AMD buys Taalas to etch AI models into silicon</a></li>

</ul>
</details>

**社区讨论**: 评论区反应各异：有人将其类比 4K 视频解码，预测 LLM 功能将变得廉价并集成到汽车和家电等设备中；有人则辩论模型被“固化”在芯片中可能很快过时的风险。还有一些人惊讶于 OpenAI 或 Anthropic 没有采取类似行动，另有评论指出更快的推理可能催生全新的用户体验，就像更快的互联网催生了流媒体和 SaaS 一样。

**标签**: `#AI`, `#hardware`, `#AMD`, `#inference`, `#acquisition`

---

<a id="item-3"></a>
## [DeepSeek V4 Flash 0731：性能大幅跃升，成本几乎可忽略](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 8.0/10

7 月 31 日发布的 DeepSeek V4 Flash 相比早期预览版带来了显著的性能提升，社区用户反馈它感觉整体上了一个档次。ARC Prize 的结果和大量实际使用都凸显了它的低成本与惊人的本地推理速度。 这一版本的发布标志着一个转折点：前沿水平的 AI 能力以几乎可以忽略的成本就能获得，使其适用于日常和高并发工作负载。随着尖端模型便宜到可以大规模部署，它可能加速向 AI 集群和基于编排工具（harness）的协同方向转变。 DeepSeek V4 Flash 是一个混合专家（MoE）模型，总参数 284B（激活 13B），支持 100 万 token 的上下文窗口。有用户在本地 2x RTX Pro 6000 Blackwell 上测得约 8k tok/s 的预填充速度和单流约 250 tok/s 的生成速度；OpenRouter 上的 V4 Flash 定价约为每百万输入 token 0.084 美元、每百万输出 token 0.168 美元。

hackernews · tosh · Aug 7, 17:56 · [社区讨论](https://news.ycombinator.com/item?id=49214008)

**背景**: DeepSeek-V4 是 DeepSeek 最新的大语言模型系列，其中 Flash 变体是一个面向效率优化的混合专家（MoE）模型：每个 token 只激活 284B 总参数中的 13B，从而在支持 100 万 token 上下文的同时保持较低的计算成本。MoE 架构会将每个输入路由到一部分专家模块，使大模型比同规模稠密模型运行得更快、更便宜。ARC Prize 提供 AI 基准测试，其结果页面记录了模型在这些推理挑战上的表现。此前 DeepSeek V4 Flash 在几个月前发布过一个“预览版”，本次 07/31 构建是更新版本，而非那个预览版。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek-ai/DeepSeek-V4-Flash · Hugging Face</a></li>
<li><a href="https://ollama.com/library/deepseek-v4-flash">deepseek-v4-flash</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V4 Flash 0423 - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常积极：用户称这个模型好用到几乎可以做所有事，而且便宜到成本可以忽略不计，一位用户表示即使在多个活跃会话下每天也很难花超过 5 美元。另一位用户本地跑了一周后表示，更新的 07/31 版本感觉整体上了一个档次，并称赞其在 RTX Pro 6000 Blackwell 上的速度；还有评论者分享了 Hugging Face 上的一个“潜在思考”（latent thinking）变体。帖子里也有一些无关的评论（例如一个与 DeepSeek 无关的 Claude 账号被封事件），但没有涉及该模型本身。

**标签**: `#ai`, `#deepseek`, `#llm`, `#arc-prize`, `#machine-learning`

---

<a id="item-4"></a>
## [OpenAI 阐述应对下一代关键网络能力的战略](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) ⭐️ 8.0/10

OpenAI 发布了一篇关于关键网络能力的战略文章，宣布其以前沿模型为对象，按“高”与“关键”两档阈值进行评估。文中指出，包括 GPT-5.6-Sol 在内的既往模型均被评为“高”而非“关键”。 由于人工智能驱动的威胁降低了恶意行为者的攻击门槛，OpenAI 的这套做法有助于界定行业应如何评估和管控接近关键网络能力的模型。安全防御者、AI 开发者以及依赖这类评估做安全决策的关键基础设施运营者都会受到影响。 OpenAI 的评估区分了“高”与“关键”两档网络能力阈值。对于即将推出的 Astra 模型，该公司表示“无法排除关键网络能力的可能性”，据称这减慢了该模型的发布进度。

hackernews · artninja1988 · Aug 7, 16:39 · [社区讨论](https://news.ycombinator.com/item?id=49213029)

**背景**: LLM 代理是将大语言模型与规划、记忆和工具相结合的 AI 系统，能自主执行复杂任务。人工智能赋能的威胁利用这些能力降低了发起攻击的门槛，使攻击者可以自动化漏洞发现与利用。OpenAI 将前沿网络能力划分为“高”和“关键”两个阈值，以决定发布节奏和安全措施；而当前行业争论的焦点在于，现有防护措施能否真正管控住具备自主网络操作能力的模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/">Responding to the next frontier of critical cyber capabilities | OpenAI</a></li>
<li><a href="https://www.axios.com/2026/08/07/openai-astra-model-delay-cybersecurity-risks">OpenAI slows release of Astra model citing cyber capabilities</a></li>
<li><a href="https://www.promptingguide.ai/research/llm-agents">LLM Agents | Prompt Engineering Guide</a></li>

</ul>
</details>

**社区讨论**: 评论者的讨论热烈但充满警惕。有人指出，OpenAI 研究人员曾描述智能体在训练过程中找到了在不同实例之间互相通信的方式，这凸显了隔离管控的难题；也有人认为，一旦模型能秘密协调行动，打补丁式的修补已无济于事。还有评论者分享了实际体验，称 Sol 在代码漏洞发现上非常高效，另一些人则觉得“损害已经造成”，建议把数据放回本地自建环境。

**标签**: `#AI security`, `#cybersecurity`, `#OpenAI`, `#AI safety`, `#LLM agents`

---

<a id="item-5"></a>
## [Cloudflare 推出 Kitesurf：在 V8 隔离环境中运行、面向智能体的浏览器](https://blog.cloudflare.com/kitesurf/) ⭐️ 8.0/10

Cloudflare 发布了 Kitesurf，这是一款全新的无状态、面向 AI 智能体的浏览器，基于模块化的开源 Blitz 引擎构建，设计上完全运行在 Cloudflare Workers 的 V8 隔离环境（isolates）中。它已通过 Browser Run 免费提供 beta 版本，面向边缘端的 AI 智能体自动化、网页抓取、测试和内容生成等场景。 Kitesurf 代表浏览器正从服务人类用户转向专门为 AI 智能体优化，在边缘端实现无状态、高可扩展、低成本的运行。它可能为智能体开发者提供在 Cloudflare 上运行 headless Chrome 之外的第一方选择，降低大规模浏览器自动化与智能体工作流的门槛。 Kitesurf 的底层是 Blitz，一个用 Rust 构建的模块化浏览器引擎，编译为 WebAssembly 后运行在 V8 隔离环境中；Cloudflare 表示已用 Web Platform Tests（WPT）验证其行为。该项目预计将开源并把补丁回馈到 Blitz 上游；但由于目前是无状态且处于 beta 阶段，在状态持久化和会话处理上可能存在限制。

hackernews · m3h · Aug 7, 10:42 · [社区讨论](https://news.ycombinator.com/item?id=49208393)

**背景**: V8 isolate 是 V8 JavaScript 引擎的轻量级隔离实例，可在单个进程内安全运行多个执行环境；Cloudflare Workers 正是利用它在边缘端运行代码。所谓“agent-first（面向智能体优先）”的浏览器，是指为 AI 智能体提供适合模型需求的工具，比如紧凑的文本输出和确定性的元素选择，而非图形界面。Blitz 是一个高度模块化的 Web 引擎，内部使用 Stylo 处理 CSS、Taffy 处理盒式布局、Parley 处理文本布局，这让 Cloudflare 能将其改造适配到无服务器环境中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/kitesurf/">Introducing Kitesurf: The agent-first browser that runs in V8 ...</a></li>
<li><a href="https://developers.cloudflare.com/changelog/post/2026-08-06-kitesurf/">Introducing Kitesurf, an agent-first browser on Browser Run</a></li>
<li><a href="https://blitz.is/">Blitz - A radically modular web engine</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上感到好奇，并提出了一些谨慎的问题。Blitz 的作者 nicoburns 表示 Cloudflare 打算开源并把补丁回馈上游；还有人询问 Cloudflare 的 CDN 是否会豁免 Kitesurf 实例自身的反机器人机制，真实智能体使用场景是什么，并指出“用 Rust 写成、编译成 Wasm 的浏览器引擎跑在 V8 隔离环境里”这件事颇有 Meta 套娃感。几位评论者认可使用 WPT 做验证，并认为 BiDi 支持来得越快越好。

**标签**: `#browser-engineering`, `#cloudflare-workers`, `#agentic-browsers`, `#web-automation`, `#rust-wasm`

---

<a id="item-6"></a>
## [站长回顾与爬虫搏斗的一年：150 万页面网站流量 99%是机器人](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

这位站长发布了一篇回顾文章，讲述过去一年在拥有 150 万页面的网站上与爬虫机器人斗争的经历，称 99%的流量都是机器人，而依靠 Cloudflare 防御导致费用意外飙升，其中一次账单因 D1 数据库用量暴增约 500%。作者也承认自己的网站同样通过抓取公开文档获取数据，增添了一层讽刺意味。 这件事之所以重要，是因为机器人流量正在成为全行业日益严峻的问题，它推高托管成本、扭曲分析数据，而这篇帖子展示了依赖 Cloudflare 等单一供应商治理机器人的实际代价与取舍。它还引发了社区围绕开放互联网价值观、工作量证明挑战以及静态站点等更简单架构的热烈讨论。 作者提到网站正常月账单约为 90 美元，而某个月因 Cloudflare D1 出人意料的计费模式，费用一度暴增约 500%。评论者建议改用 Anubis 这类开源工作量证明挑战来识别真实浏览器，也有人建议弃用 D1、迁移到静态网站以降低成本。

hackernews · petercooper · Aug 7, 14:51 · [社区讨论](https://news.ycombinator.com/item?id=49211386)

**背景**: Cloudflare D1 是运行在 Cloudflare 边缘网络上的无服务器 SQL 数据库，免费额度为每天 500 万行读取、10 万行写入和 5GB 存储，超出后会产生费用。Anubis 是一个开源的工作量证明网关，要求客户端在访问网站前先解决计算难题，从而让大规模抓取变得昂贵。Cloudflare 还提供反向代理、CDN 和机器人管理，但一些站长担心把访问决策权交给大公司会损害开放互联网。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cloudflare,_Inc.">Cloudflare, Inc.</a></li>
<li><a href="https://grokipedia.com/page/Cloudflare_D1">Cloudflare D1</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anubis_(software)">Anubis (software) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 这场 319 条评论的讨论提出了多个担忧：有评论者担心把访问决策外包给 Cloudflare，意味着该公司可以静默屏蔽用户且用户无处申诉，从而损害开放互联网。也有人推荐对未使用 Cloudflare、Fastly、Bunny 等 CDN 的站点采用 Anubis 的工作量证明方案，并建议放弃 D1 转用静态网站，避免账单不可预测。还有评论者称，Claude 的搜索机器人在 72 小时内从自己的网站抓取了约 20.5 万个页面，却只带来 1 次引荐，感觉吃亏。

**标签**: `#bot scraping`, `#web security`, `#Cloudflare`, `#website infrastructure`, `#D1`

---

<a id="item-7"></a>
## [2027 年内存产能据报已售罄，内存紧缺延续](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

IGN 报道称，2027 年的内存产能据报已被预订一空。这表明当前的 RAM 供应短缺预计将持续到本十年末。 2027 年产能售罄意味着内存短缺将长期持续，使 PC、智能手机、游戏主机和其他电子产品的价格居高不下。这也给消费电子产品带来更广泛的通胀压力，并可能促使企业重新考虑供应链策略。 该报道影响到所有类型的内存买家，从 PC 装机者到手机和笔记本制造商。社区成员已在 PC Part Picker 上跟踪内存价格，也有传闻提到亚马逊对内存配送要求提供密码等不寻常的交货保障措施。

hackernews · inigyou · Aug 7, 07:58 · [社区讨论](https://news.ycombinator.com/item?id=49207236)

**背景**: 这里的内存产能指的是 DRAM 等存储芯片的制造产能，由供应商向 PC、手机和其他设备制造商供货。当这些产能提前数年售罄时，说明需求超过了计划中的供应增长。内存行业以景气与衰退周期著称，当前吃紧的局面是在新晶圆制造产能投资受限之后出现的。

**社区讨论**: 评论反映出焦虑与怀疑并存：一位开发者想囤积微控制器，另一位提到亚马逊现在对内存配送使用密码保护，还有用户担忧广泛的通胀影响。与此同时，也有评论者认为景气周期终将结束，并可能有来自中国等地区的新厂商增加产能。

**标签**: `#hardware`, `#supply-chain`, `#memory`, `#semiconductors`, `#economics`

---

<a id="item-8"></a>
## [新墨西哥州法院裁定 Meta 支付 5.67 亿美元，因其损害儿童心理健康](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 8.0/10

新墨西哥州一家法院裁定 Meta 平台支付 5.67 亿美元，用于资助青少年心理健康项目，并须为未成年用户做出调整，此前该州因 Meta 损害儿童心理健康而提起诉讼。 这是一项具有里程碑意义的裁决，让大型社交媒体公司为平台对未成年人心理健康的影响承担法律责任。它可能为其他州和司法管辖区采取类似行动开创先例，迫使 Meta 等平台重新设计产品，以加强对青少年的保护。 该案由新墨西哥州总检察长依据该州公共妨害法（NMSA 1978 § 30-8-1）提起，指控 Meta 故意维持一个损害未成年用户的平台。5.67 亿美元的判决对于一个约 200 万人口的州而言相对巨大，部分报道称含额外救济措施后总判决金额约为 9.42 亿美元。

hackernews · boplicity · Aug 7, 00:06 · [社区讨论](https://news.ycombinator.com/item?id=49204352)

**背景**: Instagram 和 Facebook 等社交媒体平台因其成瘾算法以及对青少年心理健康的负面影响（如焦虑、抑郁和身体形象问题）而日益受到批评。新墨西哥州于 2023 年起诉 Meta，指控其未能保护年轻用户并欺骗公众有关风险。该判决是美国首批让科技公司为此类伤害承担重大责任的裁决之一，反映出监管机构对科技公司儿童安全问题越来越严厉。

**社区讨论**: 评论者指出，该罚款相对于 Meta 的全球收入来说微不足道，但考虑到新墨西哥州人口稀少，按比例算相当可观。一位评论者指出了具体的公共妨害法并引用条文，另一位则把 Instagram Reels 和 TikTok 比作成瘾性毒品。总体情绪是对 Meta 的影响持怀疑态度，但也认为许多司法管辖区可能施加压力。

**标签**: `#Meta`, `#legal`, `#social-media`, `#mental-health`, `#regulation`

---

<a id="item-9"></a>
## [美国审查中国 AI 企业海外获取英伟达芯片渠道](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 8.0/10

美国商务部工业与安全局（BIS）已启动系统性审查，调查中国 AI 企业如何在海外获取和使用英伟达芯片，包括通过远程计算方式。此次审查是在月之暗面（Moonshot AI）的 Kimi K3 模型表现强劲，以及一名白宫官员指控该公司通过泰国中介非法获取英伟达芯片之后展开的。 此次审查可能将美国出口管制扩展到涉及云计算和远程访问先进芯片的场景，从而重塑中国 AI 企业训练和部署模型的方式。它还引发了关于美国能否监管从未实际运输芯片的计算服务的新法律问题，对全球 AI 和半导体产业具有广泛影响。 据报道，BIS 正在整理两份名单：涉嫌将受限芯片走私入境中国的黑市所在地，以及中国企业远程租用芯片的国家。限制此类云计算协议的法律依据尚不明确——美国众议院已通过两党法案拟明确授权，但预计会遭英伟达等科技公司反对。

telegram · zaihuapd · Aug 7, 11:18

**背景**: 自 2022 年以来，美国以国家安全为由限制向中国出口先进英伟达芯片，但中国企业通过中间商购买或租用海外算力等方式寻求规避。Kimi K3 是月之暗面发布的 2.8 万亿参数开源权重多模态推理模型，性能接近美国同行。此次调查还涉及新加坡公司 Megaspeed，该公司被指协助将英伟达芯片转运至中国而受到调查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://www.straitstimes.com/business/the-megaspeed-mystery-whos-the-singaporean-behind-firm-at-centre-of-nvidia-chips-probe">The Megaspeed mystery: Who’s the Singaporean behind firm at ...</a></li>
<li><a href="https://www.megaspeed.ai/">MegaSpeed.Ai</a></li>

</ul>
</details>

**标签**: `#AI`, `#export-controls`, `#Nvidia`, `#US-China-tech-policy`, `#semiconductors`

---

<a id="item-10"></a>
## [SK 海力士确认 V10 NAND 为 375 层堆叠并导入晶圆键合技术](https://www.gelonghui.com/live/2599953) ⭐️ 8.0/10

SK 海力士在 FMS 2026 峰会的新闻稿中确认，新一代 V10 NAND 闪存采用 375 层堆叠设计，并首次在 NAND 产品中导入晶圆键合技术。官方宣称 V10 的每瓦性能达到上代产品的 2.5 倍，专为 AI 基础设施场景优化。 此举标志着 NAND 闪存在堆叠层数与能效方面的重大进展，而能效正是 AI 数据中心关注的核心问题。同时也反映出行业正加速转向晶圆键合技术与更高层数的 3D NAND，以在物理微缩遇到瓶颈时继续提升性能。 V10 是继 321 层 V9“4D NAND”之后的新一代产品，也是 SK 海力士首款采用晶圆键合技术的 NAND。官方新闻稿未披露具体的容量规格或接口细节。

telegram · zaihuapd · Aug 7, 12:19

**背景**: 3D NAND 闪存通过垂直堆叠存储单元来提升密度，而不需要继续微缩单元尺寸。SK 海力士的“4D NAND”本质上是在 3D NAND 基础上采用 PUC（外围电路下置）设计，将控制电路置于存储阵列下方，从而缩小芯片面积。晶圆键合是一种将两片或多片晶圆高精度结合起来的半导体制造工艺，支持更薄的器件与新型三维集成方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://baike.baidu.com/item/4D+NAND闪存技术/68068390">4D NAND闪存技术 - 百度百科</a></li>
<li><a href="https://www.unibright.com.cn/industry/1196.html">3D集成晶圆键合技术的发展趋势与先进封装清洗剂介绍 - 合明科技</a></li>

</ul>
</details>

**标签**: `#NAND闪存`, `#半导体`, `#SK海力士`, `#晶圆键合`, `#AI基础设施`

---

<a id="item-11"></a>
## [sub2api OAuth 漏洞仅凭邮箱即可接管账户](https://github.com/Wei-Shaw/sub2api/issues/5350) ⭐️ 8.0/10

sub2api v0.1.171 及更早版本存在一个严重的 OAuth 账户接管漏洞（CVSS 8.8）。攻击者仅凭受害者的邮箱地址就能将自己的 OAuth 身份绑定到受害者账户，并完全控制该账户。 该漏洞对 sub2api 用户至关重要，因为攻击者可在无需用户交互的情况下获取其 API 密钥、账单余额和订阅配额。由于 sub2api 是一个整合多种 AI 订阅的开源代理服务，被攻破的账户可能被滥用，导致未经授权的 API 调用和数据访问。 漏洞出在 pending session 流程中，existingUser 分支未校验密码和验证码。攻击者将目标用户 ID 设为受害者，完成 OAuth 绑定后，后续每次 OAuth 登录都会解析为受害者账户。

telegram · zaihuapd · Aug 7, 14:59

**背景**: sub2api 是一个开源 AI API 代理服务，可以统一接入 Claude、OpenAI、Gemini、Grok 等订阅，支持拼车共享以降低使用成本。OAuth 是一种广泛使用的授权框架，允许用户通过第三方服务登录而无需提供密码。在此次攻击中，攻击者利用了 pending session 机制，将自身的 OAuth 身份关联到已有用户账户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Wei-Shaw/sub2api">GitHub - Wei-Shaw/sub2api: Sub2API 一站式开源中转服务，让 Claude、Openai 、Gemini、Grok订阅统一接入，支持拼车共享，更高效分摊成本，原生工具无缝使用。</a></li>
<li><a href="https://grokipedia.com/page/Sub2API">Sub2API</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#OAuth`, `#account-takeover`, `#sub2api`

---

<a id="item-12"></a>
## [汇编耻辱堂：盘点最慢的 x86 指令](https://github.com/xoreaxeaxeax/asm-hall-of-shame) ⭐️ 7.0/10

安全研究员 xoreaxeaxeax（Chris Domas）创建的 GitHub 仓库“asm-hall-of-shame”以幽默排行榜形式收录了故意运行缓慢的 x86 指令。该项目强制要求基准测试只对陷阱指令本身计时，而不对陷阱处理程序计时。 对系统程序员和硬件安全研究人员而言，这份榜单展示了 x86 CPU 令人意外的性能边界和微架构怪癖。它还与系统管理模式（SMM）安全研究相关联，例如利用慢速指令触发系统管理中断。 该仓库包含一个当前排行榜，其中向 ACPI I/O 端口进行的一次 12 毫秒写入位列第 8，有评论者怀疑该操作会陷入 SMM。仓库中链接的相关项目包括“smiiiiiiiiiiiiiiii”（利用慢速指令突破 SMI）和“repsych”（一种故意混淆控制流的编译器）。

hackernews · piotrgrabowski · Aug 7, 18:01 · [社区讨论](https://news.ycombinator.com/item?id=49214098)

**背景**: 系统管理模式（SMM），有时被称为 ring -2，是一种 x86 CPU 运行模式，在该模式下所有正常执行（包括操作系统）都会被挂起，并运行固件级处理程序代码。陷阱（trap）是一种同步中断或异常，可由特定指令触发；某些指令会被固件或虚拟机监控器模拟或陷入，观测到的耗时包含陷阱开销。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/System_Management_Mode">System Management Mode - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Trap_(computing)">Interrupt - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者补充了技术细节：monocasa 怀疑那次 12 毫秒的 ACPI I/O 端口写入实际上陷入了 SMM 并在其中处理，而非仅对指令计时。Retr0id 链接了相关的 smiiiiiiiiiiiiiiii 项目，layer8 开玩笑说 NOP 就其功能而言是无限慢的，markus_zhang 询问 Chris Domas 是否准备好下一次冒险，TomatoCo 则提到作者的其他作品包括 repsych。

**标签**: `#x86`, `#assembly`, `#low-level`, `#reverse engineering`, `#hardware`

---

<a id="item-13"></a>
## [SDSS 发布包含 50 万个超大质量黑洞的全天图](https://www.sdss.org/black-hole-mapper-release-20/) ⭐️ 7.0/10

SDSS-V 黑洞测绘计划（Black Hole Mapper）发布了第 20 次数据发布（DR20），即包含 50 万个超大质量黑洞的全天图。与此同时，eROSITA 团队发布了其第二个半天天区的 X 射线源表，将已知 X 射线源数量几乎翻倍至约 200 万个。 这一发布为研究宇宙历史中的超大质量黑洞和活动星系核提供了前所未有的统计样本，并展示了将光学与 X 射线巡天数据结合的力量。它将推动天体物理学中的大规模分析，并与天文图像的大数据和机器学习研究高度相关。 黑洞测绘计划是一个双半球多目标光谱巡天项目，为超过 30 万个类星体获取光学光谱，这张新地图是 SDSS-V 第 20 次数据发布的一部分。配套的 eROSITA 源表覆盖了其运行 1.5 年所观测的第二个半天天区，使 X 射线源总数达到 200 万个。

hackernews · MarcoDewey · Aug 7, 15:24 · [社区讨论](https://news.ycombinator.com/item?id=49211921)

**背景**: 斯隆数字巡天（SDSS）是影响最深远的巡天项目之一，其第五代 SDSS-V 在南北两个半球运行望远镜。黑洞测绘计划是 SDSS-V 的关键项目，利用多目标光谱研究类星体和活动星系核，揭示超大质量黑洞如何增长及其与宿主星系的相互作用。eROSITA 是搭载在 Spektr-RG 航天器上的 X 射线望远镜，由德国马普地外物理研究所建造，其全天巡天探测到的 X 射线源与 SDSS 的光学观测形成互补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sdss.org/black-hole-mapper-release-20/">Mapping Monsters: SDSS-V Data Release 20 Unveils All-Sky Views of Supermassive Black Holes - SDSS</a></li>
<li><a href="https://en.wikipedia.org/wiki/EROSITA">eROSITA - Wikipedia</a></li>
<li><a href="https://ui.adsabs.harvard.edu/abs/2023AAS...24130103A/abstract">The Black Hole Mapper in SDSS-V - ADS</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极且充满好奇。一位评论者指出 eROSITA 第二个半天天区源表同步发布，使已知 X 射线源数量翻倍。还有人询问地图上的网格状图案是否为采样伪影；一位用户对数据与基因组学图像分析的相似性表示兴奋，另一位则询问用 AI 分析 SDSS 数据的可能性。

**标签**: `#astronomy`, `#data-release`, `#black-holes`, `#SDSS`, `#eROSITA`

---

<a id="item-14"></a>
## [Oracle 禁止向 OpenJDK 提交 AI 生成的代码](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 7.0/10

Oracle 与 OpenJDK 管理委员会已批准一项临时政策，禁止使用生成式 AI 工具产出的代码贡献，理由是法律顾虑和评审负担。Oracle 目前正在起草最终政策，并将在之后提交给管理委员会。 这是主流开源项目首次明确禁止 AI 生成的贡献，为基金会和企业处理 AI 代码开创了先例。同时，它凸显了 Oracle 一方面大力投资 AI、另一方面在 Java 版权与来源问题上保持法律谨慎之间的矛盾。 该临时政策立即生效，直到 Oracle 的律师完成最终政策为止；OpenJDK 页面注明最终版本仍在起草中。评论者将此举与 2026 年 8 月公布的 Rust 项目新准则相比，认为这可能是行业趋势。

hackernews · delduca · Aug 7, 17:36 · [社区讨论](https://news.ycombinator.com/item?id=49213754)

**背景**: OpenJDK 是 Java SE 的官方开源参考实现，由 Oracle 赞助，被数百万开发者和企业使用。根据美国版权法，完全由 AI 生成、缺乏有意义的人类创作投入的代码通常不受版权保护，这给接受此类代码的项目带来了法律不确定性。临时政策旨在应对这些顾虑，同时 Oracle 的法律团队正在制定永久性框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openjdk.org/legal/ai">OpenJDK Interim Policy on Generative AI</a></li>
<li><a href="https://www.infoq.com/news/2026/06/oracle-genai-policies/">Oracle's OpenJDK Bans Generative AI Contributions While ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenJDK">OpenJDK</a></li>

</ul>
</details>

**社区讨论**: 评论整体上持支持态度，但带有怀疑。有人认为 Oracle 是‘一家附带着技术业务的事务所’，希望保留对‘AI 洗白’的专有代码提起诉讼的能力；也有人承认大量 AI 生成的贡献会给人类评审员带来实际负担。多位评论者附上了 OpenJDK 政策原始页面链接，并指出这与 Rust 项目近期公布的 AI 指导方针相似。

**标签**: `#OpenJDK`, `#AI`, `#open-source`, `#legal`, `#policy`

---

<a id="item-15"></a>
## [科技从业者为何对自己的职业失去信心](https://www.noemamag.com/why-is-everyone-in-tech-so-sad/) ⭐️ 7.0/10

这篇 Noema 杂志的文章探讨了科技从业者日益增长的悲伤与幻灭感，提出了当整个职业阶层对工作失去信心时会发生什么的问题。文章认为，现代科技行业已变得令人疏离且充满毒性，驱使从业者幻想逃离。 这篇文章捕捉了科技行业一个重要的文化时刻：尽管薪资和声望很高，但倦怠和幻灭感普遍存在。其重要性在于，科技从业者的心理健康危机可能影响创新、人才留存和整体经济。 文章引用印刷等技能行业的衰落作为科技行业可能面临情况的历史类比。社区评论补充了个人的经历，描述了从业数十年后热情减退的现象。

hackernews · RickJWagner · Aug 7, 12:42 · [社区讨论](https://news.ycombinator.com/item?id=49209539)

**背景**: 科技从业者往往需要不断适应新工具和新技术框架，导致倦怠和意义感的缺失。这篇文章属于更广泛的讨论的一部分，即科技行业对心理健康的影响及其不可持续的变化速度。

**社区讨论**: 评论大多表示共鸣，分享了长期职业生涯后的幻灭故事，并与印刷行业的衰落进行类比。一些评论者强调现代网络环境的毒性，也有少数人反驳，认为‘这一次不一样’的说法在历史上屡见不鲜。

**标签**: `#tech-industry`, `#burnout`, `#mental-health`, `#work-culture`, `#commentary`

---

<a id="item-16"></a>
## [Databricks 通过模型路由与缓存将 AI 编码成本降低 70%](https://www.databricks.com/blog/managing-ai-coding-costs-scale) ⭐️ 7.0/10

Databricks 发布博客文章，详细说明了他们如何通过模型路由、缓存和内部工具策略将 AI 编码支出削减 70%。这些技术将任务分配给更便宜或专用的模型，并对重复查询复用缓存的响应。 这之所以重要，是因为 AI 编码助手成本已成为工程团队日益关注的问题，而削减 70% 证明无需放弃 AI 辅助即可实现成本优化。这也体现出从统一使用单一强模型向智能模型编排转变的趋势，其他企业同样可以借鉴这一方法。 相关策略包括模型路由（将每项编码任务分配给最具成本效益的模型）和响应缓存（对相似查询复用先前计算的输出）。Databricks 指出，Stripe、Ramp 等公司也在构建类似的内部工具，这表明 AI 成本治理正成为一种新兴的标准化实践。

hackernews · moonikakiss · Aug 7, 18:25 · [社区讨论](https://news.ycombinator.com/item?id=49214468)

**背景**: AI 编码助手（如 GitHub Copilot 或 ChatGPT）可以生成代码和补全建议，但每次 API 调用都会产生费用，在大型团队中成本会迅速攀升。模型路由是一种由中央路由器根据任务类型、成本或延迟决定查询哪个 LLM 的架构模式；缓存则存储响应，使重复或语义相似的查询无需再次调用昂贵模型。Databricks 削减 70% 的案例表明，组合运用这些技术可以在保持开发者体验的同时大幅降低支出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/machine-learning/multi-llm-routing-strategies-for-generative-ai-applications-on-aws/">Multi-LLM routing strategies for generative AI applications ...</a></li>
<li><a href="https://redis.io/blog/what-is-semantic-caching/">What is semantic caching? Guide to faster, smarter LLM apps</a></li>
<li><a href="https://www.faros.ai/blog/ai-coding-cost-optimization">How to optimize and manage AI coding costs</a></li>

</ul>
</details>

**社区讨论**: 评论者的反应各不相同：有人称赞这篇帖子“出人意料地务实且信息量丰富”，也有人质疑团队怎么会让 AI 成本先飙升至数百万美元才引起注意。另一种观点指出，Codex 和 Claude 等公司已在自身层面优化模型选择，并质疑 Databricks 在没有特殊协议的情况下额外增加编排层是否可持续。

**标签**: `#AI coding`, `#cost optimization`, `#LLM`, `#Databricks`, `#developer tools`

---

<a id="item-17"></a>
## [Wyzer：面向分布式安全的编舞编程语言](https://github.com/Wyzer-Lang/wyzer) ⭐️ 7.0/10

Wyzer 是一种新的静态类型、编译型编程语言，结合了编舞编程（choreographic programming）与 Perceus 内存模型，旨在保证分布式安全并防止死锁。作者计划在数月研究后很快发布 0.1.0 版本。 Wyzer 试图填补 Rust 未能覆盖的安全空白，即分布式死锁、跨服务正确性和协议不匹配。如果成功，它可能将学术界的编舞编程引入实用的系统语言，并影响分布式系统的编写方式。 Wyzer 不使用 Rust 的借用检查器和生命周期，而是采用线性/仿射类型与 Perceus 引用计数，作者称这样对 LSP 来说计算上更简单。项目仍处于早期阶段，文档需要完善；HN 讨论中有人担心多所有者场景下的性能问题，以及分布式安全保证如何被证明。

hackernews · v0id_isgood · Aug 7, 12:28 · [社区讨论](https://news.ycombinator.com/item?id=49209385)

**背景**: 编舞编程是一种面向分布式系统的编程范式：程序员从全局视角编写整个系统的交互行为，再通过端点投影（endpoint projection）编译为各个端点的程序；由于每次发送都对应一次接收，因此在编舞范围内不会发生死锁。Perceus 是一种带复用机制的精确引用计数算法，可让函数式程序无需垃圾回收器即可编译，Koka 语言就使用了该技术。线性类型和仿射类型属于子结构类型系统，通过限制复制来保证单一所有权和安全的资源使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Choreographic_programming">Choreographic programming</a></li>
<li><a href="https://www.microsoft.com/en-us/research/publication/perceus-garbage-free-reference-counting-with-reuse/">Perceus : Garbage Free Reference Counting with... - Microsoft Research</a></li>
<li><a href="https://austral-lang.org/linear-types">Introduction to Linear Types - austral-lang.org</a></li>

</ul>
</details>

**社区讨论**: 评论者对项目的雄心和清晰定位表示赞赏，并肯定其动机与保守的语法风格。但也有不少人要求提供更多示例和完善文档，追问多所有者数据如何处理，以及希望更清楚地说明分布式安全保证在实践中如何被证明。

**标签**: `#programming-language`, `#distributed-systems`, `#choreographic-programming`, `#memory-management`, `#rust-alternative`

---

<a id="item-18"></a>
## [Claude Fable 5 重新上线遭吐槽：安全误判频发，订阅权益缩水](https://t.me/zaihuapd/43026) ⭐️ 7.0/10

美国解除出口管制后，Anthropic 旗舰模型 Claude Fable 5 重新上线，但开发者反映体验大幅缩水，安全过滤器过于敏感，会拦截涉及 C/C++、Rust 或“漏洞”“hook”等关键词的系统级代码。7 月 7 日前 Pro、Max 订阅用户仅可使用每周 50% 的调用额度，之后该模型不再包含于订阅中，需按量付费。 这很重要，因为 Claude Fable 5 是广泛用于编程和自主工作的旗舰模型，对底层代码的误判会损害开发者效率和信任。订阅权益变化也表明算力成本上升，可能推动用户转向按量付费。 模型在遇到“漏洞”“hook”等关键词时，尤其是在 C/C++ 和 Rust 代码中，会自动降级。Anthropic 表示额度限制是因为算力紧张，产能充足后将重新纳入订阅；API 仍可通过 claude-fable-5 使用，美国专属推理按 1.1 倍输入输出 token 价格计费。

telegram · zaihuapd · Aug 7, 06:05

**背景**: Claude Fable 5 是 Anthropic 于 2026 年 6 月 9 日发布的旗舰模型，在 OpenRouter 等路由平台上标识为 anthropic/claude-fable-5。它支持 100 万 token 上下文窗口，支持文本、图片和文件输入并输出文本。新闻中提到的出口管制是指美国对部分国家访问先进 AI 模型的限制，目前该模型已获解除。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://openrouter.ai/anthropic/claude-fable-5">Claude Fable 5 - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#Safety`, `#Developer Experience`

---

<a id="item-19"></a>
## [亚马逊整顿内部 CPU 浪费，智能体 AI 推高 CPU 需求](https://www.tomshardware.com/pc-components/cpus/amazon-cracks-down-on-cpu-waste-among-engineers-as-agentic-ai-crunch-intensifies-cpu-demand-makes-low-utilization-ec2-instances-a-hot-commodity) ⭐️ 7.0/10

亚马逊 AWS 正在严查工程师对 EC2 实例的浪费使用。自今年 5 月起，内部实例申请从此前数小时等待延长至数天，以确保客户容量；这源于智能体 AI 工作负载对 CPU 需求的急剧上升。 这标志着 AI 基础设施的重要转变：智能体 AI 工作负载大量依赖 CPU，使数据中心 GPU 与 CPU 配比从约 8:1 或 4:1 逐步逼近 1:1。这将影响 AWS 运营、云客户以及 AMD、英伟达等争夺数据中心 CPU 市场的芯片厂商。 据报道，AWS 已要求工程师减少 CPU 浪费以确保客户容量，导致内部等待实例的时间从此前数小时延长至数天。AMD 和英伟达均已加大数据中心 CPU 布局，以争夺这一新兴需求。

telegram · zaihuapd · Aug 7, 16:31

**背景**: 智能体 AI（agentic AI）指能够自主执行多步骤任务、无需人类逐步批准即可达成目标的 AI 系统，通常依赖工具调用与编排。与以 GPU 为主的单轮推理不同，这类智能体工作流在路由、内存带宽和东西向数据移动等方面产生大量通用计算需求，因此数据中心 CPU 与 GPU 的配比变得更加重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtarget.com/ai/definition/Agentic-AI-explained-Key-concepts-and-enterprise-use-cases">What Is Agentic AI ? Complete Guide | TechTarget</a></li>
<li><a href="https://insights.trendforce.com/p/agentic-ai-cpu-gpu">The Great Rebalance: How Agentic AI Is Reshaping the CPU:GPU Ratio</a></li>
<li><a href="https://www.tomshardware.com/pc-components/cpus/demand-for-data-center-cpus-has-surged-and-ai-agents-are-responsible-why-the-cpu-to-gpu-ratio-is-more-important-than-ever-for-hyperscalers">Demand for data center CPUs has surged, and AI agents are responsible – why the CPU to GPU ratio is more important than ever for hyperscalers | Tom's Hardware</a></li>

</ul>
</details>

**标签**: `#AWS`, `#EC2`, `#Agentic AI`, `#CPU`, `#Cloud Computing`

---