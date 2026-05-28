---
layout: default
title: "Horizon Summary: 2026-05-28 (ZH)"
date: 2026-05-28
lang: zh
---

> From 31 items, 16 important content pieces were selected

---

1. [Anthropic 以 9650 亿美元估值融资 650 亿，超越 OpenAI](#item-1) ⭐️ 9.0/10
2. [只用 Postgres 实现持久化工作流](#item-2) ⭐️ 8.0/10
3. [欧盟对 Temu 罚款 2 亿欧元，因销售非法产品](#item-3) ⭐️ 8.0/10
4. [Altman 和 Amodei 收回 AI 就业末日预言](#item-4) ⭐️ 8.0/10
5. [YouTube 将自动标注 AI 生成视频](#item-5) ⭐️ 8.0/10
6. [英伟达 CEO：因出口管制，公司基本放弃中国 AI 芯片市场](#item-6) ⭐️ 8.0/10
7. [高通与字节跳动合作定制 AI ASIC 芯片](#item-7) ⭐️ 8.0/10
8. [英伟达计划每年在台湾投资 1500 亿美元，称其为 AI 革命中心](#item-8) ⭐️ 8.0/10
9. [中国将为人形机器人分配数字 ID](#item-9) ⭐️ 8.0/10
10. [比亚迪发布 4nm 智驾芯片璇玑 A3](#item-10) ⭐️ 8.0/10
11. [Anthropic 发布 Claude Opus 4.8，带来小幅改进](#item-11) ⭐️ 7.0/10
12. [LLM 写作风格痕迹清单](#item-12) ⭐️ 7.0/10
13. [永久上乌鸦：讽刺地位追逐的游戏](#item-13) ⭐️ 7.0/10
14. [60 秒游戏模拟 AI 代理权限疲劳](#item-14) ⭐️ 7.0/10
15. [DOMD：开源所见即所得 Markdown 编辑器，20KB 自研渲染引擎](#item-15) ⭐️ 7.0/10
16. [美司法部要求 Reddit 和 X 提供批评 ICE 账号信息](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 以 9650 亿美元估值融资 650 亿，超越 OpenAI](https://www.anthropic.com/news/series-h) ⭐️ 9.0/10

Anthropic 宣布了 650 亿美元的 H 轮融资，投后估值达到 9650 亿美元，并报告了 470 亿美元的年化运行率收入，在两项指标上均超越 OpenAI。 这轮融资标志着 AI 行业的重大转变，Anthropic 在估值和收入运行率上领先于 OpenAI，可能重塑竞争格局和投资者信心。 470 亿美元的年化运行率收入是自行报告的，包括了自 2026 年 2 月 G 轮融资以来的企业客户增长。9650 亿美元的估值使 Anthropic 成为全球最有价值的私营公司之一。

hackernews · meetpateltech · May 28, 18:09 · [社区讨论](https://news.ycombinator.com/item?id=48313048)

**背景**: 运行率收入是将当前月或季度收入外推至全年数字，常用于快速增长的公司。H 轮通常是 IPO 前的后期私募融资轮次。Anthropic 的崛起反映了对 Claude 等 AI 模型的需求激增。

**社区讨论**: 评论者注意到 Anthropic 收入超过 OpenAI，有人质疑如此高的私募估值是否可持续以及股票市场角色的转变。也有对运行率收入定义的好奇。

**标签**: `#AI`, `#funding`, `#Anthropic`, `#valuation`, `#industry-shift`

---

<a id="item-2"></a>
## [只用 Postgres 实现持久化工作流](https://www.dbos.dev/blog/postgres-is-all-you-need-for-durable-execution) ⭐️ 8.0/10

本文主张仅使用 PostgreSQL 作为持久化工作流执行的后端，将多个关注点整合到一个数据库中。 这简化了架构，减少了对独立工作流引擎、队列和状态存储的依赖，使系统更易于运维和调试，并降低了构建可靠工作流的门槛。 该方法利用 PostgreSQL 的事务、咨询锁和 LISTEN/NOTIFY 等特性来协调工作流步骤，无需额外基础设施。适用于许多应用，但在极大规模下可能需要迁移到专用系统。

hackernews · KraftyOne · May 28, 18:41 · [社区讨论](https://news.ycombinator.com/item?id=48313530)

**背景**: 持久化执行是一种编程范式，通过自动持久化状态并通过重放恢复，使普通代码能够抵御崩溃和故障。传统实现通常需要专用工作流引擎（如 Temporal）或任务队列。PostgreSQL 是一种流行的关系数据库，其特性超越存储，包括触发器、通过 SKIP LOCKED 实现队列以及发布/订阅，使其成为统一工作流编排的候选。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.restate.dev/what-is-durable-execution">What is Durable Execution? A Definitive Guide | Restate</a></li>
<li><a href="https://github.com/pgflow-dev/pgflow">GitHub - pgflow-dev/pgflow: Postgres-centric workflow engine ...</a></li>
<li><a href="https://sokratisvidros.github.io/pg-workflows/">pg-workflows | Postgres workflows. Durable execution built on pb-boss like Temporal, Inngest, or Trigger, powered by Postgres.</a></li>

</ul>
</details>

**社区讨论**: 评论显示出高度参与度，用户分享了替代实现，如 Armin Ronacher 的`absurd`和 pgflow。一些讨论扩展限制，指出 Postgres 在数据达到 TB 级之前足够使用，之后可能需要迁移。总体情绪积极，赞赏简化基础设施。

**标签**: `#PostgreSQL`, `#workflows`, `#durable execution`, `#database`, `#backend`

---

<a id="item-3"></a>
## [欧盟对 Temu 罚款 2 亿欧元，因销售非法产品](https://www.bbc.co.uk/news/articles/c1k2ydn1rz8o) ⭐️ 8.0/10

欧盟于 2025 年初宣布，因 Temu 平台未能阻止非法和不安全产品的销售，对其处以 2 亿欧元罚款。 这项罚款凸显了欧盟对大型电商平台严格执行《数字服务法》（DSA），表明企业必须对产品安全和合法性承担更大责任。这可能迫使 Temu 及类似平台加强审核流程。 这是根据《数字服务法》开出的最大罚单之一，专门针对 Temu 未能删除假冒伪劣和潜在危险商品的列表。欧盟调查发现 Temu 的审核系统存在不足。

hackernews · jjp · May 28, 14:18 · [社区讨论](https://news.ycombinator.com/item?id=48309302)

**背景**: Temu 是一家中国拥有的在线购物平台，以超低价格著称，通常直接从中国发货。欧盟的《数字服务法》（DSA）于 2022 年生效，要求大型平台评估并减轻与非法内容和产品销售相关的风险。此次罚款是对 DSA 执行能力的一次关键考验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Temu">Temu - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示不同反应：一些用户为 Temu 辩护，认为其提供了本地中间商的廉价替代品；而另一些人则质疑为何类似罚款不适用于亚马逊或 eBay。批评者认为，仅靠监管罚款可能无法有效应对中国电商进口的规模。

**标签**: `#EU regulation`, `#e-commerce`, `#consumer protection`, `#Temu`, `#fines`

---

<a id="item-4"></a>
## [Altman 和 Amodei 收回 AI 就业末日预言](https://fortune.com/2026/05/26/sam-altman-dario-amodei-walking-back-ai-jobs-apocalypse-prophecies-ipo/) ⭐️ 8.0/10

OpenAI 的 Sam Altman 和 Anthropic 的 Dario Amodei 公开收回了他们之前关于 AI 将导致大规模失业的预测，转而强调 AI 对就业影响的更细微观点。 这一转变意义重大，因为 Altman 和 Amodei 是 AI 领域最具影响力的两位人物；他们修正后的立场可能会改变有关 AI 监管和劳动力市场扰乱的公众及政策辩论。 此次收回观点正值公众对 AI 就业影响的担忧日益加剧之际，一些批评者认为这一转变可能是在大型 IPO 前为软化 AI 负面形象而进行的公关行动。文章报道称，两位领导人现在声称 AI 将增强而非取代大多数工人。

hackernews · ianrahman · May 28, 19:43 · [社区讨论](https://news.ycombinator.com/item?id=48314363)

**背景**: Sam Altman 是 OpenAI（ChatGPT 的创造者）的 CEO，Dario Amodei 是 Anthropic（Claude 的开发者）的 CEO。两人此前曾警告 AI 可能消除许多工作岗位，助长了末日叙事。他们新的更乐观的声明代表了 AI 行业在言辞上的重大转变。

**社区讨论**: 社区评论者持怀疑态度，认为这一转变是 IPO 前为改善公众形象而精心策划的公关举动。一些人指出，高管们仍以 AI 为由进行裁员，而另一些人则强调了从“取代开发者”到“我们爱开发者”的转变具有讽刺意味。讨论反映了对 AI 领导者动机的不信任。

**标签**: `#AI`, `#labor`, `#predictions`, `#Sam Altman`, `#Dario Amodei`

---

<a id="item-5"></a>
## [YouTube 将自动标注 AI 生成视频](https://blog.youtube/news-and-events/improving-ai-labels-viewers-creators/) ⭐️ 8.0/10

YouTube 宣布将利用自有检测工具自动为识别为 AI 生成的视频添加标签，此前的政策仅要求创作者手动标注。此举旨在提高对观众的透明度。 这一政策变更影响数百万用户和创作者，因为 AI 生成内容日益普遍，可能误导儿童和老人等弱势群体。它开创了内容平台主动标注合成媒体的先河，可能影响行业标准。 自动标注适用于检测到 AI 生成的视频，创作者也可以自愿手动标注自己的 AI 生成内容。标签将显示在视频描述或播放器中。

hackernews · nopg · May 27, 20:00 · [社区讨论](https://news.ycombinator.com/item?id=48299753)

**背景**: YouTube 等平台上的 AI 生成内容迅速增长，引发了关于错误信息和真实性的担忧。之前的政策要求创作者手动披露 AI 生成内容，但合规性不一致。自动检测旨在填补这一空白并保护观众。

**社区讨论**: 评论者表示强烈支持，指出儿童和老人易受 AI 生成内容影响，以及 AI 音乐和逼真虚假建议视频的泛滥。一些人讨论了从参与向消费转变的更大文化变迁，但整体情绪对标注举措持正面态度。

**标签**: `#AI`, `#YouTube`, `#content moderation`, `#transparency`, `#AI-generated content`

---

<a id="item-6"></a>
## [英伟达 CEO：因出口管制，公司基本放弃中国 AI 芯片市场](https://t.me/zaihuapd/41609) ⭐️ 8.0/10

英伟达 CEO 黄仁勋表示，受美国出口管制影响，公司已基本放弃中国 AI 芯片市场，将其让给华为等本土厂商。他告知投资者对获得在华销售先进芯片的许可不要抱任何期望。 这标志着全球 AI 芯片格局的重大转变，在中美科技紧张局势升级之际，英伟达将世界第二大经济体拱手让给中国竞争对手。这凸显了出口管制对半导体供应链的影响，并可能加速中国在 AI 硬件领域的自主化进程。 中国此前占英伟达数据中心收入至少五分之一。今年 4 月，特朗普政府要求对华出口芯片须取得许可证，实质上将英伟达排除在外。黄仁勋指出华为及本地芯片生态表现非常强劲，而英伟达正将资金转向供应链扩张和 800 亿美元的股票回购计划。

telegram · zaihuapd · May 28, 03:03

**背景**: 美国出口管制限制向中国销售先进 AI 芯片，旨在限制中国获取尖端技术。英伟达的高端芯片如 A100 和 H100 受这些限制。华为已开发自己的 AI 芯片，如昇腾系列，在中国市场竞争。

**标签**: `#Nvidia`, `#AI chips`, `#export controls`, `#China`, `#semiconductor industry`

---

<a id="item-7"></a>
## [高通与字节跳动合作定制 AI ASIC 芯片](https://t.me/zaihuapd/41616) ⭐️ 8.0/10

据报道，高通已与字节跳动达成协议，供应数百万颗定制 AI ASIC 芯片，以满足字节跳动 AI 服务的算力需求，并帮助其将内部芯片设计转化为可量产的半导体产品。 这一合作标志着高通将定制 ASIC 业务拓展至 AI 超大规模云服务市场，同时字节跳动获得了定制化硬件供应链，以支持其快速增长的 AI 服务，可能减少对通用 GPU 的依赖。 该合作涉及数百万颗定制 ASIC，高通此前曾宣布今年将向一家超大规模云服务商交付首款 ASIC。高通和字节跳动均未对报道正式置评。

telegram · zaihuapd · May 28, 07:09

**背景**: ASIC（专用集成电路）是为特定用途设计的芯片，在专用任务上比通用处理器效率更高、性能更强。在 AI 领域，Google 和 Meta 等超大规模云服务商越来越多地采用定制 ASIC 来加速机器学习工作负载，同时降低功耗和成本。字节跳动作为 TikTok 的母公司，需要大量 AI 算力用于推荐算法和内容审核，因此定制芯片成为战略投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Application-specific_integrated_circuit">Application-specific integrated circuit - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/custom-ai-asics-examined-from-broadcom-to-mtia">The custom AI ASIC state of play (May 2026) — Broadcom deals ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Hardware`, `#ASIC`, `#Qualcomm`, `#ByteDance`

---

<a id="item-8"></a>
## [英伟达计划每年在台湾投资 1500 亿美元，称其为 AI 革命中心](https://arstechnica.com/tech-policy/2026/05/nvidia-ceo-wants-taiwan-to-be-center-of-ai-revolution-not-us/) ⭐️ 8.0/10

英伟达 CEO 黄仁勋宣布，公司计划每年在台湾投入约 1500 亿美元，用于 AI 芯片生产、系统制造和供应链合作，远高于数年前的 100 亿至 150 亿美元。 此举将台湾定位为全球 AI 革命的核心枢纽，巩固其半导体和 AI 硬件供应链中的关键角色，对地缘政治和科技产业格局有深远影响。 英伟达计划在台北建设新总部，预计今年动工、2030 年启用，将容纳 4000 名员工。主要合作伙伴包括台积电、鸿海（富士康）、纬创和广达。

telegram · zaihuapd · May 28, 07:33

**背景**: 英伟达是领先的 AI 芯片设计公司，而台湾以台积电为首的半导体制造生态系统是其先进芯片生产的关键。公司多年来一直深化与台湾供应商的合作。

**标签**: `#NVIDIA`, `#AI`, `#Taiwan`, `#semiconductor`, `#investment`

---

<a id="item-9"></a>
## [中国将为人形机器人分配数字 ID](https://www.scmp.com/tech/policy/article/3354747/china-give-every-humanoid-robot-digital-id-push-boost-industry-standards) ⭐️ 8.0/10

中国启动了人形机器人全生命周期管理服务平台，为所有国产人形机器人分配唯一数字 ID，以追踪其从生产到回收的完整生命周期。该举措由工信部下属的人形机器人与具身智能标准化委员会牵头。 这一监管举措建立了一套全面的人形机器人追溯框架，提升了安全性、所有权问责制和性能监控能力。它表明中国在为人形机器人新兴产业制定标准方面采取了主动立场，可能影响全球监管方向。 该平台覆盖研发、制造、市场准入、销售、运营和报废回收等环节。据报道，已有超过 2.8 万台人形机器人获得了数字 ID。

telegram · zaihuapd · May 28, 09:08

**背景**: 人形机器人是模仿人体形态的机器人，通常用于与人类工具和环境交互。数字 ID 能够实现全生命周期追踪，这对于日益增长的自主机器人群体的安全、维护和问责至关重要。中国工信部一直在积极推动人工智能和机器人的标准化工作，该系统是其中的关键组成部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://technode.com/2026/05/25/china-launches-first-humanoid-robot-lifecycle-management-platform-in-beijing/">China launches first humanoid robot lifecycle management platform in Beijing · TechNode</a></li>
<li><a href="https://thenextweb.com/news/china-humanoid-robot-id-system-lifecycle-tracking">China assigns ID codes to 28,000+ humanoid robots</a></li>
<li><a href="https://www.eweek.com/news/china-humanoid-robot-digital-id-system-apac/">China Assigns Digital Identity Codes to Thousands of Humanoid ...</a></li>

</ul>
</details>

**标签**: `#robotics`, `#AI regulation`, `#humanoid robots`, `#China policy`, `#standardization`

---

<a id="item-10"></a>
## [比亚迪发布 4nm 智驾芯片璇玑 A3](https://finance.sina.com.cn/roll/2026-05-28/doc-inhznenn1371824.shtml) ⭐️ 8.0/10

比亚迪于 2026 年 5 月 28 日在'敢为'智能化战略发布会上宣布，其 4 纳米智驾芯片'璇玑 A3'已开启规模化量产，声称支持 L3 和 L4 自动驾驶，并实现算力利用率提升 100%。 这一进展意义重大，标志着比亚迪在自主研发先进自动驾驶硬件方面迈出重要一步，可能减少对外部芯片供应商的依赖，并加速高阶自动驾驶在量产车上的普及。 三颗璇玑 A3 芯片合计总算力超过 2100 TOPS。比亚迪声称通过自研算法优化，该芯片的算力利用率提升了 100%，不过具体的架构细节和基准测试结果尚未公布。

telegram · zaihuapd · May 28, 13:01

**背景**: TOPS（每秒万亿次操作）是衡量 AI 芯片性能的指标，表示芯片每秒可执行的万亿次操作次数。自动驾驶等级由 SAE 定义：L3 为有条件自动化，车辆承担大部分驾驶任务但驾驶员需随时准备接管；L4 为高度自动化，车辆在特定条件下可完成所有驾驶操作，无需驾驶员干预。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/337618803">TOPS（处理器运算能力单位） - 知乎</a></li>
<li><a href="https://www.automotiveworld.cn/zh-cn/_6/_0/20191101148.html">自 动 驾 驶 汽车中的L2 和 L 3 级 有什么不同</a></li>

</ul>
</details>

**标签**: `#autonomous driving`, `#chip`, `#BYD`, `#AI hardware`, `#4nm`

---

<a id="item-11"></a>
## [Anthropic 发布 Claude Opus 4.8，带来小幅改进](https://www.anthropic.com/news/claude-opus-4-8) ⭐️ 7.0/10

Anthropic 发布了 Claude Opus 4.8，这是继 Opus 4.6 和 4.7 之后的一个小版本更新，相比前代提供了温和但可感知的提升。 此次发布延续了 Anthropic 对前沿模型进行增量改进的趋势，同时宣布未来的 Mythos 级别模型标志着持续进步。用户在复杂算法任务中报告了显著提升，但通用能力变化不大。 Opus 4.8 允许在 Web 界面中关闭自适应思考，解决了此前输出质量不佳的问题。此外，Anthropic 宣布了 Project Glasswing 和用于网络安全的 Claude Mythos 预览版，需要加强安全防护后才能公开发布。

hackernews · craigmart · May 28, 16:49 · [社区讨论](https://news.ycombinator.com/item?id=48311647)

**背景**: Anthropic 是一家以 Claude 系列大语言模型闻名的 AI 安全公司。Opus 系列代表其最强模型，版本号表示增量改进。此次 4.8 版本是大版本 Opus 4.5（能力显著提升）后一系列小更新的一部分。

**社区讨论**: 社区成员指出，Opus 4.8 是继大版本 4.5 之后第三次小版本更新（4.6、4.7、4.8），部分用户认为改进不易察觉。但一位用户表示在算法后端工作中体验差异‘天壤之别’。另一位用户赞赏新增的关闭自适应思考功能，此前该功能常导致输出质量不佳。大家对即将到来的 Mythos 级别模型也充满期待。

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#LLM`, `#machine learning`

---

<a id="item-12"></a>
## [LLM 写作风格痕迹清单](https://shvbsle.in/various-llm-smells/) ⭐️ 7.0/10

该文章汇总了如 'honest caveat' 和 'load bearing' 等常见于 LLM 生成文本中的风格模式，作为检测的线索。 这一资源有助于开发者和写作者批判性评估文本真实性，应对日益增长的人机文本区分挑战。 列表包括 'honest caveat'、'load bearing' 等短语，以及 '不是 X，而是 Y' 这样的对比否定句式。社区还补充了 'blast radius' 和 'smoke test' 等线索。

hackernews · speckx · May 28, 19:02 · [社区讨论](https://news.ycombinator.com/item?id=48313810)

**背景**: “LLM 痕迹”指的是大型语言模型（如 GPT-4）生成文本中频繁出现的特定风格模式。这些线索源于 LLM 过度使用某些短语和句式结构，使得通过风格分析进行检测成为可能。随着 LLM 文本日益普及，此类指南有助于保持对在线内容的批判性评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.researchgate.net/publication/373898266_Stylometric_Detection_of_AI-Generated_Text_in_Twitter_Timelines">(PDF) Stylometric Detection of AI - Generated Text in Twitter Timelines</a></li>
<li><a href="https://stravoai.com/how-do-we-detect-machine-generated-text-on-social-platforms/">How Do We Detect Machine Generated Text on Social Platforms...</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了更多常见 LLM 短语，并强调 LLM 生成文本在读者缺乏专业知识的领域可能显得比人类写作更好，从而增加检测难度。一位用户指出，最近模型的写作风格在文体上并无显著改进。

**标签**: `#LLM`, `#writing`, `#detection`, `#style`, `#AI`

---

<a id="item-13"></a>
## [永久上乌鸦：讽刺地位追逐的游戏](https://permanent-upper-crow.jasonwu.ink/) ⭐️ 7.0/10

《永久上乌鸦》是一款基于网页的讽刺游戏，通过无限循环获取 CEO 头衔，突显炫耀性消费的徒劳。 游戏的循环机制和社区讨论突显了其与自动化、财富不平等及成功意义等持续辩论的相关性。 据社区成员 Tossrock 指出，游戏包含 106 个独特的 CEO 头衔和公司，之后会循环回到起点。

hackernews · whiteblossom · May 28, 15:23 · [社区讨论](https://news.ycombinator.com/item?id=48310280)

**背景**: 炫耀性消费是社会学家索尔斯坦·凡勃伦提出的术语，指通过购买奢侈品来展示经济实力。该游戏通过将这种行为简化为无意义的头衔获取循环来讽刺它，唯一的“胜利”方式就是停止游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48310280">The Permanent Upper Crow | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 评论指出游戏的讽刺之处在于其创作者是一家旨在自动化工作的 AI 初创公司的联合创始人，这与游戏的反消费主义信息形成对比。一些用户认为游戏缺乏互动性，而另一些人则指出，放弃地位象征是唯一的解脱方式。

**标签**: `#game`, `#satire`, `#web`, `#interactive`, `#status`

---

<a id="item-14"></a>
## [60 秒游戏模拟 AI 代理权限疲劳](https://llmgame.scalex.dev/) ⭐️ 7.0/10

一款名为“Continue? Y/N”的 60 秒游戏在 Hacker News 上发布，模拟审批或拒绝 AI 代理请求的繁琐过程，凸显权限疲劳问题。 该游戏创造性地展示了 AI 代理生态系统中日益严重的用户体验和安全挑战：用户对重复提示变得麻木，可能无意中批准危险操作，增加凭证泄露或数据丢失的风险。 玩家可以通过快速拒绝所有请求来“作弊”，获得完美分数徽章，同时忽略过度拦截警告；游戏的上下文跳跃设计被批评为不具代表性。

hackernews · Wirbelwind · May 28, 13:02 · [社区讨论](https://news.ycombinator.com/item?id=48308376)

**背景**: 权限疲劳是指用户被大量审批提示淹没，不再仔细评估每个请求，导致安全漏洞。一些 AI 工具提供--dangerously-skip-permissions 标志来完全绕过提示。该游戏模仿了《请出示证件》风格，在压力下快速决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scalex.dev/blog/ai-agent-permissions/">Suffering from Agent Permission Fatigue? Find out your high score | Scale X</a></li>
<li><a href="https://github.com/kstenerud/yoloai">GitHub - kstenerud/yoloai: Permission fatigue is a real problem. Sandbox escape is a real problem. yoloAI solves it. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者赞赏该游戏的概念，但也指出了缺陷：游戏作者自身的安全卫生习惯（如假设.zshrc 中有秘密）、不现实的上下文跳跃，以及代理权限模型中安全与效率之间的根本矛盾。

**标签**: `#AI safety`, `#game`, `#permission fatigue`, `#security`, `#UX`

---

<a id="item-15"></a>
## [DOMD：开源所见即所得 Markdown 编辑器，20KB 自研渲染引擎](https://github.com/do-md/domd) ⭐️ 7.0/10

DOMD 是一款全新的开源 Markdown 所见即所得编辑器，其渲染引擎完全自研，内核仅 20KB（gzip），除 React 外无运行时依赖。它支持基于 Tauri 的 macOS 原生应用、Web 版，以及一个让 AI 模型直接驱动编辑器窗口的命令行工具。 该项目证明，无需依赖 ProseMirror、Slate 等重量级框架，也能构建高性能、本地优先的 Markdown 编辑器，为注重隐私和速度的开发者和用户提供了极简且快速的替代方案。其 AI agent 集成也为直接在 Markdown 中进行 AI 辅助写作打开了可能性。 编辑器采用单一数据源和不可变状态设计，使得撤销/重做、AI 流式注入和大文件分块加载等操作都能保持同样快速。macOS 原生版自带 Quick Look 扩展，用户可在访达中按空格键直接预览 .md 文件。

telegram · zaihuapd · May 28, 05:48

**背景**: 当前大多数 Web 所见即所得编辑器都基于通用富文本框架（如 ProseMirror、Slate 或 Lexical）构建，这些框架提供了文档编辑抽象，但增加了复杂性和包体积。Tauri 是一个轻量级框架，使用 Web 前端和 Rust 后端构建跨平台桌面应用。DOMD 自研渲染引擎的做法使其能够针对 Markdown 编辑实现极小的体积和优化的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://liveblocks.io/blog/which-rich-text-editor-framework-should-you-choose-in-2025">Which rich text editor framework should you choose in 2025?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tauri_(software_framework)">Tauri (software framework)</a></li>
<li><a href="https://tauri.app/">Tauri 2.0 | Tauri</a></li>

</ul>
</details>

**标签**: `#markdown`, `#editor`, `#wysiwyg`, `#open-source`, `#local-first`

---

<a id="item-16"></a>
## [美司法部要求 Reddit 和 X 提供批评 ICE 账号信息](https://www.bloomberg.com/news/articles/2026-05-28/trump-s-doj-ramps-up-probes-of-anonymous-ice-critics-with-x-reddit-subpoenas) ⭐️ 7.0/10

美国司法部要求 Reddit 和 X 提供至少两个匿名账号的姓名、住址和银行信息，这些账号曾批评 ICE 的执法行动。这些要求已从行政传唤升级为大陪审团传票，作为刑事调查的一部分。 此举标志着政府对主要平台用户数据要求的重大升级，引发了对批评执法机构的个人言论自由和隐私保护的严重担忧。这可能为科技公司未来如何应对政府数据请求树立先例。 传票最初是行政性的，现已升级为大陪审团传票，表明涉及刑事调查，但具体罪名尚未披露。受影响的用户已收到平台通知，并聘请律师在法庭挑战这些传票。

telegram · zaihuapd · May 28, 14:22

**背景**: 美国司法部（DOJ）是负责起诉联邦犯罪的联邦执法机构。移民和海关执法局（ICE）是执行移民法律的机构。传票是强制提供证据的法律命令；大陪审团传票表明正式刑事调查。Reddit 和 X 等平台通常在用户数据被请求时通知用户，以便用户挑战该请求。

**标签**: `#privacy`, `#government surveillance`, `#free speech`, `#tech policy`, `#legal`

---