---
layout: default
title: "Horizon Summary: 2026-07-31 (ZH)"
date: 2026-07-31
lang: zh
---

> From 38 items, 12 important content pieces were selected

---

1. [DeepSeek V4 Flash 0731：前沿级 AI，低成本](#item-1) ⭐️ 9.0/10
2. [Tailscale 分析 Hugging Face 入侵事件：认证密钥泄露](#item-2) ⭐️ 8.0/10
3. [电梯算法剖析：连接调度与真实世界行为](#item-3) ⭐️ 8.0/10
4. [QM：YC 支持的多人智能体工作工具，提供个人作用域与共享房间](#item-4) ⭐️ 8.0/10
5. [DeepSeek V4 正式版 7 月中旬上线，API 引入峰谷定价](#item-5) ⭐️ 8.0/10
6. [华为开源 920 亿参数 openPangu-2.0-Flash 模型](#item-6) ⭐️ 8.0/10
7. [Anthropic 将对美国战争部供应链风险认定提起法律挑战](#item-7) ⭐️ 8.0/10
8. [SIGGRAPH 时间检验奖：获奖研究提前十年押中物理 AI](#item-8) ⭐️ 7.0/10
9. [火山引擎推出 Seedance 2.0 mini，单秒成本约 0.5 元](#item-9) ⭐️ 7.0/10
10. [特斯拉评估出售中国业务，为潜在 SpaceX 合并铺路](#item-10) ⭐️ 7.0/10
11. [MiniMax 将于 8 月 3 日开源多模态视频模型 H3](#item-11) ⭐️ 7.0/10
12. [美国最高法院拒绝受理 AI 版权案，维持人类作者要求](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Flash 0731：前沿级 AI，低成本](https://artificialanalysis.ai/models/deepseek-v4-flash) ⭐️ 9.0/10

DeepSeek 发布了 V4 Flash 0731，一个托管在 Hugging Face 上的前沿级 AI 模型，价格远低于同级别竞品。该发布在 Hacker News 上引发了热烈讨论，获得 497 分和 273 条评论。 该发布挑战了 AI 模型在性价比上的现状，以极低的成本提供接近前沿水平的智能。这可能会给 OpenAI 等竞争对手带来压力，并让日常开发者用得起先进 AI，减少『token 焦虑』。 据社区基准测试，DeepSeek V4 Flash 0731 在每百万输出 token 约 0.28 美元的价格下，可与 GLM 5.2 和 Gemini 3.6 等模型匹敌或胜出。该模型还可以通过 Unsloth 无损 Q8 量化在 162GB 的本地硬件上运行，并且预计很快会推出更新的 Pro 版本。

hackernews · theanonymousone · Jul 31, 07:59 · [社区讨论](https://news.ycombinator.com/item?id=49120299)

**背景**: DeepSeek 是一家以发布开放权重模型而闻名的中国 AI 公司。『Flash』变体针对更低成本和更快推理进行了优化，而『Pro』模型则追求最大能力。该模型托管在 Hugging Face——一个流行的模型分享平台上。Hacker News 的讨论反映出人们对价格实惠且性能出色的 AI 的需求日益增长。

**社区讨论**: 评论者非常热情，称该模型『很棒』并且是『日常主力工具』，并指出它以每百万输出 token 0.28 美元的价格提供了 GLM/Gemini 级别的智能。人们还好奇是否会出现与 Opus 5 相当的新 V4 Pro，也有评论将它与 OpenAI 的产品比较，或者询问 Hugging Face 的托管成本经济学。

**标签**: `#AI`, `#DeepSeek`, `#machine learning`, `#model release`, `#price-performance`

---

<a id="item-2"></a>
## [Tailscale 分析 Hugging Face 入侵事件：认证密钥泄露](https://tailscale.com/blog/hugging-face-intrusion) ⭐️ 8.0/10

Tailscale 发布了一篇对 Hugging Face 入侵事件的事后剖析，其中一枚可重用的认证密钥被泄露，并被用于在几天内向 Hugging Face 的 tailnet 注册了 181 个未经授权的 CI 节点。Tailscale 并未被利用，但承认未能阻止这一入侵。 这件事意义重大，因为它显示一家主流安全厂商在公开剖析自家产品在一场高调入侵中的角色，强调安全团队必须把任何入侵都当作自己的入侵来认真对待，即使产品本身未被利用。它提醒 Tailscale 用户和安全社区关注认证密钥管理与告警机制的不足。 攻击者利用了保存在环境文件中的 Tailscale 可重用认证密钥，将 181 个节点注册进 Hugging Face 的 tailnet，每个节点都获得了 CI 身份标签及相应的权限。Tailscale 指出事件中没有发现或利用 Tailscale 的漏洞，但仍认为这暴露了告警方面的改进空间。

hackernews · bluehatbrit · Jul 31, 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49127306)

**背景**: Tailscale 提供零配置的软件定义网状 VPN，可让设备通过互联网安全互联。认证密钥是向 tailnet 注册设备的凭据；如果可重用密钥泄露，攻击者就能注册恶意节点，除非该密钥被限制或撤销。这一事件凸显了访问控制系统中密钥管理和监控的重要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tailscale">Tailscale</a></li>
<li><a href="https://tailscale.com/docs/features/access-control/auth-keys">Auth keys · Tailscale Docs</a></li>
<li><a href="https://tailscale.com/docs/reference/key-secret-management">Key and secret management · Tailscale Docs</a></li>

</ul>
</details>

**社区讨论**: 评论者们大多称赞 Tailscale 的透明复盘，称这是"非常聪明的营销"，同时也有教育意义。也有人指出，对新节点大量注册缺乏告警是一个错失的机会，并建议 Tailscale 增加"安全检查"功能，帮助用户判断配置是否符合最佳实践。

**标签**: `#security`, `#Tailscale`, `#incident-response`, `#access-management`, `#CI/CD`

---

<a id="item-3"></a>
## [电梯算法剖析：连接调度与真实世界行为](https://john.fun/elevators) ⭐️ 8.0/10

一篇关于电梯算法的深度分析文章在 Hacker News 引发热议，文章将电梯调度与磁盘调度中的 SCAN、LOOK 等概念以及目的地派梯联系起来。文章探讨了这些算法在理论上和真实电梯系统中的表现。 电梯调度影响着每天数百万乘客的体验，这篇文章将日常系统与计算机科学中的基础调度概念联系起来。讨论揭示了理论算法与人类行为之间的相互作用，对系统设计者和爱好者都有参考价值。 文章涉及 SCAN、LOOK 和目的地派梯算法，并指出在随机目的地的模拟中，目的地派梯的表现可能更差。评论者补充说，真实建筑中常见大量乘客从一楼前往同一楼层的模式，这可能会影响算法效果评估。

hackernews · Jrh0203 · Jul 31, 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49124218)

**背景**: 电梯算法又称 SCAN，是一种磁盘调度策略：磁盘臂像电梯上下运行一样在盘面上往复移动，按顺序处理请求。目的地派梯（Destination Dispatch）是多电梯建筑的优化方案，乘客在键盘上输入目标楼层，系统据此将同层乘客分组。这些概念是操作系统课程中讲解请求调度与公平性的经典例子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Elevator_algorithm">Elevator algorithm - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Destination_dispatch">Destination dispatch - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/operating-systems/disk-scheduling-algorithms/">Disk Scheduling Algorithms - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论积极而热烈。评论者分享了自己的编程项目，推荐了电梯调度游戏 Elevatorsaga，并指出电梯与硬盘驱动器之间的类比。也有人不赞同文章对目的地派梯的批评，认为真实出行模式与随机目的地模拟并不一致。

**标签**: `#elevator-algorithms`, `#scheduling`, `#systems`, `#hacker-news`, `#destination-dispatch`

---

<a id="item-4"></a>
## [QM：YC 支持的多人智能体工作工具，提供个人作用域与共享房间](https://github.com/yc-software/qm) ⭐️ 8.0/10

YC 支持的 qm 发布了开源的多人在线 agent（智能体）工作工具，引入个人作用域（per-person scopes）和共享房间（shared rooms），让公司级助手可以在 Slack 和 Web 上协作。该项目源于 YC 内部运行 50 多个 agent 的经验。 这很重要，因为大多数 agent 都是按个人助手设计的，要让它们服务整个公司会很快变得复杂；qm 提供了一种作用域模型，被社区称为公司级助手的“合理答案”。它与 AQ、Buzz 等项目一起，验证了多人在线 agent 工具这一新兴方向。 QM 是开源项目，专为初创公司设计，让每位员工和每个项目都能拥有一个类似 OpenClaw 的 agent，并支持个人作用域与共享作用域。用户既可以自定义属于自己的 agent，也能在 Slack 频道和项目中协作；不过组织级上下文和安全处理仍是用户希望进一步了解的问题。

hackernews · tosh · Jul 31, 18:04 · [社区讨论](https://news.ycombinator.com/item?id=49126604)

**背景**: Agent harness（智能体框架/工具链）是围绕大语言模型（LLM）的软件基础设施，负责管理工具调用、记忆、状态持久化和反馈循环，使模型能够作为 AI agent 运行。目前大多数 agent 产品都针对个人使用优化，要让它们服务整个公司就会面临权限、上下文和协作等问题。qm 通过“个人作用域 + 共享房间”来解决这些问题，类似于人类在频道和项目中协作的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/yc-software/qm">GitHub - yc-software/qm: Multiplayer agent harness for work · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://qm.ycombinator.com/">QM — Open-Source Agent Harness from YC</a></li>

</ul>
</details>

**社区讨论**: 评论者总体持肯定态度，称其作用域方式是“合理答案”，并认为这验证了多人 agent 方向；同时也有评论将其与 Claude Cowork、Orca 等替代品进行比较。有人希望看到 qm 与 Cowork 的对比，也有人表示想深入研究组织级上下文、安全问题，以及 Hermes 是否是最好的类 OpenClaw agent。

**标签**: `#LLM`, `#agents`, `#multiplayer`, `#tooling`, `#YC`

---

<a id="item-5"></a>
## [DeepSeek V4 正式版 7 月中旬上线，API 引入峰谷定价](https://t.me/zaihuapd/42888) ⭐️ 8.0/10

DeepSeek 宣布 DeepSeek V4 正式版计划于 7 月中旬上线，并同步调整 API 定价，引入峰谷定价机制。高峰时段（北京时间每日 9:00-12:00、14:00-18:00）价格更高，调价前 24 小时会通过邮件通知用户。 这是一次重要的 AI 模型发布，直接影响开发者的使用成本和负载调度方式。峰谷定价在 LLM API 中较为少见，可能促使开发者将非紧急负载转移到非高峰时段，进而影响整个行业的定价策略。 以 deepseek-v4-pro 为例，每百万 tokens 的价格为：输入缓存命中平时 0.025 元、高峰 0.05 元；缓存未命中 3 元和 6 元；输出 6 元和 12 元。deepseek-v4-flash 的对应价格未在公告中完整展示。

telegram · zaihuapd · Jul 31, 05:50

**背景**: DeepSeek API 默认启用上下文缓存（Context Caching），命中缓存的 token 会按更低价格计费，这是 LLM API 中常见的降本功能，可复用输入前缀来减少费用。峰谷定价则在需求高峰时段加价，形成另一层成本调节手段。7 月中旬的发布延续了 DeepSeek 此前模型更新的节奏，因性能和价格优势备受开发者关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/guides/kv_cache/">DeepSeek API Docs</a></li>
<li><a href="https://chat-deep.ai/docs/deepseek-context-caching/">DeepSeek Context Caching Explained - Chat- Deep .ai</a></li>
<li><a href="https://pristren.com/blog/prompt-caching-anthropic-openai-guide/">Prompt Caching With Anthropic and OpenAI: How to... | Pristren Blog</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI`, `#API Pricing`, `#Model Release`

---

<a id="item-6"></a>
## [华为开源 920 亿参数 openPangu-2.0-Flash 模型](https://t.me/zaihuapd/42889) ⭐️ 8.0/10

2026 年 6 月 30 日，华为开源了拥有 920 亿总参数的大语言模型 openPangu-2.0-Flash。首批发布内容包括模型权重、基础推理代码以及训推算子，并已在 GitCode 的昇腾社区上线。 这是中国 AI 领域的重要举措：华为加入开源大模型行列，同时为自家昇腾硬件提供原生支持。它为开发者提供了不依赖传统 GPU 生态的另一种选择，并强化了华为构建全栈 AI 软硬件生态的战略。 该模型采用混合专家（MoE）架构，每个 token 仅激活 6 亿参数，并支持 512K 超长上下文。华为还宣布，openPangu-2.0-Pro 的模型权重和基础推理代码将于 7 月上线，更多组件将在下半年陆续开源。

telegram · zaihuapd · Jul 31, 06:50

**背景**: 华为于 2021 年 7 月首次发布盘古（Pangu）基础模型，后来扩展到气象预测、医疗等行业专用模型。openPangu 是华为的开源 AI 模型品牌，旨在为昇腾原生训练与推理提供最佳实践参考。昇腾系列是华为的 AI 处理器产品线，GitCode 的昇腾社区是这些开源资源的分发平台。MoE 模型通过每次输入只激活部分参数，在扩大总参数量的同时降低推理成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pandaily.com/huawei-openpangu-2.0-flash-open-source-jun2026">Huawei Open-Sources 92B-Parameter openPangu-2.0-Flash Model - Pandaily</a></li>
<li><a href="https://app.dealroom.co/news/feed/huawei-launches-openpangu-2-0-flash-92b-parameter-open-source-ai-model">Huawei launches openPangu-2.0-Flash, 92B-parameter open-source AI model | Dealroom.co</a></li>
<li><a href="https://www.kucoin.com/news/flash/huawei-open-sources-9-2b-parameter-openpangu-2-0-flash-model">Huawei open-sources the 9.2B-parameter openPangu-2.0-Flash model | KuCoin</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Source`, `#Huawei`, `#Large Language Model`, `#openPangu`

---

<a id="item-7"></a>
## [Anthropic 将对美国战争部供应链风险认定提起法律挑战](https://t.me/zaihuapd/42891) ⭐️ 8.0/10

Anthropic 于 2025 年 3 月 5 日宣布，将对美国战争部将其 Claude AI 模型认定为国家安全供应链风险的决定提起法律挑战。 这是领先 AI 公司与美国政府之间就 AI 供应链安全问题展开的一次重大法律对抗，可能影响 AI 采购、国家安全政策以及产业与政府关系。其结果可能为 AI 模型如何评估国家安全风险开创先例。 该认定适用范围狭窄，仅适用于客户将 Claude 直接用于与战争部合同相关的用途。过渡期内，Anthropic 将继续以名义成本向战争部及国家安全社区提供模型和工程师支持。

telegram · zaihuapd · Jul 31, 08:00

**背景**: 美国政府一直在依据《联邦采购供应链安全法案》(FASCSA) 和国防部供应链风险管理程序等授权，加强对信息和通信技术的供应链安全管控。这些措施允许政府发布供应链风险认定和命令，以降低供应商带来的威胁。Anthropic 的挑战关键在于，依据这些法律，该认定是否具备合法依据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalregister.gov/documents/2023/10/05/2023-21320/federal-acquisition-regulation-implementation-of-federal-acquisition-supply-chain-security-act">Federal Register :: Federal Acquisition Regulation: Implementation of...</a></li>
<li><a href="https://www.dau.edu/sites/default/files/2025-07/DoD+SCRM+Guidebook+FINAL+V3A+(OGC).pdf">UNCLASSIFIED UNCLASSIFIED DoD Supply Chain Risk Management Guidebook</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#Anthropic`, `#regulation`, `#national security`, `#legal challenge`

---

<a id="item-8"></a>
## [SIGGRAPH 时间检验奖：获奖研究提前十年押中物理 AI](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247908730&idx=2&sn=0b3a81693cb5f92800c95b7fc50939f1) ⭐️ 7.0/10

ACM SIGGRAPH 公布了 2026 年时间检验奖（Test-of-Time Award），表彰十多年来持续产生深远影响的论文。相关报道指出，其中一项获奖研究如今被视为在“物理 AI”概念流行之前就已提前押中了这一方向。 该奖项表明，图形学与交互技术中的基础研究可能要等到整个领域追上来之后才会获得广泛认可。它验证了物理 AI 正成为人工智能与机器人领域的重要方向，也鼓励研究者投身更具长期价值的问题。 时间检验奖是 SIGGRAPH 年度技术论文奖（Technical Papers Awards）的一部分，授予影响力持续超过十年的工作。同一条新闻汇总中还提到一个 GitHub Star 数超过 8000 的开源项目，以及机器人身体与灵巧手协同训练的研究。

rss · 量子位 · Jul 31, 06:32

**背景**: 物理 AI（Physical AI）指的是能够运用运动技能理解并与真实世界互动的 AI 模型，通常搭载于机器人或自动驾驶车辆等自主机器中。SIGGRAPH 时间检验奖今年已是第四届，旨在表彰影响力持续超过十年的技术论文，往届获奖者包括 Embree CPU 光线追踪框架。这一背景解释了为何一篇十年前发表的论文，会在今天被称赞为押中了物理 AI 浪潮。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>
<li><a href="https://www.ibm.com/think/topics/physical-ai">What is Physical AI? | IBM</a></li>
<li><a href="https://blog.siggraph.org/2026/05/siggraph-2026-technical-papers-awards-best-papers-honorable-mentions-and-test-of-time.html/">SIGGRAPH 2026 Technical Papers Awards: Best Papers, Honorable Mentions, and Test-of-Time - ACM SIGGRAPH Blog</a></li>

</ul>
</details>

**标签**: `#SIGGRAPH`, `#physical AI`, `#test-of-time award`, `#AI research`, `#robotics`

---

<a id="item-9"></a>
## [火山引擎推出 Seedance 2.0 mini，单秒成本约 0.5 元](https://t.me/zaihuapd/42885) ⭐️ 7.0/10

6 月 15 日，火山引擎旗下火山方舟体验中心上线了 Seedance 2.0 mini 视频生成模型，按 720P 规格折算单秒生成成本约 0.5 元，较上一代 Seedance 2.0 降低约 50%，近期将开放 API 服务。 这一显著的成本降低让大规模 AI 视频生成对企业更加友好，尤其适用于电商内容、营销素材和 UGC 创作等场景。同时，这也表明国内 AI 视频生成模型厂商之间的价格竞争正在加剧。 Seedance 2.0 mini 是一款轻量级模型，定位快速、高批量的创意生产而非电影级制作，支持生成 4-15 秒的片段，并具备镜头运动、角色一致性等功能。它主要面向电商内容、营销素材批量生成和特效玩法等高频率、大规模应用场景。

telegram · zaihuapd · Jul 31, 04:16

**背景**: 火山方舟（Volcano Ark）是字节跳动旗下火山引擎的大模型服务平台，于 2023 年 6 月发布，提供模型精调、评测、推理等平台服务。Seedance 是字节跳动的视频生成模型系列，mini 版本在画质上有所取舍，但显著降低了推理成本，使 AI 视频生成能够用于高频、大规模的商业场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://seedancemini.net/">Seedance 2 . 0 Mini - Lower-Cost AI Video Generator online</a></li>
<li><a href="https://kie.ai/seedance-2-0-mini">Seedance 2 . 0 Mini API – Faster, Lower-Cost Seedance AI Video Model</a></li>
<li><a href="https://baike.baidu.com/item/火山方舟/63145443">火山方舟_百度百科</a></li>

</ul>
</details>

**标签**: `#AI`, `#video-generation`, `#volcano-engine`, `#seedance`, `#cost-reduction`

---

<a id="item-10"></a>
## [特斯拉评估出售中国业务，为潜在 SpaceX 合并铺路](https://t.me/zaihuapd/42886) ⭐️ 7.0/10

据《华尔街日报》报道，特斯拉正评估出售或拆分其中国业务，以便在地缘政治风险下将中国与美国业务分离，并可能为与 SpaceX 的合并铺平道路。 中国是特斯拉第二大市场，因此出售或拆分中国业务将是一项重大战略调整。这也可能在潜在的 SpaceX 合并之前重塑特斯拉的公司架构，影响投资者、员工以及全球电动汽车格局。 报道称，马斯克曾要求高管在特斯拉美国与中国业务之间划出一道“激光线”，以便更容易拆分；他希望若两国发生地缘政治冲突，至少美国业务能够存续。目前此事仍属猜测，尚未得到官方确认。

telegram · zaihuapd · Jul 31, 04:59

**背景**: 特斯拉是美国电动汽车制造商，在中国拥有重要生产和销售业务，包括上海超级工厂。SpaceX 是马斯克创办的太空探索公司；两者合并将把汽车与航天业务结合起来，但考虑到 SpaceX 为私有公司、特斯拉为上市公司，合并将面临监管和治理方面的障碍。

**社区讨论**: 未提供社区讨论内容，因此无法总结相关观点。

**标签**: `#Tesla`, `#SpaceX`, `#China`, `#Business Strategy`, `#Geopolitics`

---

<a id="item-11"></a>
## [MiniMax 将于 8 月 3 日开源多模态视频模型 H3](https://modelscope.cn/models/MiniMax/MiniMax-H3) ⭐️ 7.0/10

MiniMax 宣布其通用多模态视频模型 H3 将于 2026 年 8 月 3 日在魔搭社区（ModelScope）开源发布。H3 原生支持在单一上下文中对文本、图像、音频和视频的理解与生成。 这一发布意义重大，因为开源权重的多模态视频模型能够使先进的视频生成与编辑能力更加普及，惠及开发者和创意从业者。同时，这也反映出 AI 视频生成领域日益激烈的竞争与开放趋势。 据第三方信息，H3 可生成 5 至 15 秒、最高 2K 分辨率、24fps 且带原生立体声的视频片段。该模型面向影视、广告、电商和游戏等商业创意场景，并具备精细化的编辑控制能力。

telegram · zaihuapd · Jul 31, 12:37

**背景**: 多模态视频模型是能够在同一模型中处理和生成多种类型数据（如文本、图像、音频和视频）的 AI 系统。MiniMax H3 也被称为 Hailuo 3.0，是一个开源权重的通用模型，可接受混合输入并生成连贯的视频输出。开源模型意味着其权重公开发布，允许开发者进行微调、自托管和集成到自己的产品中。魔搭社区（ModelScope）是一个中国的人工智能模型托管与服务平台，提供模型探索、推理、训练和部署等功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://fal.ai/minimax-h3">MiniMax H3 - Open-Weights General-Purpose Multimodal Video Model | fal</a></li>
<li><a href="https://morphic.com/resources/models/minimax-h3">MiniMax H3 (Hailuo 3.0): full specs and input limits</a></li>

</ul>
</details>

**标签**: `#multimodal`, `#video generation`, `#open-source`, `#AI model`, `#MiniMax`

---

<a id="item-12"></a>
## [美国最高法院拒绝受理 AI 版权案，维持人类作者要求](https://t.me/zaihuapd/42900) ⭐️ 7.0/10

美国最高法院于 3 月 2 日拒绝受理 Stephen Thaler 的上诉，维持下级法院关于 AI 生成作品因缺乏人类作者而不受版权保护的裁定。这实际上确认了美国版权局坚持的“人类创作”核心原则。 这一裁决为生成式 AI 领域的创作者和企业提供了明确指引：完全由 AI 生成的作品无法获得美国版权保护。这可能影响 AI 公司和用户对 AI 生成内容的权属、授权及投资安排。 该案涉及 Thaler 的 AI 系统 DABUS 独立创作的一件视觉艺术品。最高法院未发表意见，因此既有法律原则保持不变，未来案件仍存不确定性。

telegram · zaihuapd · Jul 31, 13:11

**背景**: DABUS（统一感知自主引导装置）是 Stephen Thaler 创建的人工智能系统，据报道能在无人直接指导下构思发明和创作作品。美国版权局和下级法院一直认为，版权法要求“人类作者”，这一原则源于宪法将版权视为激励人类创作者的制度。该案是全球范围内关于 AI 生成成果是否应受知识产权保护的更广泛争议的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DABUS">DABUS</a></li>
<li><a href="https://grokipedia.com/page/DABUS">DABUS</a></li>

</ul>
</details>

**标签**: `#AI版权`, `#法律`, `#生成式AI`, `#知识产权`, `#DABUS`

---