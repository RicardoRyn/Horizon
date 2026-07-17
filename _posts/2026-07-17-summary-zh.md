---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> From 36 items, 17 important content pieces were selected

---

1. [台积电再投千亿美元赴美 Q2 利润飙升 77%](#item-1) ⭐️ 9.0/10
2. [AWS 计费错误显示 17 亿美元预估账单](#item-2) ⭐️ 8.0/10
3. [SQLite 技巧：.expert 模式与备份策略](#item-3) ⭐️ 8.0/10
4. [通过鹈鹕骑自行车基准测试评估 Kimi K3](#item-4) ⭐️ 8.0/10
5. [开源 AI 现状：市场从封闭模型转向开放模型](#item-5) ⭐️ 8.0/10
6. [苹果向 OpenAI 前员工发送法律函件](#item-6) ⭐️ 8.0/10
7. [欧盟要求谷歌向对手开放 Android AI 助手权限](#item-7) ⭐️ 8.0/10
8. [Truth Social 将向华尔街出售特朗普帖子的快速访问权限](#item-8) ⭐️ 8.0/10
9. [特斯拉 Cybercab 在北美启动量产](#item-9) ⭐️ 8.0/10
10. [华为昇腾 950 超节点首发，算力达英伟达 NVL144 的 6.7 倍](#item-10) ⭐️ 8.0/10
11. [美议员要求封禁中国存储芯片并阻止进入盟友供应链](#item-11) ⭐️ 8.0/10
12. [应对问题的三种方式：否认、保留、委派](#item-12) ⭐️ 7.0/10
13. [哪个 Lisp？一篇比较 Lisp 方言的博客](#item-13) ⭐️ 7.0/10
14. [脑电图揭示大脑可同时处理两个语音流](#item-14) ⭐️ 7.0/10
15. [Pebble 发布 Index 智能戒指等重大更新](#item-15) ⭐️ 7.0/10
16. [1Password 推出 Claude 集成，AI 代登录但不接触密码](#item-16) ⭐️ 7.0/10
17. [OpenAI CFO 提出“每美元有用智能”指标](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [台积电再投千亿美元赴美 Q2 利润飙升 77%](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 9.0/10

台积电宣布将再向美国亚利桑那州投资 1000 亿美元，使在美总投资规模增至 2650 亿美元。同时，公司公布 2026 年第二季度净利润同比飙升 77%至 7066 亿新台币，创历史新高，主要受 AI 需求推动。 这一巨额投资表明台积电致力于在地缘政治紧张背景下实现制造地理多元化，并突显了 AI 对先进芯片的持续强劲需求。这可能重塑全球半导体供应链，并增强美国芯片自主能力。 台积电将 2026 年资本支出预测上调至 600 亿至 640 亿美元，并预计全年美元计价营收增长略超 40%。亚利桑那州目前已有 8 座工厂在建或规划中，未来可能再增 4 座。

telegram · zaihuapd · Jul 16, 12:29

**背景**: 台积电是全球最大的专业半导体代工厂，为苹果、英伟达和 AMD 等公司生产芯片。为满足激增的 AI 处理器需求并降低台湾集中制造的地缘政治风险，该公司一直在全球扩张。

**标签**: `#semiconductor`, `#TSMC`, `#AI`, `#manufacturing`, `#investment`

---

<a id="item-2"></a>
## [AWS 计费错误显示 17 亿美元预估账单](https://news.ycombinator.com/item?id=48945241) ⭐️ 8.0/10

AWS 计费单位计算错误导致正常用量的预估账单显示为 17 亿美元，许多用户看到天文数字般的费用。 此事件削弱了用户对 AWS 计费准确性的信任，并凸显了云计量系统中单位错误的严重性，可能引发恐慌和支持请求过载。 该错误源于混淆了千兆字节 (GB) 和字节，导致 10^9 倍的差异；AWS 在数小时内修复了问题并发布了致歉，但预估账单数据在一段时间内不准确。

hackernews · nprateem · Jul 17, 09:42

**背景**: AWS 根据来自各种服务的计量用量数据提供实时预估账单。计费系统将用量乘以单价来估算成本。单位计算错误，例如将字节解释为千兆字节或相反，可能导致巨大的账单差异。虽然罕见，但这种错误可能引起用户的极大恐慌。

**社区讨论**: 用户表达了震惊和沮丧，一些人分享了过去类似计费错误的经历。社区评论指出了单位错误（字节 vs 千兆字节），并称赞 AWS 快速修复，但对信任和准确性的担忧依然存在。

**标签**: `#AWS`, `#billing`, `#cloud`, `#incident`, `#bug`

---

<a id="item-3"></a>
## [SQLite 技巧：.expert 模式与备份策略](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 8.0/10

一篇博文分享了实用的 SQLite 技巧，包括用于索引推荐的 .expert 命令以及使用 .dump 配合 zstd 压缩的备份方法，评论者还补充了如 s3-credentials 等 AWS 备份凭据工具。 这些技巧帮助开发者更高效地优化 SQLite 查询和管理备份，减少了创建索引和保护云存储凭据等常见痛点。 SQLite CLI 中的 .expert 命令可以分析查询并建议索引，而 s3-credentials 工具能为特定 S3 存储桶生成限定范围的读写凭据。

hackernews · surprisetalk · Jul 17, 17:45 · [社区讨论](https://news.ycombinator.com/item?id=48950122)

**背景**: SQLite 是一个自包含、无服务器的数据库引擎，广泛应用于应用程序中。.expert 模式是 CLI 的一个功能，可根据查询分析推荐索引。s3-credentials 是 Simon Willison 开发的命令行工具，简化了创建仅限单个存储桶的 AWS 凭据的过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/cli.html">Command Line Shell For SQLite</a></li>
<li><a href="https://github.com/simonw/s3-credentials">GitHub - simonw/s3-credentials: A tool for creating credentials for accessing S3 buckets · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了 .expert 模式的实用性，并分享了自己使用 .dump 和 zstd 的备份脚本。有评论指出 sqlite_stat1 和 sqlite_stat4 为查询计划器提供了统计信息。

**标签**: `#SQLite`, `#database`, `#query optimization`, `#backup`, `#CLI`

---

<a id="item-4"></a>
## [通过鹈鹕骑自行车基准测试评估 Kimi K3](https://simonwillison.net/2026/Jul/16/kimi-k3/) ⭐️ 8.0/10

Simon Willison 使用其独创的鹈鹕骑自行车 SVG 基准测试评估了 Kimi K3（一个 2.8 万亿参数的开源模型），发现异常高的令牌计数，暗示存在 85 令牌的隐藏系统提示。 该基准测试提供了一种超越标准排行榜的比较模型质量、成本和速度的实用方法，而令牌化发现则凸显了隐藏提示如何模糊推理成本。 提示'Generate an SVG of a pelican riding a bicycle'在 Kimi K3 中消耗 95 个令牌，而 OpenAI 和 Anthropic 模型仅需 10 个，甚至单个'hi'也消耗 86 个令牌，这表明存在一个用于推理努力的隐藏系统提示。

hackernews · droidjj · Jul 17, 14:21 · [社区讨论](https://news.ycombinator.com/item?id=48947717)

**背景**: 鹈鹕骑自行车基准测试是 Simon Willison 创建的一个幽默但有效的测试，用于评估 LLM 生成鹈鹕骑自行车 SVG 的能力。Kimi K3 是一个 2.8 万亿参数的开源模型，于 2026 年 7 月由 Kimi 发布。令牌化是将文本拆分为子词单元的过程；不同模型使用不同的分词器，影响成本和延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2024/Oct/25/pelicans-on-a-bicycle/">Pelicans on a bicycle</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://benchlm.ai/blog/posts/llm-token-pricing">How LLM Token Pricing Works: A Complete Guide to API Costs in 2026 | BenchLM.ai</a></li>

</ul>
</details>

**社区讨论**: 社区成员讨论了鹈鹕图片是否在训练数据中，一位用户指出 Simon 自己的博客内容出现在模型中。另一位用户提供了成本速度比较，显示 Kimi K3 比 Opus 和 Fable 便宜 5 倍但慢 2 倍。还有人对如此大模型的推理硬件表示好奇。

**标签**: `#AI models`, `#benchmarking`, `#tokenization`, `#Kimi K3`, `#LLMs`

---

<a id="item-5"></a>
## [开源 AI 现状：市场从封闭模型转向开放模型](https://stateofopensource.ai/) ⭐️ 8.0/10

stateofopensource.ai 上的分析显示，开源 AI 模型在 OpenRouter 上的 Token 份额已从四个月前的 40%升至 63%，表明市场快速转变。 这一转变挑战了 OpenAI 和 Anthropic 等闭源 AI 领导者的主导地位，可能降低许可成本并实现 AI 访问民主化。开源模型的增长可能重塑竞争格局。 根据 OpenRouter 数据，开源模型最近一天处理了 4.19 万亿个 Token，与四个月前的 8880 亿个相比增长近 5 倍。但该报告的演示被批评为 AI 生成且缺乏深度。

hackernews · rellem · Jul 17, 14:31 · [社区讨论](https://news.ycombinator.com/item?id=48947825)

**背景**: 开源与闭源 AI 的争论焦点在于专有模型（如 GPT-4、Claude）还是公开可用的模型（如 Llama、Mistral）将占据主导地位。开源模型允许免费使用和修改，而闭源模型通常需要许可费。本报告基于 OpenRouter（一个将 API 调用路由到各种模型的服务）的 Token 使用数据分析了市场趋势。

**社区讨论**: 评论者意见不一：一些人认为数据证明了开源模型将超越闭源模型，可能扼杀 OpenAI 和 Anthropic 等公司。另一些人批评该报告的演示为 AI 生成且质量低下，削弱了其可信度。

**标签**: `#open source`, `#AI`, `#models`, `#machine learning`, `#community discussion`

---

<a id="item-6"></a>
## [苹果向 OpenAI 前员工发送法律函件](https://www.ft.com/content/1b8c9d52-88a9-426b-ba47-f1811f859166) ⭐️ 8.0/10

苹果已向数十名跳槽到 OpenAI 的前员工发出法律保留函件，暗示可能就商业秘密和人才挖角提起诉讼。 此举凸显了两大科技巨头在知识产权和人才流动问题上日益紧张的关系，可能为 AI 行业如何保护商业秘密树立先例。 文件保留函件是诉讼中的标准做法，但如果在提起诉讼前发送则可能被视为挑衅；苹果的时机表明它可能已掌握了商业秘密被滥用的证据。

hackernews · merksittich · Jul 17, 12:02 · [社区讨论](https://news.ycombinator.com/item?id=48946303)

**背景**: 苹果和 OpenAI 是 AI 领域的主要竞争对手，OpenAI 大量从苹果招聘。保留函件是诉讼前的证据保全步骤，常用于公司怀疑前员工将机密信息带到新雇主处时。

**社区讨论**: 评论意见不一：有人认为这些函件是标准做法，苹果可能已经晚了；另一些人则猜测苹果掌握了确凿证据，且 OpenAI 窃取内容的历史使指控可信。

**标签**: `#Apple`, `#OpenAI`, `#legal`, `#talent poaching`, `#tech industry`

---

<a id="item-7"></a>
## [欧盟要求谷歌向对手开放 Android AI 助手权限](https://t.me/zaihuapd/42615) ⭐️ 8.0/10

欧盟委员会根据《数字市场法案》发布了两项约束性命令，要求谷歌向 ChatGPT、Claude 等竞争对手的 AI 助手提供其仅限 Gemini 使用的系统级 Android 功能。这些要求仍处于草案阶段，可能会推迟。 这可能会显著增加 Android 设备上 AI 助手市场的竞争，为用户提供更多选择并推动创新。但谷歌警告称，开放系统权限可能危及用户安全和隐私。 这些命令特别针对系统级集成，例如访问通知、智能操作和文本选择等功能——这些功能目前仅限 Gemini 使用。谷歌还需要按监管条件与竞争对手分享匿名搜索数据。

telegram · zaihuapd · Jul 16, 13:19

**背景**: Android 是一个开源操作系统，但谷歌控制着核心系统服务和权限。《数字市场法案》（DMA）将谷歌指定为“守门人”，要求其公平开放平台功能。Android System Intelligence 提供智能回复、应用预测等 AI 驱动功能，谷歌一直将这些功能独家留给自己的 Gemini 助手以获得竞争优势。第三方助手目前缺乏同等级别的系统级接口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/320760/20260716/eu-gives-rival-ai-assistants-system-level-android-access-google-reserved-gemini.htm">EU Gives Rival AI Assistants System-Level Android Access Google ...</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-07-16/google-must-give-gemini-rivals-equal-access-to-android-system-eu-says">Google Must Give Gemini Rivals Equal Access to Android System, EU Says ...</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#Android`, `#AI assistants`, `#Google Gemini`, `#antitrust`

---

<a id="item-8"></a>
## [Truth Social 将向华尔街出售特朗普帖子的快速访问权限](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

Truth Social 的母公司 TMTG 于 2026 年 7 月 16 日宣布，将于 8 月 1 日起推出 Truth API，这是一项授权数据服务，以毫秒级速度向机构客户提供包括特朗普总统在内的平台前 10 名账号的实时帖子。 此举直接将总统的社交媒体活动货币化，服务于高频交易，可能导致市场信息不对称，并引发对模糊公务与商业界限的严重伦理担忧。 特朗普拥有约 1290 万粉丝的账号预计是主要吸引力；他关于关税和地缘政治事件的帖子曾引发股市和油市波动。TMTG 未披露定价。

telegram · zaihuapd · Jul 17, 01:02

**背景**: Truth Social 是特朗普媒体科技集团（TMTG）在特朗普被主要平台封禁后推出的社交媒体平台，已成为他发布政策声明的主要渠道。高频交易公司使用算法在毫秒内根据新闻进行交易，使得超快速访问特朗普帖子变得极具价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cointelegraph.com/news/trump-media-sells-wall-street-low-latency-access-to-trump-posts">Trump Media Launches Paid Feed for Market-Moving Trump Posts</a></li>
<li><a href="https://thehill.com/policy/technology/5972998-trump-media-technology-group-launch-truth-api/">Trump Media & Technology Group to launch Truth API to sell to ...</a></li>
<li><a href="https://markets.businessinsider.com/news/stocks/trump-media-and-technology-group-launches-truth-api-a-new-licensed-data-service-for-financial-services-partners-that-provides-the-fastest-access-to-truth-social-s-most-influential-accounts-1036332436">Trump Media and Technology Group Launches Truth API, a New ...</a></li>

</ul>
</details>

**标签**: `#Truth Social`, `#API`, `#高频交易`, `#数据货币化`, `#政治与金融`

---

<a id="item-9"></a>
## [特斯拉 Cybercab 在北美启动量产](https://t.me/zaihuapd/42621) ⭐️ 8.0/10

特斯拉宣布其无人驾驶电动车 Cybercab 已在北美启动量产。该车取消方向盘、踏板和后视镜，完全依靠人工智能进行自动驾驶。 这标志着特斯拉 Robotaxi 业务迈出了重要一步，因为 Cybercab 是主流汽车制造商中首款进入量产的专用自动驾驶车辆。其成功可能加速全球无人驾驶网约车服务的商业部署。 Cybercab 只有两个座位，专为自动驾驶设计，在完全自动驾驶（FSD）软件达到 L5 级别之前就已启动量产。特斯拉已在德克萨斯州奥斯汀开始测试没有方向盘和踏板的量产版本。

telegram · zaihuapd · Jul 17, 03:06

**背景**: Robotaxi（自动驾驶出租车）是指无需人类驾驶员、依靠 L4/L5 自动驾驶技术运营的出租车服务。特斯拉于 2024 年 10 月在“We, Robot”活动上展示了 Cybercab 概念车，当时 20 辆原型车在夜间提供了自动驾驶接驳。该车型是特斯拉推出商业 Robotaxi 网络的核心，但公司仍需证明其 FSD 软件能够可靠地应对无人监督驾驶。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Cybercab">Tesla Cybercab - Wikipedia</a></li>
<li><a href="https://electrek.co/2026/07/06/tesla-cybercab-production-before-autonomy/">Tesla Cybercab: mass-producing a car it can't sell or drive itself | Electrek</a></li>
<li><a href="https://techcrunch.com/2026/06/30/tesla-starts-testing-cybercab-without-pedals-or-a-steering-wheel-in-austin/">Tesla starts testing Cybercab without pedals or a steering wheel in Austin | TechCrunch</a></li>

</ul>
</details>

**标签**: `#特斯拉`, `#自动驾驶`, `#电动汽车`, `#Robotaxi`

---

<a id="item-10"></a>
## [华为昇腾 950 超节点首发，算力达英伟达 NVL144 的 6.7 倍](https://www.ithome.com/0/978/019.htm) ⭐️ 8.0/10

在 2026 世界人工智能大会上，华为首次公开展示了昇腾 950 超节点（Atlas 950 SuperPoD），声称其总算力达到英伟达 NVL144 系统的 6.7 倍，基于 1024 张昇腾 NPU 提供 1 EFLOPS FP8 和 2 EFLOPS FP4 算力。 这一发布标志着华为在 AI 算力领导地位上的重大进展，可能减少中国对英伟达硬件的依赖，并加剧全球 AI 基础设施竞争。如果 6.7 倍的性能差距得到验证，可能重塑大规模 AI 训练集群的采购决策。 昇腾 950 超节点采用华为自研的灵衢（UnifiedBus）互联协议和超节点架构，最多支持 1024 张 NPU，配备 256 TB 全局统一内存。此外，前代昇腾 384 超节点已商用落地 750 多套，广泛应用于互联网、运营商、金融等行业。

telegram · zaihuapd · Jul 17, 10:27

**背景**: 超节点架构通过高速互联将多个 AI 加速器整合为单一逻辑单元，实现大模型的高效扩展。华为的灵衢（UnifiedBus）协议是用五层协议栈替代 PCIe、NVLink 和 RDMA，支持 8192 卡无收敛全互联，这与英伟达基于 NVLink 的 NVL 系统（通常连接较少 GPU）形成对比。性能对比依据中银证券报告，尚未经独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.toutiao.com/article/7551352889764020755/">华为全联接大会 2025：发布灵衢互联协议与多系列超节点产品，引领 AI ...</a></li>
<li><a href="https://lucaberton.com/blog/huawei-atlas-950-superpod-ai-infrastructure/">Huawei Atlas 950 AI SuperPoD : 8,192 NPUs as One Machine</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#Huawei`, `#Ascend`, `#SuperNode`, `#compute`

---

<a id="item-11"></a>
## [美议员要求封禁中国存储芯片并阻止进入盟友供应链](https://www.tomshardware.com/pc-components/dram/lawmakers-want-us-government-to-ban-memory-chips-from-china-even-in-allied-supply-chains-citing-unacceptable-risk-to-national-economic-and-supply-chain-security) ⭐️ 8.0/10

美国众议员 John Moolenaar 与 George Whitesides 致信商务部长 Howard Lutnick，要求禁止美国公司采购中国存储芯片，并呼吁将长鑫存储（CXMT）列入实体清单，同时对长江存储（YMTC）施加额外限制。 此举可能重塑全球半导体供应链，切断中国存储芯片制造商进入美国及盟友市场的途径，可能增加 AI 基础设施和消费电子产品的成本，同时加剧中美技术紧张局势。 该信函明确针对长鑫存储（DRAM）和长江存储（NAND 闪存），称其与中国军方有关联，且采购可能资助军民两用技术。议员们还敦促与日本、韩国和欧盟协调，防止中国供应商在盟友供应链中扎根。

telegram · zaihuapd · Jul 17, 14:00

**背景**: 实体清单是美国商务部产业安全局公布的黑名单，列入该清单的实体需获得许可证才能购买美国技术。长鑫存储是中国 DRAM 制造商，长江存储专注于 NAND 闪存生产。这两家公司此前已受到美国出口管制，但这封信将限制范围扩大到盟友供应链。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Yangtze_Memory_Technologies">Yangtze Memory Technologies - Wikipedia</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/實體清單">实体清单 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**标签**: `#supply chain`, `#memory chips`, `#US-China tech war`, `#semiconductors`, `#policy`

---

<a id="item-12"></a>
## [应对问题的三种方式：否认、保留、委派](https://improvesomething.today/responses-to-problems/) ⭐️ 7.0/10

一篇文章概述了除解决问题之外的三种常见应对方式：否认问题的存在、保留问题以维持现状、以及把问题委派给他人。 这个框架有助于个人和组织识别解决问题时的非生产性模式，从而推动更有效的干预和系统性改进。 文章指出“保留问题”是一种尤为隐蔽的应对方式，利益相关者因问题的存在而受益，例如政府机构维持预算或专家巩固自身地位。

hackernews · surprisetalk · Jul 17, 14:00 · [社区讨论](https://news.ycombinator.com/item?id=48947490)

**背景**: 面对问题时，由于认知偏差、组织激励或权力动态，人们常常采取解决问题以外的应对方式。本文对三种此类应对进行了分类，借鉴系统思维和行为心理学，解释了为何问题尽管表面上有解决努力却持续存在。

**社区讨论**: 评论者普遍认同文章的观点，并提供了现实世界的例子：didgetmaster 指出政府因预算激励而保留犯罪、无家可归等问题；0wis 注意到公认的专家可能保持根本原因未解决以证明其角色合理性；rawgabbit 强调政治内斗导致局部优化；llm_nerd 将“保留问题”应用于软件开发中有利于开发者的低效问题。

**标签**: `#problem-solving`, `#organizational behavior`, `#cognitive biases`, `#systems thinking`

---

<a id="item-13"></a>
## [哪个 Lisp？一篇比较 Lisp 方言的博客](https://scotto.me/blog/2026-07-17-which-lisp/) ⭐️ 7.0/10

一篇博客文章比较了三种主要的 Lisp 方言——Common Lisp、Scheme 和 Clojure，突出了它们在性能、语法和开发者体验方面的权衡，并在 Hacker News 上引发了大量讨论。 这一比较帮助开发者为项目选择合适的 Lisp 方言，反映了人们对作为具有不同理念和实践优势的语言族系的 Lisp 持续的兴趣。 文章涵盖了语法、性能、生态系统和学习曲线上的差异：Common Lisp 以强大和成熟著称，Scheme 以简洁优雅见长，Clojure 则因现代特性如不可变性和 Java 互操作而备受关注。

hackernews · silcoon · Jul 17, 13:56 · [社区讨论](https://news.ycombinator.com/item?id=48947455)

**背景**: Lisp 是最古老的编程语言家族之一，以其同像性和强大的宏系统而闻名。Common Lisp 是一种标准化、多范式的语言，拥有庞大的生态系统；Scheme 是一种强调函数式编程的极简方言；Clojure 是一种运行在 JVM 上的现代 Lisp，倡导不可变性和并发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Common_Lisp">Common Lisp - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Scheme_(programming_language)">Scheme (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Clojure">Clojure - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了个人经验：一些人偏爱 Common Lisp 的性能（如 SBCL），另一些人欣赏 Scheme 的简洁或 Clojure 的数据结构。少数人质疑 Lisp 相对于现代语言的独特性，而其他人则为其在特定任务中的持续相关性辩护。

**标签**: `#Lisp`, `#Common Lisp`, `#Scheme`, `#Clojure`, `#programming languages`

---

<a id="item-14"></a>
## [脑电图揭示大脑可同时处理两个语音流](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3003876) ⭐️ 7.0/10

一项发表在《PLOS Biology》上的新脑电图研究表明，在注意力转移过程中，大脑可以同时编码两个竞争的语音流，在脱离其中一个之前短暂地双重追踪两者。 这一发现为语音的双流处理提供了直接的神经证据，挑战了大脑一次只能关注一个说话者的观点，并对理解多任务处理和听觉注意障碍具有重要意义。 该研究使用脑电图（EEG）测量对语音流的神经追踪，显示在注意力切换期间α功率降低和短暂的双重编码，支持灵活的听觉注意力。

hackernews · giuliomagnifico · Jul 17, 05:51 · [社区讨论](https://news.ycombinator.com/item?id=48943745)

**背景**: 语音处理的双流模型提出了一个背侧语音流和一个腹侧语义流。以往的研究对大脑能否同时处理多个语音流存在争议。这项研究提供了证据，表明大脑在聚焦于一个流之前可以短暂地编码两个流。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3003876">Competing speech streams are simultaneously represented in ...</a></li>
<li><a href="https://neurosciencenews.com/auditory-multitasking-eeg-dual-tracking-conversations-31064/">Brain Can Process Two Conversations at Once - Neuroscience News</a></li>
<li><a href="https://www.sciencedirect.com/science/chapter/handbook/pii/B9780128233849000037">The dual stream model of speech and language processing ...</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了个人轶事：有人指出他们可以同时计数和阅读但不能说话（费曼），另有人观察到朗读时错误从独立思绪中泄露，一位飞行员报告能处理两个音频流，还有其他人将正念练习与同时关注两个地方联系起来。这些讨论与研究的发现产生了共鸣。

**标签**: `#neuroscience`, `#cognition`, `#speech processing`, `#multitasking`

---

<a id="item-15"></a>
## [Pebble 发布 Index 智能戒指等重大更新](https://repebble.com/blog/pebble-mega-update-july-2026) ⭐️ 7.0/10

Pebble 在 2026 年 7 月的重大更新中推出了 Index 01 智能戒指，这是一款售价 75 美元、不可充电的设备，通过按钮按下即可录制语音备忘录。 Index 标志着 Pebble 以独特的“外部记忆”概念进入智能戒指市场，但其不可充电的设计和尺寸争议引发了关于可用性和环境影响的讨论。 Index 01 在轻度使用下（每天 10-20 次、每次 3-6 秒）声称电池寿命为 2 年，但实际连续使用仅 12-15 小时；它需要单独的尺寸测量套件，而该套件据报告存在精度问题。

hackernews · crazysaem · Jul 17, 03:53 · [社区讨论](https://news.ycombinator.com/item?id=48943174)

**背景**: 像 Oura 这样的智能戒指通常追踪健康指标且可充电。Pebble 的 Index 则不同：它专注于快速捕捉想法，没有健康追踪功能。不可充电的设计对于可穿戴设备来说很少见，引发了关于浪费和便利性的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://repebble.com/index">Pebble Index 01 - External Memory For Your Brain</a></li>
<li><a href="https://www.wired.com/story/pebble-index-ring/">Pebble Is Making a $75 Smart Ring - WIRED</a></li>
<li><a href="https://repebble.com/blog/meet-pebble-index-01-external-memory-for-your-brain">Meet Pebble Index 01 - External Memory For Your Brain</a></li>

</ul>
</details>

**社区讨论**: 评论显示一些用户对快速记笔记感到兴奋，但批评者指出了尺寸测量套件不准确、不可充电设计缺陷以及电池寿命的误导（2 年 vs 12-15 小时）。总体情绪复杂，但有深刻的批评。

**标签**: `#Pebble`, `#smart ring`, `#wearable`, `#hardware`, `#product update`

---

<a id="item-16"></a>
## [1Password 推出 Claude 集成，AI 代登录但不接触密码](https://9to5mac.com/2026/07/16/1password-now-lets-claude-sign-in-to-websites-without-seeing-your-passwords/) ⭐️ 7.0/10

1Password 在 Mac 端推出了与 Claude 的集成，允许 AI 代理代表用户登录网站。该功能确保密码和二次验证码不会进入 Claude 的上下文、记忆或 Anthropic 的系统。 这一集成平衡了便利性和安全性，在不妨碍凭证安全的前提下实现了 AI 代理的实际应用。它为密码管理器如何与 AI 助手安全协作树立了先例，使希望自动登录又无需担忧信任问题的用户受益。 凭证通过安全通道直接注入目标网页，用户需通过生物识别逐条审批当前会话的登录任务。若自动填充提交失败，已填内容会被立即擦除。该功能面向 Mac 的商业、家庭及个人版用户开放，需同时安装 1Password 和 Claude 的桌面及浏览器扩展。

telegram · zaihuapd · Jul 16, 15:54

**背景**: 1Password 是一款流行的密码管理器，用于存储和自动填充凭证。Claude 是 Anthropic 公司开发的 AI 助手。这一集成允许用户将登录委托给 Claude，同时保持对机密数据的完全控制，解决了 AI 访问敏感数据的担忧。

**标签**: `#password management`, `#AI integration`, `#security`, `#1Password`, `#Claude`

---

<a id="item-17"></a>
## [OpenAI CFO 提出“每美元有用智能”指标](https://openai.com/index/a-scorecard-for-the-ai-age) ⭐️ 7.0/10

OpenAI 首席财务官 Sarah Friar 提出以“每美元有用智能”作为衡量 AI 投资回报的新指标，取代传统的软件采用率指标。该框架评估完成工作的价值与成本的比率，文章还介绍了 GPT-5.6 系列，其旗舰模型 Sol 在编码任务上创下新纪录。 这一指标可能改变企业评估 AI 投资的方式，聚焦实际任务完成成本而非仅看 token 价格。它强调更强的模型尽管单 token 成本更高，但可能更具成本效益，从而加速 GPT-5.6 Sol 等前沿模型在企业工作流中的采用。 该框架包含四个维度：完成的有用工作量、每个成功任务的全成本、AI 输出的可靠性，以及随使用增长每美元是否产生更多价值。GPT-5.6 系列提供三个变体——Sol、Terra 和 Luna，其中 Sol 最强大，在编码任务上输出 token 比另一领先模型减少 54%。

telegram · zaihuapd · Jul 17, 15:00

**背景**: 传统的 AI 投资回报指标通常依赖用户数、许可证续费或 token 成本等采用指标，这可能具有误导性，因为更便宜的模型可能需要更多尝试才能完成任务。“每美元有用智能”指标旨在捕捉 AI 系统交付的真正价值。GPT-5.6 是 OpenAI 的最新模型系列，其中 Sol 是他们最好的编码模型，专为复杂推理和代理工作流设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with ... - OpenAI</a></li>

</ul>
</details>

**标签**: `#AI metrics`, `#ROI`, `#OpenAI`, `#GPT-5.6`, `#efficiency`

---