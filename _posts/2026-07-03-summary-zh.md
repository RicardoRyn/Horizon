---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> From 39 items, 21 important content pieces were selected

---

1. [欧盟议会间谍软件委员会成员遭飞马间谍软件攻击](#item-1) ⭐️ 8.0/10
2. [PostgreSQL：为何严格内存超额提交优于 OOM 杀手](#item-2) ⭐️ 8.0/10
3. [Wordgard：ProseMirror 创建者推出的新富文本编辑器](#item-3) ⭐️ 8.0/10
4. [Valve 开源 Steam Machine 电子墨水屏，支持定制](#item-4) ⭐️ 8.0/10
5. [HAT-4D：单目视频直出 4D 交互场景](#item-5) ⭐️ 8.0/10
6. [Anthropic 指控阿里巴巴对 Claude AI 发动大规模“蒸馏攻击”](#item-6) ⭐️ 8.0/10
7. [华为 Mate 80 Pro 游戏能效超越骁龙 8 Gen3，得益于鸿蒙优化](#item-7) ⭐️ 8.0/10
8. [NASA 发射救援任务拯救老化雨燕望远镜](#item-8) ⭐️ 8.0/10
9. [腾讯阿图因 AI 超越 Mythos，登顶 CyberGym 基准测试](#item-9) ⭐️ 8.0/10
10. [jj v0.43.0：新命令“jj run”与重大变更](#item-10) ⭐️ 7.0/10
11. [本地运行顶尖大模型指南](#item-11) ⭐️ 7.0/10
12. [Costco：线下批发模式对抗 Amazon](#item-12) ⭐️ 7.0/10
13. [工厂不过是个房间](#item-13) ⭐️ 7.0/10
14. [将代码转为图像以利用图像令牌定价，在 Fable 上节省 60%成本](#item-14) ⭐️ 7.0/10
15. [半成品失败原因：创始人动机与领域专业度不匹配](#item-15) ⭐️ 7.0/10
16. [螺旋蝇的兴衰](#item-16) ⭐️ 7.0/10
17. [Google Gemini Omni Flash 登顶 Video Arena 盲测榜](#item-17) ⭐️ 7.0/10
18. [Claude Fable 5 重上线后体验缩水，安全误判惹不满](#item-18) ⭐️ 7.0/10
19. [华为 Atlas 350 搭载昇腾 950PR，算力达 H20 的 2.87 倍](#item-19) ⭐️ 7.0/10
20. [中国拟规定：半年不登录账号可注销，AI 生成内容需标识](#item-20) ⭐️ 7.0/10
21. [阿里巴巴禁止员工使用 Anthropic 的 Claude](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [欧盟议会间谍软件委员会成员遭飞马间谍软件攻击](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

一名参与调查间谍软件的欧洲议会委员会成员，其设备在 2022 年和 2023 年多次被飞马间谍软件成功感染，公民实验室的法医分析已确认此事。 该事件表明，即便是负责调查间谍软件的人员也无法逃脱其威胁，凸显了国家支持的网络间谍活动的普遍风险，以及加强网络安全保护的紧迫性。 公民实验室高度确信，该设备在 2022 年 10 月 21 日左右以及 2023 年 3 月 6 日和 7 日再次被感染。攻击者利用零点击漏洞在 iPhone 上安装了飞马间谍软件。

hackernews · ledoge · Jul 3, 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: 飞马是由以色列 NSO 集团开发的一款复杂的间谍软件，能够远程秘密监控移动设备。多国政府曾广泛使用它来监视记者、活动家和政治人物。公民实验室是领先的网络安全监督机构，专门调查数字间谍活动。欧洲议会曾设立特别委员会，调查成员国对间谍软件的使用情况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>

</ul>
</details>

**社区讨论**: 用户‘elorant’指出，希腊此前也发生过类似飞马窃听丑闻，并涉及总理办公室，认为这并非针对欧洲议会的攻击，而是国内操作。‘petcat’引用了公民实验室报告中的具体感染日期。‘shevy-java’则担忧游说者将欧盟数据出售给美国企业。

**标签**: `#cybersecurity`, `#spyware`, `#pegasus`, `#espionage`, `#european parliament`

---

<a id="item-2"></a>
## [PostgreSQL：为何严格内存超额提交优于 OOM 杀手](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud 发布了一篇技术博客，解释为何对 PostgreSQL 使用严格内存超额提交，以避免 OOM 杀手终止进程。 这很重要，因为 OOM 杀手可能导致 PostgreSQL 系统广泛中断；切换到严格超额提交可将灾难性故障转化为可管理的分配错误，提高数据库可靠性。 严格内存超额提交通过设置 vm.overcommit_memory=2 配置，该模式会拒绝超出承诺限制的分配，并结合超额比率；但需谨慎，设置过低可能阻止 fork() 调用。

hackernews · furkansahin · Jul 3, 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: 在 Linux 中，OOM 杀手（内存不足杀手）是内核机制，当系统内存严重不足时终止进程以释放内存。内存超额提交允许进程分配超过物理 RAM 的虚拟内存。默认的启发式超额提交模式可能不可预测地触发 OOM 杀手。严格超额提交（模式 2）拒绝超出用户指定限制的分配，将 OOM 杀手转化为优雅的分配失败。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory ...</a></li>
<li><a href="https://www.baeldung.com/linux/memory-overcommitment-oom-killer">Linux Memory Overcommitment and the OOM Killer - Baeldung</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/what-you-should-know-about-linux-memory-overcommit-in-postgresql/">Memory overcommit and PostgreSQL | CYBERTEC PostgreSQL</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出 Linux 默认设置有问题（baq），但切换到模式 2 需谨慎，因为它可能破坏 fork()（Bender）。来自 Ubicloud 的 Ozgune 承认文章语气过强，但坚持对托管 Postgres 的建议。leononame 分享了一个真实案例，设置模式 2 导致与 Go 应用不稳定。

**标签**: `#PostgreSQL`, `#Linux`, `#memory management`, `#database operations`, `#sysadmin`

---

<a id="item-3"></a>
## [Wordgard：ProseMirror 创建者推出的新富文本编辑器](https://wordgard.net/) ⭐️ 8.0/10

ProseMirror 和 CodeMirror 的创建者 Marijn Haverbeke 发布了 Wordgard 0.1，这是一个从头构建的浏览器内富文本编辑器库，采用了不同的设计理念，且没有从 ProseMirror 升级的路径。 作为 Web 开发社区中备受尊敬的人物的高价值发布，Wordgard 在富文本编辑方面引入了新的权衡，可能影响未来的项目和像 TipTap 这样的库。 Wordgard 与 ProseMirror 共享许多概念，但不兼容，迁移需要大量工作。其代码库包含来自 CodeMirror 和 ProseMirror 的修改副本。

hackernews · indy · Jul 3, 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48772573)

**背景**: 由于缺乏原生标准，浏览器中的富文本编辑器长期以来一直是一个挑战。Marijn Haverbeke 此前创建了 ProseMirror（一个用于构建协作编辑应用的热门框架）和 CodeMirror（一个代码编辑器组件）。Wordgard 是他的新尝试，采用了不同的架构，旨在提供更简单、更灵活的方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48772573">Wordgard: In-browser rich-text editor from the creator of ProseMirror</a></li>
<li><a href="https://daily.dev/posts/wordgard-release-0-1-obvbc6n30">Wordgard Release 0.1 | daily.dev</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区普遍对 Wordgard 的设计和实现印象深刻，许多人称赞其美学和技术深度。然而，关于缺乏从 ProseMirror 升级的路径以及重新开始的理由，存在大量讨论，一些用户指出了迁移现有项目的困难。

**标签**: `#rich-text-editor`, `#prosemirror`, `#javascript`, `#web-development`, `#open-source`

---

<a id="item-4"></a>
## [Valve 开源 Steam Machine 电子墨水屏，支持定制](https://www.gamingonlinux.com/2026/07/valve-open-source-the-steam-machine-e-ink-screen-so-you-can-make-your-own/) ⭐️ 8.0/10

Valve 已开源 Steam Machine 的电子墨水屏前面板，发布设计文件，允许爱好者使用标准组件创建自己的定制电子墨水屏。 此举鼓励硬件定制和改装，围绕 Steam Machine 培育开放生态系统，并展示了 Valve 对开源硬件的承诺。 该显示屏基于标准的 Adafruit 5.83 英寸电子墨水面板，Valve 提供了用于 3D 打印前面板的 STL 文件，方便社区复制和修改。

hackernews · ahlCVA · Jul 3, 13:01 · [社区讨论](https://news.ycombinator.com/item?id=48774518)

**背景**: 电子墨水技术利用电泳粒子以低功耗和高可读性呈现图像，类似纸张。Steam Machine 是 Valve 推出的一款游戏主机，其前面板模块化，可定制。通过开源电子墨水屏设计，Valve 使社区能够为主机创建自定义显示屏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gamingonlinux.com/2026/07/valve-open-source-the-steam-machine-e-ink-screen-so-you-can-make-your-own/">Valve open source the Steam Machine e-ink screen so you can make your own | GamingOnLinux</a></li>
<li><a href="https://www.reddit.com/r/gadgets/comments/1owzai6/valve_showcases_steam_machine_with_eink_display/">r/gadgets on Reddit: Valve showcases Steam Machine with e-ink display</a></li>
<li><a href="https://en.wikipedia.org/wiki/E_Ink">E Ink - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Valve 的开放态度表示热情，一位用户希望更多硬件公司能效仿。另一位指出显示屏是标准的 Adafruit 面板，易于复制。还有用户询问更大的支持 HDMI/USB-C 输入的电子墨水屏，显示出对进一步定制的兴趣。

**标签**: `#open-source hardware`, `#valve`, `#steam machine`, `#e-ink`, `#hardware hacking`

---

<a id="item-5"></a>
## [HAT-4D：单目视频直出 4D 交互场景](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247901356&idx=3&sn=54ee94026f76691a380cd3ea214e0def) ⭐️ 8.0/10

上海交通大学研究人员提出 HAT-4D 方法，能够从单目视频直接生成 4D 交互场景，无需昂贵的多相机动捕系统。 这一突破有望让 4D 内容创作普及化，使 VR/AR、游戏和电影制作无需昂贵设备，极大降低高质量动态场景重建的门槛。 该方法可能结合了神经渲染和动态场景表示的最新进展，从标准视频推断 3D 运动和几何结构。虽然完整技术报告尚未公开，但结果显示从简单的刀切香蕉视频中能合情推理出 4D 交互。

rss · 量子位 · Jul 3, 03:43

**背景**: 4D 重建在 3D 重建基础上增加时间维度，捕捉包含运动的动态场景。传统方法需要配备多台同步相机或深度传感器的动捕棚，成本高达百万级别。HAT-4D 旨在用单台普通摄像机达到类似效果，使该技术更易获取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/4D_reconstruction">4D reconstruction</a></li>
<li><a href="https://grokipedia.com/page/4d_reconstruction">4D reconstruction</a></li>

</ul>
</details>

**标签**: `#computer vision`, `#4D reconstruction`, `#monocular video`, `#AI research`, `#motion capture`

---

<a id="item-6"></a>
## [Anthropic 指控阿里巴巴对 Claude AI 发动大规模“蒸馏攻击”](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic 致信美国参议院银行委员会，指控阿里巴巴利用近 2.5 万个欺诈账户，在 2026 年 4 月 22 日至 6 月 5 日期间与 Claude 模型进行了超过 2880 万次交互，称这已是迄今已知最大规模的蒸馏攻击。 这一事件凸显了专有 AI 模型的重大安全漏洞，并引发国家安全担忧，因为蒸馏攻击使对手能够未经授权复制前沿 AI 能力，可能削弱美国 AI 公司的出口管制和竞争优势。 此次蒸馏攻击专门针对 Anthropic 的 Claude 模型，Anthropic 称参与方包括阿里巴巴及其 Qwen 实验室。蒸馏攻击是指利用较弱的模型通过学习更强模型的输出来复制其能力。

telegram · zaihuapd · Jul 3, 06:21

**背景**: 蒸馏是一种技术，通过训练较小的、成本较低的模型来学习更大、更强模型输出，从而以较低成本实现相似性能。传统上用于模型压缩，但也可被武器化，通过数百万次查询专有模型并使用响应来训练竞争模型，从而窃取知识产权。Anthropic 一直呼吁加强出口管制和安全措施以防止此类盗窃，他们认为这构成了国家安全风险，因为蒸馏后的模型可能缺乏安全防护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://www.iaps.ai/research/ai-distillation-attacks-the-case-for-targeted-government-intervention">AI Distillation Attacks: The Case for Targeted Government ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen_(Alibaba_Cloud)">Qwen (Alibaba Cloud)</a></li>

</ul>
</details>

**标签**: `#AI security`, `#model distillation`, `#Anthropic`, `#Alibaba`, `#intellectual property`

---

<a id="item-7"></a>
## [华为 Mate 80 Pro 游戏能效超越骁龙 8 Gen3，得益于鸿蒙优化](https://www.bilibili.com/video/BV1F7T46wEyT) ⭐️ 8.0/10

极客湾评测显示，搭载麒麟 9030 芯片的华为 Mate 80 Pro 系列在原生鸿蒙优化和软硬芯云协同下，游戏能效优于骁龙 8 Gen3。 这表明华为自研芯片在理论规格较低的情况下，实际性能仍能与顶级对手竞争，标志着移动行业向软件定义硬件效率的转变。 麒麟 9030 Pro 采用 9 核 14 线程 CPU 和 6 核马良 935 GPU，晶体管规模约 150 亿。在《原神》极高画质 60 帧下，Mate 80 Pro Max 整机功耗仅 4.9W，能效优于骁龙 8 Gen3。

telegram · zaihuapd · Jul 3, 13:27

**背景**: 华为的麒麟芯片因美国制裁限制先进工艺，在理论基准测试中一直落后。但华为通过鸿蒙操作系统和“软硬芯云”协同，专注于深度软硬件整合，在不依赖尖端制程的情况下优化实际性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2p3M2R2OUR4SGhqamlTWGZQbEdTZ0FQAQ?hl=en-SG&gl=SG&ceid=SG:en">Huawei Mate 80 series features new Kirin 9030 chipsets - Overview</a></li>
<li><a href="https://nanoreview.net/en/soc/hisilicon-kirin-9030">HiSilicon Kirin 9030 Pro: specs and benchmarks</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1974893623637190453">软硬协同再攀高峰：阿里云服务器研发团队三篇论文入选国际顶会 HPCA20...</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#Kirin 9030`, `#HarmonyOS`, `#mobile gaming`, `#chipset`

---

<a id="item-8"></a>
## [NASA 发射救援任务拯救老化雨燕望远镜](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

美国宇航局于 2026 年 7 月 3 日发射了 LINK 航天器，将与老化的雨燕天文台会合，并将其轨道提升约 240 公里，以防止其坠入大气层。 此次任务是私人航天器首次尝试捕获并提升美国在役政府卫星的轨道，展示了减缓轨道碎片和延长卫星寿命的关键能力。 LINK 将使用机械臂抓取雨燕，然后在几个月内缓慢提升其轨道；如果任务成功，雨燕最早可能在 9 月恢复观测。

telegram · zaihuapd · Jul 3, 15:43

**背景**: 雨燕望远镜于 2004 年发射，是一台伽马射线暴天文台，已运行超过 20 年。由于太阳活动增加，其轨道衰减速度快于预期，面临再入大气层被摧毁的风险。在轨卫星服务是一个新兴领域，航天器可以为卫星加油、维修或提升轨道，从而减少空间碎片并延长任务寿命。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.space.com/space-exploration/launches-spacecraft/nasa-successfully-launches-rescue-mission-to-save-swift-space-telescope-from-burning-up-in-earths-atmosphere">NASA launches rescue mission to save Swift space telescope... | Space</a></li>
<li><a href="https://www.nasa.gov/image-article/link-spacecraft-set-for-mission-to-boost-nasas-swift-observatory/">LINK Spacecraft Set for Mission to Boost NASA’s Swift... - NASA</a></li>
<li><a href="https://www.nytimes.com/2026/07/03/science/nasa-swift-telescope-rescue-mission.html">A Mission to Save NASA’s Swift Telescope Launches to Orbit</a></li>

</ul>
</details>

**标签**: `#space`, `#NASA`, `#satellite rescue`, `#orbital debris`, `#Swift telescope`

---

<a id="item-9"></a>
## [腾讯阿图因 AI 超越 Mythos，登顶 CyberGym 基准测试](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

腾讯玄武实验室的阿图因 AI 在 CyberGym 基准测试中获得 84.0%的得分，超越 Anthropic 的 Claude Mythos Preview，且消耗预算不到 Mythos 的 0.1%。 这表明开源、低成本 AI 模型能在真实漏洞检测中超越专有系统，可能推动网络安全工具的普及。 阿图因基于可本地部署的开源模型 GLM-5.1 构建，在 curl、gnark、OpenSSL 等关键开源库中发现了多个 Mythos 未检出的高危逻辑漏洞（最高 9.3 分）。

telegram · zaihuapd · Jul 3, 16:12

**背景**: CyberGym 是加州大学伯克利分校推出的大规模基准测试，用于评估 AI 代理在真实漏洞分析上的能力，包含 188 个开源项目的 1507 个漏洞。GLM-5.1 是 Z.AI 推出的开源旗舰模型，专为长时间自主任务设计。gnark 是一个快速的 zk-SNARK 库，用于隐私保护计算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/sunblaze-ucb/cybergym">GitHub - sunblaze-ucb/cybergym: CyberGym is a large-scale, high-quality cybersecurity evaluation framework designed to rigorously assess the capabilities of AI agents on real-world vulnerability analysis tasks. · GitHub</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.1">zai-org/GLM-5.1 · Hugging Face</a></li>
<li><a href="https://github.com/ConsenSys/gnark">GitHub - Consensys/gnark: gnark is a fast zk-SNARK library ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#vulnerability detection`, `#benchmark`, `#Tencent`

---

<a id="item-10"></a>
## [jj v0.43.0：新命令“jj run”与重大变更](https://github.com/jj-vcs/jj/releases/tag/v0.43.0) ⭐️ 7.0/10

Jujutsu (jj) 版本 0.43.0 引入了“jj run”命令，该命令在具有私有工作副本的一组更改上执行命令，并自动处理冲突传播。同时移除了 git_head() 和 git_refs() 等废弃函数，并更改了类似 Git 的符号解析方式。 “jj run”命令增强了开发者的工作流自动化能力，允许在多个修订版本上批量执行 lint 或测试等操作。重大变更通过移除废弃功能精简了工具，但用户需要更新脚本和配置。 “jj run”命令为每个更改创建私有工作副本，执行命令，并传播产生的更改或冲突。重大变更包括移除类似 Git 的符号（如 refs/heads/main）和废弃的 ui.revsets-use-glob-by-default 选项。

github · yuja · Jul 2, 01:41

**背景**: Jujutsu (jj) 是一个用 Rust 编写的 Git 兼容版本控制系统，设计简洁且强大。它使用 Git 的磁盘格式，允许用户无缝切换。Revsets 是一种函数式查询语言，用于选择一组修订版本，灵感来自于 Mercurial。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.jj-vcs.dev/latest/">Jujutsu—a version control system - docs.jj-vcs.dev</a></li>
<li><a href="https://github.com/jj-vcs/jj/blob/main/docs/revsets.md">jj/docs/revsets.md at main · jj-vcs/jj · GitHub</a></li>

</ul>
</details>

**标签**: `#version control`, `#jj`, `#git`, `#release`, `#tools`

---

<a id="item-11"></a>
## [本地运行顶尖大模型指南](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob 发布了一份全面指南，介绍如何本地运行最先进的大语言模型，涵盖从几千到数万美元的硬件预算，附有实用建议和成本分析。 该指南帮助爱好者和研究人员评估本地运行大语言模型时成本、性能和便利性之间的权衡；随着专有 API 成本上升，这是一个日益重要的领域。 该指南涵盖从低成本方案（例如两块 RTX 3090 获得 48GB VRAM）到超过 4 万美元集群的预算，并讨论了量化、统一内存（例如 Apple Mac Studio）和云替代方案。

hackernews · livestyle · Jul 3, 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 在本地运行大语言模型需要大量显存和算力。量化通过降低数值精度来减小模型尺寸，使其能在消费级硬件上运行。GGUF 等格式简化了模型加载和推理过程。该指南针对这些因素帮助读者选择合适的硬件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://localllm.in/blog/quantization-explained">The Complete Guide to LLM Quantization - localllm.in</a></li>
<li><a href="https://en.wikipedia.org/wiki/GGUF">GGUF - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区成员指出硬件成本可能远超初始估算，而统一内存方案（如大内存 Mac）提供了有吸引力的中间选项。有人认为按需使用云服务更划算，另一些人则看重本地推理的隐私和可靠性。

**标签**: `#local LLMs`, `#hardware`, `#GPU`, `#machine learning`, `#budget`

---

<a id="item-12"></a>
## [Costco：线下批发模式对抗 Amazon](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

一篇分析文章认为，Costco 的线下批发购买模式避免了 Amazon 最后一英里送货上门带来的物流复杂性和成本，凸显了一种深思熟虑的战略选择。 这种对比揭示了零售物流中的重要权衡，表明避免最后一英里的复杂性可能是一种明智的工程和商业决策，尤其是在电商巨头面临送货成本上升的情况下。 文章强调，单个商品送货上门与批量托盘运送到仓库由顾客自行开车带回家，其成本结构完全不同。这种对最后一英里物流的战略性规避被比作工程谚语中解决问题与避免问题的区别。

hackernews · bookofjoe · Jul 3, 15:14 · [社区讨论](https://news.ycombinator.com/item?id=48776044)

**背景**: 最后一英里物流是指将货物从配送中心运送到最终客户家门口的最后一步。由于交通、配送失败和单独处理等因素，它通常是供应链中最复杂、成本最高的部分。Costco 的模式将最后一英里的负担转移给顾客，由他们自行开车到店并运送大宗商品，从而降低了零售商的成本和复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://onfleet.com/blog/first-mile-middle-mile-last-mile/">What is First Mile, Middle Mile, and Last Mile Delivery?</a></li>
<li><a href="https://digital-commerce.post.ch/en/pages/blog/2022/the-last-mile-a-focus-on-delivery-models">The last mile – a focus on delivery models | Digital-Commerce – Die...</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了其中的权衡，有人指出 Amazon 也试图集中购买以减少 SKU 数量，而另一些人则赞扬 Costco 避免最后一英里问题的智慧。一位英国观点指出 Costco 的会员制最初面向企业，增添了细微差别。

**标签**: `#retail`, `#logistics`, `#business models`, `#Amazon`, `#Costco`

---

<a id="item-13"></a>
## [工厂不过是个房间](https://interconnected.org/home/2026/07/03/factories) ⭐️ 7.0/10

文章提出，工厂本质上不过是一个房间，通过剥去不必要的复杂性来解神秘化制造业。 这种观点可能使制造业民主化，鼓励更多人将生产视为可达的而非令人生畏的。 这篇文章是哲学性的而非技术性的，通过“房间”这一简单视角来挑战关于工业工作的固有假设。

hackernews · arbesman · Jul 3, 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48776035)

**背景**: 工厂常被想象为拥有昂贵机械的庞大复杂设施。文章将其简化为最本质的形式：一个人们制造物品的房间。这种重新框定凸显了制造业的核心活动本身并不神秘。

**社区讨论**: 评论者分享了个人经历：有人提到经营小型工厂的乐趣，有人将快餐厨房比作高效工厂。大家一致认为制造业比通常认为的更容易进入，但也承认存在劳动保护等结构性障碍。

**标签**: `#manufacturing`, `#philosophy`, `#technology`, `#work`

---

<a id="item-14"></a>
## [将代码转为图像以利用图像令牌定价，在 Fable 上节省 60%成本](https://github.com/teamchong/pxpipe) ⭐️ 7.0/10

一位开发者发布了名为 pxpipe 的工具，将代码转换为图像，并通过 OCR 让 LLM 处理，利用更便宜的图像令牌定价，在 Claude Fable 上节省约 60%的成本。 这一技巧暴露了 LLM 令牌计费中的重大定价漏洞，可能影响开发者优化成本的方式，但可能是暂时的，因为服务商可能会通过收取 OCR 处理费用来堵住这个漏洞。 该工具在发送给模型（如 Claude）之前将代码转换为图像，依赖模型内置的 OCR 读取代码；节省来自图像令牌通常比文本令牌每单位信息更便宜，但这种方法可能增加延迟和资源消耗。

hackernews · dimitropoulos · Jul 3, 15:50 · [社区讨论](https://news.ycombinator.com/item?id=48776464)

**背景**: 像 Anthropic、OpenAI 和 Google 这样的 LLM 提供商按令牌收费，并对文本和图像输入分别定价。图像令牌通常根据图像分辨率计算，且相比于等效代码内容的文本令牌，每单位视觉信息的成本往往更低。开发者一直在寻求降低提示成本的方法，而这个技巧利用了文本和图像之间令牌定价的差异。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://stellaxon.com/ai/image-token-calculator">AI Image Token Calculator - Vision API Costs</a></li>

</ul>
</details>

**社区讨论**: 社区评论观点不一：有人认为这是一个聪明但可能暂时的漏洞，如果服务商调整定价可能会被关闭；其他人则担心资源浪费和延迟增加。一位用户去年尝试了类似方法，发现由于完成令牌增加，总体成本更高。

**标签**: `#LLM`, `#cost optimization`, `#OCR`, `#pricing hack`, `#token accounting`

---

<a id="item-15"></a>
## [半成品失败原因：创始人动机与领域专业度不匹配](https://weli.dev/blog/half-baked-product/) ⭐️ 7.0/10

一篇博客文章分析了为什么许多创业产品停留在‘半成品’状态，将失败归因于创始人优先考虑财富而非领域专业知识，这一点得到了社区广泛认同。 这一反思突显了创业失败的常见模式，提醒创业者真正的领域专业知识和客户理解对产品成功至关重要，而不仅仅是融资能力。 文章以缺乏烤箱专业知识却要造烤箱为类比，社区评论进一步探讨了创始人、工程师和销售人员之间的脱节。

hackernews · weli · Jul 3, 08:23 · [社区讨论](https://news.ycombinator.com/item?id=48772388)

**背景**: 文章基于常见的创业失败场景：缺乏领域知识的创始人试图颠覆他们不了解的行业，这往往导致产品无法满足真实客户需求。

**社区讨论**: 评论者基本同意这一分析，指出创始人动机与执行不匹配。一些人强调了初创公司不同角色之间的脱节，并调侃性地对比了他们在其他行业的努力。

**标签**: `#startup`, `#product development`, `#failure`, `#founder`, `#domain expertise`

---

<a id="item-16"></a>
## [螺旋蝇的兴衰](https://www.construction-physics.com/p/the-fall-and-rise-of-screwworm) ⭐️ 7.0/10

一篇来自 Construction Physics 的文章梳理了利用昆虫不育技术（SIT）根除螺旋蝇的历史、其在北美和中美洲的成功，以及 2025-2026 年在南德克萨斯等地重新出现的现象。 螺旋蝇的重新出现威胁着价值数十亿美元的畜牧业，并对昆虫不育技术作为遏制策略的长期可行性提出质疑，尤其关注可能出现的辐射抗性。 文章指出，美国于 2026 年 6 月在德克萨斯州南部确认了首例螺旋蝇病例，表明达连隘口的遏制屏障已被突破。社区成员讨论维持屏障是否比与南美合作彻底根除成本更高。

hackernews · crescit_eundo · Jul 3, 12:58 · [社区讨论](https://news.ycombinator.com/item?id=48774492)

**背景**: 新世界螺旋蝇（Cochliomyia hominivorax）是一种致命的牲畜害虫，其幼虫以活体组织为食导致蝇蛆病。昆虫不育技术（SIT）于 1950 年代开发，通过辐射大量饲养的雄蝇使其不育；释放后，它们与野生雄蝇竞争交配，导致种群崩溃。SIT 在 1990 年代前成功根除了北美和中美洲的螺旋蝇，但需要在达连隘口建立永久屏障以防止南美洲的再次入侵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Screwworm">Screwworm</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sterile_insect_technique">Sterile insect technique</a></li>
<li><a href="https://www.cdc.gov/new-world-screwworm/about/index.html">About New World Screwworm | New World Screwworm | CDC</a></li>

</ul>
</details>

**社区讨论**: 社区成员分享了 2026 年美国病例的额外资源，并讨论了维持屏障与大陆根除的经济性。一位评论者称赞该文章为“精彩阅读”。另一人提出了技术性担忧：重复释放是否可能选择出抗辐射的雄蝇，从而破坏 SIT 的有效性。

**标签**: `#screwworm`, `#pest control`, `#agriculture`, `#biology`, `#public health`

---

<a id="item-17"></a>
## [Google Gemini Omni Flash 登顶 Video Arena 盲测榜](https://x.com/Designarena/status/2072759122366509130) ⭐️ 7.0/10

Google DeepMind 的视频生成模型 Gemini Omni Flash 在 Video Arena 盲测中以 1404 分夺得第一，领先字节跳动的 Seedance 2.0 Mini 达 101 分。 这一结果标志着 AI 视频生成领域的重大变化，Google 从字节跳动手中夺回领先地位，加剧了竞争，并可能加速该领域的创新。 Video Arena 根据用户盲测投票对模型进行排名；Gemini Omni Flash 是一款原生多模态视频模型，能够生成高分辨率视频，并具备同步音频和物理感知场景的能力。

telegram · zaihuapd · Jul 3, 05:51

**背景**: Video Arena 是一个由社区驱动的基准测试平台，根据真实用户偏好评估 AI 视频生成模型。此前，字节跳动的 Seedance 系列，特别是 Seedance 2.0 Mini，长期占据榜首。Google 之前的 Veo 系列排名靠后，但新的 Gemini Omni Flash 代表了重大进步，展示了 AI 驱动视频创作的快速发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bracai.eu/post/video-arena">Best AI video models in 2026 (ranked by real users) - Bracai</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://artificialanalysis.ai/video/arena">Video Arena - Top AI Video Models</a></li>

</ul>
</details>

**标签**: `#AI`, `#video generation`, `#Google DeepMind`, `#benchmark`

---

<a id="item-18"></a>
## [Claude Fable 5 重上线后体验缩水，安全误判惹不满](https://www.bleepingcomputer.com/news/artificial-intelligence/claude-fable-relaunch-disappoints-users-with-nerfed-performance/) ⭐️ 7.0/10

Anthropic 的旗舰模型 Claude Fable 5 在美国解除出口管制后重新上线，但用户报告称订阅用户每周仅能使用 50%的额度，且安全过滤器过于敏感，在处理底层代码或安全相关关键词时会错误地降级到 Opus 4.8。 这影响了依赖 Claude 进行代码分析和安全工作的开发者，过度敏感的安全过滤器会干扰正常开发流程。同时也表明 Anthropic 在安全与可用性之间的谨慎平衡，可能影响专业用户的信任和采用。 模型核心性能确认未变，只是安全防护过于激进。配额受限系统是临时的，截至 7 月 7 日，之后订阅用户需按量付费。API 和按量付费企业客户仍可完全访问。

telegram · zaihuapd · Jul 3, 07:20

**背景**: Claude Fable 5 是 Anthropic 公开可用的最强模型，基于 Mythos 架构。最初因其发现软件漏洞的能力而被限制发布。在美国解除出口管制后，Anthropic 增加了额外安全措施后重新发布。Opus 4.8 是 Anthropic 之前的旗舰模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 开发者情绪普遍负面，许多人抱怨配额减少和安全过滤误报。一些人认为安全措施过于保守，阻碍了实际使用，而另一些人指出配额限制是暂时的。官方尚未宣布修复方案。

**标签**: `#AI`, `#Claude`, `#AI Safety`, `#Export Controls`, `#API`

---

<a id="item-19"></a>
## [华为 Atlas 350 搭载昇腾 950PR，算力达 H20 的 2.87 倍](https://t.me/zaihuapd/42329) ⭐️ 7.0/10

华为发布了搭载昇腾 950PR 处理器的 Atlas 350 加速卡，声称其算力达到英伟达 H20 的 2.87 倍，支持 FP4 精度和 112 GB HBM 内存。 这一发布加剧了 AI 硬件领域的竞争，尤其是在美国制裁背景下，它提供了性能更高的国产替代方案，可能影响中国及全球的 AI 训练与推理市场。 Atlas 350 支持 FP4 低精度推理，单卡可加载 70B 参数模型，降低延迟与成本。相比前代，在向量算力、互联带宽及自研 HBM 等方面都有显著提升。

telegram · zaihuapd · Jul 3, 08:35

**背景**: 华为的昇腾系列是在美国出口限制下开发的 AI 加速器产品线。新型 Atlas 350 采用昇腾 950PR 芯片，据称 FP4 性能可达 1.56 petaflops。FP4 是一种新兴的低精度格式，通过降低内存和计算需求来加速大语言模型推理，但需要仔细校准。英伟达 H20 是出于美国出口管制而削减性能的中国合规 AI 芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech-insider.org/huawei-ascend-950pr-ai-chip-nvidia-china-2026/">Huawei Ascend 950PR: The 1.56 PFLOP AI Chip vs Nvidia [2026]</a></li>
<li><a href="https://www.huaweicentral.com/ascend-950pr-ai-chip-everything-you-need-to-know/">Ascend 950PR AI Chip: Everything you need to know</a></li>
<li><a href="https://nerdleveltech.com/huawei-ascend-950pr-atlas-350-ai-chip-challenges-nvidia">Huawei Ascend 950PR Beats NVIDIA H20: 2.8× FP8, CUDA-Ready</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#Huawei`, `#Ascend`, `#accelerator`, `#deep learning`

---

<a id="item-20"></a>
## [中国拟规定：半年不登录账号可注销，AI 生成内容需标识](https://mp.weixin.qq.com/s/TfYZaC8ULPvu9JeTqYGkKg) ⭐️ 7.0/10

2025 年 7 月 3 日，国家互联网信息办公室发布《互联网信息服务管理办法（修订草案征求意见稿）》再次公开征求意见，提出平台可注销超过 6 个月未登录的账号，要求对 AI 生成内容进行标识，并强制提供关闭个性化推荐的选项。 该规定将深刻影响中国数亿网民及所有在华运营的数字平台，可能重塑账号管理、AI 内容透明度和用户对个性化推荐的控制权。同时，它为其他国家管理闲置账号和 AI 生成内容提供了参考先例。 草案禁止平台强制用户使用智能信息服务，并明确禁止刷量、控评、操纵热搜、制造虚假热点等行为。大型互联网平台须在 24 小时内处理违法和不良信息相关的投诉、举报和申诉。

telegram · zaihuapd · Jul 3, 11:29

**背景**: 近年来，中国持续加强互联网监管，重点关注数据隐私、算法透明度和人工智能治理。上一版《互联网信息服务管理办法》于 2011 年发布，此次修订反映了 AI 和平台经济带来的新挑战。2023 年，中国实施了专门的 AI 生成内容标识规则，要求对 AI 生成内容添加可见和机器可读的标记。新草案还针对通过虚假账号和组织化不实行为操纵公众舆论的“网络水军”问题作出规定。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://english.scio.gov.cn/pressroom/2025-03/17/content_117769570.html">China requires labeling of AI-generated online content</a></li>
<li><a href="https://aiwiki.ai/wiki/china_ai_labeling_rules">China AI-generated content labeling rules - AI Wiki</a></li>
<li><a href="https://bricscompetition.org/news/china-cyberspace-authorities-purge-internet-of-troll-farms">China Cyberspace Authorities Purge Internet of 'Troll Farms'</a></li>

</ul>
</details>

**标签**: `#internet regulation`, `#China`, `#privacy`, `#AI content`, `#account management`

---

<a id="item-21"></a>
## [阿里巴巴禁止员工使用 Anthropic 的 Claude](https://t.me/zaihuapd/42334) ⭐️ 7.0/10

阿里巴巴下令全体员工卸载并停止使用 Anthropic 的 Claude 产品，包括 Sonnet、Opus、Fable 等模型以及 Claude Code，禁令于 7 月 10 日生效。此前，Anthropic 指控阿里使用虚假账号滥用其 API。 这项内部禁令突显了主要 AI 公司在 API 使用政策和数据访问方面日益紧张的关系。它可能影响阿里巴巴的开发效率，并为大型科技公司如何管理外部 AI 工具的使用树立先例。 阿里巴巴此前曾报销员工使用 Claude、GPT、Gemini 等外部模型的费用。Anthropic 指控阿里在 4 月 22 日至 6 月 5 日间使用约 2.5 万个虚假账号与 Claude 交互超过 2800 万次，随后收紧了风控策略。

telegram · zaihuapd · Jul 3, 13:00

**背景**: 大型语言模型（如 Claude）通常通过 API 访问，按使用量计费。公司常允许员工使用外部 AI 工具进行工作，但滥用（如创建大量账号）可能违反服务条款。Anthropic 是领先的 AI 初创公司，而阿里巴巴是中国科技行业的主要参与者，获取西方 AI 模型正变得越来越受限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/overview">Models overview - Claude Platform Docs</a></li>

</ul>
</details>

**标签**: `#AI`, `#Alibaba`, `#Claude`, `#corporate policy`, `#API abuse`

---