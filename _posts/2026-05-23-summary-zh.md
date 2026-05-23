---
layout: default
title: "Horizon Summary: 2026-05-23 (ZH)"
date: 2026-05-23
lang: zh
---

> From 40 items, 22 important content pieces were selected

---

1. [80386 微码被逆向分析](#item-1) ⭐️ 9.0/10
2. [SpaceX 星舰 v3 试飞：喜忧参半](#item-2) ⭐️ 9.0/10
3. [Anthropic 的 Project Glasswing 发现超过一万个高危漏洞](#item-3) ⭐️ 9.0/10
4. [苹果开源 corecrypto，附形式化验证证明后量子算法](#item-4) ⭐️ 9.0/10
5. [特朗普政府：绿卡申请人必须离境申请](#item-5) ⭐️ 8.0/10
6. [z386：基于原始微码的开源 FPGA 80386 实现](#item-6) ⭐️ 8.0/10
7. [深度学习优化：从基本原理到硬件利用](#item-7) ⭐️ 8.0/10
8. [微软内部取消 Claude Code 许可](#item-8) ⭐️ 8.0/10
9. [腾讯收购喜马拉雅获批，须放弃独家版权](#item-9) ⭐️ 8.0/10
10. [中国八部门整治非法跨境证券期货基金经营](#item-10) ⭐️ 8.0/10
11. [Cloudflare 全球故障 25 分钟，影响 28% HTTP 流量](#item-11) ⭐️ 8.0/10
12. [微软内部推广 Claude Code，鼓励非技术人员使用](#item-12) ⭐️ 8.0/10
13. [微软财报披露 OpenAI 单季巨亏 115 亿美元](#item-13) ⭐️ 8.0/10
14. [中国对富途控股和老虎证券跨境违规行为处以罚款](#item-14) ⭐️ 8.0/10
15. [美商海盗船采用长鑫存储 DDR5 芯片，价格有望下调](#item-15) ⭐️ 8.0/10
16. [深入探讨 HTML <dl>元素的语义和历史](#item-16) ⭐️ 7.0/10
17. [向乌干达难民营寄送笔记本电脑：腐败与物流的艰辛历程](#item-17) ⭐️ 7.0/10
18. [Rubish：用纯 Ruby 编写的 Unix Shell](#item-18) ⭐️ 7.0/10
19. [Oura 收到政府索取用户健康数据的要求](#item-19) ⭐️ 7.0/10
20. [Electrobun 2.0 因 Rust 重写而与 Bun 解耦](#item-20) ⭐️ 7.0/10
21. [Antigravity 将 Gemini 速率限制提升三倍并重置周配额](#item-21) ⭐️ 7.0/10
22. [我国日均词元调用量两年增超千倍，突破 140 万亿](#item-22) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [80386 微码被逆向分析](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 9.0/10

博客 reenigne.org 发布了 Intel 80386 微码的详细反汇编和分析，涵盖了所有微码 ROM，并揭示了处理器内部的控制逻辑。 这项逆向工程工作提供了对经典 x86 处理器内部工作原理的前所未有的洞察，帮助爱好者和研究人员理解如何通过微码实现复杂指令。 反汇编包括微操作解码、流水线控制和异常处理，并且需要艰苦的黑盒分析才能从观察到的行为中重建微码。

hackernews · nand2mario · May 23, 12:11 · [社区讨论](https://news.ycombinator.com/item?id=48247004)

**背景**: 微码是一层低级控制逻辑，将机器指令翻译成硬件控制信号。1985 年发布的 Intel 80386 是英特尔首款 32 位 x86 处理器，其复杂指令集（CISC）主要通过微码而非硬连线逻辑实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microcode">Microcode - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intel_8086">Intel 8086 - Wikipedia</a></li>
<li><a href="https://nand2mario.github.io/posts/2026/z386/">z386: An Open-Source 80386 Built Around Original Microcode - Small Things Retro</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞这是一项令人难以置信的逆向工程成果，有人询问如何从芯片图像中重建微码，还有人推荐了一本关于微编程的书籍。

**标签**: `#reverse engineering`, `#microcode`, `#computer architecture`, `#Intel 80386`, `#retrocomputing`

---

<a id="item-2"></a>
## [SpaceX 星舰 v3 试飞：喜忧参半](https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-v3-megarocket-first-test-flight) ⭐️ 9.0/10

SpaceX 发射了星舰 v3 火箭的首次试飞，尽管在上升和返回过程中多次出现助推器发动机故障，但上级级成功着陆。 这次飞行是验证升级版星舰 v3 的关键一步，其经验将为未来完全可重复使用的超重型发射（用于月球和火星任务）提供参考。 测试中，助推器在上升过程中关闭了一台发动机，并未能重新点火进行返回助推，导致偏离目标的硬着陆；而星舰上级级虽损失一台发动机，但实现了精确的海上着陆，且隔热罩未出现可见热点。

hackernews · busymom0 · May 22, 23:41 · [社区讨论](https://news.ycombinator.com/item?id=48242959)

**背景**: 星舰是 SpaceX 设计的完全可重复使用两级超重型运载火箭，旨在将人员和货物运送到地球轨道、月球和火星。v3 型号升级了 Raptor 3 发动机，增加了推进剂容量，并且堆叠高度达到 124 米。本次测试是 v3 构型的首次飞行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starship">SpaceX Starship - Wikipedia</a></li>
<li><a href="https://arstechnica.com/space/2026/05/spacex-completes-fueling-test-setting-stage-for-first-launch-of-starship-v3/">Once again, SpaceX has set a new record for the tallest rocket ever built - Ars Technica</a></li>
<li><a href="https://www.spaceconnectonline.com.au/launch/6561-raptor-engine-failure-caused-starship-explosion">Raptor engine failure caused Starship explosion - Space Connect</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞隔热罩的改进和制导系统在发动机故障下仍实现了精确着陆，同时对助推器未能返回表示失望。一些人指出 SpaceX 的快速迭代方法是一个优势，一位观察者提到模拟有效载荷卫星在再入过程中燃烧殆尽。

**标签**: `#SpaceX`, `#Starship`, `#rocket launch`, `#aerospace`

---

<a id="item-3"></a>
## [Anthropic 的 Project Glasswing 发现超过一万个高危漏洞](https://www.anthropic.com/research/glasswing-initial-update) ⭐️ 9.0/10

Anthropic 宣布，其 Project Glasswing 利用 Claude Mythos Preview 模型，在一个月内从关键软件中发现了超过一万个高危或严重漏洞，合作伙伴如 Cloudflare 报告漏洞发现速率提高了十倍以上。 这展示了 AI 驱动漏洞发现的重大突破，将瓶颈从发现转移到了验证和修补，对软件安全和行业实践具有深远影响。 该项目扫描了数千个开源项目，识别出 6202 个高危漏洞，其中经过审查的 1752 个中 90.6% 为真阳性。然而，由于修补需求过大，开源维护者已请求放缓报告速度。

telegram · zaihuapd · May 23, 03:16

**背景**: Project Glasswing 是 Anthropic 的一项倡议，旨在利用 AI 保护关键软件，与负责基础设施的组织合作。Claude Mythos Preview 是 Anthropic 最强大的前沿模型，专为网络安全和自主编码设计。该项目凸显了 AI 在网络安全中日益重要的作用，同时也揭示了漏洞管理方面的新挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era</a></li>
<li><a href="https://www.anthropic.com/project/glasswing">Project Glasswing</a></li>
<li><a href="https://www-cdn.anthropic.com/8b8380204f74670be75e81c820ca8dda846ab289.pdf">Claude Mythos Preview System Card - www-cdn.anthropic.com</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#vulnerability discovery`, `#Anthropic`, `#open source`

---

<a id="item-4"></a>
## [苹果开源 corecrypto，附形式化验证证明后量子算法](https://security.apple.com/blog/formal-verification-corecrypto/) ⭐️ 9.0/10

5 月 22 日，苹果开源了 corecrypto 密码库，其中包含对后量子算法 ML-KEM 和 ML-DSA 的形式化验证证明，并公开了定制验证工具和 Isabelle 理论库。 这是一项对密码学和软件保障的重大贡献，因为 corecrypto 部署在超过 25 亿台设备上，形式化证明确保了与 NIST 标准的一致性，加速了后量子安全的应用。 形式化验证覆盖了 ML-KEM 和 ML-DSA 的 C 代码和手工优化的 ARM64 汇编实现。苹果还发布了定制验证工具和 Isabelle 理论库，供独立专家评估这些证明。

telegram · zaihuapd · May 23, 04:49

**背景**: ML-KEM (FIPS 203)和 ML-DSA (FIPS 204)是 NIST 于 2024 年标准化的基于格的后量子密码算法，旨在抵御未来量子计算机的攻击。形式化验证利用数学证明来确保软件实现与标准完全一致，提供了对漏洞和错误的高度保障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/guide/certifications/about-apple-security-certifications-apc30d0ed034/web">About Apple security certifications - Apple Support</a></li>
<li><a href="https://en.wikipedia.org/wiki/ML-KEM">ML-KEM</a></li>
<li><a href="https://en.wikipedia.org/wiki/ML-DSA">ML-DSA</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#formal verification`, `#quantum-safe`, `#Apple`, `#open source`

---

<a id="item-5"></a>
## [特朗普政府：绿卡申请人必须离境申请](https://www.nytimes.com/2026/05/22/us/politics/green-card-changes-trump.html) ⭐️ 8.0/10

2026 年 5 月 22 日，特朗普政府宣布一项政策变更，要求大多数绿卡申请人离开美国，通过领事处理程序申请，实际上终止了大部分申请人的身份调整流程。 该政策彻底改变了合法移民的格局，尤其影响持有 H-1B 等签证的技术工人，他们通常无需离境即可调整身份。这可能导致长期的家庭分离、工作中断，并对移民和美国雇主造成经济损失。 该政策适用于所有身份调整申请人，除非能向 USCIS 证明存在“特殊情形”。同时，该政策取消了所有待决的身份调整申请，迫使申请人从其母国重新启动绿卡申请流程。

hackernews · tlhunter · May 22, 21:27 · [社区讨论](https://news.ycombinator.com/item?id=48241890)

**背景**: 身份调整（AOS）是一种允许已经在美国的外国人在不离开美国的情况下成为永久居民的程序。领事处理则要求申请人前往国外的美国大使馆或领事馆完成申请。此前，大多数合法身份的绿卡申请人可以选择 AOS；这项规定几乎取消了所有人的这一选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Green_card">Green card - Wikipedia</a></li>
<li><a href="https://jarrettfirm.com/immigration-and-naturalization-lawyers/family-based-adjustment-of-status/">Guide to Adjustment of Status Laws | Jarrett & Price LLC</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍谴责该政策“疯狂”且“邪恶”，强调其给家庭和技术工人带来的巨大困难。许多评论者认为，该政策削弱了“支持合法移民”的宣称，将造成不必要的痛苦，尤其是对于已有待决申请而不得不离境的人。

**标签**: `#immigration`, `#policy`, `#tech workers`, `#US-visa`, `#politics`

---

<a id="item-6"></a>
## [z386：基于原始微码的开源 FPGA 80386 实现](https://nand2mario.github.io/posts/2026/z386/) ⭐️ 8.0/10

开发者发布了 z386，这是一个基于 FPGA 的开源 Intel 80386 实现，使用了从真实芯片提取的原始微码，成功启动了 Linux 并运行了 Doom。 该项目证明了可以在現代 FPGA 上使用原始微码忠实地复现经典 x86 CPU，使复古计算爱好者能够以硬件级别的精度运行老软件，并为 CPU 微架构提供了宝贵的教育资源。 该设计仅使用约 18,000 个 LUT，使其足够紧凑，适用于小型 FPGA，并通过运行 Doom 和修补后的 Linux 3.7 内核（gray386linux）进行了验证。

hackernews · wicket · May 23, 14:25 · [社区讨论](https://news.ycombinator.com/item?id=48248014)

**背景**: Intel 80386（i386）是 1985 年推出的 32 位 CPU，以在早期 PC 中的作用和作为首款支持 32 位运算的 x86 处理器而闻名。微码是控制 CPU 内部操作的低级指令层，允许将复杂指令作为简单步骤的序列来执行。Z386 在 FPGA 上使用从真实 80386 芯片反汇编的原始微码重新实现了该架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microcode">Microcode</a></li>
<li><a href="https://en.wikipedia.org/wiki/Soft_microprocessor">Soft microprocessor - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对使用 Doom 感到有趣，注意到 FPGA 资源使用紧凑（18K LUTs），并询问微码反汇编是否揭示后门。一条评论链接到了相关的微码反汇编项目。

**标签**: `#FPGA`, `#retrocomputing`, `#open-source hardware`, `#CPU implementation`, `#microcode`

---

<a id="item-7"></a>
## [深度学习优化：从基本原理到硬件利用](https://horace.io/brrr_intro.html) ⭐️ 8.0/10

Horace He 发表了一篇全面的博客文章，通过理解硬件瓶颈并应用内核融合、内存合并和使用 Tensor Cores 等技术，解释了如何最大化深度学习中的 GPU 利用率。该文于 2022 年发布，并已引发广泛讨论。 这篇文章提供了罕见的从基本原理出发的视角，帮助实践者超越黑盒框架，编写更高效的代码。它还突出了 NVIDIA 持续的硬件领先地位，这影响着整个深度学习生态系统。 文章强调，在 Python 执行一次 FLOP 的时间内，A100 GPU 可以执行 975 万次 FLOPS，说明了高级代码与优化代码之间的巨大差距。它涵盖了诸如分块、寄存器缓存和使用 cuDNN 融合操作等具体优化方法。

hackernews · tosh · May 23, 11:50 · [社区讨论](https://news.ycombinator.com/item?id=48246889)

**背景**: 深度学习计算高度依赖矩阵乘法和卷积，这些操作在 GPU 上使用专门的硬件如 NVIDIA 的 Tensor Cores 实现。这些 Tensor Cores 以混合精度执行乘加运算，极大加速了训练和推理。像 cuDNN 这样的库提供了自动利用此类硬件的优化例程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tensor_Cores">Tensor Cores</a></li>
<li><a href="https://developer.nvidia.com/cudnn">CUDA Deep Neural Network ( cuDNN ) | NVIDIA Developer</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该文为经典之作，并指出 NVIDIA 的硬件领先优势令人瞩目但也令人担忧。其他评论者希望更深入地讨论生产系统的故障模式，而一位评论者强调深度学习本质上是线性代数，可以在没有 GPU 的情况下理解。

**标签**: `#deep learning`, `#performance optimization`, `#GPU computing`, `#NVIDIA`, `#machine learning systems`

---

<a id="item-8"></a>
## [微软内部取消 Claude Code 许可](https://www.theverge.com/tech/930447/microsoft-claude-code-discontinued-notepad) ⭐️ 8.0/10

据泄露信息，微软正在撤销许多内部开发者的 Claude Code 许可，并强制他们改用 GitHub Copilot CLI。 这一决定揭示了微软在战略上优先推广自家 AI 编码工具而非 Anthropic 的 Claude Code，影响了开发者工作流程，并引发了关于工具质量和企业动机的讨论。 据报告，开发者更偏爱 Claude Code 而非 Copilot，但微软以成本和集成问题为由撤销许可。此变动仅影响内部许可，外部 Claude Code 仍可使用。

hackernews · robertkarl · May 22, 17:32 · [社区讨论](https://news.ycombinator.com/item?id=48238896)

**背景**: Claude Code 是由 Anthropic 开发的 AI 编码助手，基于其 Claude 大语言模型。GitHub Copilot CLI 是微软的命令行编码工具。内部工具选型常反映 AI 助手市场的竞争态势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，开发者用行动选择了 Claude Code 而非 Copilot，令牌成本和模型效果是关键考量。有人认为，有监督的人工介入使用 Claude Code 比无代理方式更高效。

**标签**: `#AI coding tools`, `#Microsoft`, `#Claude Code`, `#Copilot`, `#developer workflow`

---

<a id="item-9"></a>
## [腾讯收购喜马拉雅获批，须放弃独家版权](https://mp.weixin.qq.com/s/xnx31SOS6NMozZXnHeaaQg) ⭐️ 8.0/10

中国监管机构批准了腾讯对喜马拉雅的收购，但要求腾讯放弃在线音频版权独家授权，并在期限内解除现有独家合同。 这一条件打破了喜马拉雅的内容壁垒，可能增强中国在线音频市场的竞争，并改善用户的跨平台收听体验。 腾讯不得达成或变相达成在线音频版权独家授权，并须逐步解除现有独家合同。此要求适用于当前及未来的版权。

telegram · zaihuapd · May 22, 10:33

**背景**: 喜马拉雅是中国最大的在线音频平台，拥有大量独家播客、有声书和广播节目。独家版权使其保持竞争优势。腾讯的收购引发了反垄断担忧，因此附加了此条件。

**标签**: `#Tencent`, `#antitrust`, `#audio`, `#regulation`, `#China`

---

<a id="item-10"></a>
## [中国八部门整治非法跨境证券期货基金经营](https://t.me/zaihuapd/41525) ⭐️ 8.0/10

中国八部门联合印发整治方案，打击非法跨境证券期货基金经营活动，在两年集中整治期内只允许存量投资者单向卖出并转出资金。证监会已对老虎证券、富途证券、长桥证券非法跨境展业立案调查。 此次监管整顿直接影响数百万通过境外券商交易港股和美股的境内投资者，标志着资本管制的大幅收紧。这可能重塑跨境投资格局，迫使金融科技平台停止在华运营。 两年集中整治期自方案印发之日起计算；期间只允许存量投资者卖出持仓并转出资金，禁止新买入和转入资金。期满后，所有相关境内网站、交易软件和配套服务器必须全面关停。

telegram · zaihuapd · May 22, 13:55

**背景**: 未经批准的境外机构在中国境内开展跨境证券期货基金业务多年来一直属于非法行为，但执法力度参差不齐。2021 年对老虎和富途的整顿已表明监管趋严，而本次新方案正式确立了全面整治方针。存量投资者是指在监管行动前已在这些平台开户的投资者；方案允许他们仅平仓并提取资金，以避免金融混乱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.guancha.cn/GuanJinRong/2026_05_22_818035.shtml">m.guancha.cn/GuanJinRong/2026_05_22_818035.shtml</a></li>
<li><a href="https://news.e23.cn/wanxiang/2026-05-22/2026052200312.html">news.e23.cn/wanxiang/2026-05-22/2026052200312.html</a></li>
<li><a href="https://m.jiemian.com/article/14471841.html">m.jiemian.com/article/14471841.html</a></li>

</ul>
</details>

**标签**: `#regulation`, `#cross-border investment`, `#securities`, `#China`, `#fintech`

---

<a id="item-11"></a>
## [Cloudflare 全球故障 25 分钟，影响 28% HTTP 流量](https://t.me/zaihuapd/41527) ⭐️ 8.0/10

2025 年 12 月 5 日 08:47 UTC，Cloudflare 全球网络发生 25 分钟中断，约 28%的 HTTP 流量受影响。此次故障源于修复 CVE-2025-55182 时，导致使用旧版 FL1 代理及托管规则集的客户 WAF 功能失效。 此次事件凸显了关键互联网基础设施在部署安全补丁时的脆弱性，表明一次修复可能引发连锁反应，导致近三分之一的 Cloudflare 流量中断。 仅使用旧版 FL1 代理并部署 Cloudflare 托管规则集的客户受到影响；服务于 09:12 UTC 完全恢复。底层的 CVE-2025-55182 是 React Server Components（19.0.0–19.2.0 版本）中的一个关键预认证远程代码执行漏洞。

telegram · zaihuapd · May 22, 16:15

**背景**: Cloudflare 运营着全球内容分发网络（CDN）和 Web 应用防火墙（WAF）。FL1 代理是较旧的代理架构，Cloudflare 正在逐步迁移。CVE-2025-55182（也称 React2Shell）允许未经身份验证的攻击者在 React Server Components 上执行任意代码，属于严重安全威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2025-55182">NVD - CVE-2025-55182</a></li>
<li><a href="https://developers.cloudflare.com/cloudflare-one/traffic-policies/proxy/">Proxy · Cloudflare One docs</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#网络故障`, `#全球中断`, `#CVE`, `#WAF`

---

<a id="item-12"></a>
## [微软内部推广 Claude Code，鼓励非技术人员使用](https://t.me/zaihuapd/41535) ⭐️ 8.0/10

微软正在其工程团队中广泛推广 Anthropic 的 Claude Code，包括 CoreAI 团队和负责 Windows、Microsoft 365、Outlook 等产品的体验与设备部门。软件工程师现在需要同时使用 Claude Code 和 GitHub Copilot 并提供对比反馈。 此举表明微软愿意采用竞争对手的工具而非自家的 Copilot，可能重塑 AI 辅助编程市场，并影响全行业的开发者工具偏好。 微软鼓励没有编程经验的非技术员工使用 Claude Code 进行原型设计。公司要求工程师提供 Claude Code 与 GitHub Copilot 的详细对比反馈。

telegram · zaihuapd · May 23, 06:05

**背景**: Claude Code 是 Anthropic 推出的智能编程工具，运行在终端中，能够理解代码库、编辑文件并执行命令。目前作为有限研究预览版提供。GitHub Copilot 是微软自家的人工智能结对编程工具，集成在 VS Code 等 IDE 中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://www.anthropic.com/news/claude-3-7-sonnet">Claude 3.7 Sonnet and Claude Code \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI coding`, `#Microsoft`, `#Claude Code`, `#GitHub Copilot`, `#developer tools`

---

<a id="item-13"></a>
## [微软财报披露 OpenAI 单季巨亏 115 亿美元](https://t.me/zaihuapd/41537) ⭐️ 8.0/10

微软最新财报显示，其对 OpenAI 的权益法投资导致单季度净利润减少 31 亿美元，据此推算 OpenAI 该季度净亏损约 115 亿美元。 这一巨额亏损凸显了开发前沿 AI 模型的巨大财务负担，引发了对 AI 投资可持续性的担忧，也彰显了微软等主要投资者面临的财务风险。 根据微软持有 OpenAI 约 27%股权计算，亏损约 115 亿美元；若按税前损失和实际持股比例 32.5%计算，亏损可能超 120 亿美元。这一亏损规模是 OpenAI 2024 年上半年 43 亿美元营收的近三倍。

telegram · zaihuapd · May 23, 07:40

**背景**: 权益法会计要求微软在其损益表中报告对 OpenAI 净利润或亏损的份额。微软迄今已向 OpenAI 投入 116 亿美元，占其 130 亿美元承诺投资的绝大部分。OpenAI 的巨额亏损反映了其为了开发 GPT-4 等先进 AI 系统而在计算基础设施和人才方面的巨大支出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.yumpu.com/en/document/view/30041775/1-cch-china">1 - CCH China</a></li>
<li><a href="https://npcobserver.com/wp-content/uploads/2024/04/Accounting-Law-Draft-Amendment.pdf">标题</a></li>

</ul>
</details>

**标签**: `#AI`, `#OpenAI`, `#Microsoft`, `#Financials`, `#Investment`

---

<a id="item-14"></a>
## [中国对富途控股和老虎证券跨境违规行为处以罚款](https://t.me/zaihuapd/41539) ⭐️ 8.0/10

中国监管机构拟对富途控股处以 18.5 亿元罚款，对老虎证券处以 4.11 亿元罚款，原因是它们在中国内地无牌照开展证券、期货及公募基金销售业务。 此次执法标志着对跨境金融科技活动的重大打击，可能重塑海外券商与中国客户的业务模式，并表明监管将更加严格。 富途控股创始人兼首席执行官李华还面临 125 万元个人罚款，最终罚款金额需经法律程序后确定。

telegram · zaihuapd · May 23, 10:58

**背景**: 中国法律要求证券和期货公司获得中国证监会（CSRC）的牌照才能为内地客户服务。总部位于香港的富途控股和老虎证券此前一直在未获得相关牌照的情况下提供跨境交易服务，从而引发监管行动。

**标签**: `#fintech`, `#regulation`, `#China`, `#securities`, `#cross-border`

---

<a id="item-15"></a>
## [美商海盗船采用长鑫存储 DDR5 芯片，价格有望下调](https://thenextweb.com/news/chinese-dram-cxmt-corsair-ddr5-memory-prices) ⭐️ 8.0/10

美商海盗船（Corsair）已开始在其 DDR5 内存模组中采用长鑫存储（CXMT）的 DRAM 芯片，目前 6000 MT/s 的内存套装已上市。 这一由西方主要品牌采取的举措标志着中国 DRAM 日益被接受，可能加剧市场竞争，并在传统巨头供应受限的情况下为消费者带来更低的 DDR5 价格。 采用长鑫芯片的 DDR5 模组运行速度为 6000 MT/s，性能规格与国际主流产品一致。这一转变部分源于全球 DRAM 巨头优先为 AI 生产高带宽内存（HBM），导致消费级内存供应趋紧。

telegram · zaihuapd · May 23, 11:17

**背景**: 长鑫存储（CXMT）是一家总部位于中国安徽合肥的 DRAM 制造商，专注于动态随机存取存储器的设计、研发和生产。全球 DRAM 市场长期由三星、SK 海力士、美光三大巨头主导，它们近期将产能转向 AI 加速器所需的高带宽内存（HBM），导致消费级 DDR5 供应出现缺口。长鑫存储正通过扩产填补这一空缺，并计划于 2025 年上市。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/长鑫存储">长 鑫 存 储 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.cxmt.com/en/">About cxmt - cxmt</a></li>

</ul>
</details>

**标签**: `#DDR5`, `#memory`, `#semiconductors`, `#supply chain`, `#China`

---

<a id="item-16"></a>
## [深入探讨 HTML <dl>元素的语义和历史](https://benmyers.dev/blog/on-the-dl/) ⭐️ 7.0/10

Ben Myers 在 2021 年发表的一篇博客文章详细探讨了 HTML <dl>元素，涵盖其语义、使用模式以及源于 IBM DCF/GML 文档的历史渊源。 这篇文章加深了对语义 HTML 和无障碍性的理解，纠正了关于 ARIA 角色的常见误解，并强调了<dl>从定义列表到关联列表的演变。 该文章指出，在 HTML5 之前，<dl>被称为定义列表，但现在它表示通用的关联列表；同时还指出<dl>没有隐式 ARIA 角色，但可以赋予 group 或 list 等角色。

hackernews · ravenical · May 23, 13:03 · [社区讨论](https://news.ycombinator.com/item?id=48247325)

**背景**: HTML <dl>元素（描述列表）用于将术语和描述成对分组，例如在词汇表或元数据中。其历史根源可追溯到 20 世纪 80 年代 IBM 的文档组成设施通用标记语言（DCF/GML），该语言包括 DL、GL、OL、UL 和 SL 列表类型。

**社区讨论**: 评论中包括 chrismorgan 对<dl>上 ARIA 角色限制的纠正，提供了关于允许角色和 aria-label 用法的见解。Kqp 表达了对语义 HTML 僵化性的挫败感，而 theodpHN 和 jimbosis 提供了历史背景，链接到 IBM 手册和第一个网站。

**标签**: `#HTML`, `#Semantic HTML`, `#Accessibility`, `#Web Development`, `#History`

---

<a id="item-17"></a>
## [向乌干达难民营寄送笔记本电脑：腐败与物流的艰辛历程](https://notesbylex.com/shipping-a-laptop-to-a-refugee-camp-in-uganda) ⭐️ 7.0/10

作者详细描述了向乌干达难民营寄送一台笔记本电脑的艰难经历，揭露了运输过程中的官僚腐败和低效问题。 这个故事凸显了发展中国家海关和邮政系统的系统性腐败，影响人道主义援助和技术部署。 作者尝试使用普通邮政服务，结果导致延误、索贿，笔记本电脑险些丢失。

hackernews · lexandstuff · May 22, 21:36 · [社区讨论](https://news.ycombinator.com/item?id=48241997)

**背景**: 向发展中国家偏远地区寄送物品常常因腐败的海关行为和不可靠的邮政系统而面临挑战。许多当地人和外籍人士转而使用私人快递或托付给旅行者（线路运输）来绕过这些问题。

**社区讨论**: 评论者证实了作者的遭遇，一位乌干达用户指出系统因腐败而瘫痪。他们建议不要使用普通邮政和昂贵的快递，而应使用非洲常见的非正式货运代理。

**标签**: `#logistics`, `#Uganda`, `#corruption`, `#development`, `#hardware`

---

<a id="item-18"></a>
## [Rubish：用纯 Ruby 编写的 Unix Shell](https://github.com/amatsuda/rubish) ⭐️ 7.0/10

Rubish 是一个完全用纯 Ruby 重新实现的 Unix shell，提供了 Ruby 语法与 shell 功能的独特融合。 该项目探索了将脚本语言与 shell 结合的新途径，可能影响未来的 shell 设计，但由于受众较小，其实际影响可能有限。 Rubish 用纯 Ruby 编写，无外部依赖，支持管道和重定向等基本 shell 操作，但可能缺少 bash 或 zsh 等成熟 shell 的功能。

hackernews · winebarrel · May 23, 06:32 · [社区讨论](https://news.ycombinator.com/item?id=48245262)

**背景**: Unix shell 是一种命令行解释器，为类 Unix 操作系统提供用户界面，允许用户执行命令、管理文件和运行脚本。传统的 shell（如 bash 或 zsh）用 C 语言编写，并拥有自己的脚本语法。Rubish 提供了一个完全用 Ruby 编写的替代方案，使用户能够使用 Ruby 语法进行 shell 脚本编写，这对 Ruby 开发者来说可能更为熟悉。

**社区讨论**: 社区评论褒贬不一：有人对这一概念感到惊讶但对其实用性表示怀疑，也有人欣赏其新颖性。一位用户表示既惊讶又震惊，并提到过去尝试融合 Ruby 和 bash 的经历。另一位用户则讨论了“氛围编程”(vibe-coding) 可能让其他人更难贡献代码的问题。

**标签**: `#ruby`, `#shell`, `#unix`, `#programming-languages`

---

<a id="item-19"></a>
## [Oura 收到政府索取用户健康数据的要求](https://this.weekinsecurity.com/oura-says-it-gets-government-demands-for-user-data-will-it-share-how-many/) ⭐️ 7.0/10

Oura 承认收到政府索取其智能戒指用户数据的要求，但尚未承诺披露此类请求的数量。 这引发了严重的隐私担忧，因为 Oura 的健康数据高度敏感且未采用端到端加密，可能在用户不知情的情况下被政府获取。 Oura 的健康数据（包括心率、睡眠模式和位置）未进行端到端加密，意味着数据可在中间节点被解密。该公司未回复关于公布透明度数据的询问。

hackernews · donohoe · May 23, 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48247876)

**背景**: Oura 是一家芬兰健康科技公司，以其智能戒指闻名，该戒指可追踪睡眠、活动和其他生物指标。随着可穿戴健康设备越来越普及，政府越来越多地寻求获取此类数据，引发了有关隐私和加密的法律与伦理问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://this.weekinsecurity.com/oura-says-it-gets-government-demands-for-user-data-will-it-share-how-many/">Oura says it gets government demands for user data . Will it share...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Oura_ring">Oura ring</a></li>

</ul>
</details>

**社区讨论**: 评论者指出缺乏端到端加密，有人指出这与传输中加密的混淆。其他人质疑政府对此类数据的兴趣，而一些人表示更担心其他隐私问题，如智能电视的内容识别。

**标签**: `#privacy`, `#wearables`, `#government data requests`, `#encryption`, `#biometric data`

---

<a id="item-20"></a>
## [Electrobun 2.0 因 Rust 重写而与 Bun 解耦](https://twitter.com/YoavCodes/status/2058064720553222567) ⭐️ 7.0/10

Electrobun 2.0 将不再依赖 Bun 运行时，因为该项目正在用 Rust 重写，从而与之前基于 Bun 的架构解耦。 这一解耦标志着桌面应用程序框架向 Rust 的转变，可能提升性能并减少对 Bun 等 JavaScript 运行时的依赖，同时也凸显了 LLM 生成代码库的维护难题。 Electrobun 是一个跨平台桌面应用框架，使用原生 WebView，此前依赖 Bun 执行 JavaScript。用 Rust 重写后，它可以独立运行，体积更小、执行速度更快。

hackernews · bundie · May 23, 11:54 · [社区讨论](https://news.ycombinator.com/item?id=48246917)

**背景**: Electrobun 是一个框架，用于使用 TypeScript 构建超快、极小的桌面应用程序，类似于 Electron 但使用原生 WebView。Bun 是一个 JavaScript 运行时和工具包，旨在替代 Node.js，最初用 Zig 编写。这次解耦反映了将性能关键软件用 Rust 重写的更广泛趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/blackboardsh/electrobun">GitHub - blackboardsh/ electrobun : Build ultra fast, tiny, and...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区成员表达了对 Electrobun 作为 Electron 替代品的兴趣，并讨论了 LLM 生成代码库的风险，有人认为除非 LLM 也能维护代码，否则维护变得困难。还有人指出这一事件是 2026 年软件发展趋势的风向标。

**标签**: `#Electrobun`, `#Bun`, `#LLM`, `#software engineering`, `#Rust`

---

<a id="item-21"></a>
## [Antigravity 将 Gemini 速率限制提升三倍并重置周配额](https://t.me/zaihuapd/41523) ⭐️ 7.0/10

Antigravity 宣布，即日起将所有付费层级 Gemini 模型的速率限制提升至原来的三倍，并重置所有用户本周的 Gemini 配额。 这一调整直接回应用户对之前速率限制过于严格的反馈，使开发者和企业能够更密集地使用 Gemini 模型进行开发和部署。 速率限制提升适用于所有付费层级，团队还重置了本周配额以便用户立即受益。官方承诺将推出更多改进措施。

telegram · zaihuapd · May 22, 11:18

**背景**: Antigravity 是一个提供 Google Gemini 模型访问的服务，Gemini 是 Google 开发的多模态 AI 模型系列。速率限制是 API 在特定时间内允许的请求数量，旨在确保公平使用和系统稳定性。通过将限制提升三倍，Antigravity 旨在满足日益增长的用户需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/rate-limits">Rate limits | Gemini API | Google AI for Developers</a></li>
<li><a href="https://www.aifreeapi.com/en/posts/gemini-api-rate-limit">Gemini API Rate Limits : Complete Guide to All Tiers, Models ...</a></li>

</ul>
</details>

**标签**: `#Antigravity`, `#Gemini`, `#rate limits`, `#model service`, `#API quota`

---

<a id="item-22"></a>
## [我国日均词元调用量两年增超千倍，突破 140 万亿](https://t.me/zaihuapd/41542) ⭐️ 7.0/10

国家数据局披露，2025 年 3 月我国日均词元（Token）调用量突破 140 万亿，而 2024 年初仅为 1000 亿，2025 年底达到 100 万亿，两年间增长超千倍。 这一爆发式增长标志着中国人工智能产业商业化进程加速，围绕词元的计量、定价和交易正在形成新的价值体系。同时，这也显示出数据要素市场化配置改革下，人工智能高质量数据供给体系正在构建。 词元是大模型处理信息的最小单元，类似于字或词。调用量、分发与结算等指标正成为人工智能商业化的重要路径。

telegram · zaihuapd · May 23, 14:36

**背景**: 在大语言模型中，文本被切分为词元（Token，即单词、子词或字符）进行处理。词元调用量衡量的是 AI 服务实际处理的词元数量，反映了真实使用情况。这一快速增长表明，从聊天机器人到企业工具，AI 应用在中国已广泛普及。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/27598806064">大模型核心概念科普：Token、上下文长度、最大输出，一次讲透</a></li>
<li><a href="https://www.cnblogs.com/wzzkaifa/p/19086539">深入理解大语言模型：从token到next token prediction，小白程序员必...</a></li>
<li><a href="https://blog.csdn.net/2503_94545876/article/details/161346157">AI、大模型都离不开的Token到底是什么？-CSDN博客</a></li>

</ul>
</details>

**标签**: `#AI`, `#tokenization`, `#data economy`, `#China`, `#large language models`

---