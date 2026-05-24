---
layout: default
title: "Horizon Summary: 2026-05-24 (ZH)"
date: 2026-05-24
lang: zh
---

> From 37 items, 15 important content pieces were selected

---

1. [APKPure 上的 Telegram 官方版被植入间谍后门](#item-1) ⭐️ 9.0/10
2. [LLM 代理在代码生成中表现出约束衰减](#item-2) ⭐️ 8.0/10
3. [微软开源最早 DOS 源代码](#item-3) ⭐️ 8.0/10
4. [16 字节演示程序写录将代码压缩推向极致](#item-4) ⭐️ 8.0/10
5. [AMD Vivado 2026.1 免费版移除 Linux 支持](#item-5) ⭐️ 8.0/10
6. [微软内部大力推广 Claude Code，面向非技术员工](#item-6) ⭐️ 8.0/10
7. [微软财报披露 OpenAI 单季巨亏 115 亿美元](#item-7) ⭐️ 8.0/10
8. [监管机构拟对富途、老虎证券处以巨额罚款](#item-8) ⭐️ 8.0/10
9. [海盗船采用长鑫存储 DRAM，DDR5 价格有望下调](#item-9) ⭐️ 8.0/10
10. [我国日均词元调用量两年增千倍](#item-10) ⭐️ 8.0/10
11. [澳大利亚四天工作周研究显示生产力提升](#item-11) ⭐️ 7.0/10
12. [内存占 AI 芯片组件成本近三分之二](#item-12) ⭐️ 7.0/10
13. [Usborne 1980 年代计算机图书合集重温](#item-13) ⭐️ 7.0/10
14. [诈骗者滥用微软内部账户发送垃圾邮件](#item-14) ⭐️ 7.0/10
15. [特朗普政府拟要求绿卡申请人离境办理](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [APKPure 上的 Telegram 官方版被植入间谍后门](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

APKPure 上的 Telegram 12.6.5 版本被重新签名并注入了 DataCollector 间谍框架，可窃取聊天记录、通讯录、照片等数据。 这种供应链攻击危及广泛使用的即时通讯应用用户，泄露敏感个人数据。它凸显了第三方应用商店即使对官方应用也存在风险。 后门使用 AES-GCM 加密将数据外泄至 C2 服务器 38.190.225.166，并通过一个包含 3000 多行代码的 classes3.dex 文件注入。

telegram · zaihuapd · May 24, 11:38

**背景**: APKPure 是一个第三方 Android 应用商店，分发 Google Play 之外的 APK 文件。Telegram 是一款流行的安全即时通讯应用。此类供应链攻击发生在合法软件在分发过程中被篡改时，通常通过非官方渠道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apkpure.com/">APKPure: Download APK on Android with Free APK Downloader</a></li>
<li><a href="https://any.run/report/6e5190d6637c2657bd8a0dcb744b514c56c4d9926f62487842a31b33856003ec/b4867a69-ee19-44b3-8215-4f82f4ce2c88">Malware analysis DataCollector.exe Malicious activity | ANY ...</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#telegram`, `#supply-chain attack`, `#APKPure`

---

<a id="item-2"></a>
## [LLM 代理在代码生成中表现出约束衰减](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

研究人员的一项系统研究揭示了基于 LLM 的编码代理中存在一种称为“约束衰减”的现象，即尽管它们在无约束任务上表现出色，但在被迫遵循明确的架构规则时，其性能显著下降。 这一发现凸显了当前 LLM 代理在生产级后端开发中的不可靠性，将其应用限制在快速原型设计，并引发了对其在关键软件工程工作流中采用的担忧。 由于成本限制，该研究未全面测试前沿模型，因此具体性能数据可能无法反映最新模型。该论文聚焦于需要严格遵守架构规则的后端代码生成任务。

hackernews · wek · May 24, 12:55 · [社区讨论](https://news.ycombinator.com/item?id=48256912)

**背景**: LLM 代理是结合大型语言模型与推理、记忆和工具使用的系统，能够自主完成任务。在软件工程中，它们可以根据自然语言提示生成代码。约束衰减是指这些代理在必须处理明确的架构约束时性能下降，而与之相对的是在无限制情况下生成代码的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introduction-to-llm-agents/">Introduction to LLM Agents | NVIDIA Technical Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了与研究发现相符的个人经验，指出代理在架构约束下表现更差，并建议采用逐步引入约束或使用示例文件等技术。一位用户引入了“钙化”一词，描述代理过度遵循模式时，模式可能主导代码库的现象。

**标签**: `#LLM agents`, `#code generation`, `#software engineering`, `#AI reliability`

---

<a id="item-3"></a>
## [微软开源最早 DOS 源代码](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 8.0/10

微软开源了已知最早的 DOS 源代码，这些代码由余峰高和里奇·奇尼领导的 DOS 反汇编小组从纸质打印稿中精心数字化而来。 此次发布保留了一段基础性的计算历史，为开发者提供了窥视个人计算机软件早期发展的难得机会，突显了早期操作系统的简洁性。 该源代码由几千行汇编语言组成；微软还开源了配套的 BASIC 代码。由于没有数字副本，数字化过程需要手动转录和扫描。

hackernews · DamnInteresting · May 24, 01:21 · [社区讨论](https://news.ycombinator.com/item?id=48253386)

**背景**: DOS（磁盘操作系统）是 20 世纪 80 年代占主导地位的 PC 操作系统，最初由微软为 IBM 开发。此次开源的版本代表了已知最早的 DOS 开发阶段，早于数字存储时代。

**社区讨论**: 社区成员对微软的发布表示感谢，一些评论指出配套的 BASIC 代码同样重要。其他人则惊叹于当时仅靠几千行汇编代码就能创立一家成功的软件公司。

**标签**: `#open source`, `#DOS`, `#Microsoft`, `#software history`, `#retro computing`

---

<a id="item-4"></a>
## [16 字节演示程序写录将代码压缩推向极致](https://hellmood.111mb.de/wake_up_16b_writeup.html) ⭐️ 8.0/10

一篇关于 16 字节演示程序的详细写录已发布，该程序能产生视觉输出，展示了极致的代码压缩水平。该演示及其解释突出了将图形程序压缩到仅 16 字节的技术。 这一成就突破了演示场景和代码高尔夫社区的可能边界，激励了超紧凑编程的进一步创新。它表明即使在极端尺寸限制下，也能实现创意且视觉吸引人的结果，影响嵌入式系统和底层优化的实践。 该可执行文件仅 16 字节大小，使其成为有史以来最小的演示之一。写录解释了作者如何利用自修改代码、指令重叠以及精心选择的机器指令来实现视觉输出。

hackernews · MaximilianEmel · May 24, 00:30 · [社区讨论](https://news.ycombinator.com/item?id=48253060)

**背景**: 演示场景是一个计算机艺术亚文化，专注于创作演示：即独立产生视听展示的程序。代码高尔夫是一项竞技编程活动，参与者力求编写尽可能短的代码。尺寸受限的引导程序，如 4K 或 64K 引导程序，是常见的竞赛类别；16 字节演示是这种挑战的极端形式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Demoscene">Demoscene</a></li>
<li><a href="https://en.wikipedia.org/wiki/Code_golf">Code golf</a></li>

</ul>
</details>

**社区讨论**: 社区表达了高度热情，一位评论者指出它激发了对递归 PowerPoint 谢尔宾斯基三角等相关主题的深入探索。其他人称赞该作品为杰作，并反思了尺寸极限，建议在其他架构上进一步探索。

**标签**: `#demoscene`, `#code golf`, `#compression`, `#16-byte demo`, `#retro programming`

---

<a id="item-5"></a>
## [AMD Vivado 2026.1 免费版移除 Linux 支持](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD 的 Vivado 2026.1 从免费 Basic 版本中移除了 Linux 支持，Linux 用户需要每年支付 1200 美元订阅费。免费许可证也仅限单机 Windows 安装。 这一决定疏远了依赖 Linux 进行 FPGA 开发的学生、爱好者和研究人员，可能将他们推向 Lattice 或 Intel 等竞争对手。这表明 AMD 战略转变，可能损害其生态发展。 免费 Basic 版本现在仅支持 Windows；Linux 用户必须升级到每年 1200 美元的 Standard 付费版本。此外，免费许可证限制为单机绑定。

hackernews · zdw · May 24, 04:14 · [社区讨论](https://news.ycombinator.com/item?id=48254309)

**背景**: AMD 于 2022 年收购了 Xilinx，继承了 Vivado——Xilinx FPGA 的主要 IDE。之前的免费 WebPACK 版本支持 Linux，使得广大开发者社区能够使用。许多 FPGA 开发者偏好 Linux，因其工具链集成和脚本能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://byteiota.com/amd-vivado-drops-linux-free-tier-fpga/">AMD Vivado Drops Linux: Free FPGA Tools Cost $1,200 Now</a></li>
<li><a href="https://www.amd.com/en/products/software/adaptive-socs-and-fpgas/vivado/vivado-licensing-options.html">AMD Vivado™ Licensing Options | Flexible Subscription ...</a></li>
<li><a href="https://www.eevblog.com/forum/fpga/new-licencing-for-vivadovitis-2026-1/">New licencing for Vivado/Vitis 2026.1 - Page 1 - EEVblog</a></li>

</ul>
</details>

**社区讨论**: 社区表达了强烈反对，长期用户批评此举有悖于生态系统发展。一些用户报告称已转向 Lattice，因其更好的 Linux 支持和许可条款。对额外费用和付费许可的管理麻烦感到沮丧。

**标签**: `#FPGA`, `#AMD`, `#Linux`, `#Vivado`, `#developer tools`

---

<a id="item-6"></a>
## [微软内部大力推广 Claude Code，面向非技术员工](https://t.me/zaihuapd/41535) ⭐️ 8.0/10

微软正在其工程团队中广泛推广 Anthropic 的 Claude Code，甚至鼓励非技术员工用于原型设计，并要求软件工程师将其与 GitHub Copilot 进行对比。 这一举措标志着 AI 编程工具格局可能发生转变，微软优先考虑最佳工具而非自家产品，可能推动 Claude Code 在企业中的更广泛应用，并影响 AI 编码助手之间的竞争格局。 CoreAI 团队以及负责 Windows、Microsoft 365 和 Outlook 的部门被要求安装 Claude Code，工程师需要提供对比 GitHub Copilot 的反馈。

telegram · zaihuapd · May 23, 06:05

**背景**: Claude Code 是 Anthropic 开发的一款代理式编程工具，运行在终端中，能够理解代码库，并通过自然语言命令执行任务、解释代码和处理 git 工作流，帮助开发者更快编程。对于没有工程背景的用户来说，它也是进入软件开发的一个入口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system</a></li>
<li><a href="https://github.com/anthropics/claude-code">GitHub - anthropics/claude-code: Claude Code is an agentic ...</a></li>

</ul>
</details>

**标签**: `#AI coding`, `#Claude Code`, `#GitHub Copilot`, `#Microsoft`, `#AI tools`

---

<a id="item-7"></a>
## [微软财报披露 OpenAI 单季巨亏 115 亿美元](https://t.me/zaihuapd/41537) ⭐️ 8.0/10

微软最新财报披露，其对 OpenAI 的权益法投资导致单季度净利润减少 31 亿美元，据此推算 OpenAI 该季度净亏损约 115 亿美元。 这一披露凸显了人工智能领域极高的烧钱速度，引发了对这种高支出可持续性以及微软等主要投资者潜在回报的质疑。 基于微软持有 OpenAI 约 27%的股权计算，季度亏损约 115 亿美元；若按税前损失和实际 32.5%持股比例计算，亏损可能超过 120 亿美元。

telegram · zaihuapd · May 23, 07:40

**背景**: 权益法是一种会计处理方法，当投资者对被投资单位具有重大影响（通常持股 20%-50%）时采用。根据权益法，投资者需按持股比例将被投资单位的净利润或亏损计入自身利润表。微软持有 OpenAI 约 27%的股权，目前已投入 116 亿美元，占其承诺投资 130 亿美元的绝大部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dongao.com/zjzcgl/zjkjsw/201905131026788.shtml">权 益 法 下可辨认净 资 产公允价值与账面价值怎么调整_东奥会计在线</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Microsoft`, `#AI financials`, `#quarterly loss`, `#investment`

---

<a id="item-8"></a>
## [监管机构拟对富途、老虎证券处以巨额罚款](https://t.me/zaihuapd/41539) ⭐️ 8.0/10

中国监管机构拟对富途控股处以 18.5 亿元罚款，对老虎证券子公司处以 4.11 亿元罚款，因其未获许可开展跨境证券业务。 这标志着对离岸交易平台的一次重大打击，影响依赖这些服务进入海外市场的中国投资者，并表明监管机构对跨境证券活动采取更严格的立场。 处罚包括没收违法所得及可能的业务暂停；富途 CEO 李华还面临 125 万元的个人罚款。这些罚款是初步的，有待最终决定。

telegram · zaihuapd · May 23, 10:58

**背景**: 中国监管机构一直在收紧对跨境证券服务的规则。许多金融科技公司，如富途和老虎证券，在未获得适当牌照的情况下向内地客户提供海外交易。此次执法是确保遵守证券法的更广泛整治行动的一部分。

**标签**: `#regulatory compliance`, `#fintech`, `#China`, `#securities`, `#cross-border trading`

---

<a id="item-9"></a>
## [海盗船采用长鑫存储 DRAM，DDR5 价格有望下调](https://thenextweb.com/news/chinese-dram-cxmt-corsair-ddr5-memory-prices) ⭐️ 8.0/10

美商海盗船已开始在其 DDR5 内存模组中使用中国长鑫存储（CXMT）的 DRAM 芯片。这些 6000 MT/s 的内存模组现已上市，性能与国际主流产品一致。 这一转变标志着供应链的重大多元化，因为主要 DRAM 制造商优先生产 AI 所需的高带宽内存（HBM），导致消费级内存短缺。长鑫芯片的广泛采用可能降低 DDR5 价格，并减少对传统三大巨头（三星、SK 海力士、美光）的依赖。 采用长鑫芯片的模组运行速度为 6000 MT/s，与成熟厂商的竞品速度一致。长鑫存储计划进一步扩大产能，并考虑在 2026 年上市，业内专家预计内存价格可能在 2027 年下半年回落。

telegram · zaihuapd · May 23, 11:17

**背景**: DRAM（动态随机存取存储器）是计算机中使用的一种内存。全球 DRAM 市场由三星、SK 海力士和美光三家公司主导。然而，随着 AI 加速器所需的高带宽内存（HBM）需求激增，这些公司已将产能从消费级 DDR5 模组转移，造成供应缺口，而长鑫存储正在填补这一空缺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/ddr5/chinese-memory-maker-cxmt-enters-the-mainstream-consumer-memory-with-corsair-vengeance-ddr5-kit-chinese-made-dram-emerges-as-an-antidote-for-crushing-shortages">Chinese memory maker CXMT enters mainstream consumer memory with Corsair Vengeance DDR5 kit — Chinese-made DRAM emerges as an antidote for crushing shortages | Tom's Hardware</a></li>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>

</ul>
</details>

**标签**: `#memory`, `#DRAM`, `#supply chain`, `#hardware`, `#AI`

---

<a id="item-10"></a>
## [我国日均词元调用量两年增千倍](https://t.me/zaihuapd/41542) ⭐️ 8.0/10

国家数据局披露，我国日均词元调用量在 2026 年 3 月突破 140 万亿，而 2024 年初仅为 1000 亿，两年间增长超过千倍。 这一爆发式增长表明人工智能商业化正在加速，围绕词元调用、分发和结算的新价值体系正在形成，成为 AI 产业价值的关键指标。 词元是大模型处理信息的最小单元，具有可计量、可定价、可交易的特征。这一增长也显示，随着数据要素市场化配置改革推进，人工智能高质量数据供给体系正在形成。

telegram · zaihuapd · May 23, 14:36

**背景**: 在大语言模型中，文本被切分为词元（Token）——模型处理信息的基本单元。词元可以是单词或子词，在中文中常对应一个汉字或一个词。“词元”这一术语在 2018 年已被纳入计算机学科术语规范。数据要素市场化配置改革是指推动数据作为生产要素进行市场化配置的政策，包括数据确权、定价和交易等。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1954228700687107747">收藏！一文读懂大模型核心概念：从Token到微调的7大术语 - 知乎</a></li>
<li><a href="https://www.qstheory.cn/20260329/e73b0c6107ba436f9707f0f6847d394f/c.html">人工智能研究者：从Token到“词元”，变化背后的分量很重 - 求是网</a></li>
<li><a href="https://www.nda.gov.cn/sjj/zwgk/zjjd/1023/20241023131325305054248_pc.html">专家解读 | 加快公共数据资源开发利用，推进数据要素市场化配置改革-国家数据局</a></li>

</ul>
</details>

**标签**: `#AI`, `#tokenization`, `#data economy`, `#China tech`, `#large language models`

---

<a id="item-11"></a>
## [澳大利亚四天工作周研究显示生产力提升](https://scienceaim.com/australia-just-proved-the-four-day-work-week-works-here-is-what-the-data-actually-says/) ⭐️ 7.0/10

一项澳大利亚研究的数据表明，四天工作周可以提高生产力，挑战了传统的工作制度。 这一发现可能影响全球工作文化和政策，为各行业采用更短工作周提供基于证据的论据。 该研究基于调查数据而非对照实验，评论者质疑其科学严谨性。此外，澳大利亚正经历 60 年来的生产力低谷，这可能影响结果的普遍适用性。

hackernews · randycupertino · May 24, 18:56 · [社区讨论](https://news.ycombinator.com/item?id=48259990)

**背景**: 传统的每周五天、每天八小时工作制是在工业时代建立的。近年来，人们对缩短工作时间的兴趣日益浓厚，全球多个试点项目正在进行。然而，在这类研究中衡量生产力颇具挑战性，通常依赖于自我报告的数据。

**社区讨论**: 评论者对该研究的方法论表示怀疑，有人称其为'意见调查'而非科学研究。其他人指出，澳大利亚当前的经济背景，包括生产力低谷和税收增加，可能会干扰结果。也有人支持无论生产力指标如何都要减少工作时间。

**标签**: `#Productivity`, `#Work Culture`, `#Four-Day Week`, `#Australia`, `#Research`

---

<a id="item-12"></a>
## [内存占 AI 芯片组件成本近三分之二](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 7.0/10

最新分析显示，内存组件已占到 AI 芯片总成本的近三分之二，这一增长主要源于 AI 数据中心对高带宽内存（HBM）的旺盛需求。 这一成本变化对 AI 硬件定价、供应链动态以及 AI 推理和训练的可负担性产生重大影响。同时，内存短缺全面推高 DRAM 价格，也冲击了消费电子市场。 根据分析，内存成本目前约占 AI 芯片组件总成本的 65%，高于此前几代产品的占比。对于 AI 加速器至关重要的高带宽内存（HBM）是主要推动因素，受供应限制价格飙升。

hackernews · intelkishan · May 24, 16:31 · [社区讨论](https://news.ycombinator.com/item?id=48258684)

**背景**: 高带宽内存（HBM）是一种专门设计用于提供 AI 芯片所需极高数据传输速率的内存技术。与 PC 和智能手机中使用的标准 DRAM 不同，HBM 采用垂直堆叠并与处理器紧密集成，制造成本更高。当前的 AI 热潮导致对 HBM 的需求激增，供不应求推高了成本。结果，内存已成为 AI 加速器中最昂贵的组件，甚至超过了逻辑芯片本身。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/01/10/micron-ai-memory-shortage-hbm-nvidia-samsung.html">AI memory is sold out, causing an unprecedented surge in prices</a></li>
<li><a href="https://chip.computer/guides/understanding-hbm-memory">Understanding HBM Memory: Why It's Critical for AI Chips</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，如果 DRAM 供应满足需求，AI 硬件成本可能下降约 3 倍，并感叹内存价格上涨（例如 96GB DDR5 现在售价 1200 美元，而两年前仅为 250 美元）。一些用户推迟升级直到价格恢复正常，另一些人则批评伊朗在依赖 AI 宣传的同时阻断氦气供应的讽刺现象。

**标签**: `#AI hardware`, `#memory`, `#semiconductors`, `#cost analysis`, `#supply chain`

---

<a id="item-13"></a>
## [Usborne 1980 年代计算机图书合集重温](https://usborne.com/us/books/computer-and-coding-books) ⭐️ 7.0/10

Usborne 已将其标志性的 1980 年代计算机图书合集上线，包括《练习 BASIC》和《编写自己的冒险程序》等经典著作。 这些书籍启蒙了一代人的编程学习，对软件工程师和复古计算爱好者具有重要的怀旧和文化价值。 这些书籍最初教授针对 ZX Spectrum 和 Commodore 64 等家用计算机的 BASIC 语言，目前许多已在 Usborne 网站上提供免费 PDF 下载。

hackernews · ngram · May 24, 15:43 · [社区讨论](https://news.ycombinator.com/item?id=48258194)

**背景**: BASIC（初学者通用符号指令代码）是一种易于使用的高级编程语言，在 1980 年代的家用计算机上广泛使用。Usborne 在那个时代出版的系列计算机书籍通过简单的语言和插图，帮助年轻读者揭开了编程的神秘面纱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BASIC_programming_language">BASIC programming language</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了从这些书中学习编程的温馨个人经历，有些人描述了如何将 BASIC 代码清单移植到 JavaScript 或其他现代语言。整体情绪非常积极，强调了这些书籍对他们职业生涯和编程热爱的深远影响。

**标签**: `#retro computing`, `#programming education`, `#nostalgia`, `#BASIC`, `#history`

---

<a id="item-14"></a>
## [诈骗者滥用微软内部账户发送垃圾邮件](https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/) ⭐️ 7.0/10

诈骗者正在滥用一个微软内部账户发送垃圾邮件，利用了微软域名泛滥和安全漏洞。 这凸显了微软持续存在的安全弱点以及域名泛滥的普遍问题，使用户更难区分合法邮件和钓鱼邮件。它强调了企业整合官方邮件域名的必要性。 被滥用的微软内部账户被认为与 microsoftonline.com 相关，许多用户可能不认为该域名是合法的。微软尚未对此具体滥用事件公开评论。

hackernews · spike021 · May 24, 00:51 · [社区讨论](https://news.ycombinator.com/item?id=48253186)

**背景**: 域名泛滥是指公司拥有并使用大量不同域名来提供各种服务，这会使用户困惑并带来安全风险。例如，微软使用了数十个域名，如 microsoft.com、live.com、outlook.com 和 microsoftonline.com，导致用户难以辨别哪些是官方域名。这种不清晰的情况经常被诈骗者利用，发送看似真实的钓鱼邮件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.NameSilo.com/blog/en/domain-investing/brand-equity-domain-sprawl">The SEO Risk of Managing Too Many Domains l | NameSilo Blog</a></li>
<li><a href="https://dnsmadeeasy.com/resources/manage-multiple-domains">Taming Domain Sprawl : How SMBs Can Simplify Multi- Domain ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对微软域名混乱表示沮丧，指出即使是内部员工也可能不知道所有拥有的域名。一些人分享了相关的钓鱼经历，例如伪造的 Booking.com 邮件以及利用字体相似性的近似域名。整体情绪对微软的安全实践和缺乏集中域名管理持批评态度。

**标签**: `#security`, `#phishing`, `#microsoft`, `#spam`, `#email`

---

<a id="item-15"></a>
## [特朗普政府拟要求绿卡申请人离境办理](https://wallstreetcn.com/articles/3772964) ⭐️ 7.0/10

特朗普政府宣布一项新规，要求大多数在美持临时签证的绿卡申请人离开美国，回本国通过领事程序申请永久居留，不再允许在美国境内调整身份。 这一变化将严重影响临时签证持有者，包括 H-1B 签证的科技行业从业者、留学生以及美国公民配偶，迫使他们忍受长期分离和处理延迟，可能扰乱职业和家庭生活。 该规则仅允许“特殊情况”下的例外。目前，调整身份允许许多绿卡申请人在不离境的情况下成为永久居民，过程可能只需数月；而领事程序通常需要数年，且要求申请人留在国外直至获批。

telegram · zaihuapd · May 23, 06:33

**背景**: 调整身份（Adjustment of Status）是许多已在美移民在不离境的情况下申请绿卡的程序。领事处理（Consular Processing）则要求申请人通过海外美国大使馆或领事馆获得签证。拟议规则要求大多数案件必须通过领事处理，打破了现有平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.uscis.gov/green-card/green-card-processes-and-procedures/adjustment-of-status">Adjustment of Status - USCIS</a></li>
<li><a href="https://www.boundless.com/immigration-resources/green-card-consular-processing">How to Get a Green Card Through Consular Processing</a></li>

</ul>
</details>

**标签**: `#immigration`, `#US policy`, `#tech workers`, `#green card`

---