---
layout: default
title: "Horizon Summary: 2026-05-14 (ZH)"
date: 2026-05-14
lang: zh
---

> From 37 items, 13 important content pieces were selected

---

1. [Bun 运行时从 Zig 重写为 Rust，已合并](#item-1) ⭐️ 9.0/10
2. [NGINX 曝 18 年远程代码执行漏洞 CVE-2026-42945](#item-2) ⭐️ 9.0/10
3. [美国批准向中国主要企业销售 H200 AI 芯片](#item-3) ⭐️ 9.0/10
4. [DeepSeek 对话系统会话隔离漏洞泄露用户对话](#item-4) ⭐️ 9.0/10
5. [苹果 M5 上首个公开 macOS 内核内存损坏漏洞利用](#item-5) ⭐️ 8.0/10
6. [RTX 5090 加持 M4 MacBook Air：eGPU 游戏与 AI 突破](#item-6) ⭐️ 8.0/10
7. [MIT 校长就资金和人才管道危机发表讲话](#item-7) ⭐️ 8.0/10
8. [开发者反思 AI 让自己变笨与技能衰退](#item-8) ⭐️ 8.0/10
9. [Anthropic 与 SpaceX 合作，双倍提升 Claude Code 限额](#item-9) ⭐️ 8.0/10
10. [移除 2024 款 RAV4 混动版的调制解调器和 GPS](#item-10) ⭐️ 7.0/10
11. [全球肥胖趋势：富国趋稳，穷国加速](#item-11) ⭐️ 7.0/10
12. [京东上线 AI 硬件自营专区，包含受制裁 NVIDIA GPU](#item-12) ⭐️ 7.0/10
13. [ChatGPT 安卓版拆解发现 Codex 远程桌面控制功能](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Bun 运行时从 Zig 重写为 Rust，已合并](https://github.com/oven-sh/bun/pull/30412) ⭐️ 9.0/10

Bun JavaScript 运行时已从 Zig 完全重写为 Rust，这一大规模代码迁移的拉取请求已被合并到主分支。 这次重写标志着一个流行 JavaScript 运行时的重大范式转变，有望提升内存安全性并利用 Rust 生态系统。它可能影响其他运行时项目在语言选择和大规模迁移方面的方式。 合并后产生了超过 100 万行 Rust 代码，使 Bun 的 Rust 代码库规模与 Rust 编译器本身相当。代码库中在 736 个文件中使用了超过 10,000 个 `unsafe` 块，表明为了性能或底层操作而大量依赖 unsafe Rust。

hackernews · Chaoses · May 14, 08:15 · [社区讨论](https://news.ycombinator.com/item?id=48132488)

**背景**: Bun 是一款快速的全能 JavaScript 运行时，内置打包器、转译器和 npm 客户端。它最初使用 Zig（一种旨在替代 C 的现代系统编程语言）构建。迁移到 Rust 可能是为了利用 Rust 更强的安全性保障和更丰富的库生态系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**社区讨论**: 社区评论对一周内完成的快速迁移表示惊讶，并注意到从 Zig 到 Rust 惯用法映射的细致准备。一些用户对大量使用 unsafe Rust 以及对近期采用者的影响表示担忧，而另一些用户则讨论了现在超过 100 万行 Rust 代码库的整体复杂性。

**标签**: `#bun`, `#rust`, `#zig`, `#javascript`, `#runtime`

---

<a id="item-2"></a>
## [NGINX 曝 18 年远程代码执行漏洞 CVE-2026-42945](https://depthfirst.com/research/nginx-rift-achieving-nginx-rce-via-an-18-year-old-vulnerability) ⭐️ 9.0/10

2026 年 5 月 13 日，NGINX 的 ngx_http_rewrite_module 模块中被披露一个严重堆缓冲区溢出漏洞（CVE-2026-42945，CVSS 9.2），影响 0.6.27 至 1.30.0 版本及多个企业产品。该漏洞自 2008 年潜伏至今，允许未经身份验证的攻击者通过构造的 HTTP 请求实现远程代码执行。 NGINX 是全球使用最广泛的 Web 服务器，服务于数十亿台服务器。该漏洞潜伏期长、CVSS 评分高，对云原生基础设施构成严重威胁，尤其是 Kubernetes Ingress 控制器和 API 网关。 漏洞源于两遍执行脚本引擎中的状态不一致：当 rewrite 指令的替换字符串包含问号时，缓冲区大小被低估，导致第二遍执行时发生堆溢出。缓解措施包括升级至 NGINX 1.31.0/1.30.1，或将未命名捕获组（$1）替换为命名捕获组。

telegram · zaihuapd · May 14, 02:41

**背景**: NGINX 是一种高性能 Web 服务器和反向代理，广泛应用于现代云架构。ngx_http_rewrite_module 允许使用 PCRE 正则表达式进行 URL 重写。漏洞位于其两遍执行脚本引擎中：第一遍计算所需缓冲区长度，第二遍拷贝数据。处理问号时'is_args'标志的错误导致缓冲区大小计算错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://guo365.github.io/study/nginx.org/en/docs/http/ngx_http_rewrite_module.html">Module ngx _ http _ rewrite _ module</a></li>
<li><a href="https://blog.rankiteo.com/f51778747583-f5-vulnerability-may-2026/">F5: Critical 18-Year-Old NGINX Vulnerability Enables Remote Code Execution Attacks</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，公开的概念验证假设 ASLR 已关闭，一些人因此低估风险。但研究者声称可绕过 ASLR。其他人指出利用前提需要特定的 rewrite 和 set 指令，且使用命名捕获组的缓解措施简单直接。一些用户质疑使用内存安全语言（如 Caddy）的替代方案是否更好。

**标签**: `#nginx`, `#security`, `#vulnerability`, `#CVE-2026-42945`, `#RCE`

---

<a id="item-3"></a>
## [美国批准向中国主要企业销售 H200 AI 芯片](https://www.reuters.com/business/retail-consumer/us-clears-h200-chip-sales-10-china-firms-nvidia-ceo-looks-breakthrough-2026-05-14/) ⭐️ 9.0/10

美国商务部已批准向约 10 家中国企业（包括阿里巴巴、腾讯、字节跳动）销售英伟达 H200 AI 芯片，单一客户最多可购买 7.5 万颗。但目前尚未完成任何交付，部分中国企业在政府指导下持谨慎态度。 这一政策转变可能显著影响 AI 硬件供应链和地缘政治格局，代表了对华先进 AI 芯片出口管制的罕见放松。此举或加速中国 AI 发展，同时考验国产芯片与外来技术获取之间的平衡。 H200 GPU 基于 Hopper 架构，配备 141GB HBM3e 内存和 4.8 TB/s 带宽，容量几乎是 H100 的两倍。联想和富士康等分销商也获得许可，英伟达 CEO 黄仁勋近期访华被视为推动交易落地的一部分。

telegram · zaihuapd · May 14, 08:57

**背景**: H200 是英伟达最新 AI 芯片，专为大规模机器学习工作负载设计。对华先进 AI 芯片出口管制一直是美中科技竞争的关键战场，此前已对 H100 实施限制。与此同时，中国政府一直在推动国产 AI 芯片开发作为替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H200 GPU | NVIDIA</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#AI chips`, `#geopolitics`, `#Nvidia`, `#tech trade`

---

<a id="item-4"></a>
## [DeepSeek 对话系统会话隔离漏洞泄露用户对话](https://github.com/deepseek-ai/DeepSeek-R1/issues/840) ⭐️ 9.0/10

在 DeepSeek 的网页版和 API 对话模型中发现了一个会话隔离漏洞：在全新空对话中仅发送未闭合的 '<think' 字符串，模型就会返回其他用户的对话历史片段，其中可能包含代码、密钥和隐私等敏感信息。 这一严重漏洞对 DeepSeek 用户构成大规模隐私风险，因为它可能泄露其他用户的聊天敏感数据。该事件突显了广泛使用的 AI 聊天机器人系统中持续存在的安全挑战以及加强会话隔离的必要性。 该漏洞由报告者 cancat2024 于 2026 年 5 月 11 日负责任地披露，他并未加以利用。社区讨论指出第三方部署也同样受影响，表明该问题可能是模型幻觉而非纯粹的工程缺陷。

telegram · zaihuapd · May 14, 13:15

**背景**: 会话隔离是一种安全机制，确保每个用户的对话历史相互隔离，其他用户无法访问。在基于大语言模型（LLM）的聊天机器人（如 DeepSeek）中，不同用户的提示不应相互影响响应。该漏洞可能源于模型的训练数据或上下文处理方式：未闭合的 '<think' 令牌触发了对其他会话的意外检索，类似于 LLM 中的数据泄露问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chatbot">Chatbot - Wikipedia</a></li>
<li><a href="https://owasp.org/www-project-top-10-for-large-language-model-applications/Archive/0_1_vulns/Data_Leakage.html">LLM02:2023 - Data Leakage</a></li>

</ul>
</details>

**社区讨论**: 社区成员指出第三方部署也出现此问题，表明这可能是模型幻觉而非简单的工程缺陷。这暗示根本原因可能与模型的训练数据或架构有关。

**标签**: `#security`, `#vulnerability`, `#deepseek`, `#AI`, `#privacy`

---

<a id="item-5"></a>
## [苹果 M5 上首个公开 macOS 内核内存损坏漏洞利用](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 8.0/10

Calif 团队公开了苹果 M5 芯片上的首个内核内存损坏漏洞利用，允许本地未授权代码破坏内核内存。 这是一个重大的安全发现，因为它针对新型 M 系列芯片，可能对 macOS 安全和苹果的漏洞赏金计划产生严重影响。 该漏洞利用据报道绕过了 MTE（内存标记扩展），并且完整的 55 页报告已公开。该漏洞在苹果的赏金计划中可能价值 10 万美元，但在黑市上可以卖得更高。

hackernews · quadrige · May 14, 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48139219)

**背景**: 内核内存损坏漏洞允许攻击者获得内核级访问权限，可能危及整个系统。苹果 M5 芯片包含 MTE 等安全功能以防止此类攻击，但此漏洞利用展示了绕过技术。类似漏洞 CVE-2025-24151 已于 2025 年 3 月被苹果修复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cve.news/cve-2025-24151/">CVE-2025-24151 - macOS Kernel Memory Corruption Vulnerability ...</a></li>
<li><a href="https://core.ac.uk/download/pdf/324187567.pdf">A Study on Kernel Memory Protection and</a></li>

</ul>
</details>

**社区讨论**: 评论对 MTE 绕过表示怀疑，并讨论了该漏洞在苹果赏金计划中的估值。一些用户开玩笑说这是虚假漏洞，而其他人则担心对 M5 安全的影响。

**标签**: `#macOS`, `#kernel exploit`, `#Apple M5`, `#security`, `#vulnerability`

---

<a id="item-6"></a>
## [RTX 5090 加持 M4 MacBook Air：eGPU 游戏与 AI 突破](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 8.0/10

一位开发者成功将 RTX 5090 作为 eGPU 与 M4 MacBook Air 配合使用，运行了要求高的游戏并提升了 LLM 提示处理速度，克服了 Apple Silicon 缺乏官方 eGPU 支持的问题。 这展示了绕过 Apple Silicon eGPU 限制的方法，可能使 Mac 用户能够运行此前在这些机器上无法实现的 GPU 密集型游戏和 AI 工作负载。 该设置通过 GPU 直通到虚拟机实现，存在 1.5 GB 内存窗口限制，使过程复杂化。文章报告了 LLM 提示处理的显著改进，这是 Apple Silicon 已知的瓶颈。

hackernews · allenleee · May 14, 15:47 · [社区讨论](https://news.ycombinator.com/item?id=48137145)

**背景**: eGPU 是通过 Thunderbolt 连接的外部 GPU 扩展坞，但 Apple Silicon Mac 缺乏官方支持。GPU 直通允许虚拟机直接访问物理 GPU，但在 Apple Silicon 上需要底层变通方法。RTX 5090 是 NVIDIA 最新的高端 GPU，通常用于 PC。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-au/102363">Use an external graphics processor with your Mac – Apple Support (AU)</a></li>
<li><a href="https://forums.macrumors.com/threads/is-apple-silicon-m1-m2-chips-not-compatible-with-egpu.2370757/">Is Apple Silicon M1/M2 chips not compatible with eGPU ?</a></li>
<li><a href="https://www.youtube.com/watch?v=9OfoFAljPn4">GPU Passthrough on Linux and Docker for AI, ML, and Plex - YouTube</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞了这一技术成就，matthewfcarlson 提到他多年来一直请求 VM GPU 直通。Aurornis 强调 LLM 改进特别有价值。geerlingguy 评论了这一进展，但希望苹果能提供更好的支持。

**标签**: `#eGPU`, `#MacBook`, `#GPU passthrough`, `#LLM`, `#gaming`

---

<a id="item-7"></a>
## [MIT 校长就资金和人才管道危机发表讲话](https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline) ⭐️ 8.0/10

MIT 校长莎莉·科恩布鲁斯发布视频讲话，讨论学术研究资金和人才管道面临的挑战，指出资助率下降以及吸引和留住学生的困难。 这一讲话表明，即使是 MIT 这样的顶尖机构也面临系统性的资金压力，这可能会重塑美国的创新生态系统和学术研究的未来。 讲话聚焦财政政策和资助下降，指出未获得资助的学生不太可能接受录取，这直接影响了人才管道。

hackernews · dmayo · May 14, 14:51 · [社区讨论](https://news.ycombinator.com/item?id=48136262)

**背景**: 美国研究型大学严重依赖联邦资助来支持研究生和科研项目。资助成功率下降和津贴停滞不前使得学术界对人才的吸引力降低，可能导致关键领域的人才短缺。

**社区讨论**: 评论者对学术界普遍感到失望，指出博士项目艰苦、薪酬低、就业前景黯淡。一些人认为大学面临的预算压力早该出现，而另一些人则警告说，代际更迭可能导致许多学校关闭。

**标签**: `#academia`, `#research funding`, `#talent pipeline`, `#higher education`, `#innovation`

---

<a id="item-8"></a>
## [开发者反思 AI 让自己变笨与技能衰退](https://jpain.io/god-damn-ai-is-making-me-dumb/) ⭐️ 8.0/10

一位开发者发表了题为《AI 让我变笨》的博客文章，表达了对过度依赖 AI 编码工具正在侵蚀其编程技能和批判性思维能力的担忧。该文章在 HackerNews 上引发了热烈讨论，获得了 329 个点赞和 212 条评论。 这场讨论凸显了 AI 辅助编码带来的生产力提升与技能衰减风险之间日益加剧的张力，尤其是对于初级开发者和学习新语言的开发者而言。术语“vibe coding”已被创造出来，用以描述不加仔细审查就接受 AI 生成代码的做法，这引发了关于开发者长期能力和代码质量的质疑。 博客作者描述了自己因依赖 AI 处理之前能独立完成的任务而感到“变笨”。社区评论者分享了类似经历，有人指出 AI 使得新工作的上手变得更困难，而另一些人则表示他们仍有强迫症般地去检查 AI 的输出，从而保持了自身技能。

hackernews · Eighth · May 14, 18:19 · [社区讨论](https://news.ycombinator.com/item?id=48139148)

**背景**: “Vibe coding”一词由计算机科学家 Andrej Karpathy 于 2025 年 2 月创造，指的是一种 AI 辅助软件开发实践：开发者描述需求后直接接受 AI 生成的代码而不进行深入审查。批评者认为这种做法会导致责任缺失、可维护性问题和安全漏洞。更广泛的“技能衰减”概念描述了技能在不被积极使用时会退化，这一现象在高风险行业中已有研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://safetyinsights.org/2022/04/21/factors-influencing-attenuating-skill-decay-in-high-risk-industries-a-scoping-review/">Factors Influencing Attenuating Skill Decay in High-Risk Industries...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪存在分歧；一些开发者承认依赖 AI 会感到不安，并努力审查和补充 AI 的输出，而另一些开发者则欢迎 AI 带来的生产力提升（尤其是在个人项目中），但警告不能盲目信任。多位评论者强调技能衰退的风险是真实的，特别是对于初级开发人员或转向不熟悉语言的人而言，这与博客的担忧一致。

**标签**: `#AI`, `#developer-experience`, `#skill-attenuation`, `#HackerNews-discussion`

---

<a id="item-9"></a>
## [Anthropic 与 SpaceX 合作，双倍提升 Claude Code 限额](https://t.me/zaihuapd/41371) ⭐️ 8.0/10

Anthropic 宣布与 SpaceX 达成合作，将使用 Colossus 1 数据中心全部算力，该中心拥有超过 22 万块 NVIDIA GPU。此举使 Claude Code 所有付费方案的 5 小时速率限制翻倍，取消了 Pro/Max 用户的高峰期限制，并显著提高了 Claude Opus 的 API 速率限制。 这一合作大幅提升了 Anthropic 的算力，直接改善了 Claude Code 和 API 用户的体验。它标志着 AI 实验室从非传统合作伙伴获取大规模 GPU 集群的趋势，可能重塑基础设施竞争格局。 Colossus 1 数据中心最初由 xAI 建造，被认为是全球最大的 AI 超级计算机，一个月内可提供超过 300 兆瓦新增容量和 22 万块 GPU。这项合作引人注目，因为埃隆·马斯克与 OpenAI 存在法律纠纷，而 Anthropic 保持独立立场。

telegram · zaihuapd · May 14, 00:57

**背景**: Claude 是 Anthropic 开发的一系列大语言模型，Claude Code 是其中用于编程的智能体工具。Colossus 是由 xAI（埃隆·马斯克的 AI 公司）建造的超级计算机，于 2024 年 7 月投入使用。Anthropic 与 SpaceX（或 xAI）的合作为其提供了大量额外算力，用于训练和推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.servethehome.com/anthropic-signs-spacex-colossus-1-data-center-to-boost-capacity/">Anthropic Signs SpaceX Colossus 1 Data Center to... - ServeTheHome</a></li>
<li><a href="https://en.wikipedia.org/wiki/Colossus_(supercomputer)">Colossus (supercomputer) - Wikipedia</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Claude Code overview - Claude Code Docs</a></li>

</ul>
</details>

**标签**: `#AI`, `#infrastructure`, `#GPU`, `#Anthropic`, `#Claude`

---

<a id="item-10"></a>
## [移除 2024 款 RAV4 混动版的调制解调器和 GPS](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 7.0/10

一位用户记录了从 2024 款 RAV4 混动版中移除调制解调器和 GPS 以禁用远程信息处理数据传输的过程，并为注重隐私的车主提供了分步指南。 该指南回应了人们对车载远程信息处理日益增长的隐私担忧，特别是关于丰田与保险公司共享数据的指控，并赋予车主直接采取行动的能力。 作者警告称，即使在移除调制解调器后，通过蓝牙连接手机仍会使汽车利用手机的网络连接发送遥测数据，而有线 USB 连接则不会触发此行为。

hackernews · arkadiyt · May 14, 17:08 · [社区讨论](https://news.ycombinator.com/item?id=48138136)

**背景**: 现代车辆配备有远程信息处理控制单元（TCU），用于收集并传输位置、速度及驾驶习惯等数据至云服务。这些数据常与第三方（包括保险公司）共享，引发隐私担忧。移除 TCU 的调制解调器和 GPS 可从物理上禁用这些传输，但通过蓝牙的替代数据路径可能仍然存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telematic_control_unit">Telematic control unit</a></li>
<li><a href="https://www.laptopmag.com/news/bluetooth-is-riddled-with-nasty-security-flaws-your-devices-could-be-in-trouble">Bluetooth is riddled with nasty security flaws — your... | Laptop Mag</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，蓝牙仍可通过手机的网络连接泄露数据，并建议仅使用有线 USB 连接 CarPlay。其他人提到了如拔掉 Ford Maverick 保险丝等替代方法，另有一位用户报告了 CarPlay 的 GPS 指南针问题，而丰田拒绝修复。

**标签**: `#privacy`, `#telematics`, `#automotive`, `#hardware mod`, `#toyota`

---

<a id="item-11"></a>
## [全球肥胖趋势：富国趋稳，穷国加速](https://www.nature.com/articles/s41586-026-10383-0) ⭐️ 7.0/10

一项覆盖 200 个国家、2.32 亿人的大规模研究发现，高收入国家的肥胖率自 2000 年代以来已趋于稳定或略有下降，而中低收入国家的肥胖率仍在持续稳定或加速上升。 这种分化表明，社会经济因素可以遏制肥胖流行，但如果没有政策干预，发展中国家将面临日益严重的公共卫生危机。该发现对全球健康战略至关重要。 该研究分析了 1980 年至 2024 年的数据。在富裕国家，儿童青少年肥胖率自 1990 年代起减速，2000 年后趋于稳定，意大利、法国等国家甚至出现小幅下降；成人肥胖趋势也呈现类似模式。

telegram · zaihuapd · May 14, 09:45

**背景**: 肥胖是糖尿病、心脏病等慢性疾病的主要风险因素。以往研究认为全球肥胖率普遍上升，但这项新分析揭示了更细微的图景：高收入国家可能因食物环境改善和公共卫生措施而实现稳定。

**标签**: `#public health`, `#obesity`, `#global health`, `#epidemiology`, `#nutrition`

---

<a id="item-12"></a>
## [京东上线 AI 硬件自营专区，包含受制裁 NVIDIA GPU](https://u.jd.com/HaDkFMa) ⭐️ 7.0/10

京东开设“AI 硬件京东自营专区”，首批上架 NVIDIA GeForce RTX 5090 32G 涡轮版、RTX PRO 6000 Blackwell 服务器版及 H100 等硬件，这些产品此前因美国出口制裁而受限。 此举可能表明出口管制有所松动或被规避，使中国 AI 企业和研究人员能够获得训练大模型所需的高端 NVIDIA GPU，从而可能加速中国 AI 发展。 RTX 5090 涡轮版为无阉割的全球统一规格；RTX PRO 6000 面向专业渲染与数据中心；H100 此前因制裁而暂停对华出口。

telegram · zaihuapd · May 14, 15:15

**背景**: NVIDIA GPU，尤其是 H100 和基于 Blackwell 架构的 RTX PRO 6000，广泛用于 AI 训练和推理。自 2022 年以来，美国对向中国出口先进 AI 芯片实施限制，以限制其 AI 能力。京东是中国最大的电商平台之一，其自营专区通常确保产品正品和现货供应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/">The Engine Behind AI Factories | NVIDIA Blackwell Architecture</a></li>
<li><a href="https://www.tomshardware.com/news/nvidia-tsmc-rush-orders-before-china-sanctions">Nvidia Reportedly Asks TSMC to Rush Lucrative GPU Orders Before...</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#NVIDIA`, `#export sanctions`, `#JD.com`, `#GPU availability`

---

<a id="item-13"></a>
## [ChatGPT 安卓版拆解发现 Codex 远程桌面控制功能](https://t.me/zaihuapd/41388) ⭐️ 7.0/10

对 ChatGPT 安卓版 1.2026.125 版本的 APK 拆解发现，OpenAI 正在为 Codex 开发手机远程控制桌面会话的功能，允许用户在手机上查找并重连远程桌面会话。 该功能将允许开发者通过手机管理编程任务，提升灵活性，并可能将 Codex 的应用场景扩展到桌面环境之外。 该功能要求手机和桌面端登录同一账号，目前仍在开发中，尚未公布正式上线时间。

telegram · zaihuapd · May 14, 21:48

**背景**: OpenAI Codex 是一套 AI 代理套件，旨在自动化软件工程任务，如编码、重构和代码审查。APK 拆解是通过反编译安卓应用包来检查未发布功能或开发中的变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex">OpenAI Codex - Wikipedia</a></li>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#ChatGPT`, `#APK teardown`, `#remote desktop`

---