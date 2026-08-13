---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> From 37 items, 14 important content pieces were selected

---

1. [DRAM“意大利面化”攻击工具揭示 AMD Jaguar 隐藏内存](#item-1) ⭐️ 9.0/10
2. [选择无聊技术：明智地花掉创新代币](#item-2) ⭐️ 9.0/10
3. [谷歌发布 Gemini 3.7 Flash，主打图像转 HTML 与限时优惠定价](#item-3) ⭐️ 8.0/10
4. [Cerebras 与 OpenAI 推出 Ultrafast 模式：GPT-5.6 Sol 提速最高 14 倍](#item-4) ⭐️ 8.0/10
5. [DeepSeek 发布开源 AI 智能体开发框架开发者预览版](#item-5) ⭐️ 8.0/10
6. [特朗普签署备忘录，允许私企开展海外网络行动](#item-6) ⭐️ 8.0/10
7. [DeepMind 推手语转文字模型 SL2T，首次落地 Pixel 11](#item-7) ⭐️ 8.0/10
8. [OpenAI 推出 GPT-5.6 Sol 与 Luna，并为免费用户新增 Think 按钮](#item-8) ⭐️ 8.0/10
9. [谷歌发布 Gemini 3.6 Flash，透露 Gemini 4 已开始预训练](#item-9) ⭐️ 8.0/10
10. [45 岁的 Donkey.BAS：比尔·盖茨的经典游戏被移植到浏览器](#item-10) ⭐️ 7.0/10
11. [Oxide 上的 Kubernetes：客户需求催生新集成](#item-11) ⭐️ 7.0/10
12. [浙大开源方案 3D 指标超越 Nano Banana Pro，让平面图像立体编辑更真实](#item-12) ⭐️ 7.0/10
13. [Claude 浏览器会话可续传桌面端，技能与连接器同步](#item-13) ⭐️ 7.0/10
14. [苹果洽谈为 Siri AI 授权新闻内容，拟按使用量付费](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DRAM“意大利面化”攻击工具揭示 AMD Jaguar 隐藏内存](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Christopher Domas 发布了“skitter-creek-bath-salts”，这是一个针对 AMD Family 16h（Jaguar）CPU 的 DRAM 操控工具。它演示了一种重映射物理内存的技术，使 ring-0 软件能够访问通常为更深层 CPU 特权级别保留的受保护区域。 该发布暴露了一个巨大的 DRAM 攻击面，对采用 Jaguar 芯片的 Xbox 和 PlayStation 可能至关重要。它表明，拥有内核权限的攻击者可以进一步获得 hypervisor 或 SMM 级别的可见性，从而扩大本已严重的入侵的影响范围。 该攻击在 AMD Family 16h 上开发并测试，这是最后一代数据手册中记录 DRAM 控制器翻译寄存器且显示其无法锁定的 CPU 家族。README 指出 Zen 3 的上述寄存器基地址不同，因此对其他 CPU 家族的具体影响尚不清楚。

hackernews · matt_d · Aug 13, 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**背景**: DRAM 控制器会将 CPU 的物理地址转换为内存芯片内部的行、列、Bank 和 Rank 地址，而不是使用线性映射。在 AMD Family 16h 上，这些翻译寄存器被公开记录且保持未锁定状态，因此特权软件可以重新配置它们。通过调整这种翻译，ring-0 攻击者可以“意大利面化”内存布局，并暴露供 hypervisor 或 System Management Mode 等更低层固件使用的区域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49286341">Spaghettifying DRAM | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spaghettification">Spaghettification - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对即将举行的 Black Hat 演讲感到兴奋，并称赞 Domas 之前的研究。一些人质疑该技术的实际影响范围，指出 AMD Jaguar 是 2013 年的产品，而且关于 Zen 3 等更新 CPU 的细节很少。另一些人则认为 Xbox 和 PlayStation 的安全团队有理由感到紧张，因为 ring-0 权限现在会打开“负环”领域。

**标签**: `#security`, `#DRAM`, `#hardware`, `#exploit`, `#reverse engineering`

---

<a id="item-2"></a>
## [选择无聊技术：明智地花掉创新代币](https://mcfunley.com/choose-boring-technology) ⭐️ 9.0/10

Dan McKinley 于 2015 年发表的这篇文章主张，公司应优先选用无聊、成熟的技术，而每次创新选择都要消耗一枚有限的"创新代币"。这篇文章至今仍被广泛引用和讨论，在该合集评分为 9.0/10。 它为工程领导者提供了一个简单的思维模型，用来控制技术风险并把创新集中在真正的差异化方向上。在 AI/Agent 时代，这一理念尤其重要：团队可以把创新代币花在 Agent 上，同时让底层支撑技术保持无聊和可预测。 文章普及了"三枚创新代币"的概念，并澄清"无聊"不等于过时——PostgreSQL 虽然无聊但非常可靠。有评论者将这一思想延伸到 Agent 领域，建议使用"分布内技术"，例如选 Rust 而非 Zig（如果 Agent 更擅长 Rust）；也有人批评代币设定很随意，"新"只是风险的弱替代指标。

hackernews · tosh · Aug 13, 17:48 · [社区讨论](https://news.ycombinator.com/item?id=49289512)

**背景**: 前 Etsy 软件工程师 Dan McKinley 在 2015 年的文章中推广了"无聊技术"这一术语。其核心思想是每家公司对技术风险的承受能力都有限，因此每个非标准的技术选择都要花掉一枚有限的"创新代币"。让大部分基础设施保持标准和可预测，才能把代币留给真正能为业务带来差异化的领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lessannoyingbusiness.com/post/innovation-tokens">Innovation Tokens - When to break from the status quo</a></li>
<li><a href="https://mattrickard.com/innovation-tokens">Innovation Tokens | Matt Rickard</a></li>
<li><a href="https://www.peal.dev/blog/boring-technology-principle-why-we-pick-proven-tools">The Boring Technology Principle : Why We Reach for... — peal.dev</a></li>

</ul>
</details>

**社区讨论**: 评论区总体评价很高：一位 PM/工程负责人称"创新代币"是职业生涯中最有用的概念之一。有评论者将这一理念应用到 AI Agent 上，建议把创新代币集中投入到 Agent 中，并让 Agent 使用的技术保持无聊。也有反对声音认为"代币"的设定显得随意，工程师应直接评估风险与权衡；还有用户说这篇文章"出人意料地有争议"。

**标签**: `#technology strategy`, `#engineering management`, `#software engineering`, `#innovation`, `#architecture`

---

<a id="item-3"></a>
## [谷歌发布 Gemini 3.7 Flash，主打图像转 HTML 与限时优惠定价](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

谷歌推出了 Gemini 3.7 Flash，这是一款新 AI 模型，提供限时优惠定价，并具备突出的“图像转 HTML”能力。该模型距离 Gemini 3.6 Flash 发布仅三周，其促销价格将在 2026 年 12 月 31 日翻倍。 此次发布通过新增一款低成本、擅长视觉和编程任务的 Flash 级模型，增强了谷歌在快速发展的 LLM 市场中的竞争力。然而，来自 GPT-5.6 Luna 等对手的价格压力可能会影响开发者和企业的采用。 优惠定价将在 2026 年 12 月 31 日翻倍，考虑到模型发布节奏之快，一些社区成员对此表示不解。在社区测试中，Gemini 3.7 在图像转 HTML 方面表现不错，但在 DeepSWE 1.1 等基准上仍落后于 Opus 5 和 GPT-5.6 Luna (Max)，默认思考级别下的输出有时会出现错误。

hackernews · thisisauserid · Aug 13, 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**背景**: Gemini 3.7 Flash 属于谷歌 Flash 系列模型，主打低成本、高容量场景，如摘要、解析和格式化文本。“图像转 HTML”功能依赖视觉语言模型（VLM），它将视觉编码器与语言模型结合，将屏幕截图或草图转换为 HTML 代码，WebSight 等数据集已对此类方法进行探索。这类技术被认为有望加速前端开发并支持无代码解决方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vision-language_model">Vision-language model - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2403.09029v1">Unlocking the conversion of Web Screenshots into HTML Code with the WebSight Dataset</a></li>
<li><a href="https://alain-airom.medium.com/what-are-vision-language-models-vlms-and-how-do-they-work-592ad38e0d3e">What Are Vision-Language Models (VLMs) and How Do They Work? | by Alain Airom (Ayrom) | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区反馈褒贬不一：jjcm 测试图像转 HTML 后认为 Opus 5 仍是同类最佳，但 Gemini 3.7 在同价位中表现不错；simonw 批评其优惠定价计划在 2026 年 12 月翻倍，而 3.6 Flash 三周前才发布，显得奇怪；Alifatisk 和 wxw 则将其与 GPT-5.6 Luna/Terra 比较，认为 Luna 更便宜且 DeepSWE 1.1 表现更好，但 wxw 也指出 3.7 的基准更接近 Terra 而非 Luna。

**标签**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#Machine Learning`

---

<a id="item-4"></a>
## [Cerebras 与 OpenAI 推出 Ultrafast 模式：GPT-5.6 Sol 提速最高 14 倍](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras 宣布为 OpenAI API 新服务层级 Ultrafast 提供算力，使 GPT-5.6 Sol 的运行速度最高达到标准处理的 14 倍，每秒最多可输出 750 个 token。在 Cerebras 的评估中，Ultrafast 模式下的 GPT-5.6 Sol 在 11 小时 11 分钟内完成了全部 2500 道 HLE 问题，比 Claude Fable 5 的 78 小时 27 分钟快了近 7 倍。 这标志着 OpenAI 与 Cerebras 之间首批重大的公开合作之一，也表明 Cerebras 的晶圆级芯片能够加速前沿模型的推理。更快的推理支持更多迭代并降低时延，有助于时间敏感、关键任务的 AI 工作负载，也可能加剧基于 GPU 的推理服务商的竞争压力。 公告称 Ultrafast“毫无质量折损”，但社区评论者指出，Cerebras 和 OpenAI 都没有明确说明其准确性与标准版 GPT-5.6 Sol 完全一致。该新服务层级尚未公布定价，而且 HLE 基准本身也曾因部分答案的正确性受到独立审查。

hackernews · pr337h4m · Aug 13, 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**背景**: HLE（即“人类最后的考试”）是一个包含 2500 道由专家审核的数学、科学、人文学科等问题的基准测试，用来评估前沿 AI 能力。Cerebras 制造全球最大的 AI 处理器——晶圆级引擎，此前用于大规模训练，近来也开始为 GPT-5.6 Sol 等模型提供低延迟推理。Ultrafast 是 OpenAI API 中率先由 Cerebras 支持的新服务层级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI</a></li>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Humanity's_Last_Exam">Humanity's Last Exam - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者总体感到惊艳但保持谨慎：csallen 强调速度通过迭代提升答案质量，而 Topfi 等人指出，公告并未明确说明 Ultrafast 与标准版模型准确率完全相同。GodelNumbering 注意到没有定价信息，johnfn 则提醒高 token 吞吐只能解决部分瓶颈，不能解决所有端到端延迟问题。

**标签**: `#AI`, `#LLM`, `#performance`, `#hardware`, `#speedup`

---

<a id="item-5"></a>
## [DeepSeek 发布开源 AI 智能体开发框架开发者预览版](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek 以 MIT 许可证发布了其 AI 智能体开发框架 DeepSeek Harness 的开发者预览版。该预览版引入了完整的会话可追踪性、可回放事件流，以及基于 Cordis v4 的可热重载插件系统。 这一发布意义重大，因为它将一家重要 AI 实验室的智能体基础设施开放出来，可能加速 AI 智能体生态中的实验与标准化进程。其完整的可追踪性与一些美国模型加密或混淆的轨迹形成对比，为开发者提供了前所未有的智能体行为可见性。 每次运行都会记录在仅追加的会话日志中，包括系统提示、推理过程、工具调用与结果、子智能体调度以及上下文注入，轨迹视图可按来源检查这些记录。该架构将所有东西都视为插件，Cordis v4 支持热加载与卸载，并能回滚状态和副作用；不过作者提醒这仍是早期预览版，后续会有破坏性变更。

hackernews · bjin · Aug 13, 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49285244)

**背景**: Agent harness（智能体开发框架）是包裹在大语言模型之外的软件基础设施，负责处理工具调用、记忆、状态持久化和反馈循环，而不是模型自身的推理。可回放事件流将数据视为一等资产，系统可以通过重放事件来重建任意时刻的状态。热重载是一种运行时能力，允许在不重启宿主应用的情况下替换插件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://www.conduktor.io/glossary/event-stream-fundamentals">Event Streams: The Foundation of Real-Time Architectures | Conduktor</a></li>
<li><a href="https://inferensys.com/glossary/tool-calling-and-api-execution/plugin-architectures/hot-reloading">Hot Reloading: Definition & Use in Plugin Systems</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者总体热情高涨，称完整的可追踪性是“杀手级功能”，而美国模型的加密轨迹无法提供这一点。还有人讨论了底层的 Cordis v4 插件系统，一位评论者指出它已在 Koishi 项目中使用多年；也有少数人表达了“插件疲劳”，对“一切皆插件”的架构持怀疑态度。DeepSeek Harness 的一位作者也出现在讨论中，欢迎大家对这个早期预览版提出反馈。

**标签**: `#deepseek`, `#agent-harness`, `#open-source`, `#traceability`, `#AI-agents`

---

<a id="item-6"></a>
## [特朗普签署备忘录，允许私企开展海外网络行动](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 8.0/10

特朗普总统签署备忘录，允许私营企业在政府背书下开展海外监控和网络攻击，以打击针对美国人的外国犯罪集团。国土安全部将负责该项目，并由司法部协调监督。 这标志着私营企业在国家赞助的进攻性网络行动中角色的显著扩大，引发了关于责任、监督和法律边界的担忧。这可能为政府如何利用商业能力进行监控和网络战树立先例。 参与企业须维持至少 100 万美元的保证金或托管款，如不遵守合同约定，该款项将被没收。该项目要求国土安全部和司法部之间进行协调。

telegram · zaihuapd · Aug 13, 05:10

**背景**: 政府长期以来一直与私营公司签订网络安全支持合同，但进攻性行动和监控通常保留给国家机构。这份备忘录似乎扩大了私营部门在联邦直接控制下参与此类活动的法律空间，引发了新的法律和伦理问题。

**标签**: `#cybersecurity`, `#surveillance`, `#government policy`, `#private sector`, `#offensive operations`

---

<a id="item-7"></a>
## [DeepMind 推手语转文字模型 SL2T，首次落地 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

DeepMind 发布了手语转文字模型 SL2T，已在 Pixel 11 的 Gboard 和 Live Transcribe 中上线，首批支持美国手语转英语。该模型使用超过 10 万小时、50 多种手语的数据进行训练。 这标志着手语 AI 首次进入主流消费产品，为聋人和听障人士的沟通带来更大便利。同时，它在 FLEURS-ASL 基准上表现出很强的零样本能力，为多语言手语模型树立了新标杆。 该模型只处理手部和身体姿态关键点，不读取原始视频，以保护隐私。目前仅支持美国手语转英语，未来计划扩展更多语言和手语生成模型。

telegram · zaihuapd · Aug 13, 08:55

**背景**: 手语翻译模型通过视频或姿态关键点将视觉手势转换为文字。DeepMind 的 SL2T 在大型多语言数据集上训练，并在 FLEURS-ASL 上进行评估；FLEURS-ASL 是 FLORES/FLEURS 基准扩展到美式手语的版本，使用 BLEURT 这一学习型指标来衡量流畅度和语义保真度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cryptopolitan.com/google-deepmind-sign-language-on-pixel-11/">Google DeepMind ships SL2T sign-language model on Pixel 11 - Cryptopolitan</a></li>
<li><a href="https://aclanthology.org/2025.naacl-long.314/">FLEURS-ASL: Including American Sign Language in Massively Multilingual Multitask Evaluation - ACL Anthology</a></li>
<li><a href="https://arxiv.org/abs/2004.04696">[2004.04696] BLEURT: Learning Robust Metrics for Text Generation</a></li>

</ul>
</details>

**标签**: `#DeepMind`, `#Sign Language AI`, `#Accessibility`, `#Translation`, `#Consumer AI`

---

<a id="item-8"></a>
## [OpenAI 推出 GPT-5.6 Sol 与 Luna，并为免费用户新增 Think 按钮](https://t.me/zaihuapd/43176) ⭐️ 8.0/10

OpenAI 宣布了 GPT-5.6 系列升级：Plus 和 Pro 订阅用户将获得 GPT-5.6 Sol 模型，并新增思考深度滑块；免费用户本周起默认使用 GPT-5.6 Luna，下周起可用无限文本对话和新的 Think 按钮。 此次更新首次将高级推理功能带给免费用户，同时提升了付费用户的事实可靠性，可能加剧 AI 聊天机器人厂商之间的竞争。这也表明 OpenAI 试图通过推理控制来区分不同模型层次的策略。 OpenAI 的内部评估显示，GPT-5.6 Luna 在财经、医疗和法律问题上比前代模型事实错误更少，而 GPT-5.6 Sol 的事实错误减少了 68%。旧版 GPT-5.5 Instant 已完全退役，免费用户仍需面对文件上传、图片和其他工具的用量限制。

telegram · zaihuapd · Aug 13, 17:04

**背景**: GPT-5.6 是 OpenAI 最新的模型系列，其中 Sol 面向付费用户的旗舰版本，Luna 是免费和 Go 用户的轻量默认模型。Think 按钮用于触发针对复杂问题的扩展推理模式，思考深度滑块则让用户调整模型在回答时投入的计算量。此次更新是 OpenAI 在兼顾免费可及性与商业变现之间的一次尝试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/improving-gpt-5-6-sol-in-chatgpt/">Improving GPT ‑ 5 . 6 Sol in ChatGPT—and expanding access... | OpenAI</a></li>
<li><a href="https://aibreakfast.beehiiv.com/p/openai-adds-reasoning-depth-slider-to-gpt-5-6-sol">OpenAI adds reasoning depth slider to GPT - 5 . 6 Sol</a></li>
<li><a href="https://aicatchup.com/news/chatgpt-gpt-5-6-sol-luna-access-reasoning-controls">ChatGPT GPT-5.6 Luna: Unlimited Chats and Reasoning Slider</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#GPT-5.6`, `#AI Model Update`, `#Free Tier`

---

<a id="item-9"></a>
## [谷歌发布 Gemini 3.6 Flash，透露 Gemini 4 已开始预训练](https://t.me/zaihuapd/43177) ⭐️ 8.0/10

谷歌发布了 Gemini 3.6 Flash，其输出 Token 比 Gemini 3.5 Flash 减少 17%，并能以更少的推理步骤和工具调用完成多步任务。谷歌同时宣布 Gemini 4 已进入预训练阶段，并将知识截止日期更新至 2026 年 3 月。 此次发布表明谷歌在 LLM 推理效率上积极发力，直接降低开发者的成本和延迟，这对规模化 AI 应用至关重要。透露 Gemini 4 已开始预训练，说明其迭代周期非常快，很可能影响前沿 AI 模型的竞争格局。 Gemini 3.6 Flash 的 API 定价为每百万输入 Token 1.5 美元、每百万输出 Token 7.5 美元，并在代码生成、知识工作和计算机操作能力上有所提升。谷歌还同步推出了面向高吞吐、低延迟场景的 Gemini 3.5 Flash 版本。

telegram · zaihuapd · Aug 13, 17:32

**背景**: 在大语言模型中，文本会被切分成称为 Token 的小单元，模型据此理解并生成回答；减少输出 Token 能直接降低计算成本和延迟。工具调用（也称函数调用）允许模型在生成过程中调用外部 API 或执行操作，是完成智能体式多步任务的关键。计算机操作则指模型通过界面（如查看截图、返回界面动作）来操作软件，从而实现更广泛的自动化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/tool-calling">What is tool calling? - IBM</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/tools-computer-use">Computer use | OpenAI API</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#Model Release`

---

<a id="item-10"></a>
## [45 岁的 Donkey.BAS：比尔·盖茨的经典游戏被移植到浏览器](https://donkeybas.com/) ⭐️ 7.0/10

为庆祝 IBM PC 诞生 45 周年，一个基于浏览器的 DONKEY.BAS 移植版已发布。DONKEY.BAS 是比尔·盖茨参与编写的 1981 年 BASIC 驾驶游戏；该移植版在 donkeybas.com 上重现了这段 131 行的原始程序。 这个怀旧项目突显了 DONKEY.BAS 的历史意义——它是微软最早的遊戲之一，也展示了 BASIC 语言在 IBM PC 上的能力。它引起了一代通过微软 BASIC 解释器学习编程的人的共鸣，同时表明复古计算文化在浏览器时代依然活跃。 原版游戏是一个俯视视角的驾驶游戏，玩家需要避开驴子；它由比尔·盖茨和 Neil Konzen 于 1981 年编写，并随 PC DOS 1.00 分发。浏览器移植版力求还原，但有评论指出其音效比原装 PC 扬声器更先进；另有一位开发者正在独立开发一个在浏览器中完全忠实的 QBasic/QuickBasic 4.5 模拟器。

hackernews · jkrauska · Aug 13, 17:45 · [社区讨论](https://news.ycombinator.com/item?id=49289465)

**背景**: DONKEY.BAS 是 1981 年编写的一款视频游戏，随早期版本的 IBM PC DOS 一同分发。它常被视为微软 BASIC 解释器随 IBM PC 发布的早期示例，并因由比尔·盖茨参与编写而闻名。游戏仅用 131 行 BASIC 代码便实现了一个完整的驾驶小游戏，展示了早期家庭电脑游戏可以用不多的编程工作量完成，如今已成为复古计算领域的文化符号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DONKEY.BAS">DONKEY.BAS</a></li>
<li><a href="https://www.pcjs.org/software/pcx86/app/ibm/basic/1.00/donkey/">DONKEY.BAS from PC DOS 1.00 (1981) - PCjs</a></li>

</ul>
</details>

**社区讨论**: 评论者们分享了怀旧情绪和技术见解：有人称赞移植版，但指出音效对于原始 PC 扬声器来说过于先进；另有人正在开发一个忠实的浏览器版 QBasic/QuickBasic 模拟器。还有人回忆起 GORILLA.BAS 等同类游戏，并讨论了“DONKEY.BAS 是比尔·盖茨在微软亲自编写的最后一段代码”这一传闻。

**标签**: `#retrocomputing`, `#BASIC`, `#browser port`, `#history`, `#IBM PC`

---

<a id="item-11"></a>
## [Oxide 上的 Kubernetes：客户需求催生新集成](https://oxide.computer/blog/kubernetes-on-oxide) ⭐️ 7.0/10

Oxide 宣布了直接由客户反馈推动的 Kubernetes 集成，包括云控制器管理器（Cloud Controller Manager）、Rancher 节点驱动程序和 Omni 基础设施提供程序。这些集成大约在 2024 年底开始成形，当时客户希望在没有受支持路径的情况下在 Oxide 上运行 Kubernetes。 这很重要，因为 Oxide 的目标是成为本地部署基础设施的完整『云计算机』，而 Kubernetes 支持是现代平台团队的入门要求。这让 Oxide 成为传统虚拟化和超大规模云方案的更有力替代选择。 这些集成包括在 Kubernetes 上游之外构建的『现代』云控制器管理器、Rancher 节点驱动程序和 Omni 基础设施提供程序（详见 Oxide 的 RFD 0493）。Oxide 的工程方法据称会重新审视这些组件的构建方式，而不是简单移植传统的 in-tree（树内）代码。

hackernews · stevehipwell · Aug 13, 14:26 · [社区讨论](https://news.ycombinator.com/item?id=49286485)

**背景**: Oxide Computer Company 打造了一款机架级『云计算机』，将计算、存储、网络和软件整合为单一本地部署产品。Kubernetes 是主流的容器编排平台；要在 Oxide 上运行它，需要云控制器管理器（管理云资源）、用于集群置备的节点驱动程序以及面向 Kubernetes 平台的基础设施提供程序等组件。在这些集成出现之前，客户不得不自行拼凑解决方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oxide.computer/blog/kubernetes-on-oxide">Kubernetes on Oxide : How Customer Needs Shaped Our Integrations</a></li>
<li><a href="https://rfd-site.vercel.app/rfd/0493">493 - Initial Kubernetes Integrations / RFD / Oxide</a></li>
<li><a href="https://techfieldday.com/video/oxide-integrations-empowering-platform-teams-and-developers-with-oxide-computer/">Oxide Integrations : Empowering Platform Teams... - Tech Field Day</a></li>

</ul>
</details>

**社区讨论**: 评论者热情且充满好奇：有人期待看到 Oxide 的云控制器管理器与旧式 in-tree CCM 的对比，并预测会出现『karpenter-provider-oxide』；还有人开玩笑说希望 40 年后能在二手拍卖会上买到 Oxide 机架。其他人询问 Oxide 与 KubeVirt/Proxmox 的重叠之处，并希望 Oxide 开源其文档系统，同时还有人借机推介 Kubernetes 原生的数据平台。

**标签**: `#kubernetes`, `#oxide`, `#infrastructure`, `#systems-design`, `#cloud-computing`

---

<a id="item-12"></a>
## [浙大开源方案 3D 指标超越 Nano Banana Pro，让平面图像立体编辑更真实](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247912028&idx=4&sn=c106858467e16b7df780265696c61fe3) ⭐️ 7.0/10

浙江大学团队开源了一种基于显式 3D 几何约束的 AI 图像编辑方法，在 3D 一致性指标上声称超过 Nano Banana Pro。该工作与 ACM MM'26 相关。 3D 一致性一直是 AI 图像编辑的关键瓶颈，开源方案若能在该指标上超越主流商业模型，将推动整个领域进步。它也可能让更多开发者和用户用上高质量的 3D 感知编辑能力。 报道仅提供了高层描述，未给出完整实现细节，强调该方法通过显式 3D 几何约束避免了对文本提示的盲目猜测。超越 Nano Banana Pro 的说法基于 3D 相关指标，而非全面图像质量。

rss · 量子位 · Aug 13, 07:38

**背景**: 以 Nano Banana Pro 为代表的 AI 图像编辑模型能从文本提示生成高质量图像，但在平面图像中编辑物体时，往往难以保持几何、深度和透视的一致性。显式 3D 几何约束通过加入空间信息来引导编辑过程，近期 Arbor 等研究已在 3D 生成中展示了这一思路。浙大的新方案将类似思路应用于图像编辑，直击当前模型的弱点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nano_Banana_Pro">Nano Banana Pro</a></li>
<li><a href="https://nanobanana.com/nano-banana-pro">Nano Banana Pro - AI Image Generator Online</a></li>
<li><a href="https://arxiv.org/html/2606.23514v1">Arbor: Explicit Geometric Conditioning for Controllable 3D ...</a></li>

</ul>
</details>

**标签**: `#AI图像编辑`, `#3D几何约束`, `#开源`, `#ACM MM`, `#图像生成`

---

<a id="item-13"></a>
## [Claude 浏览器会话可续传桌面端，技能与连接器同步](https://techmymoney.com/2026/08/12/claude-in-chrome-now-carries-your-session-to-the-desktop/) ⭐️ 7.0/10

Anthropic 重构了 Claude 的 Chrome 扩展，使其以完整的 Cowork 会话运行：浏览器中的任务可无缝续传到桌面、网页和移动 App，对话、技能与连接器随账户同步。Max 和 Team 用户即日可用，Pro 用户未来几周开放，企业版默认关闭、由管理员启用。 这一更新让 AI 智能体任务能在不同设备间无中断地延续，并省去重复配置技能与连接器的成本。新增的“自动批准”权限模式在提升效率的同时，仍对敏感操作保留人工确认，兼顾了企业等场景的安全需求。 新“自动批准”模式仍会对表单提交、消息和文件下载等操作与原指令比对，购买与个人数据操作必须人工确认。Anthropic 承认这些措施只能降低风险而无法根除，网页内恶意指令仍是难题；本地文件、其他 Chromium 浏览器和移动端暂不支持。

telegram · zaihuapd · Aug 13, 04:10

**背景**: Claude Cowork 是一种使用与 Claude Code 相同智能体架构、但无需终端的模式，允许 Claude 承担复杂的多步骤任务并代表用户执行。技能（Skills）和连接器（Connectors）是 Claude 的扩展能力，跨所有界面生效，例如 Slack 只需连接一次即可处处使用。此前 Claude 在 Chrome 扩展中提供“手动批准”权限模式，新的权限菜单加入了带防护措施的“自动批准”选项。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/13345190-get-started-with-claude-cowork">Get started with Claude Cowork | Claude Help Center</a></li>
<li><a href="https://support.claude.com/en/articles/15520349-use-claude-cowork-on-web-desktop-and-mobile">Use Claude Cowork on web, desktop, and mobile</a></li>
<li><a href="https://support.claude.com/en/articles/12902446-claude-in-chrome-permissions-guide">Claude in Chrome permissions guide | Claude Help Center</a></li>

</ul>
</details>

**标签**: `#Claude`, `#Anthropic`, `#AI tools`, `#browser extension`, `#session sync`

---

<a id="item-14"></a>
## [苹果洽谈为 Siri AI 授权新闻内容，拟按使用量付费](https://9to5mac.com/2026/08/12/report-apple-seeks-publisher-deals-to-give-siri-ai-better-access-to-current-events/) ⭐️ 7.0/10

苹果正与出版商洽谈多年期内容协议，为 Siri AI 提供最新新闻与信息，并讨论按内容使用量付费的方案。消息称潜在预算可能达九位数美元，Siri AI 预计于 2026 年晚些时候推出。 这有别于大型 AI 公司常见的预付固定授权费模式，显示苹果试图以实时新闻内容和差异化功能来提升 Siri AI 的竞争力。若达成合作，可能重塑新闻出版商在 AI 时代的内容变现方式，并影响 AI 助手获取实时资讯的模式。 苹果讨论的是按实际内容使用量向出版商付费，而非一次性固定授权费；预算或达九位数美元。苹果尚未宣布任何合作，Siri AI 预计 2026 年晚些时候推出，苹果拒绝置评。

telegram · zaihuapd · Aug 13, 04:40

**背景**: AI 助手和聊天机器人越来越需要最新、可信的新闻内容来回答时事问题。许多大型 AI 公司通过一次性预付费方式授权出版商内容，用于训练模型或提供引用。据报道，苹果提出的按使用量付费模式，将根据 Siri AI 实际调用文章的次数来结算，这种模式可能缓解出版商对内容被低价使用的担忧。Siri AI 是苹果计划推出的 AI 增强版 Siri，预计在 2026 年晚些时候上线，将与其它 AI 助手竞争。

**标签**: `#Apple`, `#Siri`, `#AI`, `#News Licensing`, `#Publisher Deals`

---