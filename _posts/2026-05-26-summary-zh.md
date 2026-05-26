---
layout: default
title: "Horizon Summary: 2026-05-26 (ZH)"
date: 2026-05-26
lang: zh
---

> From 37 items, 16 important content pieces were selected

---

1. [Rust 性能分析：与 C 和 C++对比](#item-1) ⭐️ 8.0/10
2. [荷兰阻止美国收购 Solvinity 以保护数字身份系统](#item-2) ⭐️ 8.0/10
3. [LLM 的睡眠式巩固机制](#item-3) ⭐️ 8.0/10
4. [教宗良十四世通谕警告 AI 权力集中](#item-4) ⭐️ 8.0/10
5. [半活人脑用于药物测试引发伦理争议](#item-5) ⭐️ 8.0/10
6. [马斯克称 xAI 将于 2026 年底开源 0.5T 参数模型](#item-6) ⭐️ 8.0/10
7. [伊朗计划永久断网，仅允许通过审查者上网](#item-7) ⭐️ 8.0/10
8. [美团发布跑腿 Skill，AI 助手一句话下单](#item-8) ⭐️ 8.0/10
9. [中国审查 Meta 收购 Manus 并限制创始人离境](#item-9) ⭐️ 8.0/10
10. [Dropbox CEO Drew Houston 因增长停滞辞职](#item-10) ⭐️ 7.0/10
11. [拥有房屋的隐性成本](#item-11) ⭐️ 7.0/10
12. [DynIP 推出支持 RFC 2136、IPv6、DNSSEC 的现代动态 DNS](#item-12) ⭐️ 7.0/10
13. [Stack Overflow 论坛衰落但公司仍盈利](#item-13) ⭐️ 7.0/10
14. [年轻人中结直肠癌发病率上升](#item-14) ⭐️ 7.0/10
15. [欧盟初步裁定：谷歌或违反《数字市场法》](#item-15) ⭐️ 7.0/10
16. [支付宝推出 Token Pay 及 AI 钱包，助力智能体经济](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Rust 性能分析：与 C 和 C++对比](https://github.com/yugr/rust-slides/) ⭐️ 8.0/10

一项题为《Rust 语言性能》的技术分析将 Rust 与 C 和 C++的性能进行了比较，结论是 Rust 与 C 相当，但现代 C++因其更具表现力的编译时设施而往往表现更优。 这项分析很重要，因为它为系统编程中的性能权衡提供了经验证据，影响着对性能关键应用的语言选择。它指出，尽管 Rust 提供了内存安全，但在利用编译时优化以获得最大性能时，C++可能仍然是更好的选择。 分析指出，与 C++相比，Rust 的边界检查可能导致平均约 3%的性能损失，最坏路径可达 15%。此外，Rust 缺少提升的边界检查和不稳定的内部表示限制了 C++可以在编译时执行的某些优化。

hackernews · tanelpoder · May 25, 23:37 · [社区讨论](https://news.ycombinator.com/item?id=48273147)

**背景**: C++提供了如 constexpr 和模板这样的编译时设施，允许在编译时执行计算，从而减少运行时开销。Rust 强调零成本抽象，即高级构造不应产生运行时成本，但其安全保证（如边界检查）可能会带来运行时检查。社区讨论强调，Rust 的内存安全性牺牲了一些性能，特别是与现代 C++相比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://doc.rust-lang.org/beta/embedded-book/static-guarantees/zero-cost-abstractions.html">Zero Cost Abstractions - The Embedded Rust Book</a></li>
<li><a href="https://www.geeksforgeeks.org/cpp/templates-cpp/">Templates in C++ - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 社区成员分享了经验：jandrewrogers 指出 Rust 与 C 相当，但现代 C++因编译时表现力而性能更优；gobdovan 指出了 Rust 边界检查优化的局限性；Animats 质疑了边界检查提升的问题；encodedrose 总结了约 3%的平均性能损失；suis_siva 根据实践分享，编写高性能代码在 C++中最容易。

**标签**: `#Rust`, `#performance`, `#C`, `#C++`, `#compiler optimization`

---

<a id="item-2"></a>
## [荷兰阻止美国收购 Solvinity 以保护数字身份系统](https://www.politico.eu/article/netherlands-blocks-us-takeover-vital-digital-supplier/) ⭐️ 8.0/10

这一决定凸显了全球对关键数字基础设施（尤其是处理敏感公民数据的系统）被外国控制的抵制日益加剧。它可能促使其他国家也对威胁数据主权的收购施加类似限制。 荷兰议会此前曾投票终止与 Solvinity 的政府合同，但政府却延长了合同，因此阻止收购成为唯一剩下的保护措施。Kyndryl 包含 IBM 前数字基础设施业务，于 2025 年 11 月宣布了该交易。

hackernews · vrganj · May 26, 11:46 · [社区讨论](https://news.ycombinator.com/item?id=48278406)

**背景**: DigiD 是荷兰的数字身份系统，公民用它在线访问政府服务，如报税和医疗。Solvinity 提供托管 DigiD 的安全管理云平台。被美国公司收购引发担忧，因为美国《云法案》等法律可能迫使美方获取数据，危及荷兰数据主权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nltimes.nl/2026/05/26/netherlands-blocks-us-takeover-digid-operator-solvinity-security-concerns">Netherlands blocks U.S. takeover of DigiD operator Solvinity over security concerns | NL Times</a></li>
<li><a href="https://www.democrata.es/en/economy/netherlands-vetoes-the-purchase-of-dutch-cloud-company-solvinity-by-us-company-kyndryl/">Netherlands halts Solvinity purchase by Kyndryl | Demócrata</a></li>
<li><a href="https://www.nldigitalgovernment.nl/overview/identity/digid/">DigiD - Digital Government</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍欢迎这一阻止，认为政府必须保护公民数据免受外国控制。一些人主张自建开源身份解决方案，以避免依赖任何供应商。另一些人批评政府不顾议会反对，最初延长了与 Solvinity 的合同。

**标签**: `#data sovereignty`, `#digital identity`, `#geopolitics`, `#privacy`

---

<a id="item-3"></a>
## [LLM 的睡眠式巩固机制](https://arxiv.org/abs/2605.26099) ⭐️ 8.0/10

研究人员提出一种新颖的类睡眠巩固机制，让大语言模型在离线期间定期将近期上下文写入快速权值状态，灵感来源于生物记忆巩固。 该方法通过预计算降低推理成本，同时实现持续学习而不发生灾难性遗忘，有望显著提升 LLM 的记忆和效率。它连接了神经科学与 AI，可能催生更自适应、长上下文能力的模型。 快速权值状态是可快速应用的轻量级权重更新，与慢权值（模型参数）相对。该机制在“睡眠”期间运行，无需额外训练数据即可巩固上下文，并与现有微调技术兼容。

hackernews · juxtapose · May 26, 15:36 · [社区讨论](https://news.ycombinator.com/item?id=48281226)

**背景**: 在生物记忆中，睡眠对将新体验巩固为长期存储至关重要。类似地，人工神经网络可通过离线回放旧记忆来提升性能。快慢权值的概念将瞬时上下文与持久知识分离，使 LLM 快速适应而不覆盖核心能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.12484">Learning, Fast and Slow: Towards LLMs That Adapt Continually</a></li>

</ul>
</details>

**社区讨论**: 评论中既有关注也有质疑，用户提及 E2E-TTT 和 FLANN 研讨会等先前工作。有人将其与 Claude 的自动梦功能类比，也有人开玩笑建议模型半脑睡眠。社区就新颖性和生物学合理性展开了实质性技术辩论。

**标签**: `#AI`, `#LLMs`, `#memory`, `#training`, `#neuroscience`

---

<a id="item-4"></a>
## [教宗良十四世通谕警告 AI 权力集中](https://www.vaticannews.va/en/pope/news/2026-05/pope-leo-xiv-encyclical-magnifica-humanitas-ai.html) ⭐️ 8.0/10

这是全球宗教领袖直接针对 AI 治理的重要伦理声明，与当前关于 AI 伦理和权力集中的辩论高度相关。它可能影响全球 AI 发展的公共讨论和政策。 通谕批评了埃隆·马斯克和彼得·蒂尔等硅谷领袖推崇的超人类主义愿景，谴责 AI 研发中将特定人群判定为低效、无用与多余的精英主义倾向。强调技术从来不是中立的，不应被少数人垄断。

telegram · zaihuapd · May 25, 13:00

**背景**: 教宗良十四世是天主教会的领袖，通谕是涉及道德问题的权威信函。该文件加入了关于 AI 伦理的全球对话，目前 Anthropic、Google、OpenAI 等科技巨头正在开发强大的 AI 模型。梵蒂冈此前曾参与技术伦理讨论，但这是首份专注于 AI 的通谕。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/anthropic-ai-redefining-future-safe-reliable-anand-ramavarapu-xezxf">Anthropic AI: Redefining the Future of Safe, Reliable Artificial ...</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#AI governance`, `#Pope Leo XIV`, `#technology ethics`, `#artificial intelligence`

---

<a id="item-5"></a>
## [半活人脑用于药物测试引发伦理争议](https://www.science.org/content/article/not-alive-not-dead-disembodied-human-brains-used-drug-testing) ⭐️ 8.0/10

美国生物科技公司 Bexorg 利用 BrainEx 灌流系统，在捐献人脑死亡数小时后恢复其部分代谢和细胞活动，用于测试阿尔茨海默病和帕金森病药物。 这一突破挑战了医学对生命与死亡的界定，并可能通过使用真实人脑组织彻底改变药物测试方式，有望减少对动物模型的依赖，提高神经药物研发成功率。 研究人员强调，这些大脑并未恢复意识或完整的神经活动，但大脑既非完全存活也非完全死亡的状态引发了伦理担忧，涉及知情同意和死亡定义的质疑。

telegram · zaihuapd · May 25, 14:57

**背景**: BrainEx 灌流系统是一种在体外为脑组织输送营养并清除废物的技术，可实现部分代谢恢复。生物伦理学中的争议常围绕生命、意识和人格的边界，尤其在神经科学和生物技术取得进展时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebral_circulation">Cerebral circulation - Wikipedia</a></li>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/8791815/">Brain perfusion systems for studies of drug uptake and metabolism in...</a></li>

</ul>
</details>

**标签**: `#neuroscience`, `#bioethics`, `#drug testing`, `#brain research`, `#ethics`

---

<a id="item-6"></a>
## [马斯克称 xAI 将于 2026 年底开源 0.5T 参数模型](https://x.com/i/status/2058796067592736866) ⭐️ 8.0/10

埃隆·马斯克在 X 平台上宣布，xAI 将在 2026 年底前开源一个 0.5 万亿参数的模型，外界普遍推测该模型为 Grok 4.2 基座模型。 开源如此大规模模型将极大推动尖端 AI 的民主化，可能超越其他开源模型，并加速全球 AI 研发进程。 该模型拥有 0.5 万亿参数，很可能采用混合专家（MoE）架构，延续了 xAI 此前以 Apache 2.0 许可证发布 314B 参数的 Grok-1 的做法。

telegram · zaihuapd · May 26, 02:46

**背景**: Grok 是由埃隆·马斯克创立的 xAI 开发的生成式 AI 聊天机器人，于 2023 年 11 月推出。混合专家（MoE）是一种神经网络架构，每次输入仅激活部分参数，从而实现高效扩展。0.5 万亿参数模型一旦开源，将成为最大的开源模型之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.banandre.com/blog/grok-05t-open-source-ai-arms-race">Grok’s 0 . 5 T Bet: The Model That’s Either Open-Source... - Banandre</a></li>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 提供的评论表达了怀疑态度，质疑是否真的会有人使用如此大的开源模型，并将其与中国 AI 产品“豆包”相比。总体来看，社区讨论有限但揭示了对其实用性的疑虑。

**标签**: `#AI`, `#open-source`, `#xAI`, `#Grok`, `#large language models`

---

<a id="item-7"></a>
## [伊朗计划永久断网，仅允许通过审查者上网](https://t.me/zaihuapd/41574) ⭐️ 8.0/10

如果实施，这将成为全球最极端的互联网审查形式之一，严重限制伊朗公民的数字权利，并为其他试图收紧信息管控的威权政权树立危险先例。 当前的全国性互联网封锁始于 2026 年 1 月 8 日，此前发生了 12 天的动荡。Filterwatch 的报告指出，该永久计划要求大多数用户使用国内内联网，只有通过政府安全审查的人才能访问经过过滤的全球互联网。

telegram · zaihuapd · May 26, 06:36

**背景**: 伊朗长期以来一直运行称为“国家信息网络”（NIN）的国营内联网，并对国际内容进行严格过滤，屏蔽了 Twitter、Facebook 和 YouTube 等平台。政府经常在抗议期间切断互联网以压制异议。Filterwatch 是一个监测伊朗互联网审查和政策的组织。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://filter.watch/english/">FilterWatch - Study of Iran's Internet Policies, Internet Shutdowns...</a></li>
<li><a href="https://military.china.com/news/13004177/20260119/49177665.html">伊朗拟永久退网 政府审查互联网接入_军事频道_中华网</a></li>
<li><a href="https://www.al-monitor.com/zh-hans/originals/2026/01/yilanghulianwangfengsuojinrudisanzhoubufenwangluojieruyikaishihuifu">伊朗互联网封锁进入第三周，部分网络接入已开始恢复。 - AL-Monitor...</a></li>

</ul>
</details>

**标签**: `#internet censorship`, `#Iran`, `#network policy`, `#digital rights`, `#geopolitics`

---

<a id="item-8"></a>
## [美团发布跑腿 Skill，AI 助手一句话下单](http://client.sina.com.cn/news/2026-05-26/doc-inhzffss1481138.shtml) ⭐️ 8.0/10

美团发布了“跑腿 Skill”，这是一个开放 API 和开源库，允许任意 AI 助手通过自然语言下达跑腿订单，无需打开美团 App 或手动填写表单。 这一集成将 AI 助手与现实本地服务连接起来，显著增强了 AI 代理的实用性，为日常生活中无缝的语音驱动任务自动化铺平了道路。 该 API 是开放的，集成无需开发工作，兼容 OpenClaw 等客户端；代码已在 GitHub 上开源，服务覆盖所有开通美团跑腿的城市。

telegram · zaihuapd · May 26, 08:29

**背景**: 美团是中国主要的服务平台，提供外卖、跑腿等服务。此前，它在自家 App 内通过“AI 帮我办事”测试了对话下单。现在，通过向第三方 AI 助手开放该技能，美团旨在将其服务嵌入更广泛的 AI 生态系统，如 OpenClaw——一个允许 AI 代理通过消息平台执行任务的开源框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/meituan/MT-Paotui-For-Client">GitHub - meituan /MT- Paotui -For-Client · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw</a></li>

</ul>
</details>

**标签**: `#AI Assistants`, `#API Integration`, `#Open Source`, `#Meituan`, `#Natural Language Ordering`

---

<a id="item-9"></a>
## [中国审查 Meta 收购 Manus 并限制创始人离境](https://t.me/zaihuapd/41577) ⭐️ 8.0/10

中国监管机构正在审查 Meta 收购 AI 初创公司 Manus 是否违反投资规定，并已限制其首席执行官肖鸿和首席科学家季一超离境。 此次审查可能阻止 Meta 在 AI 智能体技术领域的扩张，并标志着中美科技紧张局势升级，同时影响创始人的全球业务运营能力。 收购于 2024 年 12 月宣布，但交易金额未公开。创始人本月与国家发改委会面后被告知不得离境，但可在国内出行。

telegram · zaihuapd · May 26, 09:56

**背景**: Manus 是一家开发通用型 AI 智能体的初创公司，由蝴蝶效应公司创立，该公司最初在中国成立，现总部位于新加坡。Meta 于 2024 年 12 月宣布收购该初创公司，旨在将 AI 推向全球企业。中国对外国收购的安全审查机制可在涉及国家安全或出口管制问题时施加限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus ( AI agent) - Wikipedia</a></li>
<li><a href="https://www.silicon.co.uk/e-innovation/artificial-intelligence/china-manus-meta-628254">Chinese Authorities Review Meta 's Manus Acquisition | Silicon UK</a></li>

</ul>
</details>

**标签**: `#AI`, `#Acquisition`, `#Regulation`, `#China`, `#Meta`

---

<a id="item-10"></a>
## [Dropbox CEO Drew Houston 因增长停滞辞职](https://www.cnbc.com/2026/05/26/dropbox-ceo-drew-houston-ashraf-alkarmi.html) ⭐️ 7.0/10

Dropbox 联合创始人兼 CEO Drew Houston 宣布将卸任，公司博客发布了这一消息。该新闻引发了社区对公司未来的讨论。 此次领导层变动发生在 Dropbox 面临增长停滞以及来自苹果、谷歌和微软等资金雄厚竞争对手激烈竞争之际。这一决定可能预示着这家云存储公司将进行战略调整。 Dropbox 的股价估值长期徘徊在 60 亿美元左右，增长停滞，年收入约 25 亿美元。公司正面临艰难的市场环境，主要竞争对手均提供深度集成的云解决方案。

hackernews · aghuang · May 26, 13:18 · [社区讨论](https://news.ycombinator.com/item?id=48279453)

**背景**: Dropbox 是一家成立于 2007 年的云存储和文件同步服务公司。它曾是这一领域的早期领导者，但面对苹果、谷歌和微软的集成式产品，增长乏力。

**社区讨论**: 社区评论中，一位前员工称赞 Houston 是他们见过的最优秀的 CEO，而其他人则认为增长停滞是市场因素而非领导层问题。一位用户分享了因账户删除导致数据丢失的令人痛心的经历，并质疑 Dropbox 的客户支持。

**标签**: `#Dropbox`, `#CEO`, `#Leadership Change`, `#Cloud Storage`, `#Tech Industry`

---

<a id="item-11"></a>
## [拥有房屋的隐性成本](https://ericturner.dev/posts/cost-of-home-ownership/) ⭐️ 7.0/10

一篇个人反思文章量化了拥有房屋的真实成本，包括时间、维护以及财务指标之外的心理负担。 这项分析对考虑购房的科技工作者等人群意义重大，因为它突显了常被忽视的非财务成本，这些成本可能影响生活方式和幸福感。 作者认为，拥有房屋需要投入大量时间进行维护和改造，而独自负责的心理负担可能带来压力。

hackernews · ggcr · May 26, 16:04 · [社区讨论](https://news.ycombinator.com/item?id=48281611)

**背景**: 拥有房屋常被视为一种财务投资，但也伴随着时间、压力和灵活性降低等隐性成本。相比之下，租房提供了可预测性，但控制权较少。这篇文章从个人财务角度探讨了这些权衡。

**社区讨论**: 评论者分享了不同的经历：一些人强调维护的时间负担，而另一些人则强调控制权和稳定性带来的心理好处。少数人指出租房也有隐性成本，如不稳定性。总体而言，讨论证实了作者细致入微的观点。

**标签**: `#personal finance`, `#housing`, `#home ownership`, `#lifestyle`, `#cost analysis`

---

<a id="item-12"></a>
## [DynIP 推出支持 RFC 2136、IPv6、DNSSEC 的现代动态 DNS](https://dynip.dev/) ⭐️ 7.0/10

DynIP 是一项新的动态 DNS 服务，原生支持 RFC 2136/TSIG 更新、IPv6、DNSSEC 以及自带域名（BYOD）。它允许 FortiGate 和 MikroTik 路由器等设备无需自定义客户端即可更新 DNS 记录。 大多数现有动态 DNS 服务依赖专有的 HTTP-only 协议，缺乏对 IPv6 的完善支持，且忽视 DNSSEC。DynIP 填补了这些空白，使动态 DNS 更安全，并与现代网络和路由器兼容。 该服务将 RFC 2136 DNS UPDATE 和 TSIG 认证作为首要方法，同时提供 HTTP API。它支持端到端 IPv6 和 DNSSEC 签名，以实现认证的数据完整性。

hackernews · dynip · May 26, 07:35 · [社区讨论](https://news.ycombinator.com/item?id=48276363)

**背景**: 动态 DNS（DDNS）允许拥有变化 IP 地址的设备保持固定的域名。RFC 2136 定义了动态 DNS 更新的标准协议，而 DNSSEC 则对 DNS 响应添加了加密安全性。许多 DDNS 服务使用自定义 HTTP API，与企业路由器不兼容且缺乏安全特性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ietf.org/rfc/rfc2136.txt">ietf.org/ rfc / rfc 2136 .txt</a></li>
<li><a href="https://en.wikipedia.org/wiki/DNSSEC">DNSSEC</a></li>

</ul>
</details>

**社区讨论**: 创建者 Daniel 解释了动机和功能，评论者称赞了 RFC 2136 支持以及与 external-dns 和 Kubernetes 的兼容性。有人指出登录页面缺乏个性，但整体兴趣很高，用户将 DynIP 与自建 BIND 方案进行了比较。

**标签**: `#DNS`, `#Dynamic DNS`, `#IPv6`, `#DNSSEC`, `#Networking`

---

<a id="item-13"></a>
## [Stack Overflow 论坛衰落但公司仍盈利](https://sherwood.news/tech/stack-overflow-forum-dead-thanks-ai-but-companys-still-kicking-ai/) ⭐️ 7.0/10

由于 ChatGPT 等 AI 工具的兴起以及长期存在的有毒社区文化，Stack Overflow 论坛的用户参与度大幅下降，但公司本身仍然保持盈利。 这凸显了 AI 对传统知识共享平台构成的生存威胁，并引发了关于在大型语言模型时代社区驱动型问答网站可持续性的问题。 作者指出，论坛下滑与 2021 年被私募股权公司 Prosus 收购以及 ChatGPT 的推出相关，但许多评论者认为平台的文化问题早于这些事件。

hackernews · geerlingguy · May 26, 17:17 · [社区讨论](https://news.ycombinator.com/item?id=48282709)

**背景**: Stack Overflow 是一个面向程序员的流行问答平台，托管了数百万个问题和答案。多年来，它一直是获取编程帮助的首选资源，但严格的审核和游戏化系统为新手营造了不友好的环境。能够直接回答编码问题的 AI 模型的兴起，进一步降低了访问论坛的必要性。

**社区讨论**: 评论者表达了复杂的情绪：有些人因论坛的有毒文化而乐见其衰落，而另一些人则担心人类 curated 的知识流失会影响未来的 AI 训练。还有人批评文章忽视了私募股权收购对平台衰落的影响。

**标签**: `#stack-overflow`, `#ai-impact`, `#community-culture`, `#knowledge-platforms`, `#tech-industry`

---

<a id="item-14"></a>
## [年轻人中结直肠癌发病率上升](https://dynomight.net/crc-rates/) ⭐️ 7.0/10

一篇分析流行病学数据的博文指出，结直肠癌（CRC）在年轻一代中的发病率正在上升，这与历史趋势相反。文章强调，虽然绝对风险仍然较低，但增长幅度显著，值得关注。 这一趋势挑战了结直肠癌只影响老年人的普遍观念，可能导致年轻人诊断延误。提高意识可以促使更早筛查和生活方式改变，降低死亡率并改善预后。 在多个国家和出生队列中都观察到了这一增长，饮食和肥胖等生活方式因素被怀疑是原因之一。但文章警告不要在年轻人群中广泛筛查，因为绝对风险较低且存在潜在危害。

hackernews · surprisetalk · May 26, 16:00 · [社区讨论](https://news.ycombinator.com/item?id=48281539)

**背景**: 结直肠癌是全球第三大常见癌症，传统上发生在老年人中。结肠镜检查可以通过切除癌前息肉来预防癌症。最近的研究表明，50 岁以下人群的 CRC 发病率正在上升，饮食、久坐生活方式和微生物组变化可能是驱动因素。

**社区讨论**: 评论者分享了个人经历，许多人强调结肠镜检查没有想象的那么可怕，并且可以挽救生命。一些人看到同龄人受影响后改变了饮食习惯。总体情绪支持提高意识和筛查，并对博文的坦诚分析表示感谢。

**标签**: `#health`, `#colorectal cancer`, `#preventive healthcare`, `#epidemiology`

---

<a id="item-15"></a>
## [欧盟初步裁定：谷歌或违反《数字市场法》](https://t.me/zaihuapd/41566) ⭐️ 7.0/10

欧盟委员会发布初步调查结果，认为 Alphabet/谷歌通过在其搜索结果中优先展示自家服务，并在 Google Play 商店中设置限制，违反了《数字市场法》（DMA）。 这可能为谷歌等“守门人”在欧盟的运营树立重要先例，迫使它们改变搜索排名和应用商店政策，从而增加竞争和消费者选择。 初步意见聚焦于谷歌搜索在购物、航班和酒店等领域的自我偏好行为，以及 Play 商店规则限制开发者引导用户至其他购买渠道。尽管谷歌已采取合规措施，但委员会认为这些措施仍不足。

telegram · zaihuapd · May 26, 00:27

**背景**: 《数字市场法》（DMA）是欧盟的一项法规，适用于被指定为“守门人”的大型在线平台，要求它们确保公平竞争。该法于 2023 年 5 月全面适用，禁止自我偏好等行为。Alphabet 因其多项核心平台服务（包括谷歌搜索和 Android）被指定为守门人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Markets_Act">Digital Markets Act</a></li>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>

</ul>
</details>

**标签**: `#EU`, `#Google`, `#Digital Markets Act`, `#antitrust`, `#regulation`

---

<a id="item-16"></a>
## [支付宝推出 Token Pay 及 AI 钱包，助力智能体经济](https://finance.sina.com.cn/jjxw/2026-05-26/doc-inhzffss1524895.shtml) ⭐️ 7.0/10

2026 年 5 月 26 日，支付宝发布了两项新服务：面向大模型公司的支付方案 Token Pay，以及让消费者管理 AI 智能体支付的 AI 钱包。MiniMax、阶跃星辰等合作伙伴已接入支付宝的相关服务。 此次发布标志着大型金融科技公司正式进军 AI 原生支付领域，为 AI 智能体自主执行交易的“智能体经济”提供支撑，有望确立 AI 生态中支付处理的标准。 Token Pay 支持全球用户订阅和端内充 Token 等场景；AI 钱包直接集成在支付宝 App 内，用户可在交易前、中、后全程监督和管理 AI 智能体的支付行为。支付宝的 AI 支付套件现已支持 95% 的通用智能体框架。

telegram · zaihuapd · May 26, 12:31

**背景**: 支付宝是蚂蚁集团旗下的核心数字支付平台。Token Pay 是为大模型公司设计的结算产品，用于处理全球用户的支付；AI 钱包则为消费者提供了对 AI 智能体发起支付的管控层。这两项服务是支付宝为智能体商业时代打造的全栈式 AI 支付基础设施的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thepaypers.com/payments/news/alipay-launches-full-stack-ai-payment-suite-with-ai-wallet-and-token-pay">Alipay launches AI Wallet and Token Pay for agentic... | The Paypers</a></li>
<li><a href="https://www.techrepublic.com/article/news-apac-alipay-ai-wallet-token-pay-ai-agents/">Alipay Launches AI Payment Tools for Shopping Agents - TechRepublic</a></li>
<li><a href="https://coinlaw.io/alipay-ai-wallet-token-pay-agentic-commerce/">Alipay Debuts AI Wallet to Power Agentic Commerce</a></li>

</ul>
</details>

**标签**: `#Alipay`, `#Token Pay`, `#AI wallet`, `#fintech`, `#payment`

---