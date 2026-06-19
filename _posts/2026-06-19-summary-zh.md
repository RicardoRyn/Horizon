---
layout: default
title: "Horizon Summary: 2026-06-19 (ZH)"
date: 2026-06-19
lang: zh
---

> From 37 items, 18 important content pieces were selected

---

1. [Project Valhalla 抵达 JDK 28：值类型与堆扁平化](#item-1) ⭐️ 9.0/10
2. [EFF 推动免费法庭记录，新法案取代 PACER](#item-2) ⭐️ 8.0/10
3. [业余语言学家借助 AI 声称部分破译 Linear A](#item-3) ⭐️ 8.0/10
4. [零接触 OAuth 简化 MCP 企业认证](#item-4) ⭐️ 8.0/10
5. [中国就分布式数字身份互通互认征求意见](#item-5) ⭐️ 8.0/10
6. [桑德斯提案：美国人每年获 AI 分红 1000 美元](#item-6) ⭐️ 8.0/10
7. [苹果同意在巴西开放第三方应用商店](#item-7) ⭐️ 8.0/10
8. [ATProto 没有实例：架构澄清](#item-8) ⭐️ 7.0/10
9. [现代汽车完全收购波士顿动力公司](#item-9) ⭐️ 7.0/10
10. [新法案旨在限制政府对在线平台的言论压制](#item-10) ⭐️ 7.0/10
11. [亚马逊放弃山姆·奥特曼传记片](#item-11) ⭐️ 7.0/10
12. [GitHub Models 停止新用户注册，现有用户不受影响](#item-12) ⭐️ 7.0/10
13. [美国施压 ASML 怀疑 EUV 光刻机流入中国](#item-13) ⭐️ 7.0/10
14. [谷歌为 Android 侧载未验证应用引入 24 小时等待期](#item-14) ⭐️ 7.0/10
15. [印度封锁 Telegram 致 VPN 注册量飙升 150%](#item-15) ⭐️ 7.0/10
16. [SpaceX IPO 前向中国及俄罗斯投资者出售股份](#item-16) ⭐️ 7.0/10
17. [英国总检察长因假信息担忧弃用 X 平台](#item-17) ⭐️ 7.0/10
18. [北航前博士生指控教授论文造假](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Project Valhalla 抵达 JDK 28：值类型与堆扁平化](https://www.jvm-weekly.com/p/project-valhalla-explained-how-a) ⭐️ 9.0/10

经过十年研发，Project Valhalla 在 JDK 28 中引入了值类型和堆扁平化，从根本上改变了 Java 应用的内存布局和性能特性。 这对 JVM 来说是一次重大范式转变，使 Java 在保持类型安全和抽象的同时，实现接近手动内存管理语言的内存密度和性能。 值类型允许对象直接存储在数组和字段中，无需对象头和不必要间接引用，但堆扁平化仅适用于能容纳在 64 位内的对象；更大的对象仍有开销。JEP 401 引入了无身份的值类，其行为类似基本类型。

hackernews · philonoist · Jun 19, 06:35 · [社区讨论](https://news.ycombinator.com/item?id=48595511)

**背景**: Project Valhalla 是一个 2014 年宣布的 OpenJDK 项目，由 Brian Goetz 领导，旨在通过值类型增强 Java 对象模型。目前 Java 中每个对象都有身份和对象头；值类型去除了这些以实现更紧凑的内存布局。堆扁平化将值对象密集地打包到数组和字段中，减少内存使用和缓存未命中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Valhalla_(Java_language)">Project Valhalla (Java language) - Wikipedia</a></li>
<li><a href="https://openjdk.org/projects/valhalla/">Project Valhalla - OpenJDK</a></li>
<li><a href="https://cr.openjdk.org/~jrose/values/flattened-values.html">encodings for flattened heap values</a></li>

</ul>
</details>

**社区讨论**: 评论呈现复杂情绪：有人批评扁平化仅适用于小于 64 位对象的限制，也有人为设计选择辩护并称赞进展。一个常见主题是许多评论者对 Java 的看法已过时，而这个长达十年的项目被视为重大成就。

**标签**: `#project valhalla`, `#java`, `#jvm`, `#value types`, `#jdk 28`

---

<a id="item-2"></a>
## [EFF 推动免费法庭记录，新法案取代 PACER](https://www.eff.org/deeplinks/2026/06/court-records-should-be-free) ⭐️ 8.0/10

电子前哨基金会（EFF）正在推动一项法案，该法案将用现代化、统一且免费访问的平台取代过时的 PACER 和 CM/ECF 系统，用于联邦法庭记录。 该法案可能取消当前按页收费的模式，这种模式阻碍了公众获取法庭记录，从而大幅提升司法系统的透明度和公平性。 拟议立法旨在用现代化平台取代老旧的 PACER 和 CM/ECF 系统，从而改善网络安全、降低长期成本，并确保公众免费访问。

hackernews · hn_acker · Jun 19, 17:34 · [社区讨论](https://news.ycombinator.com/item?id=48600946)

**背景**: PACER（公共访问法院电子记录）是当前访问联邦法庭文件的系统，但按页收费（每页 10 美分），被广泛批评为过时且昂贵。CM/ECF 是法院用于电子归档的系统。虽存在 CourtListener 和 Recap 浏览器扩展等免费替代方案，但它们依赖于用户自愿分享已购买的文档。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pacer.uscourts.gov/">Public Access to Court Electronic Records | PACER : Federal Court ...</a></li>
<li><a href="https://upsolve.org/learn/pacer-guide/">PACER Guide: How To Get Your Court Notices Without an Attorney</a></li>
<li><a href="https://blogs.ubalt.edu/legaldatadesign/links/court-document-research-tools-beta/">Court Document Research Tools – Legal Data & Design Clinic</a></li>

</ul>
</details>

**社区讨论**: 社区评论提到了 CourtListener 和 Recap 等现有工具，这些工具有助于绕过 PACER 收费，有人希望该法案能让这些工具过时。一位评论者开玩笑说"可能只对人类免费"，表达了怀疑态度，另一个人则指出网站 courtwatch.us 是另一个免费替代方案。

**标签**: `#legal tech`, `#open government`, `#PACER`, `#court records`, `#transparency`

---

<a id="item-3"></a>
## [业余语言学家借助 AI 声称部分破译 Linear A](https://aiclambake.com/clamtakes/linear-a/) ⭐️ 8.0/10

业余语言学家 Tom Di Mino 使用 AI 编码代理 Claude Code 创建了 Python 脚本，交叉比对 Linear A 语料库，声称已部分翻译超过 300 个单词，该工作正在罗格斯大学和剑桥大学接受专家审查。 如果得到验证，这将是首个成功破译 Linear A 的案例，该文字一个多世纪以来一直困扰着学者。这也展示了像 Claude Code 这样的 AI 工具如何加速历史语言学和密码学领域的研究。 翻译基于“奠酒公式”——Linear A 中最常被研究的重复短语。语料库非常小，仅约 7500 个字符，分散在 1500 条铭文中。Di Mino 的方法产生了一致的结果，还解决了一些与 Linear A 相关的 Linear B 文字中的问题。

hackernews · Kosturdistan · Jun 19, 16:04 · [社区讨论](https://news.ycombinator.com/item?id=48600107)

**背景**: Linear A 是米诺斯文明在公元前 1800 年至 1450 年间使用的一种未破译文字，于 1900 年由亚瑟·埃文斯重新发现。该文字与 Linear B 共享许多字形，后者在 1950 年代被破译为早期希腊语。由于语料库极小且缺乏已知的双语文本，破译工作极其困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Linear_A_script">Linear A script</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 评论持谨慎乐观态度，指出该工作正在接受学术审查。一位认识 Di Mino 的评论者证实了其可信度，并指出他的方法产生了成果。另一位评论者强调，Claude Code 被用于构建工具而非作为黑箱求解器，这被认为是 AI 的积极应用。

**标签**: `#Linear A`, `#AI`, `#linguistics`, `#Claude Code`, `#cryptography`

---

<a id="item-4"></a>
## [零接触 OAuth 简化 MCP 企业认证](https://blog.modelcontextprotocol.io/posts/enterprise-managed-auth/) ⭐️ 8.0/10

Anthropic 与合作伙伴为 MCP 推出了企业托管授权（EMA），采用零接触 OAuth 流程和新 ID-JAG 令牌格式，通过企业身份提供商实现自动认证。 这消除了终端用户的逐应用 OAuth 配置，为企业集中化安全控制，极大简化了 AI 工具在大型组织中的采用。 该零接触流程使用名为 ID-JAG（身份断言 JWT 授权授权）的新令牌格式，这是一种 OAuth 断言，可在共享同一 SSO 提供商的应用程序间工作。

hackernews · niyikiza · Jun 18, 21:54 · [社区讨论](https://news.ycombinator.com/item?id=48592163)

**背景**: MCP（模型上下文协议）是一种开放协议，使 AI 代理能够访问外部工具和数据。此前，每个 MCP 服务器需要单独的 OAuth 设置。企业托管授权（EMA）标准化了这一过程，允许组织通过其身份提供商控制访问，用户无需额外步骤。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.modelcontextprotocol.io/posts/enterprise-managed-auth/">Enterprise-Managed Authorization: Zero - touch OAuth for MCP</a></li>
<li><a href="https://modelcontextprotocol.io/docs/tutorials/security/authorization">Understanding Authorization in MCP - Model Context Protocol</a></li>
<li><a href="https://dev.to/kanywst/id-jag-deep-dive-1mhp">ID-JAG Deep Dive - DEV Community</a></li>

</ul>
</details>

**社区讨论**: 社区反馈总体积极，突出了安全和用户体验的改进。开发者指出 ID-JAG 令牌并非 MCP 专用，可用于通用的跨应用数据共享。一些用户对当前的 Entra ID 实现表示沮丧，但 Anthropic 的 David 表示他们正在扩展支持。

**标签**: `#OAuth`, `#MCP`, `#AI Authentication`, `#Enterprise`, `#Security`

---

<a id="item-5"></a>
## [中国就分布式数字身份互通互认征求意见](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

国家网信办于 2026 年 6 月 18 日发布《促进分布式数字身份互通互认应用规定（征求意见稿）》，向社会公开征求意见至 2026 年 7 月 18 日，旨在利用区块链技术推动分布式数字身份的互通互认。 该规定可能为中国建立分布式数字身份的国家框架，实现跨金融、交通、海关、税务及数字人民币等领域的安全、用户自主的身份验证，影响数百万用户和企业。 征求意见稿将分布式数字身份定义为由标识符、密钥、可验证凭证和可验证声明构成，基于区块链技术。其提出依托国家区块链网络建设身份链，允许境内外个人、机构和工业设备自愿注册。

telegram · zaihuapd · Jun 19, 01:39

**背景**: 分布式数字身份（DDID）允许用户拥有并控制自己的身份数据，无需依赖中央权威机构，通常使用 W3C 标准定义的去中心化标识符（DID）和可验证凭证（VC）。区块链提供防篡改账本以锚定 DID 并建立信任。该规定旨在与国际标准接轨，同时在中国法律框架下解决数据安全和隐私问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://identitymanagementinstitute.org/distributed-digital-identity-and-decentralized-identifier/">Distributed Digital Identity and Decentralized Identifier</a></li>
<li><a href="https://en.wikipedia.org/wiki/Verifiable_credentials">Verifiable credentials</a></li>
<li><a href="https://w3c-ccg.github.io/did-primer/">A Primer for Decentralized Identifiers</a></li>

</ul>
</details>

**标签**: `#distributed digital identity`, `#blockchain`, `#regulation`, `#China`, `#data security`

---

<a id="item-6"></a>
## [桑德斯提案：美国人每年获 AI 分红 1000 美元](https://www.washingtonpost.com/business/2026/06/18/bernie-sanders-proposes-wealth-fund-give-americans-stake-ai/) ⭐️ 8.0/10

参议员伯尼·桑德斯提出立法，要求大型人工智能公司每年向每位美国公民支付 1000 美元分红，从而让公众直接持有这些公司的股权。 这一提案是一项重要的政策努力，旨在将人工智能未来创造的财富广泛分配给全体民众，而非集中于少数企业。它可能重塑 AI 利润的分配方式，并影响更广泛的监管讨论。 该立法要求最大的 AI 公司让美国人直接持有所有权股份，转化为每人每年 1000 美元的分红。总统特朗普此前也表达过类似想法，让政府在这些公司中拥有权益。

telegram · zaihuapd · Jun 19, 09:45

**背景**: 随着人工智能的持续发展，人们对财富不平等以及 AI 经济利益集中在少数科技巨头手中的担忧日益加剧。像桑德斯这样的政策制定者正在探索如何确保 AI 带来的繁荣能够与更广泛的公众共享，类似于来自自然资源的主权财富基金。

**标签**: `#AI政策`, `#财富分配`, `#桑德斯`, `#美国政治`, `#人工智能`

---

<a id="item-7"></a>
## [苹果同意在巴西开放第三方应用商店](https://t.me/zaihuapd/42059) ⭐️ 8.0/10

苹果已与巴西反垄断监管机构达成协议，允许 iPhone 用户在 App Store 之外购买应用和服务，并支持第三方应用商店分发，从而结束了一项反竞争行为调查。 该协议标志着苹果在重要市场上对 iOS 应用分发和支付控制的显著放松，可能为其他国家树立先例，迫使苹果在全球范围内调整其商业模式。 苹果需在 105 天内落实相关改变，协议为期三年；开发者可展示外部支付方式和替代购买链接，苹果的支付系统将与 App Store 解耦，但苹果仍可能对交易收取费用。

telegram · zaihuapd · Jun 19, 11:15

**背景**: 苹果的 App Store 长期以来被批评要求应用内购买必须使用其支付系统并收取高达 30%的佣金。欧盟《数字市场法案》下的类似监管行动已迫使苹果在欧洲允许替代应用商店和外部支付。巴西的决定与移动生态系统更加开放的全球趋势一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/118110">About alternative app distribution - Apple Support</a></li>
<li><a href="https://www.inspirevisual.com/blog/top-best-ios-app-store-list-alternatives/">The Best Alternative App Stores for iOS in 2026</a></li>
<li><a href="https://support.apple.com/en-us/117767">Installing apps through alternative app distribution - Apple Support</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#App Store`, `#Apple`, `#Brazil`, `#third-party payments`

---

<a id="item-8"></a>
## [ATProto 没有实例：架构澄清](https://overreacted.io/there-are-no-instances-in-atproto/) ⭐️ 7.0/10

文章解释称，Bluesky 背后的 ATProto 协议没有像 Mastodon 那样的“实例”；相反，它将中继、应用视图和个人数据服务器（PDS）分离为独立的模块化组件，并用 RSS 类比来说明架构。 这一澄清解决了对 Bluesky 去中心化模型的常见误解，并凸显了与 ActivityPub 在架构上的根本差异，这可能导致在可扩展性、可移植性和运营复杂性方面出现不同的权衡。 在 ATProto 中，中继充当内容无关的数据传输通道，应用视图消费中继的 firehose 以提供应用特定的索引和搜索，而 PDS 托管用户数据。这种分离允许每个组件独立扩展，这与 Mastodon 单个实例处理所有功能不同。

hackernews · danabramov · Jun 19, 15:10 · [社区讨论](https://news.ycombinator.com/item?id=48599515)

**背景**: ATProto 是 Bluesky 开发的去中心化社交网络协议。在 Mastodon 和其他基于 ActivityPub 的系统中，每个服务器（实例）负责存储用户数据、提供内容以及与其他实例联邦。ATProto 将这些角色解耦为独立的服务：中继（数据分发）、应用视图（内容索引和展示）和个人数据服务器（用户数据存储）。这种设计旨在提高性能和灵活性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.bsky.app/docs/advanced-guides/atproto">The AT Protocol | Bluesky - docs.bsky.app</a></li>
<li><a href="https://atproto.wiki/en/wiki/reference/core-architecture/appview">AppViews | AT Protocol Community Wiki</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了 RSS 类比的准确性，指出 RSS 源是自给自足的，而 ATProto 的应用视图依赖于中继；还有人认为，尽管实现了模块化分离，架构本质上仍是客户端-服务器模式而非对等网络。

**标签**: `#ATProto`, `#Bluesky`, `#decentralized social media`, `#protocol comparison`, `#ActivityPub`

---

<a id="item-9"></a>
## [现代汽车完全收购波士顿动力公司](https://startupfortune.com/hyundai-takes-full-control-of-boston-dynamics-as-softbank-exits-for-325-million/) ⭐️ 7.0/10

软银行使看跌期权，将其持有的波士顿动力剩余 9%股份出售给现代汽车，从而使现代完全拥有这家机器人公司。 此举正式确立了现代对波士顿动力的控制权，可能加速先进机器人在制造业及其他领域的商业化，尤其是在韩国机器人密度高且劳动力老龄化背景下。 现代汽车于 2020 年 12 月以 8.8 亿美元收购了波士顿动力 80%的股份，当时公司估值 11 亿美元，软银现已行使看跌期权出售剩余 9%股份。

hackernews · ck2 · Jun 19, 16:28 · [社区讨论](https://news.ycombinator.com/item?id=48600312)

**背景**: 波士顿动力以 Atlas（人形机器人）和 Spot（四足机器人）等先进机器人闻名。此次收购符合现代向机器人和自动化领域拓展的战略，尤其是在制造业方面。韩国在制造业中拥有全球最高的机器人密度，2024 年每万名员工拥有 1220 台机器人。

**社区讨论**: 评论者就人形机器人与专用机器人的优劣展开辩论，有人质疑现代对人形设计的侧重。另有人指出此次收购可利用韩国劳动年龄人口下降和高机器人密度的趋势，暗示其可拓展至汽车制造之外的工业自动化领域。

**标签**: `#robotics`, `#acquisition`, `#Boston Dynamics`, `#Hyundai`, `#manufacturing automation`

---

<a id="item-10"></a>
## [新法案旨在限制政府对在线平台的言论压制](https://www.eff.org/deeplinks/2026/06/new-bill-takes-aim-government-pressure-silence-lawful-online-speech) ⭐️ 7.0/10

参议员克鲁兹和怀登提出了一项两党法案，旨在防止政府机构施压在线平台删除合法言论，电子前哨基金会对此表示强烈支持。 该法案解决了政府对内容审核过度干预的日益担忧，保护了在线言论自由，代表了科技政策领域罕见的跨党派合作。 该法案由共和党人泰德·克鲁兹和民主党人罗恩·怀登共同提出，体现了广泛的政治支持。EFF 以其为代表的 ICEBlock 应用创建者案例来说明政府施压行为。

hackernews · hn_acker · Jun 19, 17:34 · [社区讨论](https://news.ycombinator.com/item?id=48600950)

**背景**: 政府机构日益施压社交媒体平台删除内容，且往往未经正当程序。这引发了第一修正案方面的担忧，尤其是当内容本身合法时。该法案旨在为此类互动设定明确界限。

**社区讨论**: EFF 文章下的评论反应不一：一些人称赞两党合作和巧妙的缩写（JAWBONE），而另一些人则对克鲁兹的动机表示怀疑。有用户提出在言论自由与平台问责之间取得平衡的挑战。

**标签**: `#online speech`, `#government regulation`, `#EFF`, `#privacy`, `#tech policy`

---

<a id="item-11"></a>
## [亚马逊放弃山姆·奥特曼传记片](https://www.the-independent.com/arts-entertainment/films/news/sam-altman-biopic-amazon-openai-deal-b2999321.html) ⭐️ 7.0/10

亚马逊在宣布与 OpenAI 合作后，决定不发行关于 OpenAI CEO 山姆·奥特曼的传记片《Artificial》，并表示该片由其他工作室发行会更合适。 这凸显了科技巨头拥有电影制片厂时产生的利益冲突，亚马逊与 OpenAI 的商业关系可能影响其放弃一部可能负面描绘奥特曼的电影。 该片由卢卡·瓜达尼诺执导，试映反响良好，亚马逊正在为其寻找新发行商（如 A24），而非完全搁置该项目。

hackernews · theanonymousone · Jun 19, 20:03 · [社区讨论](https://news.ycombinator.com/item?id=48602639)

**背景**: 亚马逊通过其米高梅工作室投资原创电影。山姆·奥特曼是 OpenAI（ChatGPT 背后的公司）的 CEO。这一情况反映了当媒体由拥有其他商业利益的公司所有时，媒体独立性的更广泛担忧。

**社区讨论**: 社区评论指出，亚马逊处理得当，帮助寻找新发行商而非封杀该片。一些评论者指出科技平台拥有工作室的政教分离问题，其他人则就相关话题开玩笑。

**标签**: `#Amazon`, `#OpenAI`, `#Sam Altman`, `#biopic`, `#corporate conflict`

---

<a id="item-12"></a>
## [GitHub Models 停止新用户注册，现有用户不受影响](https://github.blog/changelog/2026-06-16-github-models-is-no-longer-available-to-new-customers/) ⭐️ 7.0/10

GitHub 宣布其 AI 模型服务 GitHub Models 自 2026 年 6 月 16 日起停止接受新客户。现有用户可继续使用该服务，但这是完全退役的第一步。 这一变化影响计划使用 GitHub Models 进行 AI 原型开发和集成的开发者和组织。它标志着新项目应转向 Azure AI Foundry 作为推荐平台。 GitHub Models 提供了来自 OpenAI、Meta、Microsoft 等模型的 Playground 和 API 访问。该服务对现有用户仍可用，直至未来确定的退役日期，并提供了迁移到 Azure AI Foundry 的指导。

telegram · zaihuapd · Jun 19, 00:54

**背景**: GitHub Models 是一个通过网页 Playground 和 API 推理进行 AI 模型原型设计和实验的平台。它提供了来自多个提供商的模型访问。Azure AI Foundry 是微软用于构建和部署 AI 代理的托管平台，提供超过 1,800 个模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/GitHub_Models">GitHub Models</a></li>
<li><a href="https://grokipedia.com/page/Microsoft_Foundry_Agent_Service">Microsoft Foundry Agent Service</a></li>

</ul>
</details>

**标签**: `#GitHub Models`, `#AI model service`, `#GitHub`, `#Azure AI`, `#product update`

---

<a id="item-13"></a>
## [美国施压 ASML 怀疑 EUV 光刻机流入中国](https://www.bloomberg.com/news/articles/2026-06-19/us-tells-asml-it-s-concerned-china-may-have-top-chip-tool) ⭐️ 7.0/10

美国商务部长卢特尼克向 ASML 表示，担心一台顶级 EUV 光刻机可能已违反出口管制流入中国，但 ASML 坚决否认。 这一争端可能加剧中美技术战紧张局势，并影响全球半导体供应链，因为 ASML 的 EUV 光刻机是先进芯片制造的关键。 ASML 表示，全球运行的 314 台 EUV 光刻机均不在中国，且从未向中国出口过整机或专用组件。美国声称有证据但未出示。

telegram · zaihuapd · Jun 19, 03:09

**背景**: 极紫外（EUV）光刻是一种用于制造最先进微芯片的尖端技术，波长仅为 13.5 纳米。ASML 是 EUV 光刻机的独家制造商，使其成为半导体制造的关键工具。美国已实施出口管制以防止中国获得此类技术，但在合规问题上仍存在紧张局势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography">Extreme ultraviolet lithography - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/ASML">ASML - Wikipedia</a></li>

</ul>
</details>

**标签**: `#ASML`, `#US-China tech war`, `#semiconductor`, `#export controls`, `#EUV`

---

<a id="item-14"></a>
## [谷歌为 Android 侧载未验证应用引入 24 小时等待期](https://t.me/zaihuapd/42054) ⭐️ 7.0/10

谷歌公布了 Android 安装未验证开发者应用的新‘高级流程’，要求用户在安装前等待 24 小时。流程包括开启开发者模式、确认并非被诱导、重启手机并重新验证身份。 这一变化旨在降低用户被诈骗分子诱导安装不安全应用的风险。它为侧载增加了摩擦，可能保护不太懂技术的用户，但也可能给合法的高级用户带来不便。 在 24 小时冷静期后，用户必须通过指纹、面容识别或设备 PIN 确认才能继续安装。完成后，这项权限可设为 7 天或长期有效。

telegram · zaihuapd · Jun 19, 07:59

**背景**: Android 允许从官方 Google Play 商店之外侧载应用，这提供了灵活性但也带来了安全风险。诈骗分子经常诱导用户侧载恶意应用。谷歌逐步增加了安全措施，如验证开发者身份，以应对这一问题。

**标签**: `#Android`, `#sideloading`, `#security`, `#Google`

---

<a id="item-15"></a>
## [印度封锁 Telegram 致 VPN 注册量飙升 150%](https://t.me/zaihuapd/42058) ⭐️ 7.0/10

印度于 6 月 16 日至 22 日临时封锁 Telegram，以防止医学入学重考（NEET-UG）中出现作弊。此举导致印度 VPN 注册量激增 150%，Proton VPN 报告其每小时注册量较平日飙升超过 150%。 这一事件凸显了政府审查与互联网自由之间的紧张关系，以及使用 BGP 劫持进行审查可能带来的意外全球影响。同时也反映出用户对绕过限制的 VPN 依赖日益增加。 封锁通过印度电信运营商实施 BGP 路由劫持强行阻断流量，意外导致阿联酋等其他国家的 Telegram 用户也无法使用。BGP 劫持是指破坏互联网路由表来重定向流量。

telegram · zaihuapd · Jun 19, 10:30

**背景**: BGP（边界网关协议）是互联网上用于引导数据的路由协议。BGP 劫持发生在某个网络虚假声明拥有 IP 前缀所有权，从而将流量重定向到自身。Telegram 是一款以加密著称的即时通讯应用，在印度广泛使用。印度政府此前曾因考试作弊问题下令关闭互联网。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BGP_hijacking">BGP hijacking - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proton_VPN">Proton VPN</a></li>
<li><a href="https://www.cloudflare.com/learning/security/glossary/bgp-hijacking/">What is BGP hijacking? - Cloudflare</a></li>

</ul>
</details>

**标签**: `#internet censorship`, `#Telegram`, `#VPN`, `#BGP hijacking`, `#India`

---

<a id="item-16"></a>
## [SpaceX IPO 前向中国及俄罗斯投资者出售股份](https://www.propublica.org/article/spacex-elon-musk-ipo-foreign-investors-china) ⭐️ 7.0/10

ProPublica 获得的法院解密文件显示，SpaceX 在 2018 年至 2021 年间通过中间商 Tomales Bay Capital 向位于中国大陆、香港和俄罗斯的投资者出售股份，尽管后来因合规风险禁止这些投资者参与其 IPO。 这项调查凸显了 SpaceX 因承担美国敏感军事项目而面临的重大合规和地缘政治风险，也揭示了科技公司在管理外国投资（尤其是来自潜在利益冲突国家的投资）所面临的挑战。 每笔股份购买金额从 80 万到 4000 万美元不等，投资者包括与中国军工承包商有联系的个人以及卡塔尔王室关联实体。投资者被承诺可获得季度更新、参观公司及采访首席财务官等特殊接触。

telegram · zaihuapd · Jun 19, 12:00

**背景**: SpaceX 是美国主要的航空航天制造商和发射服务提供商，经常承担机密军事合同。该公司上周上市，估值从 2019 年的 333 亿美元飙升至 2.7 万亿美元。IPO 通常涉及严格的合规审查，以确保没有受禁实体持有股份。

**标签**: `#SpaceX`, `#IPO`, `#compliance`, `#geopolitics`, `#investigation`

---

<a id="item-17"></a>
## [英国总检察长因假信息担忧弃用 X 平台](https://www.theguardian.com/technology/2026/jun/18/uk-attorney-general-tells-staff-stop-using-x-disinformation-concerns) ⭐️ 7.0/10

英国总检察长理查德·赫默要求其部门停止在 X（原推特）上发帖，使该部门成为首个因担忧假信息和煽动暴力而弃用该平台的英国政府机构。 此举标志着英国政府在社交媒体监管方面可能转向更严格的立场，尤其是在与在线仇恨言论相关的暴力事件发生后。它可能为其他政府部门树立先例，并影响关于平台责任的公共辩论。 这一决定是在 6 月初南安普敦和贝尔法斯特发生暴力事件后做出的，这些事件加剧了对 X 被用来散播种族仇恨和分裂社区的担忧。赫默是推动加强在线监管的内阁成员之一，包括禁止 16 岁以下青少年使用社交媒体以及修订《在线安全法》。

telegram · zaihuapd · Jun 19, 15:30

**背景**: X（原推特）是一个主要社交媒体平台，2022 年被埃隆·马斯克收购后，内容审核政策有所放松。英国 2023 年通过的《在线安全法》要求平台处理非法内容，但批评者认为执法不力。总检察长是英国政府的首席法律顾问，负责监督严重犯罪的起诉，并在法律政策中发挥关键作用。

**标签**: `#social media`, `#disinformation`, `#government regulation`, `#UK`, `#X`

---

<a id="item-18"></a>
## [北航前博士生指控教授论文造假](https://www.zaobao.com.sg/news/china/story20260619-9231002) ⭐️ 7.0/10

前北航博士生耿江涛指控该校两名教授——常凌乾和王军——在发表论文中伪造数据，大量网民涌入学校官网查阅，导致网站一度瘫痪。 这一事件突显了中国学术界对科研诚信的持续担忧，以及独立科学监督者在社交媒体上的影响力日益增强，能够迅速引发公众关注和机构回应。 耿某称常凌乾在《自然》杂志上发表的论文数据“完美到诡异”，王军的两篇论文数据前后矛盾。耿某此前曾举报其他高校的五名研究人员，均已被处理。

telegram · zaihuapd · Jun 19, 16:02

**背景**: 学术不端行为（包括数据伪造）是中国科研界长期存在的问题。像耿某这样的独立博主已成为监督者，利用公共平台曝光疑似造假行为。公众的迅速反应可以迫使高校展开调查。

**标签**: `#academic misconduct`, `#Beihang University`, `#paper falsification`, `#research integrity`

---