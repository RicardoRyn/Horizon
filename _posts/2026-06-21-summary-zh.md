---
layout: default
title: "Horizon Summary: 2026-06-21 (ZH)"
date: 2026-06-21
lang: zh
---

> From 35 items, 8 important content pieces were selected

---

1. [宁可重复代码，也不要错误的抽象](#item-1) ⭐️ 9.0/10
2. [如何用 Python 编写一个 Lisp 解释器（2010）](#item-2) ⭐️ 9.0/10
3. [新型三维光纤微镊实现十万倍传统光镊力](#item-3) ⭐️ 9.0/10
4. [Anthropic 要求使用 Claude 须提交政府身份证](#item-4) ⭐️ 8.0/10
5. [Loupe iOS 应用揭示原生应用数据访问](#item-5) ⭐️ 8.0/10
6. [开发者普遍不懂 CORS，2019 年文章揭示](#item-6) ⭐️ 8.0/10
7. [Polymarket 被指雇佣创作者制作虚假交易视频](#item-7) ⭐️ 8.0/10
8. [刘强东承诺对 70 万名快递员进行再培训以应对 AI 替代](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [宁可重复代码，也不要错误的抽象](https://sandimetz.com/blog/2016/1/20/the-wrong-abstraction) ⭐️ 9.0/10

Sandi Metz 在 2016 年的博客文章中提出，用错误的抽象消除代码重复比保留重复本身危害更大，倡导在正确的抽象浮现之前容忍重复。 这篇文章挑战了盲目应用 DRY 原则的做法，通过鼓励开发者优先考虑清晰性和灵活性而非过早抽象，影响了软件设计实践，有助于降低维护成本和错误风险。 Metz 强调错误的抽象会创建远距离耦合，且比重复代码更难重构；她建议在出现三个及以上实例之前，容忍重复是合理的。

hackernews · rafaepta · Jun 21, 16:08 · [社区讨论](https://news.ycombinator.com/item?id=48620090)

**背景**: DRY（不要重复自己）是一个旨在通过抽象减少重复的软件原则，但过早应用会导致代码僵化且脆弱。这篇文章是软件工程中关于平衡抽象与实用性更广泛讨论的一部分。

**社区讨论**: 评论者普遍同意盲目 DRY 有害，但就抽象的阈值和“单一事实来源”的角色存在争议。一些人认为函数式方法减少了抽象陷阱，另一些则强调共享代码必须真正服务于所有调用者。

**标签**: `#software engineering`, `#abstraction`, `#DRY`, `#code quality`, `#best practices`

---

<a id="item-2"></a>
## [如何用 Python 编写一个 Lisp 解释器（2010）](https://norvig.com/lispy.html) ⭐️ 9.0/10

Peter Norvig 发布了一篇详细指南，教读者如何用不到 100 行 Python 代码实现一个 Lisp 解释器，展示了语言实现的核心概念。 这篇教程为编写解释器和编译器提供了浅显易懂的入门指导，启发了无数开发者，并成为编程社区中广泛引用的经典资源。 该指南包含两个版本：一个不到 100 行的最小解释器，以及一个扩展版本，增加了宏、续延等特性，全部用 Python 编写。

hackernews · tosh · Jun 21, 15:36 · [社区讨论](https://news.ycombinator.com/item?id=48619831)

**背景**: Lisp 是最古老的编程语言之一，以其简洁的语法和强大的宏系统而闻名。解释器直接执行代码而无需编译，编写解释器有助于理解编程语言的内部工作原理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lisp_(programming_language)">Lisp (programming language) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区高度赞扬了这篇教程，称其为学习语言实现的最佳起点。评论中还提到了相关项目，如超轻量级的 R4RS Lisp 实现 Ribbit，以及 Norvig 的第二部分教程，增加了更多功能。

**标签**: `#Lisp`, `#Python`, `#interpreter`, `#compiler`, `#tutorial`

---

<a id="item-3"></a>
## [新型三维光纤微镊实现十万倍传统光镊力](https://www.stdaily.com/web/gdxw/2026-06/19/content_534836.html) ⭐️ 9.0/10

安徽大学与中国科学技术大学的研究团队利用飞秒激光复合制造方法，发明了一种新型三维光纤微镊。该成果发表于《自然》，其输出力是传统光镊的十万倍以上，能够对微米尺度物体进行高精度、低损伤的操控。 这一突破显著扩展了光操控的能力，不仅能操控透明物体，还能以高力操控不透明物体。它为单细胞操作、显微手术和生命科学研究提供了新工具，可能变革微尺度精密操作领域。 该微镊将光传输、光热转换、材料响应和微结构力学输出高度集成于同一根商用光纤。通过调节输入光功率即可连续精密控制输出力，其力达到了传统光镊的十万倍以上。

telegram · zaihuapd · Jun 20, 15:19

**背景**: 传统光镊利用高度聚焦的激光束捕获和操控微小物体，但作用力较弱（通常皮牛级），且无法操控不透明物体。传统机械微夹持器在狭小空间内精度受限。新方法采用飞秒激光复合制造，在光纤端部构建了聚合物微结构尖端，结合光刻胶支架和掺银纳米颗粒温敏水凝胶，将光能转化为机械力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wap.sciencenet.cn/mobile.php?type=detail&cat=news&id=566898&mobile=1">科学网-新型 三 维 光 纤 微 镊 面世</a></li>
<li><a href="https://news.sciencenet.cn/htmlnews/2026/6/566898.shtm">新型 三 维 光 纤 微 镊 面世—新闻—科学网</a></li>
<li><a href="https://www.cls.cn/detail/2404945">cls.cn/detail/2404945</a></li>

</ul>
</details>

**标签**: `#optical tweezers`, `#femtosecond laser`, `#micro-manipulation`, `#biomedical engineering`, `#nanotechnology`

---

<a id="item-4"></a>
## [Anthropic 要求使用 Claude 须提交政府身份证](https://support.claude.com/en/articles/14328960-identity-verification-on-claude) ⭐️ 8.0/10

Anthropic 宣布用户必须提交政府颁发的身份证和实时自拍才能使用 Claude 的部分功能，验证过程由第三方服务商 Persona 处理。 这一政策转变引发了重大的隐私担忧，可能限制全球对 AI 模型的访问，并引发了关于数据隐私和 AI 技术地缘政治限制的辩论。 Anthropic 表示不会将身份数据用于训练模型，但 Persona 可以使用这些数据改进欺诈预防系统。验证失败的用户可能被永久禁止访问顶级模型，这与 OpenAI 的政策类似。

hackernews · bathory · Jun 21, 12:44 · [社区讨论](https://news.ycombinator.com/item?id=48618455)

**背景**: 身份验证通常称为 KYC（了解你的客户），在金融服务中常见，用于防止欺诈。AI 公司越来越多地采取此类措施以符合法规并防止滥用。Anthropic 使用 Persona 等第三方供应商，将验证数据与模型训练数据分离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/14328960-identity-verification-on-claude">Identity verification on Claude | Claude Help Center</a></li>
<li><a href="https://www.explainx.ai/blog/anthropic-claude-id-verification-persona-fable-5-2026">Anthropic Claude ID Verification & Fable 5 Suspension ...</a></li>
<li><a href="https://cybersecuritynews.com/anthropic-updated-privacy-policy/">Anthropic Updated Privacy policy to Include Identity ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了强烈的隐私担忧，指出 Persona 可以使用身份数据训练自己的模型，非美国用户因访问限制增加而认为价值下降。有用户将这与网络中立性类比，担心用户被静默封禁。部分用户已取消订阅以示抗议。

**标签**: `#Anthropic`, `#Claude`, `#identity verification`, `#privacy`, `#AI policy`

---

<a id="item-5"></a>
## [Loupe iOS 应用揭示原生应用数据访问](https://github.com/mysk-research/loupe) ⭐️ 8.0/10

Loupe 是一款由 Mysk Research 开发的 iOS 应用，它向用户展示原生应用可以通过公共 iOS API 访问哪些私人数据。该应用读取系统 API 中的真实值并将其显示出来，凸显了任何第三方应用可访问的广泛指纹识别面。 这款应用提高了人们对 iOS 隐私漏洞的认识，因为许多用户不知道原生应用可以静默收集细粒度数据。它可能会促使苹果限制此类 API 访问或改进隐私透明度，最终影响开发者处理用户数据的方式。 Loupe 无需特殊权限即可读取诸如卷创建日期、剪贴板更改计数和已安装应用探测等值。该应用在 GitHub 和 App Store 上开源，其演示也可通过 Techlore 视频观看。

hackernews · Cider9986 · Jun 20, 12:08 · [社区讨论](https://news.ycombinator.com/item?id=48608645)

**背景**: iOS 原生应用可以访问各种系统 API，这些 API 可能泄露设备特定信息，从而实现指纹识别。例如，卷创建日期是一个唯一标识符，剪贴板更改计数可以追踪用户活动。苹果已添加了一些限制（例如要求使用白名单 URL scheme 进行应用检测），但许多 API 仍然开放。Loupe 通过展示任何应用可访问的真实数据来证明这一差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/mysk-research/loupe">GitHub - mysk-research/loupe: A privacy-focused iOS app that ...</a></li>
<li><a href="https://apps.apple.com/us/app/loupe-what-apps-can-see/id6766152470">Loupe: What Apps Can See App - App Store</a></li>
<li><a href="https://stateofsurveillance.org/news/loupe-ios-fingerprint-surface-passive-tier-2026/">Loupe Shows What iOS Apps See. The App Privacy Report Doesn't.</a></li>

</ul>
</details>

**社区讨论**: 评论者对卷创建日期和剪贴板更改计数等细粒度数据表示惊讶，并指出已安装应用探测比 Android 更有限但仍然令人担忧。一些人建议操作系统层面的模糊处理或网络访问选择加入作为缓解措施，而另一些人则赞赏与 Android 当前状态的比较。

**标签**: `#privacy`, `#iOS`, `#security`, `#mobile apps`, `#data access`

---

<a id="item-6"></a>
## [开发者普遍不懂 CORS，2019 年文章揭示](https://fosterelli.co/developers-dont-understand-cors) ⭐️ 8.0/10

一篇 2019 年的文章指出，大多数开发者根本误解了跨源资源共享（CORS），导致配置错误和安全风险。随之而来的 Hacker News 讨论（超过 300 条评论）证实了开发者对 CORS 目的和机制的普遍困惑。 CORS 是一项关键的 Web 安全机制，但持续存在的误解可能导致数据泄露和 CSRF 攻击等漏洞。这篇文章及社区讨论揭示了影响前后端开发者的重大教育缺口。 文章指出常见误解，例如认为 CORS 能阻止来自其他源的请求，而实际上它只限制读取响应。讨论还指出 CORS 头部经常配置错误，许多开发者靠试错而非理解同源策略来解决问题。

hackernews · toilet · Jun 21, 01:35 · [社区讨论](https://news.ycombinator.com/item?id=48614844)

**背景**: 跨源资源共享（CORS）是一种机制，允许 Web 服务器放宽浏览器的同源策略。同源策略通常限制一个源的脚本访问另一个源的资源。CORS 通过 HTTP 头部（如 Access-Control-Allow-Origin）工作，并由浏览器强制执行。对于某些复杂请求，浏览器会发送预检 OPTIONS 请求以检查服务器权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CORS">CORS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cross-origin_resource_sharing">Cross-origin resource sharing - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CORS">Cross-Origin Resource Sharing (CORS) - MDN Web Docs</a></li>

</ul>
</details>

**社区讨论**: 评论观点不一：部分用户认为文章本身也曲解了 CORS（例如声称 CORS 能限制哪些网站可以发起请求，这并不正确）。其他人坦承对 CORS 感到困扰，称他们调整头部直到生效，但并不真正理解。少数人指出 MDN 文档是有帮助的资源，而一位评论者称该讨论是他们见过的最无知的 HN 讨论。

**标签**: `#CORS`, `#web security`, `#developer misconceptions`, `#HTTP`

---

<a id="item-7"></a>
## [Polymarket 被指雇佣创作者制作虚假交易视频](https://www.wsj.com/business/media/polymarket-social-media-bets-prediction-market-441cdeb5) ⭐️ 8.0/10

《华尔街日报》调查发现，预测市场平台 Polymarket 雇用数十名年轻创作者，在模拟网站上制作虚假盈利交易视频，且未披露付费合作关系，此举可能违反美国联邦广告法。 这种做法破坏了人们对预测市场的信任，并可能使 Polymarket 面临监管处罚，尤其是该平台自 2022 年起已被禁止在美国提供主要加密交易服务。这也引发了人们对加密行业虚假营销的更广泛担忧。 在分析的 1,105 个视频中，70% 展示了总计 190 万美元的虚假下注；其中 118 个视频宣称赢得近 90 万美元，但这些交易实际上会亏损超过 16.6 万美元。Polymarket 回应称致力于市场透明，并计划全面审计现有推广内容。

telegram · zaihuapd · Jun 21, 06:31

**背景**: Polymarket 是一个去中心化的预测市场平台，于 2020 年推出，用户可以对选举或经济指标等未来事件的结果进行下注。预测市场允许参与者交易代表不同结果的份额，价格反映了市场对事件概率的估计。该平台自 2022 年起因监管问题被禁止向美国用户提供基于加密的交易服务，但仍通过社交媒体推广保持可访问性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/Polymarket">Polymarket - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**标签**: `#Polymarket`, `#prediction markets`, `#fake trading`, `#regulatory compliance`, `#crypto`

---

<a id="item-8"></a>
## [刘强东承诺对 70 万名快递员进行再培训以应对 AI 替代](https://finance.sina.com.cn/tob/2026-06-21/doc-inieeaqr2983650.shtml) ⭐️ 8.0/10

京东集团创始人刘强东在 2026 年 APEC 工商领导人中国论坛上宣布了'涅槃计划'，旨在对公司现有的 70 万名蓝领快递员进行技术培训，以应对人工智能和机器人取代送货岗位的趋势。 这一计划凸显了一位科技领袖对人工智能导致岗位流失的主动应对，可能为物流行业乃至更广泛领域的劳动力再培训树立先例。 刘强东表示，机器人最终将负责所有送货任务，但人类工人仍然需要进行维护和修理。经过再培训的工人将被转移到办公室岗位，改善工作条件。

telegram · zaihuapd · Jun 21, 08:05

**背景**: 京东运营着中国最大的配送网络之一，拥有约 70 万名蓝领工人。随着人工智能和自动化技术的发展，物流公司面临调整劳动力的压力。'涅槃计划'是京东的战略，旨在将这些工人过渡到技术岗位，而非裁员。

**标签**: `#AI`, `#automation`, `#workforce training`, `#logistics`, `#JD.com`

---