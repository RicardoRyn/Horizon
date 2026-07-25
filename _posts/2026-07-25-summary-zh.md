---
layout: default
title: "Horizon Summary: 2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> From 34 items, 16 important content pieces were selected

---

1. [Android 可能限制设备端 ADB 访问](#item-1) ⭐️ 8.0/10
2. [开放权重 AI 的 Kubernetes 时刻](#item-2) ⭐️ 8.0/10
3. [Tile 安全缺陷使跟踪成为可能](#item-3) ⭐️ 8.0/10
4. [Telegram 零点击崩溃漏洞已静默修复](#item-4) ⭐️ 8.0/10
5. [Anthropic 发布 Claude Opus 5：性能接近 Fable 5，价格减半](#item-5) ⭐️ 8.0/10
6. [中国离岸信托个税新规：装入财产及收益须申报纳税](#item-6) ⭐️ 8.0/10
7. [上海携程因数据出境违规被罚 1000 万元](#item-7) ⭐️ 8.0/10
8. [市场监管总局对携程罚没 51.79 亿元](#item-8) ⭐️ 8.0/10
9. [微软将用 TPM 芯片封堵盗版 Windows 激活](#item-9) ⭐️ 8.0/10
10. [私刑者拆除 Flock 监控摄像头以抗议隐私侵犯](#item-10) ⭐️ 7.0/10
11. [AI 自动化数学定理证明引发存在危机](#item-11) ⭐️ 7.0/10
12. [Fedora 45 构建管道指南](#item-12) ⭐️ 7.0/10
13. [Vivix 发布首个实时多模态交互模型](#item-13) ⭐️ 7.0/10
14. [黄仁勋：美国应允许使用中国开源 AI 模型](#item-14) ⭐️ 7.0/10
15. [马斯克支持库克称内存价格暴涨前所未见，美光 CCO 指责苹果压价](#item-15) ⭐️ 7.0/10
16. [AMD 确认 Zen 7 EPYC 2028 年发布，Zen 8 2030 年登场](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Android 可能限制设备端 ADB 访问](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

Android 正考虑限制设备端 ADB（Android 调试桥）访问，尤其是限制通过 TCP 进行的远程调试。 这一限制将严重影响依赖无线 ADB 进行调试和测试的开发者，凸显了安全改进与开发者工作流自由之间的张力。 拟议的变更可能涉及将 ADB 连接限制到特定 IP 地址或接口，而非允许所有连接，部分人呼吁采用白名单方式。

hackernews · shscs911 · Jul 25, 06:57 · [社区讨论](https://news.ycombinator.com/item?id=49045159)

**背景**: Android 调试桥（ADB）是一个多功能命令行工具，允许开发者通过 USB 或 TCP 与 Android 设备通信，用于调试、应用安装和文件传输。设备端 ADB 允许直接在设备本身上运行 ADB 命令，无需计算机。拟议的变更针对的是通过 TCP 的远程 ADB，这通常是开发者为无线调试而启用的功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge ( adb ) | Android Studio | Android Developers</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人支持安全改进，但质疑其益处，因为开启开发者选项和远程 ADB 是前提条件。另一些人担心 Google 会借此控制开发，而一些人则认为白名单方式会是更好的折衷方案。

**标签**: `#Android`, `#ADB`, `#security`, `#development`, `#privacy`

---

<a id="item-2"></a>
## [开放权重 AI 的 Kubernetes 时刻](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

这篇文章认为，开放权重 AI 模型正成为 AI 基础设施的标准，就像 Kubernetes 标准化云计算一样。 如果开放权重模型成为标准，它可以普及 AI 访问，减少对单一供应商的依赖，并降低企业和开发者的成本，类似于 Kubernetes 对云可移植性的影响。 开放权重模型并不一定意味着完全开源；训练数据和代码通常不公开。此外，权重是数值，无法追溯到原产国，使得禁止变得不可行。

hackernews · tknaup · Jul 25, 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: 开放权重 AI 指的是一类模型，其训练后的权重公开发布，允许他人运行或微调，但训练数据和代码可能仍为专有。Kubernetes 是一个用于自动化容器化应用程序部署、扩展和管理的开源系统，已成为云基础设施的事实标准。本文将其与开放权重 AI 类比，认为开放权重模型可能类似地标准化 AI 基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**社区讨论**: 评论者质疑禁止中国模型的可行性，指出权重只是数字，没有来源归属。还有人讨论专有 API 定价的不稳定性（“代币经济学”），认为开放权重模型提供了成本基准。还有呼吁像 Linux 那样进行协作开发。

**标签**: `#open-weight AI`, `#Kubernetes`, `#AI infrastructure`, `#open source`, `#AI models`

---

<a id="item-3"></a>
## [Tile 安全缺陷使跟踪成为可能](https://blog.adafruit.com/2026/03/05/tiles-security-is-so-bad-its-a-feature-for-stalkers/) ⭐️ 8.0/10

安全研究人员发表论文，详细描述了 Life360 的 Tile 蓝牙追踪器中的多个漏洞，包括缺乏加密和能够绕过反跟踪措施，从而允许未经授权跟踪用户。 这些漏洞影响了数百万 Tile 用户，带来严重的隐私和跟踪风险，并凸显了物联网追踪设备需要更强加密的必要性。该发现可能推动行业采用类似苹果和谷歌端到端加密追踪器的更安全标准。 这些漏洞包括敏感数据（如 MAC 地址和位置）未加密传输、能够覆盖 Tile 的防盗窃模式，以及跟踪者可在不被发现的情况下秘密监控受害者的可能性。论文可在 arXiv 上获取，编号 2510.00350。

hackernews · sambellll · Jul 25, 18:18 · [社区讨论](https://news.ycombinator.com/item?id=49050152)

**背景**: Tile 追踪器是用于定位丢失物品的小型蓝牙设备，依赖众包应用网络报告位置。与使用端到端加密的苹果 AirTags 等追踪器不同，Tile 以明文传输数据，使其易被拦截和滥用。这些设计缺陷已被 MIT 和 EFF 等机构的研究人员指出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.malwarebytes.com/blog/news/2025/09/tile-trackers-plagued-by-weak-security-researchers-warn">Tile trackers plagued by weak security, researchers warn | Malwarebytes</a></li>
<li><a href="https://www.eff.org/deeplinks/2025/10/tiles-lack-encryption-danger-users-everywhere">Tile’s Lack of Encryption Is a Danger for Users Everywhere | Electronic Frontier Foundation</a></li>
<li><a href="https://www.wired.com/story/tile-tracking-tags-can-be-exploited-by-tech-savvy-stalkers-researchers-say/">Tile Tracking Tags Can Be Exploited by Tech-Savvy Stalkers, Researchers Say | WIRED</a></li>

</ul>
</details>

**社区讨论**: 论文的末位作者 Michael Specter 评论表示愿意回答问题。用户 Ollien 指出苹果和谷歌等其他追踪器使用端到端加密，并询问私钥的处理方式。另一位评论者认为 Temu 上存在更便宜的专用跟踪设备，质疑破解 Tile 的实际意义。

**标签**: `#security`, `#IoT`, `#privacy`, `#tracking`, `#vulnerabilities`

---

<a id="item-4"></a>
## [Telegram 零点击崩溃漏洞已静默修复](https://x.com/Fried_rice/status/2080200610985689222) ⭐️ 8.0/10

安全研究人员 Kimi K3 披露了一个影响 Telegram Desktop 和 iOS 客户端的零点击崩溃漏洞，攻击者可通过特制消息导致应用崩溃。Telegram Desktop 已在最近更新中静默修复，但 iOS 尚未修补。 该漏洞无需用户交互即可利用，极易用于拒绝服务攻击，因此意义重大。桌面版用户应立即更新，iOS 用户仍需等待修复。 概念验证机器人 @kimifuckingbot 可使未修复的客户端崩溃，且桌面版更新未在更新日志中提及此修复。该漏洞通过特制消息导致内存耗尽。

telegram · zaihuapd · Jul 24, 15:06

**背景**: 零点击漏洞允许攻击者在用户无需任何操作（如点击链接或打开文件）的情况下远程攻击设备。在此案例中，漏洞存在于 Telegram 的消息处理逻辑中，恶意消息可导致桌面版和可能的 iOS 客户端内存耗尽崩溃。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Zero-click_exploit">Zero-click exploit</a></li>
<li><a href="https://www.kaspersky.com/resource-center/definitions/what-is-zero-click-malware">Zero-Click Exploits</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Telegram`, `#zero-click`, `#crash`

---

<a id="item-5"></a>
## [Anthropic 发布 Claude Opus 5：性能接近 Fable 5，价格减半](https://www.anthropic.com/news/claude-opus-5) ⭐️ 8.0/10

Anthropic 发布了 Claude Opus 5，该模型性能接近旗舰 Claude Fable 5，但使用成本仅为后者的一半。它在 Frontier-Bench、ARC-AGI 3 和 Zapier AutomationBench 等基准测试中刷新了纪录。 此次发布提供了一款比旗舰 Fable 5 更具成本效益的替代方案，使开发者和企业能够更轻松地获得高端 AI 能力。这也展示了 Anthropic 在优化模型性能和成本效率方面的持续进步。 Opus 5 现已成为 Claude Max 的默认模型，也是 Claude Pro 上最强的模型，定价与上一代 Opus 4.8 相同。然而，它在网络安全任务上仍落后于 Mythos 5，并且部分基准测试结果存在细微差异（例如 Agentic coding 53.4% vs 53.5%）。

telegram · zaihuapd · Jul 24, 17:03

**背景**: Anthropic 的 Claude 模型按级别划分：Opus（中高端）、Fable（高端，带有安全护栏）和 Mythos（限制访问，最强大）。Opus 5 是 Opus 系列的最新版本，而 Fable 5 和 Mythos 5 于 2026 年 6 月发布。ARC-AGI 3 是近期推出的交互式推理基准，旨在评估智能体智能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/redeploying-fable-5">Redeploying Claude Fable 5 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>

</ul>
</details>

**社区讨论**: 有评论指出 Agentic coding 基准测试分数存在细微差异（53.4% vs 53.5%），并暗示官网已通过 OTA 更新。这反映了社区对基准细节和模型比较的密切关注。

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#模型发布`, `#大语言模型`

---

<a id="item-6"></a>
## [中国离岸信托个税新规：装入财产及收益须申报纳税](https://liaoning.chinatax.gov.cn/art/2026/7/24/art_5869_7823.html) ⭐️ 8.0/10

2026 年 7 月 24 日，财政部和税务总局发布 2026 年第 21 号公告，规定居民个人将财产装入离岸信托须按财产转让所得缴纳个税，信托存续期间产生的收益无论是否分配均须按年申报纳税。 该新规彻底封堵了高净值人群利用离岸信托延迟或规避中国个人所得税的避税空间，标志着跨境税务征管显著收紧，可能影响众多家族信托的架构设计。 全流程所有收益的法定税率统一为 20%，仅对增值部分（现值减原值减成本）征税。新规采用穿透式征税原则，委托人须按年对信托收益纳税，即使未实际分配；对 2023 年至 2025 年期间已装入但未缴税的部分，允许在 90 天内补缴且不加收滞纳金。

telegram · zaihuapd · Jul 25, 00:31

**背景**: 离岸信托是指在委托人居住国以外的司法管辖区设立的信托，常被用于资产保护和税务规划。此前，装入离岸信托的收益在中国仅在实际分配给受益人时才征税，使得高净值人士能够延迟甚至规避个人所得税。新规引入穿透式征税原则，将信托的经济实质直接归属于居民个人按年征税，取消延迟纳税的好处。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.jiemian.com/article/13116239_sina.html">投教· 信 托 | 离 岸 信 托 是 什 么 ？ 家族 信 托 为何风险频出？ | 界面新闻</a></li>
<li><a href="https://fly63.com/tool/gerenshui/zhuanrang.html">财 产 转 让 所 得 个 税 计算器</a></li>
<li><a href="https://www.hengtai-law.com/insight/research/data_109.html">hengtai-law.com/insight/research/data_109.html</a></li>

</ul>
</details>

**标签**: `#税务`, `#离岸信托`, `#个人所得税`, `#政策法规`

---

<a id="item-7"></a>
## [上海携程因数据出境违规被罚 1000 万元](https://t.me/zaihuapd/42758) ⭐️ 8.0/10

2025 年 6 月 13 日，上海网信办对上海携程商务有限公司处以 1000 万元罚款，原因是其未落实数据出境安全评估要求、违法向境外提供个人信息。该公司已配合整改。 此次执法行动表明中国正加大数据出境合规的打击力度，尤其是针对处理个人信息的互联网企业。这强烈提醒各组织必须遵守《数据安全法》和《个人信息保护法》下的数据安全评估和跨境数据传输规定。 罚款 1000 万元（约合 140 万美元）的原因是违反了数据出境安全评估要求和个人信息保护法。该公司须在规定期限内整改，并已开始配合调查。

telegram · zaihuapd · Jul 25, 02:24

**背景**: 中国的数据出境安全评估要求是根据《数据安全法》（2021 年）和《个人信息保护法》（2021 年）制定的，规定组织在向境外提供重要数据或个人信息前必须通过安全评估。国家互联网信息办公室（CAC）发布了详细指南，包括《数据出境安全评估办法》和《促进和规范数据跨境流动规定》。此次罚款是针对旅游、电商等行业互联网企业未合规的更广泛执法趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cac.gov.cn/2025-06/27/c_1752652339765002.htm">国家互联网信息办公室发布《数据出境安全评估申报指南（第三版）》_中央网络安全和信息化委员会办公室</a></li>
<li><a href="https://www.secrss.com/articles/52080">我国数据出境安全评估管理政策解读与合规建议 - 安全内参 | 决策者的网络安全知识库</a></li>
<li><a href="https://www.cac.gov.cn/2024-03/22/c_1712776611775634.htm">促进和规范数据跨境流动规定_中央网络安全和信息化委员会办公室</a></li>

</ul>
</details>

**标签**: `#data privacy`, `#regulatory compliance`, `#China`, `#data export`, `#enforcement`

---

<a id="item-8"></a>
## [市场监管总局对携程罚没 51.79 亿元](https://t.me/zaihuapd/42767) ⭐️ 8.0/10

7 月 25 日，国家市场监管总局依据反垄断法对携程集团滥用市场支配地位行为作出行政处罚，没收违法所得 16.58 亿元，并处罚款 35.21 亿元，罚没合计 51.79 亿元。 这是针对中国科技公司最大的反垄断罚单之一，标志着中国科技行业监管力度加强，并将影响在线旅游市场的竞争格局。 携程还被责令退还强制扣除酒店经营者的订单储备金 1.22 亿元，并要求全面整改并公开整改措施。

telegram · zaihuapd · Jul 25, 11:56

**背景**: 中国《反垄断法》禁止滥用市场支配地位，如不公平定价或搭售行为。携程作为中国最大的在线旅行社，因涉嫌抑制竞争、损害酒店经营者利益而被调查。

**标签**: `#Antitrust`, `#Regulation`, `#Ctrip`, `#Chinese Tech`, `#Monopoly`

---

<a id="item-9"></a>
## [微软将用 TPM 芯片封堵盗版 Windows 激活](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

微软宣布将为其批量激活服务 KMS 增加基于 TPM 芯片的硬件安全验证，从下一版 Windows Server 开始实施。这种“TPM 证明”机制将确保只有经过认证且未被篡改的 KMS 服务器才能处理激活请求，从而有效封堵伪造激活工具。 此举显著增强了 Windows 授权安全性，可能导致许多现有的基于 KMS 的盗版激活方法失效。企业 IT 管理员和反盗版工作将直接受到影响，但与 Massgrave 的 TSforge 等激活绕过工具的攻防战可能会持续。 新要求将从下一版 Windows Server 起成为强制，自 2026 年 8 月起在 Windows Server 2025 中推送准备提示。TPM 证明要求 KMS 主机通过 TPM 生成加密证明，微软验证该证明及平台完整性后，才允许处理激活请求。

telegram · zaihuapd · Jul 25, 15:55

**背景**: TPM（可信平台模块）是一种硬件安全芯片，提供加密操作和安全存储，常用于 BitLocker 和 Windows Hello 等功能。KMS（密钥管理服务）是微软面向企业提供的批量激活技术，允许组织在局域网内激活多个 Windows 和 Office 安装。多年来，第三方工具通过设置伪造的 KMS 服务器来激活盗版副本，微软一直试图封堵这种方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eet-china.com/news/202107060732.html">Win11要的 TPM 2.0不一定 是 独立 芯 片 ，你的CPU...</a></li>
<li><a href="https://post.smzdm.com/p/apqzrzr0/">白嫖纪元终结！ 微软出手整顿Windows盗版 KMS 激 活 _IT...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/24002737516">TSforge，Windows/Office最新激活方案 - 知乎</a></li>

</ul>
</details>

**标签**: `#Windows`, `#security`, `#TPM`, `#anti-piracy`, `#KMS`

---

<a id="item-10"></a>
## [私刑者拆除 Flock 监控摄像头以抗议隐私侵犯](https://www.theguardian.com/us-news/ng-interactive/2026/jul/25/flock-surveillance-cameras) ⭐️ 7.0/10

据《卫报》报道，一场日益壮大的私刑运动正在美国各地物理破坏 Flock 监控摄像头，其动机源于对隐私的担忧和对政府的不信任。 这场运动凸显了公共安全监控与公民自由之间的紧张关系，可能标志着公众对大规模监控技术接受度的转变。 Flock 摄像头是自动车牌识别系统，能够捕捉并存储车辆位置数据。试图破坏这些摄像头可能面临法律风险，包括违反《计算机欺诈与滥用法案》的指控。

hackernews · bookofjoe · Jul 25, 19:02 · [社区讨论](https://news.ycombinator.com/item?id=49050538)

**背景**: Flock Safety 是一家向执法机构和社区提供具备 ALPR 技术的监控摄像头的公司。这些摄像头持续扫描车牌并标记可疑车辆。然而，有关警员滥用系统以及缺乏监督的报道助长了隐私方面的反弹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Automatic_number-plate_recognition">Automatic number-plate recognition - Wikipedia</a></li>
<li><a href="https://www.cnet.com/home/security/when-flock-comes-to-town-why-cities-are-axing-the-controversial-surveillance-technology/">When Flock Comes to Your Town: I Asked Experts What to Do... - CNET</a></li>
<li><a href="https://trafficvision.live/blog/flock-cameras">Flock Cameras : What They Are & Can You Watch... | TrafficVision.Live</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了多种观点：有人将破坏行为视为对政府越权的回应，而另一些人则质疑真正的问题在于对执法的不信任而非隐私本身。还有少数人提出了细致的监管框架建议。

**标签**: `#surveillance`, `#privacy`, `#civil disobedience`, `#Flock`, `#technology and society`

---

<a id="item-11"></a>
## [AI 自动化数学定理证明引发存在危机](https://kirwinhampshire.substack.com/p/the-dark-night-of-mathematics) ⭐️ 7.0/10

文章《数学的黑暗之夜》探讨了自动化定理证明（尤其是结合 Lean 4 等 AI 工具）的进展如何导致数学家们质疑自身角色和该领域的未来。 这很重要，因为它反映了知识工作者在 AI 自动化智力任务时面临的更广泛危机，并迫使人们重新评估人类在数学等创造性和严谨学科中的贡献意义。 该文章引发了超过 125 条评论，显示出活跃的社区讨论。自动化定理证明（ATP）使用计算机程序生成形式化证明，而 Lean 4 等 AI 辅助工具正在加速进展，mathlib4 已包含超过 150 万个定理。

hackernews · rmdmphilosopher · Jul 25, 15:54 · [社区讨论](https://news.ycombinator.com/item?id=49048681)

**背景**: 自动化定理证明是计算机科学和数理逻辑的一个子领域，旨在使用计算机程序自动证明数学定理。最近的进展，特别是 Lean 4 等交互式定理证明器和大语言模型，使得证明以前只能由人类完成的复杂定理成为可能。这一进展引发了关于数学研究未来和人类数学家角色的哲学讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Automated_theorem_proving">Automated theorem proving</a></li>
<li><a href="https://leandojo.org/">AI -Driven Formal Theorem Proving in the Lean Ecosystem</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了多样化的观点：一些人认为这与知识工作者面临的其他危机类似，而另一些人则欢迎探索更多问题的能力。有人质疑现在 AI 能够反驳的开放猜想的质量，少数人指出即使对世界不是新发现，个人探索仍然有价值。

**标签**: `#mathematics`, `#AI`, `#philosophy`, `#work`

---

<a id="item-12"></a>
## [Fedora 45 构建管道指南](https://supakeen.com/weblog/the-fedora-45-sausage-factory/) ⭐️ 7.0/10

一份全面解释 Fedora 发布版本端到端构建流程的指南已发布，详细介绍了 Koji 和 Bodhi 等工具的使用。 这份文档帮助贡献者和用户排查构建问题并理解发布流程，提高了 Fedora 生态系统的透明度和可重复性。 该指南涵盖了从源代码到发布镜像的整个流程，包括使用 Mock 和 Koji 的洁净室构建。它还讨论了历史细节，例如过去因意外依赖而成功的构建案例。

hackernews · 6581 · Jul 25, 11:04 · [社区讨论](https://news.ycombinator.com/item?id=49046525)

**背景**: Fedora 使用 Koji 作为其 RPM 构建系统，该系统依赖 Mock 创建隔离的 chroot 环境以实现可重复构建。Bodhi 管理 Fedora 版本的更新和仓库。理解这一流程对于任何为 Fedora 做贡献或排查构建问题的人来说都至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.fedoraproject.org/en-US/package-maintainers/Using_the_Koji_Build_System/">Using the Koji build system :: Fedora Docs</a></li>
<li><a href="https://fedoraproject.org/wiki/Koji">Koji - Fedora Project Wiki</a></li>
<li><a href="https://fedoraproject.org/wiki/Bodhi">Bodhi - Fedora Project Wiki</a></li>

</ul>
</details>

**社区讨论**: 评论者赞赏这份文档的故障排查价值，并询问哪里可以找到志愿者机会。一位用户指出洁净室构建历史上的不一致性，强调严格的隔离并非始终得到执行。

**标签**: `#Fedora`, `#Linux`, `#build pipeline`, `#open source`, `#reproducibility`

---

<a id="item-13"></a>
## [Vivix 发布首个实时多模态交互模型](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247907132&idx=1&sn=d7a8826cdab0a961a7c666cf765f4db9) ⭐️ 7.0/10

Vivix 发布了首个实时交互多模态模型，单卡吞吐量达每秒 10000 视频 token。该模型强调开源、隐私优先和本地优先的设计理念。 这一突破使得在消费级硬件上实现实时多模态生成（如视频、音频、文本）成为可能，有望推动 AI 媒体创作普及化。其开源和隐私优先的立场可能引导行业向更易获取、更可信赖的 AI 系统转变。 该模型采用 E-GRM（基于熵的生成式奖励模型），动态决定是否使用思维链推理，并用混合损失判别评分器替代传统投票。它采用统一流式架构，覆盖全多模态生成链路。

rss · 量子位 · Jul 24, 12:00

**背景**: 实时交互多模态模型能同时处理并生成多种数据类型（视频、音频、文本）且延迟低。Token 吞吐量（如每秒视频 token）衡量模型处理视觉信息的速度，数值越高交互越流畅。“本地优先”方法在设备上存储和处理数据，增强隐私性。

**标签**: `#AI`, `#multimodal`, `#real-time`, `#open source`, `#model`

---

<a id="item-14"></a>
## [黄仁勋：美国应允许使用中国开源 AI 模型](https://t.me/zaihuapd/42749) ⭐️ 7.0/10

英伟达 CEO 黄仁勋表示，中国开源 AI 模型非常优秀，美国企业绝对应该获准使用，反对以国家安全为由的限制。 这标志着一位重要的行业领袖反对日益增长的地缘政治壁垒，主张开放以推动创新和市场扩张。 黄仁勋提议使用安全沙箱来控制下载的中国模型，并指出开放代码有助于研究人员发现漏洞，反对全面禁令。

telegram · zaihuapd · Jul 24, 13:26

**背景**: 美国政府出于国家安全考虑，一直在考虑限制中国 AI 模型。黄仁勋认为全面禁令适得其反，而受控访问和开放研究是更好的方法。

**标签**: `#AI`, `#open-source`, `#geopolitics`, `#Nvidia`, `#policy`

---

<a id="item-15"></a>
## [马斯克支持库克称内存价格暴涨前所未见，美光 CCO 指责苹果压价](https://t.me/zaihuapd/42761) ⭐️ 7.0/10

埃隆·马斯克公开支持蒂姆·库克关于内存价格涨幅空前的评论，称这是他见过的最大涨幅，并呼吁大幅提升产量，同时联系到特斯拉的 Terafab 项目。美光首席商务官则暗示，苹果在 2023 年行业低迷期采取激进压价策略，导致内存厂商利润转负、投资停滞，从而加剧了供应紧张。 这一互动凸显了内存供应链中日益加剧的紧张关系——苹果的定价权可能反噬自身，也表明内存需求（尤其是 AI 和数据中心）正在超过供应。马斯克推动 Terafab 项目意味着芯片制造向垂直整合的重大转变。 马斯克提及特斯拉的 Terafab 项目，这是一个计划中的芯片工厂，将整合多条内存和逻辑制造上下游在同一园区，目标每年超过 1 太瓦的算力产出。美光首席商务官萨达纳表示，2023 年部分客户压价太狠导致美光亏损，延迟了必要的产能扩张。

telegram · zaihuapd · Jul 25, 04:02

**背景**: 内存价格具有周期性，存在供过于求和短缺的交替。2023 年内存行业遭遇严重低迷，美光等公司出现亏损。苹果以强力压价供应商著称，这可能加剧了行业投资不足的问题。马斯克的 Terafab 计划旨在为特斯拉的 AI 和机器人需求保障芯片供应，可能重塑制造格局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.chinaflashmarket.com/newsflash/37139">特 斯 拉 ： TERAFAB ...</a></li>
<li><a href="https://www.cls.cn/detail/2325743">海外研选 | 巴克莱详解 特 斯 拉 Terafab ...</a></li>

</ul>
</details>

**标签**: `#memory`, `#supply chain`, `#Apple`, `#Elon Musk`, `#pricing`

---

<a id="item-16"></a>
## [AMD 确认 Zen 7 EPYC 2028 年发布，Zen 8 2030 年登场](https://www.techspot.com/news/113233-amd-confirms-zen-7-epyc-florence-2028-previews.html) ⭐️ 7.0/10

AMD 已官方确认，基于 Zen 7 架构的第七代 EPYC 'Florence'处理器将于 2028 年推出，而基于 Zen 8 的第八代 EPYC 'Ravenna'将于 2030 年登场。 这一长期路线图表明 AMD 持续致力于服务器市场主导地位，承诺新的内存和 AI 功能，可能加剧与英特尔和英伟达在数据中心和 AI 基础设施领域的竞争。 Florence 将提供 Zen 7 和 Zen 7c 核心，支持新型 MRDIMM 和 LPDDR 内存，并采用 SP7 和 SP8 平台用于下一代'Ferrara' AI 机架系统；Zen 8 的制程和核心数量等规格尚未公布。

telegram · zaihuapd · Jul 25, 14:05

**背景**: MRDIMM（多路复用 Rank DIMM）是一种提升带宽超过标准 DDR5 的内存技术，对 AI 和高性能计算工作负载至关重要。AMD 的 SP7/SP8 平台专为高核心数处理器设计，而 Ferrara AI 机架系统（类似之前的 Helios）通过 GPU-CPU 集成针对 AI 工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lenovopress.lenovo.com/lp2028-introduction-to-mrdimm-memory-technology">Introduction to MRDIMM Memory Technology > Lenovo Press</a></li>
<li><a href="https://www.techpowerup.com/351030/msi-launches-6th-gen-amd-epyc-server-portfolio">MSI Launches 6th Gen AMD EPYC Server Portfolio | TechPowerUp</a></li>

</ul>
</details>

**标签**: `#AMD`, `#Zen 7`, `#Zen 8`, `#EPYC`, `#server processors`

---