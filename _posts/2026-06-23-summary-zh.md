---
layout: default
title: "Horizon Summary: 2026-06-23 (ZH)"
date: 2026-06-23
lang: zh
---

> From 42 items, 19 important content pieces were selected

---

1. [中国“灵晟”超算登顶 TOP500，首台纯 CPU 超 2 ExaFLOPS](#item-1) ⭐️ 10.0/10
2. [FUTO 发布媲美 Gboard 的滑动输入模型](#item-2) ⭐️ 8.0/10
3. [无限 OCR：一次性长视距解析](#item-3) ⭐️ 8.0/10
4. [斯坦福研究：AI 招聘工具存在种族偏见](#item-4) ⭐️ 8.0/10
5. [即将到来的循环：AI 代理与规范驱动编程](#item-5) ⭐️ 8.0/10
6. [Anthropic 推出 Slack 协作工具 Claude Tag](#item-6) ⭐️ 8.0/10
7. [Mistral AI 发布 OCR 4，增强多语言支持](#item-7) ⭐️ 8.0/10
8. [麦迪逊广场花园建立档案监控反对人脸识别的活动人士](#item-8) ⭐️ 8.0/10
9. [近半数 LG 智能电视应用含住宅代理 SDK](#item-9) ⭐️ 8.0/10
10. [美国人形机器人依赖中国零部件](#item-10) ⭐️ 8.0/10
11. [三星发布 UFS 5.0，带宽 10.8 GB/s 面向端侧 AI](#item-11) ⭐️ 8.0/10
12. [SpaceX 猎鹰重型火箭将于 2028 年发射欧洲罗莎琳德·富兰克林火星车](#item-12) ⭐️ 8.0/10
13. [FFmpeg 严重漏洞可致远程代码执行](#item-13) ⭐️ 8.0/10
14. [研究发现随机洗牌需 14 次才能充分随机化](#item-14) ⭐️ 8.0/10
15. [Swift Package Index 加入苹果](#item-15) ⭐️ 7.0/10
16. [TikZ 编辑器：LaTeX 图形的所见即所得工具](#item-16) ⭐️ 7.0/10
17. [F3：内嵌 WASM 解码器的列式存储新格式](#item-17) ⭐️ 7.0/10
18. [巨型卡车和 SUV 的致命崛起](#item-18) ⭐️ 7.0/10
19. [OpenAI 推出 AI 动画电影《Critterz》，成本低于 3000 万美元](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [中国“灵晟”超算登顶 TOP500，首台纯 CPU 超 2 ExaFLOPS](https://news.mydrivers.com/1/1131/1131573.htm) ⭐️ 10.0/10

部署于深圳国家超算中心的“灵晟”超算，在 6 月 23 日公布的 TOP500 榜单中以 2.198 ExaFLOPS 的 HPL 性能排名第一，成为全球首台纯 CPU 设计突破 2 ExaFLOPS 的系统。 这标志着中国超算时隔八年重回世界第一，展示了国产 CPU 架构和自主可控的重大进展，对国内 HPC 和半导体生态具有战略重要性。 灵晟基于国产灵鲲平台与 LX2 处理器，采用纯 CPU 架构；同时还在 HPCG 基准测试中排名第一，HPL-MxP 混合精度测试排名第四。

telegram · zaihuapd · Jun 23, 15:30

**背景**: TOP500 榜单通过 HPL 基准测试（测量双精度浮点性能）对全球超算排名。HPCG 基准测试补充 HPL，评估更贴近实际应用的内存带宽和延迟模式。HPL-MxP 基准测试专注于混合精度工作负载，与 AI 融合相关。LX2 处理器是基于 Arm 架构的高性能低功耗处理器（如 LX2160A），常用于网络和边缘计算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ldteq.com/article/4143.html">NXP LX2162A处理器：适用于边缘计算的高性能、低功耗紧凑型处理器</a></li>
<li><a href="https://hpl-mxp.org/">HPL-MxP Mixed-Precision Benchmark</a></li>
<li><a href="https://blog.csdn.net/gitblog_00306/article/details/141117385">HPCG 基准测试项目教程-CSDN博客</a></li>

</ul>
</details>

**标签**: `#HPC`, `#超算`, `#TOP500`, `#国产芯片`, `#自主可控`

---

<a id="item-2"></a>
## [FUTO 发布媲美 Gboard 的滑动输入模型](https://swipe.futo.tech/) ⭐️ 8.0/10

FUTO 为其注重隐私的安卓键盘发布了一款新的滑动输入模型，显著提升了滑动准确度，媲美 Gboard。该模型采用 FUTO 模型许可证，推理库则采用 GPLv3 许可证。 此次更新解决了隐私键盘的主要短板——此前滑动输入体验不佳，使 FUTO 键盘成为注重隐私用户更可行的 Gboard 替代品。同时展示了社区贡献数据在改进机器学习模型方面的潜力。 滑动库采用 GPLv3 许可证，但安卓键盘应用使用 FUTO 许可证，这引发了一些用户的批评。模型本身采用 FUTO 模型许可证，后续将发布论文详细介绍训练和架构。

hackernews · futohq · Jun 23, 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48648619)

**背景**: FUTO 是一个致力于开发和资助开源软件的组织，旨在让用户掌控自己的计算机，挑战大型科技公司。其安卓键盘一直是受欢迎的隐私替代品，但滑动输入准确度落后于 Gboard，这是用户犹豫是否切换的主要原因。新模型使用机器学习，部分训练数据来自用户贡献，类似于 Gboard 改进其模型的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://swipe.futo.tech/">FUTO Swipe</a></li>
<li><a href="https://futo.tech/">FUTO - Computers Belong to You</a></li>
<li><a href="https://www.futo.org/about/what-is-futo/">What is FUTO?</a></li>

</ul>
</details>

**社区讨论**: 用户反馈非常积极，许多人表示新的滑动模型足以让他们永久从 Gboard 切换过来。但也指出一些细微问题，如大小写错误和缺乏上下文单词建议。少数用户对键盘应用的 FUTO 许可证表示担忧，尽管滑动库是 GPLv3 的。

**标签**: `#privacy`, `#android`, `#keyboard`, `#open-source`, `#machine-learning`

---

<a id="item-3"></a>
## [无限 OCR：一次性长视距解析](https://github.com/baidu/Unlimited-OCR) ⭐️ 8.0/10

百度开源了 Unlimited-OCR，该模型通过一种架构技巧避免了 KV 缓存导致的内存增长，实现了对整个多页 PDF 的一次性解析，无需分块处理。 这一突破解决了长文档 OCR 中的根本性内存限制，使得一次性转录数百页而不耗尽显存成为可能。它有望大幅简化文档数字化流程，并且开源，便于广泛采用。 该技巧将 KV 缓存增长从 O(N)降低到接近常数，防止长序列期间内存爆炸。该模型借鉴了 Deepseek-OCR 和 PaddleOCR 的思路，论文已发布在 arXiv 上（2606.23050）。

hackernews · ingve · Jun 23, 11:35 · [社区讨论](https://news.ycombinator.com/item?id=48643426)

**背景**: 传统的基于 Transformer 的 OCR 模型逐页处理文档，因为 KV 缓存随输入长度线性增长，迅速耗尽 GPU 内存。这迫使开发者对 PDF 进行分块，增加了复杂性并丢失了跨页上下文。Unlimited-OCR 引入了一种类似流式的机制，压缩或丢弃 KV 缓存，从而实现长文档的端到端处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.explainx.ai/blog/baidu-unlimited-ocr-one-shot-long-horizon-parsing-2026">Baidu Unlimited-OCR: One-Shot Long-Horizon Document Parsing Explained ...</a></li>
<li><a href="https://github.com/baidu/Unlimited-OCR">Welcome the Era of One-shot Long-horizon Parsing. - GitHub</a></li>
<li><a href="https://arxiv.org/html/2606.23050v1">Unlimited OCR Works Welcome the Era of One-shot Long-horizon Parsing</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞了解决内存问题的架构技巧，有用户解释了 KV 缓存增长问题。其他人提到了实际应用场景，如光学音乐识别，并感谢团队致谢 Deepseek-OCR。还有评论指出名称引用自 Fate/stay night 中的无限剑制。

**标签**: `#OCR`, `#Machine Learning`, `#Long-Context`, `#Memory Optimization`, `#Document Parsing`

---

<a id="item-4"></a>
## [斯坦福研究：AI 招聘工具存在种族偏见](https://hai.stanford.edu/news/ai-hiring-tools-can-yield-racial-bias-and-systemic-rejection) ⭐️ 8.0/10

斯坦福大学的一项研究发现，AI 招聘工具存在种族偏见和系统性拒绝模式，被拒绝的申请者更可能在多个职位上被拒绝。 这引发了对自动化招聘公平性的担忧，此类工具被世界 500 强公司广泛使用，可能影响数万名求职者。 该研究使用美国平等就业机会委员会（EEOC）的“五分之四规则”衡量不利影响，标记某个群体被推荐的比率低于最受推荐群体 80%的职位。

hackernews · sizzle · Jun 23, 18:56 · [社区讨论](https://news.ycombinator.com/item?id=48649673)

**背景**: AI 招聘工具通常使用算法筛选简历或评估候选人。偏见可能来自训练数据或设计选择。欧盟的《人工智能法案》将招聘 AI 列为高风险，要求透明度和人工监督。

**社区讨论**: 一些评论者对研究方法提出质疑，认为拒绝模式可能反映候选人质量差异而非偏见。另一些人指出，现有的法律框架如欧盟《人工智能法案》可以解决这些问题。

**标签**: `#AI ethics`, `#algorithmic bias`, `#hiring`, `#racial discrimination`, `#fairness`

---

<a id="item-5"></a>
## [即将到来的循环：AI 代理与规范驱动编程](https://lucumr.pocoo.org/2026/6/23/the-coming-loop/) ⭐️ 8.0/10

Armin Ronacher 的博文《即将到来的循环》讨论了在迭代编码循环中使用 AI 代理的挑战和策略，强调事前规范对于成功至关重要，而当前的大语言模型方法存在局限性。 这很重要，因为随着 AI 编码代理越来越普遍，理解如何有效地将其整合到开发工作流程中——特别是代理循环与规范驱动开发之间的权衡——对于生产力和代码质量至关重要。 该文指出，即使有手动引导，某些代码模式也无法自然由大语言模型生成，而过度的 null 检查是一个常见问题。有效使用需要先编写细致的规范，类似于交给初级开发人员。

hackernews · ingve · Jun 23, 11:06 · [社区讨论](https://news.ycombinator.com/item?id=48643180)

**背景**: AI 编码代理使用“代理循环”——一个推理、行动、观察和重复的循环——来自主完成编码任务。然而，没有明确的规范，这些循环可能会浪费迭代。规范驱动开发，即用户首先与 AI 一起定义详细的规范，已成为更可靠的方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mindstudio.ai/blog/what-is-loop-engineering-ai-coding-agents">What Is Loop Engineering? The New Meta for AI Coding Agents | MindStudio</a></li>
<li><a href="https://addyosmani.com/blog/ai-coding-workflow/">AddyOsmani.com - My LLM coding workflow going into 2026</a></li>
<li><a href="https://arxiv.org/html/2601.03878v1">Understanding Specification-Driven Code Generation with LLMs: An Empirical Study Design**This paper is a Stage 1 Registered Report. The study protocol and analysis plan were peer reviewed and accepted at SANER 2026 with a Continuity Acceptance (CA) score for Stage 2.</a></li>

</ul>
</details>

**社区讨论**: 评论者一致认为，事前规范是一个瓶颈，有人指出他们“受限于规范”，而清晰度需要时间来迭代有缺陷的版本。另一评论者强调了难以说服开发者减少由大语言模型生成的代码中的过度 null 检查。

**标签**: `#AI agents`, `#software engineering`, `#LLM`, `#code generation`, `#developer experience`

---

<a id="item-6"></a>
## [Anthropic 推出 Slack 协作工具 Claude Tag](https://www.anthropic.com/news/introducing-claude-tag) ⭐️ 8.0/10

Anthropic 宣布推出 Claude Tag，这是一个多玩家 AI 队友，可以在 Slack 频道中被@提及进行协作。团队成员可以与一个持久的 Claude 实例交互，该实例跨对话保留上下文。 这标志着从单用户 AI 助手向共享、持久的 AI 队友的转变，可能改变团队协作方式。它满足了企业通信工具中需要保留上下文的 AI 需求。 Claude Tag 是多玩家模式：每个 Slack 频道只有一个 Claude，任何人都能看到它在处理什么并继续对话。它会随着时间学习，尽管一些用户指出它在区分记忆内容方面存在挑战。

hackernews · adocomplete · Jun 23, 17:09 · [社区讨论](https://news.ycombinator.com/item?id=48648039)

**背景**: Slack 是一个流行的团队通信平台，用户可以创建不同主题的频道。像 Claude Tag 这样的 AI 助手集成到这些频道中，提供代码生成和任务管理等协作功能。然而，企业安全和合规性担忧涉及权限继承和数据访问。

**社区讨论**: 社区评论显示出不同的反应：一些用户质疑企业安全和权限对齐，而另一些用户则称赞多玩家持久性。一位用户指出 Claude 的学习局限性，认为它倾向于基于错误假设进行构建。另一位用户则担心默认无限制支出可能导致意外费用。

**标签**: `#AI`, `#Slack`, `#Anthropic`, `#Collaboration`, `#Enterprise`

---

<a id="item-7"></a>
## [Mistral AI 发布 OCR 4，增强多语言支持](https://mistral.ai/news/ocr-4/) ⭐️ 8.0/10

Mistral AI 宣布推出 OCR 4，这是其光学字符识别模型的新版本，在八个语言组中提供了改进的多语言能力。 此次发布展示了 OCR 技术的持续进步，这对于文档数字化和实现多语言自动文本提取至关重要，可能对邮政服务、档案管理和数据录入等行业产生影响。 根据 Mistral 的内部评估，OCR 4 在八个语言组中领先，包括英语、西欧、东欧、中东、中文、东亚、东南亚和专门语言。公告页面的初始版本因将某些语言称为“次要”而受到批评，随后进行了修正。

hackernews · meetpateltech · Jun 23, 14:03 · [社区讨论](https://news.ycombinator.com/item?id=48645152)

**背景**: 光学字符识别（OCR）技术将文本图像转换为机器可读文本。Mistral AI 是一家以大型语言模型闻名的欧洲人工智能公司。新的 OCR 模型旨在处理多种文字和语言，由于书写系统和字体的差异，这具有挑战性。

**社区讨论**: 社区评论涵盖了对该技术的赞扬，以及对 Mistral 基准可视化选择和初始语言标签的批评。一些人将其与 Unlimited-OCR 等开源替代品进行比较，而另一些人则注意到尽管 Mistral 是一家欧洲公司，但拍摄地点却在旧金山，这令人惊讶。

**标签**: `#OCR`, `#Mistral`, `#AI`, `#Machine Learning`, `#Natural Language Processing`

---

<a id="item-8"></a>
## [麦迪逊广场花园建立档案监控反对人脸识别的活动人士](https://www.404media.co/madison-square-garden-made-dossier-on-activists-who-opposed-facial-recognition/) ⭐️ 8.0/10

麦迪逊广场花园（MSG）针对反对其人脸识别技术的活动人士建立了一份档案，揭露了一家大公司对监控技术的严重滥用。 这一事件凸显了人脸识别技术可能被用来对付批评者，引发了关于隐私、企业权力以及监控技术伦理边界的紧迫问题。 该档案包含了律师和活动人士的信息，MSG 自 2018 年起使用人脸识别技术阻止任何与公司有诉讼关联的人入场，即便当事人并未亲自参与诉讼。

hackernews · cdrnsf · Jun 23, 13:36 · [社区讨论](https://news.ycombinator.com/item?id=48644781)

**背景**: 人脸识别是一种通过分析面部特征来识别个人的生物识别技术。MSG 部署该技术以执行一项禁止与公司存在法律纠纷人员入场的政策，但批评者认为这导致了无节制的监控和对异议的报复。

**社区讨论**: 评论强调了关于人脸识别的更广泛担忧，一些人认为技术本身不是问题，而是谁控制它以及透明度如何。其他评论链接了关于 MSG 监控实践和数据泄露的进一步报道。

**标签**: `#facial recognition`, `#privacy`, `#surveillance`, `#ethics`, `#corporate abuse`

---

<a id="item-9"></a>
## [近半数 LG 智能电视应用含住宅代理 SDK](https://spur.us/blog/smart-tv-apps-residential-proxy-sdks) ⭐️ 8.0/10

一项针对 6038 款 LG 和三星智能电视应用的扫描发现，2058 款应用含有住宅代理 SDK，其中 LG 平台受影响比例接近一半。这些 SDK 可在用户不知情的情况下将家庭网络转化为代理端点。 这暴露了影响数百万智能电视设备的重大隐私和安全漏洞，可能导致僵尸网络滥用和未经授权的 IP 使用。亚马逊和 Roku 已采取行动，给 LG 和三星带来应对压力。 受影响的应用包括屏保、时钟和小游戏，部分应用在用户关闭后仍可继续运行代理功能。亚马逊已禁止电视应用提供第三方代理服务，Roku 也已封堵类似 SDK，但 LG 和三星尚未发布同等限制。

telegram · zaihuapd · Jun 23, 02:26

**背景**: 住宅代理 SDK 是一种软件开发工具包，能将网络代理功能嵌入应用中，允许设备通过用户的家庭 IP 地址转发第三方流量。这类 SDK 通常用于网络爬虫或广告验证，其工作原理是将用户设备变成住宅代理网络的节点。与数据中心代理不同，住宅代理使用 ISP 分配的真实 IP，更难被检测。这项研究凸显了智能电视——作为常开且用户监督有限的设备——已成为此类隐蔽代理网络的目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.secrss.com/articles/91102">智能电视正在成为全球AI数据爬虫的住宅代理节点 - 安全内参 | 决策者的网络安全知识库</a></li>
<li><a href="https://blog.csdn.net/candice931020/article/details/127961172">住宅代理详细介绍——助您快速入门！_oxylabs 住宅代理 使用-CSDN博客</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#IoT`, `#smart TV`, `#residential proxy`

---

<a id="item-10"></a>
## [美国人形机器人依赖中国零部件](https://t.me/zaihuapd/42129) ⭐️ 8.0/10

《华尔街日报》报道称，美国人形机器人在关键机体零部件（如电机、关节、磁体和传感器）上越来越依赖中国供应链。迪士尼的“奥拉夫”机器人使用了中国宇树科技的部件，特斯拉也正与中国供应商合作推进 Optimus 的量产准备。 这种依赖暴露了美国机器人产业的战略风险——中国主导供应链并具备成本优势，最多可将制造成本压低三分之二。这也凸显了政策干预的必要性，美国国会议员已提出法案，拟评估美国机器人竞争力及供应链风险。 2025 年，中国推出了 28 款人形机器人，数量接近美国企业的 3 倍。摩根士丹利估算，中国供应链最多可将人形机器人制造成本压低三分之二。

telegram · zaihuapd · Jun 23, 07:47

**背景**: 人形机器人旨在模仿人类外观和动作，需要电机、关节、磁体和传感器等复杂零部件。中国宇树科技成立于 2016 年，最初专注于四足机器人，2024 年进入人形机器人领域，提供高性价比的部件。随着机器人产业成为战略行业，美国对供应链依赖中国感到担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics</a></li>
<li><a href="https://grokipedia.com/page/unitree_robotics">Unitree Robotics</a></li>

</ul>
</details>

**标签**: `#humanoid robotics`, `#supply chain`, `#US-China competition`, `#robot manufacturing`, `#technology dependency`

---

<a id="item-11"></a>
## [三星发布 UFS 5.0，带宽 10.8 GB/s 面向端侧 AI](https://news.samsung.com/global/samsung-unveils-industrys-fastest-ufs-5-0-solution-for-next-gen-on-device-ai-applications) ⭐️ 8.0/10

三星电子宣布开发出 UFS 5.0 闪存存储，号称业界最快的 UFS 产品，顺序读取速度最高 10.8 GB/s，顺序写入速度最高 9.5 GB/s，基于最新的 JEDEC 标准，计划今年第四季度量产。 这一显著的性能和能效提升将直接惠及旗舰手机、XR 头显和 AI 可穿戴设备中的下一代端侧 AI 应用，实现更快的数据处理和更低的功耗。它为嵌入式存储设定了新的性能标杆，加速了支持 AI 的移动生态系统发展。 UFS 5.0 的顺序读取速度较 UFS 4.1 提升一倍，功耗效率提升超过 40%，封装尺寸缩小 16.7%。最大容量可达 1 TB，符合最新 JEDEC 嵌入式存储接口标准。

telegram · zaihuapd · Jun 23, 09:17

**背景**: UFS（通用闪存存储）是移动设备中常用的高性能存储标准，比 eMMC 提供更快的数据传输速度。端侧 AI 需要快速访问大模型和数据，因此存储带宽至关重要。三星 UFS 5.0 旨在以前所未有的读写速度和能效满足这些需求。

**标签**: `#storage`, `#AI`, `#hardware`, `#mobile`, `#Samsung`

---

<a id="item-12"></a>
## [SpaceX 猎鹰重型火箭将于 2028 年发射欧洲罗莎琳德·富兰克林火星车](https://t.me/zaihuapd/42133) ⭐️ 8.0/10

美国宇航局确认，SpaceX 的猎鹰重型火箭将于 2028 年底发射欧洲航天局的罗莎琳德·富兰克林火星车，结束了长达 20 多年的延误，为任务提供了明确的前进方向。 SpaceX、NASA 和 ESA 之间的合作标志着火星探索的一个重要里程碑，罗莎琳德·富兰克林火星车旨在寻找火星地表下可能存在的过去生命迹象。该任务在地缘政治紧张导致挫折后的复兴，展示了国际合作在太空探索中的重要性。 猎鹰重型火箭将于 2028 年底从佛罗里达州肯尼迪航天中心发射。NASA 将提供关键硬件支持，包括发射服务，可能还包括额外仪器，而 ESA 则继续开发火星车和着陆平台。

telegram · zaihuapd · Jun 23, 10:47

**背景**: 罗莎琳德·富兰克林火星车是 ExoMars 计划的一部分，这是 ESA 的一项天体生物学计划，最初计划与俄罗斯联邦航天局合作。在 2022 年俄罗斯入侵乌克兰后，ESA 暂停了合作并寻求新伙伴。2024 年 4 月，该任务获得资金重启，改用欧洲着陆平台，NASA 同意提供发射服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ExoMars_Programme">ExoMars Programme</a></li>

</ul>
</details>

**标签**: `#space exploration`, `#SpaceX`, `#Mars rover`, `#NASA`, `#ESA`

---

<a id="item-13"></a>
## [FFmpeg 严重漏洞可致远程代码执行](https://cybernews.com/security/critical-ffmpeg-vulnerability-enables-complete-compromise/) ⭐️ 8.0/10

FFmpeg 的 MagicYUV 解码器中被发现存在一个严重的远程代码执行漏洞（CVE-2026-8461，CVSS 8.8），攻击者通过播放或存储恶意视频文件即可完全控制系统。FFmpeg 已发布 8.1.2 版本进行修复。 该漏洞影响众多使用 FFmpeg 的应用，包括 VLC、Jellyfin、Kodi 以及许多物联网设备，具有高影响力。用户应尽快更新以防止潜在利用。 该漏洞位于 MagicYUV 解码器，CVSS 评分为 8.8。即使在服务器、NAS 和智能电视上自动生成缩略图或媒体库扫描也可能触发。如果不需要 MagicYUV 解码器，可在编译时禁用它。

telegram · zaihuapd · Jun 23, 15:00

**背景**: FFmpeg 是一个广泛使用的开源多媒体库，为许多媒体应用和设备提供音频视频的编解码和流媒体功能。MagicYUV 解码器用于解码特定的无损视频编码格式。此类核心组件的漏洞可能导致严重的安全问题。

**标签**: `#FFmpeg`, `#security`, `#vulnerability`, `#CVE`, `#critical`

---

<a id="item-14"></a>
## [研究发现随机洗牌需 14 次才能充分随机化](https://www.quantamagazine.org/seven-perfect-shuffles-randomize-a-deck-of-cards-but-how-many-sloppy-ones-20260617/) ⭐️ 8.0/10

一项新研究发现，普通人随机洗牌（不精准鸽尾式）大约需要 14 次才能将一副 52 张牌充分随机化，是 1992 年经典结论（7 次）的两倍。 该研究将经典洗牌理论扩展到更现实的场景，为不精准混合下的随机化动力学提供了新的数学洞察。 研究团队为每张牌分配二进制'条形码'，追踪其在左右牌堆间的跳跃路径，并发现残留有序的'冷点'区域，证明了不精准洗牌也存在'截止现象'。不过，当前模型仍假设牌是一张张交错落下，而非成沓掉落。

telegram · zaihuapd · Jun 23, 16:04

**背景**: 1992 年，数学家证明七次完美的鸽尾式洗牌（每次将牌组精准对半分并完美交错）足以随机化一副牌。该结论假设接近魔术师水平的洗牌。新研究放宽了这一假设，以反映大多数人的实际洗牌方式，因此所需次数更高。

**标签**: `#数学`, `#概率论`, `#随机化`, `#洗牌算法`

---

<a id="item-15"></a>
## [Swift Package Index 加入苹果](https://swiftpackageindex.com/blog/swift-package-index-joins-apple) ⭐️ 7.0/10

Swift Package Index（SPI），一个社区构建的 Swift 包发现工具，已被苹果收购，其团队将加入苹果共同改进 Swift 生态系统。 此次收购标志着苹果对 Swift 包生态系统的更深投入，可能带来更紧密的 Xcode 集成和更好的工具支持，但也引发了对苹果监管下集中控制和开放性的担忧。 SPI 博客宣布了此举，未来计划包括开发者身份功能，一些社区成员担心这可能引入障碍或限制包索引。

hackernews · JDevlieghere · Jun 23, 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48648779)

**背景**: Swift Package Index 是一个帮助开发者发现与 Swift Package Manager (SPM) 兼容的 Swift 包的流行网站。它由社区成员创建，以弥补缺少中央包注册中心的空缺。苹果也运营着自己的 Swift Package Registry，这导致了一些混淆。

**社区讨论**: 社区反应不一：有人为团队的成功感到高兴，也有人担心苹果在开源和开发者服务方面的过往表现。一位评论者计划构建一个竞争对手，因为 SPI 目前仅支持 GitHub 仓库的限制。

**标签**: `#Swift`, `#Package Manager`, `#Apple`, `#Open Source`, `#Ecosystem`

---

<a id="item-16"></a>
## [TikZ 编辑器：LaTeX 图形的所见即所得工具](https://tikz.dev/editor/) ⭐️ 7.0/10

一款开源的所见即所得 TikZ 编辑器发布，允许用户通过拖拽和调整元素大小来可视化编辑，同时实时同步源代码和渲染图形。 该工具解决了 LaTeX 用户通常手动编写图形代码的主要痛点，可能节省时间并减少学术出版和技术文档中的错误。 该编辑器通过解析 TikZ 代码并跟踪源位置来实现精确的坐标覆盖；它主要使用 Codex 编码代理构建，并包含从 SVG、PPTX 和 IPE 格式转换的功能。

hackernews · DominikPeters · Jun 23, 14:24 · [社区讨论](https://news.ycombinator.com/item?id=48645437)

**背景**: TikZ 是一个强大的 LaTeX 包，用于通过文本命令创建矢量图形，但需要手动调整坐标和重新编译。虽然存在其他编辑 LaTeX 图形的工具，但很少有提供同时编辑源代码的所见即所得模式。

**社区讨论**: 评论者称赞了用户界面和概念，但批评生成的代码不必要地使用了绝对坐标。一些人建议使用 Quiver 等替代工具用于特定场景。

**标签**: `#LaTeX`, `#TikZ`, `#WYSIWYG`, `#open-source`, `#academic publishing`

---

<a id="item-17"></a>
## [F3：内嵌 WASM 解码器的列式存储新格式](https://github.com/future-file-format/f3) ⭐️ 7.0/10

F3 是一种新型列式存储格式，在每个文件中嵌入 WebAssembly（Wasm）二进制解码器，旨在解决 Apache Parquet 在跨平台兼容性等方面的局限。 通过嵌入解码器，F3 承诺无需依赖特定平台的 SDK 即可实现通用兼容性，有望减少数据交换的摩擦。然而，由于面临 Parquet 等成熟格式的竞争以及当前文档缺口，其采纳面临重大挑战。 每个 F3 文件包含数据、元数据和用于解码数据的 Wasm 二进制文件（仅几 KB），实现了自描述性。该格式通过 Flatbuffers 描述，源代码可在 GitHub 上获取。

hackernews · tosh · Jun 23, 16:53 · [社区讨论](https://news.ycombinator.com/item?id=48647799)

**背景**: 像 Parquet 这样的列式存储格式按列组织数据，而非按行，从而能够为分析型工作负载提供高效的压缩和查询性能。Parquet 已成为大数据生态系统的事实标准，但其依赖特定平台的解码器限制了跨平台使用。F3 试图通过嵌入 Wasm 解码器来解决这一问题，Wasm 解码器可在任何支持 Wasm 运行时的系统上运行。

**社区讨论**: 社区评论褒贬不一：有人称赞嵌入 Wasm 解码器的想法'相当天才'，因为它提供了回退兼容性；也有人批评文档不足，并质疑 F3 如何超越 Parquet 广泛工具支持的优势。由于 Parquet 的网络效应，对 F3 的采纳存在怀疑。

**标签**: `#data-storage`, `#columnar-format`, `#parquet`, `#wasm`, `#file-format`

---

<a id="item-18"></a>
## [巨型卡车和 SUV 的致命崛起](https://www.nytimes.com/interactive/2026/06/21/us/trucks-suv-pedestrian-crashes.html) ⭐️ 7.0/10

《纽约时报》的一项调查显示，美国卡车和 SUV 车型尺寸的增大与 2009 年以来行人死亡人数的上升直接相关。 这一趋势构成了严重的公共安全威胁，对行人和骑行者影响尤为严重，凸显了加强车辆设计监管和政策改革的必要性。 文章指出，自 2009 年以来，美国行人死亡人数增加了约 75%，这与市场向大型车辆转变的趋势一致。社区评论还就智能手机分心作为替代解释展开了讨论。

hackernews · xnx · Jun 21, 22:42 · [社区讨论](https://news.ycombinator.com/item?id=48623347)

**背景**: 大型卡车和 SUV 拥有更高的前端和较钝的形状，在碰撞中会造成更严重的伤害。尽管其他国家也出现了车辆尺寸增大的趋势，但它们通过更好的基础设施和更严格的监管减少了行人死亡，这与美国的情况形成了对比。

**社区讨论**: 评论者意见不一：一些人引用安全数据，呼吁立即对车辆尺寸进行监管；另一些人则认为驾驶员行为或智能手机使用是更重要的因素。与国际数据的比较显示出对主要原因的分歧。

**标签**: `#pedestrian safety`, `#vehicle design`, `#SUVs`, `#traffic policy`, `#public health`

---

<a id="item-19"></a>
## [OpenAI 推出 AI 动画电影《Critterz》，成本低于 3000 万美元](https://t.me/zaihuapd/42125) ⭐️ 7.0/10

OpenAI 正在支持制作一部名为《Critterz》的动画长片，主要使用包括 GPT-5 在内的自家 AI 工具完成，预算不到 3000 万美元，制作周期仅为 9 个月。 该项目展示了 AI 大幅降低动画电影制作成本与时间的潜力，可能颠覆传统动画产业，并彰显 OpenAI 在创意领域的实力。 该片计划在戛纳电影节首映，并于 2026 年在全球影院上映；其预算和制作周期远低于传统动画电影，后者通常预算超 1 亿美元、耗时数年。

telegram · zaihuapd · Jun 23, 03:11

**背景**: 传统动画电影（如迪士尼或皮克斯作品）通常耗资 1.5 亿至 2 亿美元，制作周期 4-6 年。OpenAI 的《Critterz》旨在证明生成式 AI 可以处理从故事板到最终渲染的创意流程，利用 GPT-5 等模型进行剧本和视觉生成。

**标签**: `#OpenAI`, `#AI animation`, `#film production`, `#GPT-5`, `#technology demonstration`

---