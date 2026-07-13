---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> From 14 items, 9 important content pieces were selected

---

1. [三星将删除不同意 AI 训练的健康数据](#item-1) ⭐️ 8.0/10
2. [苹果 SpeechAnalyzer vs Whisper：速度更快，准确率略低](#item-2) ⭐️ 8.0/10
3. [前沿 LLM 的真实成本：Token 价格对比](#item-3) ⭐️ 8.0/10
4. [Climate.gov 被毁，开放数据拯救了它](#item-4) ⭐️ 8.0/10
5. [Sega CD 游戏 Silpheed 的艺术与工程](#item-5) ⭐️ 8.0/10
6. [洛杉矶警察局因隐私顾虑终止与 Flock 的监控合同](#item-6) ⭐️ 8.0/10
7. [Telegram 的 t.me 域名被注册商暂停](#item-7) ⭐️ 7.0/10
8. [无需打开 Xcode 即可构建和发布 Mac/iOS 应用](#item-8) ⭐️ 7.0/10
9. [DOM-docx: 将 HTML 转换为原生可编辑 Word 文档的高保真库](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [三星将删除不同意 AI 训练的健康数据](https://neow.in/cWsyMTV3) ⭐️ 8.0/10

三星宣布，如果用户不同意将其健康数据用于 AI 训练，公司将删除这些数据，这实质上使得未经同意就无法使用某些设备功能。 该政策引发了严重的隐私担忧，它迫使用户要么失去自己的健康数据，要么允许三星将其用于 AI 训练，可能为其他公司树立先例。 该政策涵盖四类数据：睡眠、药物、医疗记录和周期跟踪详情。拒绝同意的用户的数据将被删除，并可能失去相关功能的访问权限。

hackernews · bundie · Jul 13, 20:01 · [社区讨论](https://news.ycombinator.com/item?id=48897991)

**背景**: 三星的健康设备和软件，例如 Galaxy Watch 和 Samsung Health 应用，会收集敏感的健康数据。AI 训练这类数据可以改善功能，但也带来隐私风险。欧洲的 GDPR 等法规可能影响该政策的可执行性。

**社区讨论**: 评论者表达了不满，其中一位用户质疑是否会提供部分退款，因为功能变得无法使用。另一位指出声称尊重隐私却强迫同意的讽刺之处，还有一位提到了谷歌的类似做法。一些人认为数据删除防止了滥用，也有积极的一面。

**标签**: `#privacy`, `#data policy`, `#Samsung`, `#AI training`, `#health data`

---

<a id="item-2"></a>
## [苹果 SpeechAnalyzer vs Whisper：速度更快，准确率略低](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 8.0/10

Inscribe 发布的一项新基准测试将苹果的 SpeechAnalyzer API 与 OpenAI 的 Whisper 及苹果旧版 SFSpeechRecognizer 进行了对比，结果显示 SpeechAnalyzer 比 Whisper Small 快三倍，在 LibriSpeech 上更准确，但在某些使用场景（如数学讲座）中略逊一筹。 这项基准测试意义重大，因为它表明苹果的设备端语音识别现已能与云端模型竞争，可能颠覆依赖 Whisper 的第三方转录应用，同时提供更好的隐私保护和离线能力。 SpeechAnalyzer 的运行速度大约是 Whisper Small 的三倍，在 LibriSpeech 的干净和噪声部分均优于所有 Whisper 模型，但旧版 SFSpeechRecognizer 甚至落后于 Whisper Tiny。SpeechAnalyzer API 完全离线、模块化，并在 iOS 26 中引入。

hackernews · get-inscribe · Jul 13, 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48894752)

**背景**: 苹果的 SpeechAnalyzer 是一个新的设备端语音识别 API，取代了旧版 SFSpeechRecognizer，专为性能和离线运行而设计。OpenAI 的 Whisper 是一个广泛使用的开源语音识别模型，有多种尺寸（tiny、base、small 等）。Inscribe 的基准测试在标准数据集上对它们进行了对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://get-inscribe.com/blog/apple-speech-api-benchmark.html">Apple's New Speech API vs Whisper: The First Real Benchmark</a></li>
<li><a href="https://developer.apple.com/documentation/speech/speechanalyzer">SpeechAnalyzer | Apple Developer Documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Whisper_(speech_recognition_system)">Whisper (speech recognition system) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Whisper 已经过时，并建议使用更好的模型，如 Nvidia 的 Nemotron 和 Parakeet，或 Mistral 的 Voxtral。一些人称赞 SpeechAnalyzer 的速度，但表示在其使用场景中仅略逊一筹。另一些人预测苹果的原生集成可能会消灭那些仅包装 Whisper 的付费应用。

**标签**: `#Apple`, `#speech recognition`, `#benchmarking`, `#Whisper`, `#API`

---

<a id="item-3"></a>
## [前沿 LLM 的真实成本：Token 价格对比](https://playcode.io/blog/real-price-of-frontier-models) ⭐️ 8.0/10

一项实际分析揭示了 OpenAI 的 GPT-4o 和 Anthropic 的 Claude 等前沿 LLM 在考虑分词器效率后，实际 Token 价格存在显著差异。 这很重要，因为依赖 LLM 的开发者或企业若使用低效分词器，可能面临意外高昂的成本，从而影响预算和模型选择。 OpenAI 的 o200k 分词器在代码和文本处理上比 Anthropic 的当前分词器高效约 1.6 至 2 倍，从而降低了每 Token 的实际成本。

hackernews · ianberdin · Jul 13, 18:32 · [社区讨论](https://news.ycombinator.com/item?id=48896800)

**背景**: 前沿模型是最先进的 AI 系统，如 GPT-4 和 Claude，训练成本高昂。分词器将文本转换为 Token；更高效的分词器意味着每个输入使用更少的 Token，从而降低成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Frontier_model">Frontier model</a></li>
<li><a href="https://www.linkedin.com/pulse/deep-dive-tokenizer-performance-prashant-lakhera-sqz5c">A Deep Dive into Tokenizer Performance - LinkedIn</a></li>
<li><a href="https://llm-calculator.com/blog/tokenization-performance-benchmark/">Tokenization Speed and Efficiency Benchmarks (July 2025)</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 OpenAI 的分词器文档和效率优于 Anthropic，一些用户分享了测试结果，显示 GPT 在代码处理上使用更少 Token。还有人讨论了缓存成本和输出 Token 定价的假象。

**标签**: `#LLM`, `#pricing`, `#tokenizer`, `#OpenAI`, `#Anthropic`

---

<a id="item-4"></a>
## [Climate.gov 被毁，开放数据拯救了它](https://werd.io/climate-gov-was-destroyed-open-data-saved-it/) ⭐️ 8.0/10

Climate.gov 网站被毁，但开放数据倡议和社区努力成功保存并归档了其气候数据，确保公众能继续访问。 这一事件凸显了集中式政府数据存储库的脆弱性，以及去中心化开放数据在保护公共信息（尤其是气候科学和政策方面）中的关键作用。 数据救援依赖志愿者和开放数据存储库（如 Data.gov）以及去中心化归档工具（如 IPFS），但可持续性仍令人担忧，因为工作依赖捐款而非稳定的政府资金。

hackernews · benwerd · Jul 13, 19:57 · [社区讨论](https://news.ycombinator.com/item?id=48897945)

**背景**: 开放数据指的是任何人都可以自由访问、使用和共享的数据。像 NOAA 这样的政府机构运营 climate.gov 以提供公共气候数据。然而，集中式网站可能面临删除、篡改或资金削减的风险。去中心化归档，例如使用 IPFS（星际文件系统），将数据分布到多个节点，从而抵抗单点故障。数据救援项目（Data Rescue Project）等倡议已成立，系统地备份高风险公共数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datarescueproject.org/">Data Rescue Project</a></li>
<li><a href="https://data.gov/">Data.gov Home - Data.gov</a></li>
<li><a href="https://www.kyve.network/">KYVE Network | Decentralized Data Lake for Reliable Insights</a></li>

</ul>
</details>

**社区讨论**: 评论者感谢数据被保存，但表达了对长期可持续性和依赖捐款的担忧。有人建议将 IPFS 作为政府静态内容的默认发布方式，而其他人则质疑可行性以及纳税人在资助此类工作中的角色。

**标签**: `#open data`, `#climate`, `#government`, `#archival`, `#data preservation`

---

<a id="item-5"></a>
## [Sega CD 游戏 Silpheed 的艺术与工程](https://fabiensanglard.net/silpheed/index.html) ⭐️ 8.0/10

Fabien Sanglard 发布了对 Sega CD 游戏《Silpheed》的深入技术分析，解释了如何通过巧妙的工程在有限硬件上实现令人印象深刻的全动态视频和伪 3D 图形。 这一分析凸显了复古游戏开发者的巧思，为理解 Sega CD 时代的技术限制和创造性解决方案提供了宝贵见解。 文章详细说明了《Silpheed》如何利用精灵缩放、调色板操作和精心预渲染的 FMV 序列来模拟 3D 视觉效果。Sega CD 没有 3D 渲染硬件，所有效果都是通过其 2D 能力和 CD 的额外带宽实现的。

hackernews · ibobev · Jul 13, 14:52 · [社区讨论](https://news.ycombinator.com/item?id=48893639)

**背景**: 伪 3D 渲染技术（如光线投射和精灵缩放）在 16 位时代很常见，用于在 2D 硬件上创造深度 illusion。Sega CD 是 Sega Genesis 的附加组件，提供了 CD-ROM 存储和额外的处理能力，但仍依赖 Genesis 的 2D 图形能力。开发者往往需要创新，以在这些限制下提供视觉效果令人印象深刻的游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2.5D">2.5D - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sega_CD">Sega CD - Wikipedia</a></li>
<li><a href="https://www.extentofthejam.com/pseudo/">Lou's Pseudo 3D Page</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了这篇文章并分享了怀旧体验，其中一位指出《Silpheed》感觉就像在控制一部电影。另一位提到了 Mega Drive 演示场景作品《Overdrive 2》作为类似硬件实力的例子。有人对 Sega CD 的声音设置提出了修正，澄清说 Mega Drive 的扩展端口可以混合音频，无需单独的连接线。

**标签**: `#retro gaming`, `#game development`, `#Sega CD`, `#FMV`, `#technical deep-dive`

---

<a id="item-6"></a>
## [洛杉矶警察局因隐私顾虑终止与 Flock 的监控合同](https://techcrunch.com/2026/07/13/lapd-lets-contract-with-surveillance-giant-flock-expire-citing-serious-concerns-over-civil-liberties-and-privacy/) ⭐️ 8.0/10

洛杉矶警察局（LAPD）允许与监控公司 Flock Safety 的合同到期，理由是对公民自由和隐私的严重担忧。 一个主要警察部门的这一决定凸显了执法监控与公民权利之间日益紧张的关系，可能影响其他机构以及关于数据隐私的公共政策辩论。 尽管合同到期，但 Flock 拥有摄像头和立杆，这意味着摄像头继续运行并收集数据，Flock 可以将其出售给其他机构，LAPD 仍可通过其他方式访问这些数据。

hackernews · forks · Jul 13, 15:11 · [社区讨论](https://news.ycombinator.com/item?id=48893947)

**背景**: Flock Safety 是一家向执法部门和社区提供自动车牌识别（ALPR）摄像头和监控系统的公司。这些摄像头捕捉车辆图像，将车牌数据转换为可搜索信息，由于大规模数据收集和潜在滥用，常常引发隐私担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://www.aclu.org/news/privacy-technology/flock-roundup">Flock’s Aggressive Expansions Go Far Beyond Simple Driver Surveillance | American Civil Liberties Union</a></li>

</ul>
</details>

**社区讨论**: 社区评论表示怀疑，指出 Flock 设计的系统能够抵御政治压力；即使没有合同，摄像头仍继续记录，数据仍可访问。一些人认为，政府购买自己无法合法收集的数据应属非法。

**标签**: `#surveillance`, `#privacy`, `#civil liberties`, `#LAPD`, `#Flock`

---

<a id="item-7"></a>
## [Telegram 的 t.me 域名被注册商暂停](https://www.whois.com/whois/t.me) ⭐️ 7.0/10

Telegram 使用的域名 t.me（用于其 URL 短链接服务）已被注册商 GoDaddy 暂停，WHOIS 状态码如 clientRenewProhibited 显示涉及法律纠纷。 这次暂停影响了数百万依赖 t.me 链接的用户和频道，并凸显了集中式域名服务在面对不同国家法律行动时的脆弱性。 诸如 clientRenewProhibited 和 serverDeleteProhibited 这样的域名状态码并不常见，通常在法律纠纷或域名面临删除时启用。此次暂停可能与俄罗斯、法国和印度正在进行的法律调查有关。

hackernews · Tiberium · Jul 13, 19:52 · [社区讨论](https://news.ycombinator.com/item?id=48897878)

**背景**: 域名暂停发生在注册商或注册局因法律命令、滥用投诉或无法验证 WHOIS 信息而采取行动时。GoDaddy 是最大的域名注册商之一，以严格执行此类政策而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48897878">Telegram's t . me domain has been suspended | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区成员对 Telegram 依赖 GoDaddy 表示惊讶，因为后者以缺乏透明度著称。一些人讨论了使用重定向或替代域名等变通方法，而另一些人则认为这验证了他们将社区迁离 Telegram 的决定。

**标签**: `#Telegram`, `#domain suspension`, `#DNS`, `#internet governance`, `#security`

---

<a id="item-8"></a>
## [无需打开 Xcode 即可构建和发布 Mac/iOS 应用](https://scottwillsey.com/building-and-shipping-mac-and-ios-apps-without-ever-opening-xcode/) ⭐️ 7.0/10

一位开发者发布了一份详细指南，展示了如何完全使用命令行工具（如 xcodebuild、notarytool 和 altool）并借助 AI 助手 Claude Code 来构建、签名、公证和发布 Mac 和 iOS 应用。 这展示了一种替代工作流程，减少了对 Xcode 图形界面的依赖，实现了自动化、CI/CD 集成，并为 Apple 平台开发者提供了更轻量的开发环境。 该工作流依赖 Apple 的命令行工具（xcodebuild、notarytool、altool），并可由 Claude 等大语言模型编排。社区成员还提到了 xtool、Sweetpad CLI 和 Axiom 等补充项目，进一步简化了这一流程。

hackernews · speckx · Jul 13, 18:22 · [社区讨论](https://news.ycombinator.com/item?id=48896665)

**背景**: Xcode 是 Apple 官方的集成开发环境（IDE），用于在 macOS 和 iOS 上创建应用。但 Apple 也提供了一套命令行工具（如 xcodebuild、notarytool、altool），允许开发者无需图形界面即可构建、签名、公证和上传应用。这些工具通常用于持续集成（CI）流水线中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/library/archive/technotes/tn2339/_index.html">Technical Note TN2339: Building from the Command Line with ...</a></li>
<li><a href="https://developer.apple.com/documentation/xcode/installing-the-command-line-tools">Installing the command-line tools - Apple Developer</a></li>
<li><a href="https://stackoverflow.com/questions/56436345/how-to-upload-to-app-store-from-command-line-with-xcode-11">ios - How to upload to App Store from command line... - Stack Overflow</a></li>

</ul>
</details>

**社区讨论**: 讨论总体积极，一些人指出这种方法在 CI 构建中是标准的，但作为主要工作流程则较为新颖。多位评论者分享了替代工具，如 xtool（用于 Linux 上的 iOS 开发）和 Sweetpad CLI（面向 VSCode 的封装）。还提到了 Axiom，该项目提供了适合大语言模型的 Apple 开发工具。

**标签**: `#Apple development`, `#Xcode alternatives`, `#iOS development`, `#command-line tools`, `#LLM assistance`

---

<a id="item-9"></a>
## [DOM-docx: 将 HTML 转换为原生可编辑 Word 文档的高保真库](https://github.com/floodtide/dom-docx) ⭐️ 7.0/10

DOM-docx 是一个新的开源 TypeScript 库，能够将 HTML 转换为高保真的原生可编辑 Word 文档，已在 GitHub 上以 MIT 许可证发布。 该库解决了文档生成中的常见痛点，生成真正可编辑的 DOCX 输出，不同于现有方案常产生的无效或不可编辑文件。它使开发者能够使用 Vue 或 React 等 Web 技术编写文档模板，从而简化工作流程。 该库采用视觉回归循环，先在 Chromium 中渲染 HTML，再转换为 docx，确保布局保真度。它支持段落、列表、表格和链接，这些元素在 Microsoft Word 中仍然可编辑。

hackernews · fishbone · Jul 13, 11:51 · [社区讨论](https://news.ycombinator.com/item?id=48891267)

**背景**: 原生 Word 文档（DOCX）基于 Office Open XML (OOXML) 标准，该标准复杂且难以从 HTML 正确生成。许多现有的 HTML 转 docx 库生成扁平、不可编辑的输出，因为它们没有将 HTML 语义正确映射到 OOXML 结构。DOM-docx 旨在通过将语义 HTML 直接映射为真实的 Word 可编辑构造来弥合这一差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dom-docx.com/">dom - docx — HTML to Word converter in the browser</a></li>
<li><a href="https://github.com/dom-docx/dom-docx">GitHub - dom - docx / dom - docx : Convert semantic HTML fragments to...</a></li>

</ul>
</details>

**社区讨论**: 作者分享说后端 docx 生成是一个常见痛点，现有库会产生无效的可编辑结构。评论者赞赏其 TypeScript 实现，计划用于生成简历，并注意到巧妙的基于截图的验证循环。

**标签**: `#open-source`, `#document-generation`, `#typescript`, `#html-to-docx`, `#javascript`

---