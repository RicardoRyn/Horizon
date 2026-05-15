---
layout: default
title: "Horizon Summary: 2026-05-15 (ZH)"
date: 2026-05-15
lang: zh
---

> From 45 items, 23 important content pieces were selected

---

1. [Project Zero 披露 Pixel 10 零点击漏洞利用链](#item-1) ⭐️ 9.0/10
2. [5 天内借助 AI 完成首个公开 Apple M5 内核利用](#item-2) ⭐️ 9.0/10
3. [arXiv 对未核查 LLM 内容禁投 1 年](#item-3) ⭐️ 9.0/10
4. [Mitchellh 警告企业出现“AI 精神病”](#item-4) ⭐️ 8.0/10
5. [Zulip 转型为非营利基金会，创始人加入 Anthropic](#item-5) ⭐️ 8.0/10
6. [OCaml 太空应用：无 GC 的数据包处理](#item-6) ⭐️ 8.0/10
7. [支付宝否认关闭支付后 184 万捐赠扣款责任](#item-7) ⭐️ 8.0/10
8. [苹果与 OpenAI 合作裂痕加深，OpenAI 或起诉](#item-8) ⭐️ 8.0/10
9. [特朗普与习近平讨论 AI 护栏与英伟达 H200 芯片](#item-9) ⭐️ 8.0/10
10. [Palantir 聘用超 30 名英国政府高级官员](#item-10) ⭐️ 7.0/10
11. [加州法案要求在线游戏停服时提供离线补丁或退款](#item-11) ⭐️ 7.0/10
12. [美国司法部要求苹果和谷歌披露 10 万汽车应用用户](#item-12) ⭐️ 7.0/10
13. [Waymo 召回 3800 辆机器人出租车因涉水故障](#item-13) ⭐️ 7.0/10
14. [Meta 获 33 亿美元税收优惠，建百亿美元数据中心](#item-14) ⭐️ 7.0/10
15. [ABC 新闻下线所有 FiveThirtyEight 文章](#item-15) ⭐️ 7.0/10
16. [像 Windows XP 桌面一样浏览维基百科](#item-16) ⭐️ 7.0/10
17. [Jason Scott 的 ASCII 博客：数字保存获赞誉](#item-17) ⭐️ 7.0/10
18. [Radicle 推出主权去中心化 Git 锻造平台](#item-18) ⭐️ 7.0/10
19. [新书探讨乔布斯在 NeXT 的岁月](#item-19) ⭐️ 7.0/10
20. [累积上下文破解气象预测长期误差难题](#item-20) ⭐️ 7.0/10
21. [英伟达市值盘中突破 5.5 万亿美元](#item-21) ⭐️ 7.0/10
22. [ChatGPT Android 版拆解发现 Codex 远程桌面控制功能](#item-22) ⭐️ 7.0/10
23. [AMD 确认 FSR 4.1 将于 7 月支持 RX 7000，2027 年初覆盖 RX 6000](#item-23) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Project Zero 披露 Pixel 10 零点击漏洞利用链](https://projectzero.google/2026/05/pixel-10-exploit.html) ⭐️ 9.0/10

Google Project Zero 研究人员发布了对 Pixel 10 零点击漏洞利用链的详细分析，展示了如何通过远程 Dolby 音频解码漏洞实现完全内核控制。 这项研究凸显了 AI 功能在用户交互前自动解码媒体所带来的攻击面扩大问题，并强调了厂商及时修补漏洞对移动安全的重要性。 该漏洞利用链利用了 2026 年 1 月之前影响所有 Android 设备的 Dolby 音频漏洞（CVE-2025-54957）以及一个在披露后 90 天内修补的 Google Pixel 驱动程序漏洞，实现了无需用户交互的零点击远程攻击。

hackernews · happyhardcore · May 15, 13:39 · [社区讨论](https://news.ycombinator.com/item?id=48148460)

**背景**: 零点击漏洞利用无需用户任何操作（如打开文件或点击链接），因此极其危险。Project Zero 是 Google 的精英安全团队，负责发现并报告广泛使用软件中的漏洞。Pixel 手机的 AI 功能会自动解码收到的消息以实现搜索和上下文理解，这增大了此类漏洞的攻击面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://projectzero.google/2026/05/pixel-10-exploit.html">A 0-click exploit chain for the Pixel 10: When a Door Closes, a Window ...</a></li>
<li><a href="https://cyberpress.org/zero-click-exploit-chain-for-pixel-10/">Google Project Zero Reveals Zero-Click Exploit Chain for Pixel 10</a></li>

</ul>
</details>

**社区讨论**: 评论者对 AI 功能未经用户同意预处理短信表示担忧，认为这扩大了攻击面。有人称赞 Google 迅速修补了驱动程序漏洞，也有人质疑漏洞披露率是否因 AI 热潮而增加。此外，还出现了关于 AI 对 NSO Group 等商业间谍软件厂商影响的猜测。

**标签**: `#security`, `#exploit`, `#android`, `#vulnerability`, `#pixel`

---

<a id="item-2"></a>
## [5 天内借助 AI 完成首个公开 Apple M5 内核利用](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

Calif 与 AI 系统 Mythos Preview 合作，在短短五天内实现了 Apple M5 macOS 上首个公开的内核内存破坏利用，绕过了 Apple 的 MIE 硬件保护。 这一利用表明，AI 辅助的漏洞发现和利用能够迅速击败即使是多年的硬件安全工程，可能重塑进攻和防御网络安全的格局。 该利用链针对 M5 硬件上的 macOS 26.4.1，利用两个漏洞，仅通过正常系统调用从非特权用户提升至 root shell，完全绕过了 MIE。完整的 55 页技术报告将在 Apple 修复后发布。

telegram · zaihuapd · May 15, 02:15

**背景**: Apple 的 MIE 是随 M5 芯片引入的硬件-软件安全特性，通过结合增强内存标记扩展(EMTE)、安全内存分配器和标签保密性来防止内存破坏攻击。Apple 花费五年开发 MIE 以强化内核。Mythos Preview 是 Anthropic 的 AI 系统，在网络安全任务中展现了先进能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www-cdn.anthropic.com/8b8380204f74670be75e81c820ca8dda846ab289.pdf">Claude Mythos Preview System Card - www-cdn.anthropic.com</a></li>
<li><a href="https://security.apple.com/blog/memory-integrity-enforcement/">Memory Integrity Enforcement: A complete vision for memory safety in...</a></li>
<li><a href="https://blog.calif.io/p/first-public-kernel-memory-corruption">First public macOS kernel memory corruption exploit on Apple M5</a></li>

</ul>
</details>

**标签**: `#security`, `#exploit`, `#macOS`, `#Apple M5`, `#AI-assisted`

---

<a id="item-3"></a>
## [arXiv 对未核查 LLM 内容禁投 1 年](https://x.com/tdietterich/status/2055000956144935055) ⭐️ 9.0/10

arXiv 宣布对含有未核查 LLM 生成内容（如幻觉引用或占位数据）的投稿实施 1 年禁投，恢复投稿前需先被同行评审会议接收。 该政策直接应对学术预印本中日益严重的 AI 生成垃圾内容问题，强化了学术出版的责任与诚信。 禁令涵盖的内容包括幻觉引用、LLM 留下的元注释以及“表格数据仅为示例、请替换为真实实验数据”等占位数据。禁投结束后，作者需先被可信的同行评审会议接收，才能再次提交 arXiv。

telegram · zaihuapd · May 15, 04:30

**背景**: arXiv 是物理学、数学、计算机科学及相关领域广泛使用的开放获取预印本仓库。近年来，大型语言模型（LLM）的兴起导致大量未经作者充分核查的 AI 生成文本投稿涌入，削弱了预印本的可信度。该政策明确了 arXiv 的立场与执行措施。

**标签**: `#arXiv`, `#LLM`, `#academic publishing`, `#policy`, `#AI ethics`

---

<a id="item-4"></a>
## [Mitchellh 警告企业出现“AI 精神病”](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 8.0/10

著名软件工程师 Mitchellh 在 Twitter 上发帖称，许多公司因将决策权完全外包给 AI 而患上“AI 精神病”，这可能导致灾难性后果。 这一警告凸显了科技行业中日益增长的风险：盲目信任 AI 输出会削弱批判性思维，并导致系统不稳定、难以维护。 Mitchellh 区分了将 AI 用作工具和依赖 AI 进行思考两种行为，后者被他称为“AI 精神病”。社区成员指出，完全由 AI 编写的系统可能复杂到人类无法理解或修复。

hackernews · reasonableklout · May 15, 20:26 · [社区讨论](https://news.ycombinator.com/item?id=48153379)

**背景**: “AI 精神病”最初指的是一种临床现象，即个体因与聊天机器人互动而出现类似精神病的症状。在此上下文中，Mitchellh 用该术语比喻那些放弃人类判断、依赖 AI 做出关键决策的企业，这种做法可能导致系统性风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chatbot_psychosis">Chatbot psychosis - Wikipedia</a></li>
<li><a href="https://nam.edu/news-and-insights/what-is-ai-psychosis/">What is AI Psychosis? Psychiatrist Answers 12 Questions About Chatbots & Mental Health</a></li>
<li><a href="https://www.psychologytoday.com/us/blog/urban-survival/202507/the-emerging-problem-of-ai-psychosis">The Emerging Problem of "AI Psychosis" | Psychology Today</a></li>

</ul>
</details>

**社区讨论**: 社区基本同意 Mitchellh 的观点，评论警告称 AI 编写的系统将扩展到无法持续的复杂度，缺陷率最终可能上升。一些用户还指出，与那些相信 AI 代理能以非人速度修复 bug 的人争论很困难。

**标签**: `#AI`, `#software engineering`, `#critical thinking`, `#decision-making`

---

<a id="item-5"></a>
## [Zulip 转型为非营利基金会，创始人加入 Anthropic](https://blog.zulip.com/2026/05/15/announcing-zulip-foundation/) ⭐️ 8.0/10

Zulip 的创始人将退出全职领导岗位加入 Anthropic，同时将公司捐赠给新成立的独立非营利 Zulip 基金会，以确保长期稳定。 这确保了 Zulip 这一重要的开源团队聊天平台将独立治理，不依赖于任何单一公司，从而保持其开源性质和社区信任。 Zulip 12.0 于几周前发布，新基金会设立了咨询委员会，包含来自社区的志愿者成员。

hackernews · boramalper · May 15, 18:37 · [社区讨论](https://news.ycombinator.com/item?id=48152168)

**背景**: Zulip 是一个开源团队聊天平台，以其独特的基于主题的线程化而闻名，结合了电子邮件和聊天的优点。它于 2012 年推出，由 Kandra Labs 维护。转为基金会是大型开源项目确保长期治理和独立性的常见举措。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/zulip/zulip">GitHub - zulip/zulip: Zulip server and web application. Open ... Zulip Chat: Open Source Alternative to Slack and Teams (2026 ... Zulip: The Open Source Alternative to Slack & Teams Zulip — organized team chat Self-host Zulip Zulip - GitHub</a></li>
<li><a href="https://zulip.com/">Zulip — organized team chat</a></li>

</ul>
</details>

**社区讨论**: 社区成员对 Zulip 的界面表示赞赏，认为其优于严肃讨论的界面，但有人指出在周五下午宣布可能是为了减少关注度。一位用户推测同时发布的 Bun/Rust 新闻可能影响了时间安排。一位志愿咨询委员会成员确认这些变化有利于 Zulip 的长期稳定。

**标签**: `#open-source`, `#zulip`, `#foundation`, `#team-chat`

---

<a id="item-6"></a>
## [OCaml 太空应用：无 GC 的数据包处理](https://gazagnaire.org/blog/2026-05-14-borealis.html) ⭐️ 8.0/10

一篇新文章描述了如何通过使用带有 exclave 栈注解的 OxCaml，在卫星上实现低延迟数据包处理，从而消除了热路径上的垃圾回收压力。 这表明像 OCaml 这样的垃圾回收语言可用于硬实时太空系统，挑战了常见假设，并扩展了高级语言在嵌入式环境中的适用性。 在调度热路径上使用带 exclave 栈注解的 OxCaml，将每个数据包的 p99.9 延迟从 29 纳秒降低到 9 纳秒，并消除了所有次要 GC（在 2500 万个数据包中从 394 次降为零），同时保持相当的吞吐量。

hackernews · yminsky · May 15, 10:55 · [社区讨论](https://news.ycombinator.com/item?id=48147058)

**背景**: GC 压力指的是频繁内存分配给垃圾回收器带来的负载，可能导致暂停和延迟峰值。在卫星等系统中，低延迟数据包处理至关重要。OCaml 的垃圾回收器是分代的，通过注解进行栈分配可以避免堆分配，从而降低 GC 压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/adrianbailador/reducing-garbage-collector-gc-pressure-in-net-practical-patterns-and-tools-5al3">Reducing Garbage Collector (GC) Pressure in .NET: Practical Patterns and Tools - DEV Community</a></li>
<li><a href="https://www.janestreet.com/tech-talks/safe-at-any-speed/">Safe at Any Speed: Building a Performant, Safe, Maintainable Packet Processor :: Jane Street</a></li>

</ul>
</details>

**社区讨论**: 社区成员指出之前 OCaml 在太空中的使用，例如 2016 年的 GHGSat-D，并讨论了在实时系统中使用垃圾回收语言与手动内存管理之间的权衡。一些人质疑，鉴于现有协议的复杂性，内存安全是否是主要问题。

**标签**: `#OCaml`, `#garbage collection`, `#satellite software`, `#systems programming`, `#real-world OCaml`

---

<a id="item-7"></a>
## [支付宝否认关闭支付后 184 万捐赠扣款责任](https://m.thepaper.cn/newsDetail_forward_33181083) ⭐️ 8.0/10

山西用户反映其支付宝账户在关闭支付功能后，于 2023 年被扣款 184 万元用于公益捐赠。支付宝于 2025 年 5 月 15 日回应称不承担责任，称账户可能被共用，并已向警方寻求帮助。 该事件引发对中国最大移动支付平台支付安全及用户信任的严重担忧。若关闭支付功能后仍可执行交易，将削弱安全控制的可靠性，可能影响数百万用户。 银行调查发现，关闭支付功能后，公益捐赠渠道仍保持付款功能。资金转至中国乡村发展基金会，该基金会称款项已用于公益。

telegram · zaihuapd · May 15, 07:00

**背景**: 支付宝是中国广泛使用的移动支付平台，提供多种支付和捐赠功能。用户可出于安全原因关闭支付功能，但本案表明捐赠等特定功能可能绕开这些控制。该争议凸显了支付系统安全的复杂性以及在发生未经授权交易时确定责任的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.newsglobenow.com/new354383.html">Shanxi Woman Says Alipay Donated CNY 1.84 Million</a></li>
<li><a href="https://min.news/en/tech/9f7403e85bdcd91ae2b4a8ffbba4f2a7.html">What is the reason why the Alipay account payment function is ...</a></li>

</ul>
</details>

**标签**: `#security`, `#fintech`, `#Alipay`, `#payment`, `#user trust`

---

<a id="item-8"></a>
## [苹果与 OpenAI 合作裂痕加深，OpenAI 或起诉](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight) ⭐️ 8.0/10

OpenAI 正考虑对苹果采取法律行动，指责苹果未充分将 ChatGPT 集成到 iOS 中，导致订阅转化率远低于预期。苹果计划在 2026 年 6 月的 WWDC 上向 Claude、Gemini 等第三方模型开放 Siri。 两大 AI 巨头之间的裂痕可能重塑移动 AI 生态系统，苹果正在多样化 AI 合作伙伴，而 OpenAI 则面临失去数亿设备独家接入的风险。结果可能为 AI 集成合同和平台权力动态树立先例。 据报道，iOS 中 ChatGPT 的集成入口隐蔽且功能受限，多数用户仍使用独立的 ChatGPT 应用。苹果也对 OpenAI 的隐私标准、硬件业务以及挖角苹果工程师表示不满。

telegram · zaihuapd · May 15, 12:59

**背景**: 苹果与 OpenAI 于 2024 年宣布合作，将 ChatGPT 集成到 Siri 和其他 iOS 功能中。该合作原本预计通过 ChatGPT Plus 订阅转化带来数十亿美元收入。然而，集成挑战和战略分歧削弱了双方关系，苹果现在正探索与 Anthropic 和 Google 等竞争对手的合作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_AI">Claude AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_AI">Gemini AI</a></li>

</ul>
</details>

**标签**: `#AI`, `#Apple`, `#OpenAI`, `#partnership`, `#legal`

---

<a id="item-9"></a>
## [特朗普与习近平讨论 AI 护栏与英伟达 H200 芯片](https://www.bloomberg.com/news/articles/2026-05-15/trump-says-he-discussed-ai-guardrails-nvidia-s-chips-with-xi) ⭐️ 8.0/10

美国总统特朗普在访华期间与习近平讨论了 AI 安全护栏以及英伟达 H200 芯片出口问题。特朗普称中国选择不购买 H200 芯片，旨在自主研发芯片。 此次高层对话凸显了 AI 安全与半导体出口管制的交集，对全球科技供应链和中美关系具有重大影响。中国放弃 H200 的决定可能加速其本土芯片研发，重塑 AI 硬件市场竞争格局。 美国此前已允许英伟达向中国客户供应 H200，但北京尚未批准任何采购。商务部长 Lutnick 指出，尽管有出口许可，但中国企业未获得政府放行，因此尚无 H200 芯片交付。此前中国曾拒绝性能较低的 H20 芯片。

telegram · zaihuapd · May 15, 15:13

**背景**: AI 护栏是确保 AI 系统在可接受范围内运行、防止有害或有偏见输出的安全机制。此次讨论部分源于 Anthropic 的 Mythos 模型引发的全球网络安全担忧——该模型被认为过于危险而无法公开发布。中美科技竞争导致对先进芯片（如英伟达 H200）实施出口管制，该芯片专为 AI 工作负载设计，但性能低于受更严格限制的顶级型号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms ...</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-guardrails">What are AI guardrails? - IBM</a></li>

</ul>
</details>

**标签**: `#AI`, `#semiconductors`, `#US-China`, `#Nvidia`, `#export controls`

---

<a id="item-10"></a>
## [Palantir 聘用超 30 名英国政府高级官员](https://www.thenational.scot/news/26055524.palantir-hired-30-senior-uk-government-officials/) ⭐️ 7.0/10

据《国家报》报道，Palantir 已聘用超过 30 名英国政府高级官员，这再次引发了关于私营部门影响力与利益冲突的辩论。 此次大规模聘用凸显了政府与私营科技公司之间的所谓“旋转门”现象，引发了关于不当影响及内幕信息可能被滥用的伦理担忧。 在被聘用的 32 名官员中，有 14 人已不在 Palantir 工作，该公司辩称聘用退伍军人是其社会再融入的一部分。批评者则认为这反映了系统性的旋转门策略。

hackernews · Symbiote · May 15, 20:06 · [社区讨论](https://news.ycombinator.com/item?id=48153183)

**背景**: “旋转门”指的是个人在政府职务与私营部门工作之间的流动，通常发生在同一行业内。Palantir 是一家美国数据分析公司，以与情报机构的合同而闻名。此类招聘模式可能引发利益冲突，并削弱公众对政府公正性的信任。

**社区讨论**: 社区评论对旋转门操作表示讽刺，一位用户称这是英国政府的标准操作。另一用户提到一位朋友被一家防务公司以高薪挖走。部分评论批评 Palantir 利用退伍军人就业作为挡箭牌，而一条讽刺评论建议前政府雇员永远不得在私营部门工作。

**标签**: `#Palantir`, `#government transparency`, `#revolving door`, `#ethics`, `#tech industry`

---

<a id="item-11"></a>
## [加州法案要求在线游戏停服时提供离线补丁或退款](https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/) ⭐️ 7.0/10

该法案可能为游戏行业的数字保存和消费者权利树立先例，迫使发行商考虑其在线游戏的长期可玩性。 该法案适用于在加州销售的游戏，并要求在服务器关闭前发出通知；但娱乐软件协会（ESA）认为，对于依赖音乐或 IP 限期许可的游戏，这在技术和法律上可能不可行。

hackernews · Lihh27 · May 15, 19:48 · [社区讨论](https://news.ycombinator.com/item?id=48152994)

**背景**: 许多在线游戏在发行商关闭服务器后变得无法游玩，消费者没有追索权。该法案旨在通过追究发行商责任来解决这一问题，类似于欧洲近期针对数字商品的消费者保护措施。

**社区讨论**: 评论者建议开源服务器代码或对逆向工程者给予豁免作为更好的替代方案，也有人讨论许可和托管基金等实际挑战。消费者保护获得广泛支持，但对该法案的可行性存在怀疑。

**标签**: `#gaming`, `#legislation`, `#digital preservation`, `#consumer rights`

---

<a id="item-12"></a>
## [美国司法部要求苹果和谷歌披露 10 万汽车应用用户](https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/) ⭐️ 7.0/10

美国司法部要求苹果和谷歌披露超过 10 万名汽车篡改应用用户的身份，该应用被用于禁用排放控制，司法部引用非法使用证据。传票针对分发该软件的应用商店。 此案为政府监控与用户隐私之间的平衡树立重要先例，可能抑制数字权利和维修权运动。它还凸显了环境法规与可规避法规的技术工具之间的紧张关系。 该应用用于 OBD-II 调校以禁用排放控制系统，例如删除氧传感器或修改燃油映射。司法部已收集论坛帖子和社交媒体证据显示非法篡改，现在寻求用户身份以采访证人。

hackernews · tencentshill · May 15, 17:28 · [社区讨论](https://news.ycombinator.com/item?id=48151383)

**背景**: 排放 defeat device 是指禁用或绕过车辆排放控制系统的软件或硬件修改，常被用于提升性能。OBD-II 诊断端口原本用于排放测试，而某些应用可通过它修改发动机控制单元（ECU）来进行调校。根据《清洁空气法》，凡在公共道路上行驶的车辆使用此类改装均属非法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Volkswagen_emissions_scandal">Volkswagen emissions scandal - Wikipedia</a></li>
<li><a href="https://www.motortrend.com/how-to/0508ch-program-obd-ii-powertrain-module">Program an OBD-II Powertrain Control Module - Tech Article - Chevy High Performance Magazine</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人批评政府为寻找证人而进行无差别搜查，也有人对为“喷黑烟”等有害行为禁用排放控制的用户表示同情有限。有人担忧先例会被用来针对其他改装，如禁用 GPS 追踪，并警告非法使用可能损害维修权，类似于媒体盗版事件。

**标签**: `#privacy`, `#government surveillance`, `#digital rights`, `#Apple`, `#Google`

---

<a id="item-13"></a>
## [Waymo 召回 3800 辆机器人出租车因涉水故障](https://www.cnbc.com/2026/05/12/waymo-recalls-3800-robotaxis-after-able-drive-into-standing-water.html) ⭐️ 7.0/10

Waymo 正在召回 3800 辆机器人出租车，以修复一个软件缺陷，该缺陷导致部分车辆尽管系统检测到危险并减速，仍然驶入积水中。 此次召回凸显了自动驾驶中的一个关键边缘案例——感知涉水危险，并强调了确保机器出租车在各类天气条件下安全性的挑战。 据美国国家公路交通安全管理局（NHTSA）称，Waymo 的软件足以识别危险并减速，但随后却允许车辆继续前进驶入积水中。此次召回涉及所有当前 Waymo 车辆，正通过空中升级部署软件更新。

hackernews · drob518 · May 15, 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48151767)

**背景**: 自动驾驶汽车依靠摄像头、激光雷达和雷达来感知环境。检测积水尤其困难，因为它看起来与湿路面或反光相似。Waymo 的系统设计用于处理极端条件，但此缺陷表明仅靠推理可能不足以应对所有场景；一些专家建议增加专用的涉水传感器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://waymo.com/waymo-driver/">Self-Driving Car Technology for a Reliable Ride - Waymo Driver</a></li>
<li><a href="https://www.motor1.com/news/781316/waymo-driving-in-flood/">'My Car Is Driving In the Middle Of It': San Francisco Rider Takes a Waymo During a Storm. Then They Look Out the Window</a></li>
<li><a href="https://www.khou.com/article/news/nation-world/waymo-recalls-robotaxis-software-flaw-allowed-vehicles-to-drive-into-floodwater/507-f4a92f83-4cda-4393-9807-fe1b460fc894">Waymo recalls nearly 3,800 robotaxis after software flaw allowed vehicles to drive into floodwater | khou.com</a></li>

</ul>
</details>

**社区讨论**: 社区评论讨论了这一问题的难度，一位用户指出人类也会犯同样错误，并建议像 DARPA 大挑战赛车辆那样增加涉水传感器。另一位评论者质疑是否可以通过车辆行为（减速、转向校正）与机器视觉相结合进行推理，从而避免使用专用传感器；还有一位开玩笑说 Waymo 正在研发潜艇，并询问特斯拉会如何处理这种情况。

**标签**: `#autonomous driving`, `#Waymo`, `#robotaxi`, `#safety`, `#AI perception`

---

<a id="item-14"></a>
## [Meta 获 33 亿美元税收优惠，建百亿美元数据中心](https://fortune.com/2026/05/14/meta-data-center-tax-break-hyperion-louisiana/) ⭐️ 7.0/10

Meta 从路易斯安那州获得了 33 亿美元的税收减免，用于其 100 亿美元的 Hyperion 数据中心项目，该交易通过保密协议和闭门政治达成。 此事凸显了围绕 AI 基础设施公共补贴的争议，以及当地社区难以从中获益的问题，因为数据中心很少创造就业机会且消耗大量资源。 税收优惠免除 Meta 未来 20 年对数据中心设备（包括用于 AI 训练的 GPU）的州和地方销售税，预计在 350 亿美元设备支出上节省约 33 亿美元。

hackernews · logickkk1 · May 15, 19:32 · [社区讨论](https://news.ycombinator.com/item?id=48152825)

**背景**: 数据中心是存放服务器和计算硬件的大型设施，需要大量电力和水资源。相对于其高昂成本，数据中心创造的永久就业岗位很少，因此地方政府为吸引科技公司而提供的慷慨税收激励措施常遭批评。

**社区讨论**: 评论者对公共利益表示怀疑，批评交易保密、缺乏地方意见以及环境影响。有人讽刺地称赞“小公司得到扶持”，质疑公平性。

**标签**: `#data centers`, `#tax incentives`, `#AI infrastructure`, `#Meta`, `#public policy`

---

<a id="item-15"></a>
## [ABC 新闻下线所有 FiveThirtyEight 文章](https://twitter.com/baseballot/status/2055309076209492208) ⭐️ 7.0/10

ABC 新闻已移除 FiveThirtyEight 网站上的所有文章，实际上终结了该品牌在当前所有权下的数字存在。 此举标志着一个备受尊敬的数据新闻品牌的终结，引发了对媒体资产企业管理的担忧以及独特公共利益内容的流失。 FiveThirtyEight 创始人 Nate Silver 据称曾提出回购该品牌，但因批评 ABC 的管理而被拒绝；该网站的 GitHub 仓库仍然可用。

hackernews · cmsparks · May 15, 19:07 · [社区讨论](https://news.ycombinator.com/item?id=48152553)

**背景**: FiveThirtyEight 由 Nate Silver 于 2008 年创立，2013 年被 ABC 新闻收购，以数据驱动的新闻报道政治、体育和科学而闻名。尽管拥有忠实的细分受众，该网站在总统选举年之外难以盈利，导致裁员并最终关闭。

**社区讨论**: 社区评论表达了沮丧和悲伤，一些人批评 ABC 品牌管理不善。Nate Silver 声称 ABC 因他个人的批评而拒绝将 IP 卖回给他，这被视为小气。其他人指出该网站最好的可视化作品和文章现已丢失，并呼吁备份其 GitHub 仓库。

**标签**: `#journalism`, `#data-visualization`, `#media`, `#five-thirty-eight`, `#news`

---

<a id="item-16"></a>
## [像 Windows XP 桌面一样浏览维基百科](https://explorer.samismith.com/) ⭐️ 7.0/10

一个新的 Web 应用程序 Explorer.samismith.com 重现了 Windows XP 桌面环境，让用户通过熟悉的怀旧界面浏览维基百科文章。 该项目引发了对 UI 范式和心智模型的讨论，展示了经典设计如何改善信息浏览体验并唤起强烈的怀旧共鸣。 该应用模拟了 Windows XP 的视觉风格，包括窗口边框、大滚动条和文件夹图标，将维基百科类别映射为文件夹，文章映射为文档。

hackernews · smusamashah · May 15, 08:45 · [社区讨论](https://news.ycombinator.com/item?id=48146129)

**背景**: Windows XP 于 2001 年发布，以其 Luna 主题和基于文件夹的导航隐喻而闻名，许多用户认为这种设计直观易用。该项目利用对那个时代的怀旧情绪，探索旧的 UI 惯例如何为现代内容浏览服务。

**社区讨论**: 评论者对这一怀旧设计表达了强烈赞赏，指出文件夹/文档隐喻很好地对应了人们心中知识组织的方式。有人指出其风格更像 Windows XP Media Center Edition 而非标准 XP，但总体反馈高度正面。

**标签**: `#UI design`, `#retro computing`, `#information browsing`, `#web project`

---

<a id="item-17"></a>
## [Jason Scott 的 ASCII 博客：数字保存获赞誉](https://ascii.textfiles.com/) ⭐️ 7.0/10

Hacker News 的一篇帖子重点介绍了 Jason Scott 的博客'ASCII by Jason Scott'（ascii.textfiles.com），赞扬了他持续的数字保存工作，包括数字化超过 1,300 盘磁带以及在十年间将 13,000 份手册归档至互联网档案馆。 这一认可突显了数字保存在保护文化和历史遗产方面的关键作用，Jason Scott 的丰硕成果激励了整个存档社区。 该博客托管在 ascii.textfiles.com 上，帖子中的社区评论提到了 Scott 的个人魅力及其工作的规模，例如数字化了来自个人收藏的 1,300 盘磁带，并在十年间保持每天约 3.5 份手册的归档速度。

hackernews · bookofjoe · May 15, 14:02 · [社区讨论](https://news.ycombinator.com/item?id=48148726)

**背景**: textfiles.com 是 Jason Scott 于 1998 年创建的网站，旨在保存 BBS 时代的文本文件，内容涵盖黑客指南到 ASCII 艺术。Scott 还是 Archive Team 的联合创始人，并在互联网档案馆工作，领导诸如在浏览器中模拟老平台等举措。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Textfiles.com">Textfiles.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/Archive_Team">Archive Team - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区表达了强烈的赞赏，一位评论者（rhgraysonii）分享了 Scott 数字化他们收集的超过 1,300 盘磁带的个人经历。其他人则强调了那令人印象深刻的存档速度——十年间每天 3.5 份手册——并提到 Scott 正在 Twitch 上进行直播。

**标签**: `#digital preservation`, `#archiving`, `#Jason Scott`, `#ASCII`, `#textfiles`

---

<a id="item-18"></a>
## [Radicle 推出主权去中心化 Git 锻造平台](https://radicle.dev/) ⭐️ 7.0/10

Radicle 发布了其“主权锻造平台”，这是一个基于 Git 的去中心化点对点代码协作平台，现已成熟，支持本地优先和私有仓库。 这提供了一个可行的去中心化替代方案，取代了 GitHub 等中心化锻造平台，赋予开发者对其数据和工作的完全控制权。对于关注供应商锁定的代理工作流和社区尤为重要。 Radicle 结合 Git 的架构、密码学和 gossip 协议进行点对点复制。它支持私有仓库，新更新不会公开，但历史记录仍可访问。

hackernews · KolmogorovComp · May 15, 12:07 · [社区讨论](https://news.ycombinator.com/item?id=48147603)

**背景**: 代码锻造平台是托管和协作源代码仓库的平台，通常如 GitHub 或 GitLab 是中心化的。本地优先软件强调离线能力和用户数据所有权。Radicle 旨在以去中心化方式结合这些概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://radicle.dev/">The Radicle forge is an open source, peer-to-peer code collaboration...</a></li>
<li><a href="https://decrypt.co/223462/decentralized-github-radicle-launches-1-0-pioneering-decentralized-code-collaboration">“Decentralized Github” Radicle Launches 1.0, Pioneering ...</a></li>
<li><a href="https://www.cosmicjs.com/blog/cosmic-rundown-radicle-docker-google-search-api-changes">Cosmic Rundown: Radicle's Sovereign Forge, Docker Identity ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论对缺乏 AGPL 许可表示担忧，这可能导致 SaaS 公司进行“拥抱、扩展、消灭”。其他人赞扬其本地优先设计和私有仓库支持，并指出其对代理工作流的实用性。还有用户提到域名迁移以及过去仓库删除的问题。

**标签**: `#decentralized`, `#git`, `#code forge`, `#licensing`, `#open source`

---

<a id="item-19"></a>
## [新书探讨乔布斯在 NeXT 的岁月](https://spectrum.ieee.org/steve-jobs-next-computer) ⭐️ 7.0/10

IEEE Spectrum 出版了一本新书，详细介绍了史蒂夫·乔布斯在 NeXT Computer 的“被遗忘的流放岁月”，涵盖 NeXTSTEP 操作系统和面向对象编程概念的发展，这些后来重塑了苹果。 这本书深入揭示了 NeXT 的创新如何成为现代苹果（包括 macOS 和 iOS）的基础，挑战了将乔布斯的天才简单归因于其个性的片面叙述。 这本书审视了乔布斯在 NeXT 12 年间的成长，既突出了 NeXTSTEP 和首个网页浏览器等技术突破，也提到了公司财务困境，最终导致苹果在 1996 年收购 NeXT。

hackernews · rbanffy · May 15, 10:34 · [社区讨论](https://news.ycombinator.com/item?id=48146908)

**背景**: NeXT 由史蒂夫·乔布斯在 1985 年离开苹果后创立，专注于面向教育和商业的高端工作站。其操作系统 NeXTSTEP 是面向对象的，基于 Mach 内核和 BSD Unix，并孕育了蒂姆·伯纳斯-李创建的第一个网页浏览器。1996 年，苹果收购 NeXT 以取代老化的经典 Mac OS，NeXT 技术成为 macOS 及后来 iOS 的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spectrum.ieee.org/steve-jobs-next-computer">Steve Jobs Next Computer : His Forgotten Exile Years - IEEE Spectrum</a></li>
<li><a href="https://en.wikipedia.org/wiki/NeXT">NeXT - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/NeXTSTEP_(operating_system)">NeXTSTEP (operating system)</a></li>

</ul>
</details>

**社区讨论**: 评论者对这本书表示期待，并讨论乔布斯的遗产，许多人指出现代苹果很大程度上是 NeXT 的延续。一些人认为 NeXT 在商业上是失败的，但在技术上是胜利的，而另一些人则纠正文章对 Apple II 成功的忽视，并强调乔布斯贡献的复杂性。

**标签**: `#Steve Jobs`, `#NeXT`, `#Apple`, `#book`, `#tech history`

---

<a id="item-20"></a>
## [累积上下文破解气象预测长期误差难题](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247890898&idx=4&sn=d075b46de39b2318be648f978a45257e) ⭐️ 7.0/10

一篇名为《Efficient Multi-Scale Transformer for Accumulative Context Weather Forecasting》的论文被 ICML 2026 接收，提出了一种利用累积上下文的新型多尺度 Transformer 架构，能显著降低气象预测的长期误差。 该工作解决了气象预测中限制机器学习模型实际部署的关键难题——长期误差累积。通过提升精度和效率，它可能惠及气候研究、灾害预警等时效性强的应用领域。 EMFormer（高效多尺度 Transformer）模型利用累积上下文捕获跨多个时空尺度的短程和长程依赖关系，在气象基准测试上取得优越性能，并展现出对视觉任务的跨域适应能力。

rss · 量子位 · May 15, 02:10

**背景**: Transformer 模型在许多领域表现出色，但在气象预测等长序列预测任务中因误差累积而表现不佳。多尺度架构以不同分辨率处理特征，提升效率和准确性。“累积上下文”的概念通过随时间聚合信息来减轻误差累积。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.sina.com.cn/tech/csj/2026-05-15/doc-inhxxwvr3389268.shtml">气象预测长期误差太难搞？Icml 2026 这项成果用"累积上下文"给出了最优解_创事记_新浪科技_新浪网</a></li>
<li><a href="https://www.itsolotime.com/archives/34768">ICML 2026论文：EMFormer破解气象预测三大痛点，精度效率双提升还能跨界视觉任务 - 鲸林向海</a></li>
<li><a href="https://channel.ccino.org/posts/6636627">量子位气象预测长期误差太难搞？ICML 2026 这项成果用"累积上下文"给出了最优解 Telegraph | 原文 | 科技频道 [奇诺 ...</a></li>

</ul>
</details>

**标签**: `#机器学习`, `#Transformer`, `#气象预测`, `#多尺度`, `#ICML`

---

<a id="item-21"></a>
## [英伟达市值盘中突破 5.5 万亿美元](https://www.ithome.com/0/950/303.htm) ⭐️ 7.0/10

2025 年 5 月 13 日，英伟达盘中市值首次突破 5.5 万亿美元，成为首家达到这一里程碑的上市公司。 这一里程碑凸显了英伟达在 AI 硬件领域的主导地位和投资者的巨大信心，其市值已超过世界第三大经济体德国的名义 GDP。 该股早盘上涨 3%，自 2026 年初以来市值增长 19.58%。相比之下，Alphabet 市值为 4.86 万亿美元，苹果为 4.39 万亿美元，微软为 3.01 万亿美元。

telegram · zaihuapd · May 14, 16:43

**背景**: 英伟达是图形处理单元（GPU）和 AI 加速器的领先设计者，这些硬件对于训练大型语言模型和其他 AI 工作负载至关重要。近年来，由于 AI 热潮，该公司市值飙升，成为全球最有价值的公司之一。这一里程碑反映了市场基于 AI 普及相关未来盈利预期对英伟达的估值。

**标签**: `#Nvidia`, `#market cap`, `#AI hardware`, `#finance`

---

<a id="item-22"></a>
## [ChatGPT Android 版拆解发现 Codex 远程桌面控制功能](https://t.me/zaihuapd/41388) ⭐️ 7.0/10

对 ChatGPT Android 1.2026.125 版本的 APK 拆解发现，OpenAI 正在为 Codex 开发远程桌面控制功能，用户可通过手机查找并重连远程桌面会话。 该功能将极大扩展 Codex 的实用性，允许开发者通过手机管理编码会话，使其在需要远程监控或控制工作时更加灵活。 该功能仍在开发中，目前尚无可用预览或公布发布日期；使用时要求桌面端与手机端登录同一账号。

telegram · zaihuapd · May 14, 21:48

**背景**: OpenAI Codex 是一个 AI 编程代理，可在本地或云端运行，能执行代码生成、重构和调试等任务。它通过文件访问、shell 执行和沙盒机制封装了 OpenAI 的前沿模型，为智能编程提供了一个指挥中心。远程桌面功能将允许用户从手机控制桌面上的 Codex 会话，提高了灵活性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI</a></li>
<li><a href="https://www.freecodecamp.org/news/the-codex-handbook-a-practical-guide-to-openai-s-coding-platform/">The Codex Handbook: A Practical Guide to OpenAI's Coding Platform</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai/codex: Lightweight coding agent that runs in ...</a></li>

</ul>
</details>

**标签**: `#ChatGPT`, `#Codex`, `#OpenAI`, `#remote desktop`, `#Android`

---

<a id="item-23"></a>
## [AMD 确认 FSR 4.1 将于 7 月支持 RX 7000，2027 年初覆盖 RX 6000](https://videocardz.com/newz/amd-fsr-upscaling-4-1-officially-coming-to-radeon-rx-7000-gpus-in-july-rx-6000-in-2027) ⭐️ 7.0/10

AMD 宣布，基于机器学习的 FSR 4.1 超分辨率技术将于 2025 年 7 月在 Radeon RX 7000 系列（RDNA 3）上推出，并计划于 2027 年初支持 RX 6000 系列（RDNA 2）。 这一官方时间表为 PC 玩家提供了明确预期，让他们知道何时能享受到 FSR 4.1 带来的图像质量和性能提升。该版本针对使用 INT8 指令的第一代 AI 加速器进行了优化，发布时即支持超过 300 款游戏。 FSR 4.1 相比 FSR 4.0 提升了锐度，并对超高性能模式和动态分辨率缩放模式进行了优化。RX 6000 系列（RDNA 2）由于缺乏专用 AI 加速器，将稍后获得支持。

telegram · zaihuapd · May 15, 04:57

**背景**: AMD FidelityFX Super Resolution (FSR) 是一种超分辨率技术，通过以较低分辨率渲染再重建高质量图像来提升帧率，与 NVIDIA 的 DLSS 竞争。FSR 4.1 利用 RDNA 3 GPU 第一代 AI 加速器上的机器学习和 INT8 指令，而早期的 FSR 版本是纯空间上采样器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.amd.com/en/products/graphics/technologies/fidelityfx/super-resolution.html">AMD FSR ™ Technologies</a></li>
<li><a href="https://www.tomshardware.com/reference/amd-fsr-fidelityfx-super-resolution-explained">What Is AMD FSR ? FidelityFX Super Resolution Explained</a></li>
<li><a href="https://en.wikipedia.org/wiki/RDNA_(microarchitecture)">RDNA (microarchitecture) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AMD`, `#FSR`, `#GPU`, `#Upscaling`, `#Gaming`

---