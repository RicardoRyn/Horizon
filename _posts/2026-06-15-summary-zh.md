---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> From 39 items, 19 important content pieces were selected

---

1. [百度复旦用 ROI 压缩 KV 缓存 80%](#item-1) ⭐️ 9.0/10
2. [全球地下真菌网络首张地图发布](#item-2) ⭐️ 9.0/10
3. [美国政府以国安为由要求 Anthropic 关闭两个 AI 模型](#item-3) ⭐️ 9.0/10
4. [领英招聘中的后门攻击开发者](#item-4) ⭐️ 8.0/10
5. [Iroh 1.0: 稳定的点对点连接库](#item-5) ⭐️ 8.0/10
6. [Hacker News 讨论用本地模型替代 Claude/GPT 进行日常编程](#item-6) ⭐️ 8.0/10
7. [福克斯提议收购 Roku，引发中立性担忧](#item-7) ⭐️ 8.0/10
8. [Typst 0.15.0 新增多参考文献和 MathML 导出](#item-8) ⭐️ 8.0/10
9. [字节跳动洽购天数智芯 AI 芯片，并考虑百度昆仑芯](#item-9) ⭐️ 8.0/10
10. [哪吒监控探针高危路径穿越漏洞 (CVSS 9.1)](#item-10) ⭐️ 8.0/10
11. [开发者分享家庭实验室 AI 开发平台](#item-11) ⭐️ 7.0/10
12. [《指挥官基恩》引擎白皮书](#item-12) ⭐️ 7.0/10
13. [Hetzner 宣布云服务器大幅涨价](#item-13) ⭐️ 7.0/10
14. [TimescaleDB Hypercore 压缩：最高 98%压缩比](#item-14) ⭐️ 7.0/10
15. [自制真空管中的玻璃-金属密封技术](#item-15) ⭐️ 7.0/10
16. [蚂蚁集团测试 AI 版支付宝，原生 AI 界面](#item-16) ⭐️ 7.0/10
17. [小红书传月底在港秘密提交 IPO 申请](#item-17) ⭐️ 7.0/10
18. [Rio 3.5 模型被曝套壳中国开源模型](#item-18) ⭐️ 7.0/10
19. [消费者起诉 Anthropic，称 AI 订阅计划限额不实](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [百度复旦用 ROI 压缩 KV 缓存 80%](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247897349&idx=2&sn=14ceeec45a2f6803e40bc7b029964120) ⭐️ 9.0/10

百度与复旦大学的研究人员提出了一种基于投资回报率（ROI）的 KV 缓存压缩方法，选择性保留缓存条目，实现了 80%的压缩率，性能损失仅为 0.52%。该论文已被 ICML 2026 录用。 这一突破显著降低了大语言模型的内存消耗和推理延迟，使其更便于部署。通过智能管理 KV 缓存，解决了 transformer 推理中的关键瓶颈，对扩展 LLM 至关重要。 该方法应用 ROI 指标——平衡重新计算的计算成本与缓存收益——来决定哪些键值对被驱逐。在长上下文任务中实现了 80%的压缩率，同时保持了高准确性。

rss · 量子位 · Jun 14, 04:00

**背景**: KV 缓存存储 LLM 推理过程中注意力层的中间键（K）和值（V）矩阵，避免重新计算并加速生成。但它随序列长度线性增长，消耗大量 GPU 内存。传统的压缩方法统一丢弃缓存，常常损害性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/coding-the-kv-cache-in-llms">Understanding and Coding the KV Cache in LLMs from Scratch</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Machine_Learning">International Conference on Machine Learning - Wikipedia</a></li>
<li><a href="https://www.investopedia.com/terms/r/returnoninvestment.asp">investopedia.com/terms/r/returnoninvestment.asp</a></li>

</ul>
</details>

**标签**: `#KV Cache`, `#LLM Inference`, `#Compression`, `#ICML`, `#AI Efficiency`

---

<a id="item-2"></a>
## [全球地下真菌网络首张地图发布](https://insideclimatenews.org/news/11062026/earths-massive-underground-fungal-networks/) ⭐️ 9.0/10

地下网络保护协会（SPUN）绘制了首张全球丛枝菌根真菌网络地图，揭示了总长度达 110 千万亿公里、每年封存约 10 亿吨碳的庞大地下系统。 该地图凸显了真菌网络在碳封存和生态系统健康中的关键作用，对气候变化缓解和农业实践具有重要意义，尤其农田真菌密度仅为野生生态系统的一半。 真菌网络总长度接近地球与太阳距离的近十亿倍；其质量约为全体人类体重的 5 倍。拥有全球 40%该类真菌生物量的野生草原正以森林 4 倍的速度转为农田。

telegram · zaihuapd · Jun 14, 14:58

**背景**: 丛枝菌根真菌与约 80%的维管植物形成共生关系，帮助植物吸收养分。地下网络保护协会（SPUN）是一个成立于 2021 年的科学倡议组织，致力于绘制和保护这些地下网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Arbuscular_mycorrhiza">Arbuscular mycorrhiza - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Society_for_the_Protection_of_Underground_Networks">Society for the Protection of Underground Networks</a></li>

</ul>
</details>

**标签**: `#fungal networks`, `#carbon sequestration`, `#ecology`, `#agriculture`, `#climate change`

---

<a id="item-3"></a>
## [美国政府以国安为由要求 Anthropic 关闭两个 AI 模型](https://t.me/zaihuapd/41960) ⭐️ 9.0/10

美国商务部依据出口管制和国家安全权限向 Anthropic 发函，要求暂停任何外国公民在美国境内外访问 Fable 5 和 Mythos 5 模型。Anthropic 已按要求关闭了这两款模型对所有客户的访问，包括其外籍员工。 这标志着美国政府首次直接限制先进 AI 模型的访问，为前沿 AI 的国家安全管控开创了先例。此举可能扰乱全球 AI 的研发与部署，影响世界各地的研究者和企业。 仅两款特定模型（Fable 5 和 Mythos 5）受影响，其他 Claude 模型仍可使用。Anthropic 表示正在争取尽快恢复访问。据报道，限制原因是担心模型可能被越狱带来安全风险。

telegram · zaihuapd · Jun 15, 08:55

**背景**: AI 模型越狱是指强制模型绕过内置安全准则的技术，可能导致有害输出。对 AI 模型的出口管制正成为防止敏感技术落入对手手中的政策工具。Mythos 5 是 Anthropic 最先进的模型之一，其公开发布本就受到限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-04-20/anthropic-s-mythos-ai-model-questions-answered">Anthropic 's Mythos AI Model , Questions Answered - Bloomberg</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#export control`, `#national security`, `#Anthropic`, `#AI policy`

---

<a id="item-4"></a>
## [领英招聘中的后门攻击开发者](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 8.0/10

一位开发者在面试任务中发现，招聘人员发送的 Node.js 仓库中隐藏了一个后门，该后门在安装时通过 npm 的 prepare 脚本执行任意代码。 此事件揭示了一种新型社会工程攻击，求职者被诱骗安装恶意包，威胁软件供应链安全，并凸显了招聘过程中需要更高警惕性。 后门被隐藏在注释掉的测试代码中，并在 npm install 运行 prepare 脚本时自动触发（这是一个常见的生命周期钩子）。攻击者伪装成一家加密初创公司的招聘人员，要求审查一个故障概念验证。

hackernews · lwhsiao · Jun 15, 20:00 · [社区讨论](https://news.ycombinator.com/item?id=48546294)

**背景**: 软件供应链攻击通过将恶意代码插入依赖项或工具来破坏开发过程。社会工程利用人类心理欺骗个人执行操作。npm（Node.js 流行的包管理器）在安装过程中会执行生命周期脚本（如 prepare），这可能被滥用来运行恶意代码。此次攻击结合了这两种技术，专门针对开发者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>
<li><a href="https://www.cloudflare.com/learning/security/what-is-a-supply-chain-attack/">What is a supply chain attack?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Social_engineering_attack">Social engineering attack</a></li>

</ul>
</details>

**社区讨论**: 帖子评论指出这种情况构成犯罪，并呼吁建立集中的网络犯罪报告系统。用户分享了类似的过往事件，并批评微软（GitHub 所有者）未删除恶意仓库。许多人指出这一场景与典型面试任务极为相似，使其尤其危险。

**标签**: `#security`, `#backdoor`, `#Node.js`, `#supply chain attack`, `#social engineering`

---

<a id="item-5"></a>
## [Iroh 1.0: 稳定的点对点连接库](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

Iroh 1.0 在经过四年多和超过 65 个版本后正式发布稳定版，提供使用公钥而非 IP 地址的直接点对点连接库，目前每月处理超过 2 亿个端点连接。 该库通过抽象网络复杂性简化了去中心化应用的构建，使应用实例无需管理 IP 地址或网络配置即可直接连接，对点对点和边缘计算应用至关重要。 Iroh 1.0 使用基于 QUIC 的协议，支持中继和打洞，原生支持 IPv4、IPv6 和中继传输，并允许通过插件系统实现自定义传输。v1 版本保证线路协议和语言 API 的稳定性。

hackernews · chadfowler · Jun 15, 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48542480)

**背景**: 传统网络依赖可能变化的 IP 地址，导致连接中断。Iroh 使用公钥作为稳定标识符，类似于 Tailscale 在网络层的工作方式，但 Iroh 在应用层运作。它由专注于去中心化基础设施的公司 n0 开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.iroh.computer/blog/v1">Iroh 1.0 - Dial Keys, not IPs - Iroh</a></li>
<li><a href="https://github.com/n0-computer/iroh">GitHub - n0-computer/iroh: IP addresses break, dial keys ...</a></li>
<li><a href="https://www.iroh.computer/docs/overview">What is iroh? - iroh</a></li>

</ul>
</details>

**社区讨论**: 部分评论者将 Iroh 与 Tailscale 比较，也有人质疑其相比现有 IP 网络的必要性。开发者澄清，Iroh 支持自定义传输，专为希望简化 P2P 连接而不需要管理网络配置的应用开发者设计。

**标签**: `#peer-to-peer`, `#networking`, `#distributed-systems`, `#iroh`, `#release`

---

<a id="item-6"></a>
## [Hacker News 讨论用本地模型替代 Claude/GPT 进行日常编程](https://news.ycombinator.com/item?id=48542100) ⭐️ 8.0/10

Hacker News 用户正在分享他们成功用本地大语言模型替代 Claude 和 GPT 等付费 AI 编程助手的设置，理由是隐私、成本和性能方面的优势。 这一讨论突显出在消费级硬件上完全离线运行的隐私保护型免费 AI 编程工具的发展趋势，可能会减少对云端服务的依赖。 用户报告使用 Qwen3.6（35B、27B）和 Gemma 4-26B 等模型，在配备 128GB RAM 的 Mac Studio 或双 RTX 3090 等设备上，分别实现每秒 25-40 tokens 或高达每秒 150 tokens 的速度，并使用 Pi 和 LM Studio 等工具。

hackernews · cloudking · Jun 15, 14:46

**背景**: 本地大语言模型完全运行在用户自己的硬件上，无需将数据发送到外部服务器。llama.cpp 和 GGUF 格式等工具使得在消费级 GPU 或 Mac 上进行高效推理成为可能。每秒 tokens (toks/s) 是衡量实时编程辅助性能的关键指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.quietlycode.org/">Quietly - Offline AI IDE & Local Chat</a></li>
<li><a href="https://localaimaster.com/blog/best-ollama-models">Best Ollama Models 2026: 15 Ranked ( Coding ...) | Local AI Master</a></li>
<li><a href="https://www.bentoml.com/blog/beyond-tokens-per-second-how-to-balance-speed-cost-and-quality-in-llm-inference">Beyond Tokens-per-Second: How to Balance Speed, Cost, and Quality in LLM Inference</a></li>

</ul>
</details>

**社区讨论**: 社区总体持积极态度，许多用户分享了详细的硬件和模型配置。也存在一些怀疑，认为积极的体验可能是真实的，或者是 AI 提供商发布的。总的来说，用户强调本地模型对于日常编程来说“足够好”，同时免费且隐私。

**标签**: `#local-llm`, `#coding-assistant`, `#AI-privacy`, `#hacker-news-discussion`

---

<a id="item-7"></a>
## [福克斯提议收购 Roku，引发中立性担忧](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9) ⭐️ 8.0/10

福克斯公司提议收购领先的流媒体硬件和平台提供商 Roku，引发了对潜在内容偏见和服务无关架构丧失的担忧。 此次收购可能集中控制内容和分发，影响依赖 Roku 中立平台的数百万用户的观看体验。 据报道，该交易正在讨论中但尚未达成最终协议；Roku 的硬件运行专有操作系统，目前汇集了多个流媒体服务的内容，不偏向任何单一提供商。

hackernews · thm · Jun 15, 12:50 · [社区讨论](https://news.ycombinator.com/item?id=48540499)

**背景**: Roku 以其服务无关架构而闻名，意味着其平台不偏向任何流媒体服务。这种中立性受到希望获得硬件无关体验的用户的重视。福克斯作为大型内容提供商，拥有 Roku 可能会通过推广自身内容而破坏这种中立性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@imranmsa93/agnostic-vs-non-agnostic-services-the-balancing-act-of-modern-software-architecture-f712a9e4f1ec">Agnostic vs. Non-Agnostic Services: The Balancing Act of ...</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了强烈的悲观情绪，许多人认为不应允许福克斯购买对美国大量家庭电视硬件的直接访问权。用户还担心广告增加和潜在的偏见，一些人已转向 Nvidia Shield 等替代方案。

**标签**: `#acquisition`, `#media`, `#streaming`, `#hardware`, `#Roku`

---

<a id="item-8"></a>
## [Typst 0.15.0 新增多参考文献和 MathML 导出](https://typst.app/docs/changelog/0.15.0/) ⭐️ 8.0/10

Typst 0.15.0 支持在单个文档中使用多个参考文献，改进了数学公式的 HTML 和 MathML 导出，并持续优化脚注处理。 此次发布增强了 Typst 作为 LaTeX 严肃替代方案的地位，提供了更好的网页兼容性和灵活的参考文献管理，满足了用户的核心需求。 多参考文献功能允许每章或每节拥有独立的参考列表；数学公式在 HTML 导出时会自动转换为 MathML，提升了网页的可访问性和渲染效果。

hackernews · schu · Jun 15, 17:24 · [社区讨论](https://news.ycombinator.com/item?id=48544396)

**背景**: Typst 是一个开源的排版系统，旨在以更简单的语法和更快的编译速度取代 LaTeX。MathML（数学标记语言）是一种基于 XML 的标准，用于在网页中表示数学符号，是 HTML5 的一部分，可在浏览器中原生渲染。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MathML">MathML</a></li>

</ul>
</details>

**社区讨论**: 用户赞赏多参考文献和 MathML 导出功能，有人称多参考文献是他们的‘个人最爱’。然而，一名从软件开发转行的学生指出脚注仍有问题，尤其是在议论性脚注和参考文献引用方面。一位新用户询问 Typst 相比 org-mode 和 Pandoc 工作流的优势。

**标签**: `#typst`, `#typesetting`, `#release`, `#document-formatting`, `#open-source`

---

<a id="item-9"></a>
## [字节跳动洽购天数智芯 AI 芯片，并考虑百度昆仑芯](https://www.reuters.com/world/china/bytedance-talks-with-chinas-iluvatar-corex-purchase-ai-chips-sources-say-2026-06-15/) ⭐️ 8.0/10

字节跳动正与上海天数智芯洽谈采购用于推理任务的 AI 芯片，并同时考虑引入百度的昆仑芯。若交易达成，天数智芯将成为字节跳动继华为、寒武纪之后的第三大国产 GPU 供应商。 此举可能进一步多元化字节跳动的 AI 芯片供应链，并在美国出口限制下增强中国本土半导体生态系统。同时，随着字节跳动扩大其 AI 聊天机器人豆包的用户基础，对推理芯片的需求正日益增长。 天数智芯今年有望向字节跳动交付至少 5 万颗芯片，主要用于推理任务。字节跳动还考虑将百度的昆仑芯纳入供应商名单，凸显其国产芯片多元化战略。

telegram · zaihuapd · Jun 15, 06:53

**背景**: 由于美国制裁，字节跳动等中国科技巨头难以获得英伟达先进 GPU，转而寻求国产替代方案。天数智芯是一家总部位于上海的 GPGPU 初创公司，专注于 AI 计算；百度昆仑芯则是自主研发的 AI 加速器。字节跳动的 AI 聊天机器人豆包需要大量推理算力，这推动了对高效芯片的需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/world/china/bytedance-talks-with-chinas-iluvatar-corex-purchase-ai-chips-sources-say-2026-06-15/">Exclusive: ByteDance in talks with China's Iluvatar CoreX to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Iluvatar_CoreX">Iluvatar CoreX - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kunlunxin">Kunlunxin - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#ByteDance`, `#semiconductor`, `#supply chain`, `#China tech`

---

<a id="item-10"></a>
## [哪吒监控探针高危路径穿越漏洞 (CVSS 9.1)](https://github.com/nezhahq/nezha/security/advisories/GHSA-5c25-7vpj-9mqh) ⭐️ 8.0/10

哪吒监控（Nezha）v2.0.13 以下版本存在一个未授权路径穿越漏洞（CVE-2026-53519，CVSS 9.1），攻击者可通过构造 GET 请求（如 /dashboard../data/config.yaml）读取配置文件，获取其中的 JWT 密钥。 该漏洞极为危险，因为攻击者无需认证即可获取 JWT 密钥，可能完全控制监控系统，并对被管理的服务器发起进一步攻击。 该漏洞影响 Nezha v2.0.13 以下版本，CVSS 评分为 9.1（高危）。攻击者利用类似 /dashboard../data/config.yaml 的路径穿越模式即可绕过访问控制。

telegram · zaihuapd · Jun 15, 09:25

**背景**: 哪吒监控（Nezha）是一款开源自托管的服务器监控与运维工具。路径穿越（目录遍历）攻击利用对用户提供的文件名清理不足，使攻击者能读取预期目录之外的文件。JWT 密钥用于生成身份认证令牌，一旦泄露，攻击者可以伪造令牌获得管理员权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/nezhahq/nezha">GitHub - nezhahq/nezha: :trollface: Self-hosted, lightweight ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Path_traversal_vulnerability">Path traversal vulnerability</a></li>

</ul>
</details>

**标签**: `#security vulnerability`, `#path traversal`, `#Nezha`, `#open source`, `#CVSS 9.1`

---

<a id="item-11"></a>
## [开发者分享家庭实验室 AI 开发平台](https://rsgm.dev/post/ai-dev-platform/) ⭐️ 7.0/10

一位开发者发布了一篇详细的博客文章，介绍其使用 OpenCode 和 Forgejo 等开源工具搭建的个人家庭实验室 AI 开发平台。该文章引发了技术社区关于类似自托管 AI 开发环境的热烈讨论。 这篇文章突显了开发者自托管 AI 编码代理以保持对工具和数据控制的趋势。它鼓励知识共享，并为那些希望在家中构建自己的 AI 开发平台的人提供了一个实用的蓝图。 该设置包括一个持久的 OpenCode 服务器，并与 Forgejo 集成以进行版本控制。评论者指出了资源限制和测试速度等挑战，有些人更倾向于在主开发机器上运行编码代理。

hackernews · rsgm · Jun 15, 15:09 · [社区讨论](https://news.ycombinator.com/item?id=48542433)

**背景**: 家庭实验室 AI 开发平台是指开发者在自己的硬件上运行 AI 驱动的编码代理和开发工具的个人化自托管环境。编码代理是能够自主执行编写、审查和编辑代码等任务的 AI 系统。这种方法提供了隐私和定制性，但需要大量资源和技术知识。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Coding_agent">Coding agent</a></li>
<li><a href="https://www.faros.ai/blog/best-ai-coding-agents-2026">Best AI Coding Agents for 2026: Real-World Developer Reviews</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了热情，许多人分享了类似的设置。一些人指出了挑战，如资源限制（例如，OpenCode 的虚拟机性能）和测试速度。一位用户感谢这篇文章激励他们撰写自己的 AI 实验室，而另一位用户则提出了 Quad9 DNS 阻止域名的问题。

**标签**: `#homelab`, `#AI development`, `#self-hosting`, `#coding agent`

---

<a id="item-12"></a>
## [《指挥官基恩》引擎白皮书](https://forgottenbytes.net/commander_keen.html) ⭐️ 7.0/10

一篇详细分析《指挥官基恩》游戏引擎的白皮书已发布，重点介绍了其用于平滑滚动的创新自适应瓦片刷新技术。 这一深入的技术探讨突出了早期 PC 游戏开发中的关键突破，展示了约翰·卡马克的工作如何在图形能力有限的硬件上实现了流畅的平台游戏，并影响了整个行业。 自适应瓦片刷新技术利用 EGA/VGA 适配器的硬件偏移来滑动屏幕缓冲区，当可视区域到达缓冲区边缘时仅重新绘制变化的瓦片，这在《指挥官基恩》和《基恩之梦》中均有体现。

hackernews · mfiguiere · Jun 15, 17:52 · [社区讨论](https://news.ycombinator.com/item?id=48544781)

**背景**: 在 20 世纪 90 年代初，PC 缺乏专门的滚动硬件，使得平滑移动变得困难。id Software 的约翰·卡马克开发了自适应瓦片刷新（ATR）技术，利用显卡的偏移寄存器高效滚动。该技术对《指挥官基恩》等游戏至关重要，将主机级别的横版滚动体验带到了 PC 上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Adaptive_tile_refresh">Adaptive tile refresh - Wikipedia</a></li>
<li><a href="https://fabiensanglard.net/ega/">Commander Keen's Adaptive Tile Refresh - Fabien Sanglard</a></li>
<li><a href="https://retrocomputing.stackexchange.com/questions/22141/did-john-carmack-really-invent-adaptive-tile-refresh">Did John Carmack really invent "Adaptive Tile Refresh"?</a></li>

</ul>
</details>

**社区讨论**: 评论者对白皮书表示赞赏，有人推荐《毁灭战士大师》一书以了解卡马克和罗梅罗工作的背景。其他人提到需要解释为什么强大的 PC 在精灵渲染方面落后于 SNES 等主机，并提供了游玩《指挥官基恩》和分析类似游戏（如 Cosmodoc）的链接。

**标签**: `#game development`, `#retro gaming`, `#id Software`, `#game engines`, `#John Carmack`

---

<a id="item-13"></a>
## [Hetzner 宣布云服务器大幅涨价](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers) ⭐️ 7.0/10

Hetzner 宣布大幅提高云服务器价格，部分价格上涨至原来的三倍，原因是硬件稀缺和人工智能工作负载需求激增。 这家欧洲主要云服务商的调价行为，反映了人工智能驱动的硬件需求对云成本的广泛影响，可能冲击依赖 Hetzner 廉价价格的初创企业和中小企业。 新价格适用于云服务器，部分机型涨幅达三倍。Hetzner 还标准化了其服务器产品线，这也可能促成了价格变动。

hackernews · tuhtah · Jun 15, 13:19 · [社区讨论](https://news.ycombinator.com/item?id=48540844)

**背景**: Hetzner 是一家德国网络托管和云计算提供商，以价格低廉著称。该公司将此次涨价归因于全球硬件短缺，尤其是内存和存储的短缺，而人工智能热潮加剧了对计算资源的需求，进一步推高了成本。

**社区讨论**: 社区反应不一，用户对三倍涨价表示震惊，指出 25-50%的涨幅可以理解，但三倍价格过于极端。部分评论者将涨价与人工智能驱动的硬件短缺及贫富差距扩大联系起来，而另一些人则指出 Hetzner 近年来缺乏硬件更新。

**标签**: `#cloud pricing`, `#hardware scarcity`, `#Hetzner`, `#AI infrastructure`, `#HackerNews discussion`

---

<a id="item-14"></a>
## [TimescaleDB Hypercore 压缩：最高 98%压缩比](https://roszigit.com/en/blog/timescaledb-compression-hypercore) ⭐️ 7.0/10

TimescaleDB 的压缩功能利用 hypercore 列式存储和类型感知算法，在时间序列数据上实现高达 98%的压缩比，这在一篇技术博客文章中得到了详细说明。 这使得 PostgreSQL 能够在大幅降低存储成本的同时处理大规模时间序列工作负载，同时保持可查询性，对物联网、监控和分析应用具有吸引力。 压缩通过 segmentby 和 orderby 参数配置，并依赖于名为 Hypercore 的混合行-列式存储引擎。它需要额外的许可证，而非 TimescaleDB 核心使用的 Apache 2.0。

hackernews · lkanwoqwp · Jun 15, 17:29 · [社区讨论](https://news.ycombinator.com/item?id=48544451)

**背景**: TimescaleDB 是一个开源的时间序列数据库，作为 PostgreSQL 的扩展构建。时间序列数据因重复模式和可预测结构而通常压缩效果好。传统的行式存储牺牲了分析效率以换取插入速度，但列式存储可以提高压缩和分析查询性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://roszigit.com/en/blog/timescaledb-compression-hypercore">TimescaleDB Compression: Hypercore and Columnar Storage with up to 98% Ratio in PostgreSQL</a></li>
<li><a href="https://docs.timescale.com/use-timescale/latest/hypercore/">Tiger Data Documentation | Hypercore</a></li>
<li><a href="https://dev.to/philip_mcclarence_2ef9475/timescaledb-compression-a-complete-guide-to-95-storage-reduction-2mo4">TimescaleDB Compression: A Complete Guide to 95%+ Storage ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了压缩与查询性能之间的权衡，有人指出字典编码可能会拖慢读取速度。用户还讨论了 deltax 扩展等替代方案，并质疑 TimescaleDB 压缩是否使有损压缩在物联网中变得多余。一条批评意见称‘高达’的说法具有误导性，另一条指出许可证限制可能导致标准软件包不包含压缩支持。

**标签**: `#TimescaleDB`, `#compression`, `#time-series`, `#PostgreSQL`, `#database`

---

<a id="item-15"></a>
## [自制真空管中的玻璃-金属密封技术](https://maurycyz.com/projects/glass/1/) ⭐️ 7.0/10

一位爱好者发布了一份详细指南，介绍如何为自制真空管制作玻璃-金属密封，涵盖实用技术和材料。该文章探讨了通过匹配热膨胀实现气密密封的挑战。 这一知识对于有志于从零搭建真空管的 DIY 电子爱好者至关重要，有助于保存历史技术。它还为材料科学和精密玻璃加工提供了见解，可应用于其他高真空场景。 该指南可能区分了匹配密封与非匹配密封，使用热膨胀系数接近硼硅玻璃的 Kovar 或 Dumet 等金属。社区成员补充了 Galinstan、Fernico 等材料，并指出了形成适当氧化层的重要性。

hackernews · zdw · Jun 14, 15:52 · [社区讨论](https://news.ycombinator.com/item?id=48528587)

**背景**: 玻璃-金属密封是真空管的关键部件，用于为电引线提供气密通道。主要挑战是匹配玻璃和金属的热膨胀系数（CTE）以防止冷却时开裂。常见的解决方案包括使用 Kovar 或 Dumet 等热膨胀系数与硼硅玻璃相近的合金，或对非匹配材料采用压缩密封。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Glass-to-metal_seal">Glass-to-metal seal - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区成员贡献了技术见解：tliltocatl 讨论了 Galinstan 低蒸汽压但附着力问题；alister 询问工业方法；crispyambulance 建议使用带 O 型圈的金属端板；tyingq 指出预制霓虹灯电极是廉价替代品；mmmlinux 强调了历史上使用的 Fernico 和 Dumet 材料。

**标签**: `#vacuum tubes`, `#glassworking`, `#DIY electronics`, `#materials science`

---

<a id="item-16"></a>
## [蚂蚁集团测试 AI 版支付宝，原生 AI 界面](https://www.chinastarmarket.cn/detail/2399277) ⭐️ 7.0/10

据报道，蚂蚁集团正在测试一款 AI 版支付宝，该版本拥有原生 AI 界面，用户可一键进入更智能的服务和资金管理。上线时间未定，蚂蚁集团拒绝评论。 这标志着支付宝这一全球最大支付平台之一的重大 UI 转变，将 AI 直接融入用户交互。如果得到确认，可能为金融科技领域的 AI 优先设计树立先例，影响数亿用户。 据报道，新版本将改变现有用户界面，实现一键进入原生 AI 界面，使服务和资金管理更加智能。不过，该报道基于 Telegram 频道的传闻，尚无官方确认。

telegram · zaihuapd · Jun 14, 12:43

**背景**: 支付宝是蚂蚁集团运营的中国主流移动支付平台，拥有超过十亿用户。在此类广泛使用的应用中集成 AI，可能改变人们与金融服务交互的方式，从手动导航转向 AI 驱动式辅助。

**标签**: `#AI`, `#fintech`, `#Alipay`, `#Ant Group`, `#mobile payment`

---

<a id="item-17"></a>
## [小红书传月底在港秘密提交 IPO 申请](https://www.bloomberg.com/news/articles/2026-06-15/xiaohongshu-is-said-to-ready-hong-kong-ipo-filing-this-month) ⭐️ 7.0/10

据知情人士透露，小红书正筹备在 2026 年 6 月底前向香港交易所秘密提交 IPO 申请，这可能成为近年港交所最大的上市交易之一。 IPO 将为小红书投资者提供重要的流动性机会，并可能为中国社交电商平台树立估值基准。这也表明对香港 IPO 市场的信心，并凸显生活方式与社交电商日益增长的全球影响力。 小红书在 2024 年融资时估值约 170 亿美元，二次交易中升至 310 亿美元。公司预计 2025 年利润约 30 亿美元。IPO 的具体时间、规模和估值仍在讨论中。

telegram · zaihuapd · Jun 15, 11:03

**背景**: 小红书常被称为中国版 Instagram，是中国重要的生活方式与社交电商平台，与抖音竞争。去年 TikTok 在美短暂遭禁期间，其国际版 RedNote 一度爆红。在香港的秘密 IPO 申请允许公司在审核过程中保密财务细节，这是大型上市企业的常见做法。

**标签**: `#IPO`, `#Xiaohongshu`, `#Hong Kong`, `#social commerce`, `#tech news`

---

<a id="item-18"></a>
## [Rio 3.5 模型被曝套壳中国开源模型](https://mp.weixin.qq.com/s/0oYevRBT8PPxG5hudOXxug) ⭐️ 7.0/10

Nex 团队揭露之前被誉为开源 SOTA 的 Rio 3.5 模型其实是 Nex 和 Qwen 的混合产物，混合比例约 0.57:0.43。Rio 团队随后致歉并从 HuggingFace 下架该模型。 这一事件凸显了开源 AI 社区中模型“套壳”的持续问题，引发了关于透明度和归属的伦理担忧。同时也侧面证明了中国开源基础模型的强大，以至于被他人用作基底。 Nex 团队发现，去掉系统提示词后，Rio 3.5 有 79% 的概率自称 Nex，并能复述 Nex 独有的机构介绍。权重分析显示，Rio 的权重精确落在 Nex 与 Qwen 的连线上，共线性超过 0.98。

telegram · zaihuapd · Jun 15, 12:39

**背景**: “套壳”是指将现有模型（通常通过 API 或权重混合）包装成新界面并冒充自有模型的做法。Rio 3.5 模型自称新的开源 SOTA，但被发现是两种现有中国开源模型——Nex 和 Qwen（阿里通义千问）的线性组合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260615A04B7E00">一夜反转！「杀进第一梯队」的巴西LLM竟「套壳缝合」了国产模型</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen_(Alibaba_Cloud)">Qwen (Alibaba Cloud)</a></li>

</ul>
</details>

**标签**: `#开源模型`, `#套壳`, `#AI伦理`, `#社区争议`

---

<a id="item-19"></a>
## [消费者起诉 Anthropic，称 AI 订阅计划限额不实](https://www.wsj.com/tech/ai/anthropic-sued-over-limits-on-its-200-a-month-ai-plans-e2a109e4) ⭐️ 7.0/10

华盛顿特区一名消费者对 Anthropic 提起集体诉讼，指控其每月 100 美元和 200 美元的'Max 5x'和'Max 20x'订阅计划实际使用上限低于宣传承诺。 这起诉讼是对 AI 订阅透明度最早的法律挑战之一，可能迫使公司明确披露使用上限和退款政策，影响数百万用户。 原告要求为自 2024 年 4 月以来购买这些计划的用户退款，并引用 Anthropic 在 2025 年 7 月的一封内部邮件作为证据。

telegram · zaihuapd · Jun 15, 14:17

**背景**: Anthropic 是一家以 Claude 系列语言模型闻名的 AI 公司。它提供分层订阅计划，包括 Claude Pro（每月 20 美元）以及更昂贵的'Max'计划，声称提供 5 倍或 20 倍于 Pro 版本的用量。诉讼认为这些宣传具有欺骗性，因为实际使用上限低得多且未明确告知。

**标签**: `#Anthropic`, `#AI订阅`, `#消费者诉讼`, `#透明度`

---