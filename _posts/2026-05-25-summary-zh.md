---
layout: default
title: "Horizon Summary: 2026-05-25 (ZH)"
date: 2026-05-25
lang: zh
---

> From 35 items, 16 important content pieces were selected

---

1. [教皇通谕批判技术伦理影响](#item-1) ⭐️ 9.0/10
2. [APKPure 上的 Telegram 官方版发现间谍后门](#item-2) ⭐️ 9.0/10
3. [加州拟豁免 Linux 免于年龄验证法律，此前遭强烈反对](#item-3) ⭐️ 8.0/10
4. [C 语言扩展与编译器间可移植性](#item-4) ⭐️ 8.0/10
5. [从 Go 迁移到 Rust：指南与权衡辩论](#item-5) ⭐️ 8.0/10
6. [华为提出“韬定律”：时间缩微替代摩尔定律](#item-6) ⭐️ 8.0/10
7. [Epic 公布虚幻引擎 6，《火箭联盟》从 UE3 直接升级](#item-7) ⭐️ 8.0/10
8. [Mullvad 推出 VPN 出口 IP 指纹识别缓解措施](#item-8) ⭐️ 7.0/10
9. [荷兰查封 800 台服务器，逮捕 2 名网络犯罪帮凶](#item-9) ⭐️ 7.0/10
10. [IBM 剥离出首家纯代工量子芯片工厂](#item-10) ⭐️ 7.0/10
11. [Audiomass：免费开源的多轨网页音频编辑器](#item-11) ⭐️ 7.0/10
12. [DeepSeek Reasonix：原生编码智能体，高缓存低成本](#item-12) ⭐️ 7.0/10
13. [微软因社区反对取消 244 英亩数据中心计划](#item-13) ⭐️ 7.0/10
14. [人工智能时代网络安全招聘激增](#item-14) ⭐️ 7.0/10
15. [马斯克宣布 Grok V9-Medium 模型训练完成](#item-15) ⭐️ 7.0/10
16. [离体人脑用于药物测试](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [教皇通谕批判技术伦理影响](https://www.vatican.va/content/leo-xiv/en/encyclicals/documents/20260515-magnifica-humanitas.html) ⭐️ 9.0/10

教皇利奥十四世于 2026 年 5 月 15 日发布通谕《崇高人性》，对包括人工智能和生物技术在内的现代技术进行了全面的伦理批判。 作为重要机构的声音，梵蒂冈在技术伦理上的立场可能影响全球讨论和政策。该通谕挑战技术构建者和监管者去思考技术权力的社会与道德维度。 文件警告技术绝非中立，设计者和资助者承担特殊的伦理责任。它还质疑谁掌握着人工智能等技术的权力以及如何使用这些权力。

hackernews · theletterf · May 25, 10:11 · [社区讨论](https://news.ycombinator.com/item?id=48265206)

**背景**: 教皇通谕是教皇就重要问题向天主教会及更广泛世界发表的正式信件。《崇高人性》延续了梵蒂冈关注现代伦理困境的传统，此前已有关于生态和社会正义的声明。

**社区讨论**: 评论者普遍赞扬该通谕的深思熟虑，一位无神论者称其为机构对技术的最佳见解之一。其他人则强调了对构建者考虑其影响的呼吁，一些人讨论了历史案例和阿米什人对技术评估的方法。

**标签**: `#technology ethics`, `#papal encyclical`, `#AI`, `#society`, `#power dynamics`

---

<a id="item-2"></a>
## [APKPure 上的 Telegram 官方版发现间谍后门](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

在 APKPure 上发现一个被重新打包的 Telegram 12.6.5 版本，其中包含名为 DataCollector 的间谍框架，嵌入在 classes3.dex 中，代码超过 3000 行。 这款广泛使用的消息应用在热门第三方应用商店中被植入后门，构成了严重的隐私威胁，因为该后门可以窃取聊天记录、通讯录、照片、GPS 等信息，可能影响数百万用户。 该间谍软件使用 AES-GCM 加密窃取的数据，并上传至命令与控制服务器 38.190.225.166。它针对的是 APKPure 上的 Telegram 官方版本，而非 Google Play 或 Telegram 官方网站的版本。

telegram · zaihuapd · May 24, 11:38

**背景**: APKPure 是一个第三方 Android 应用商店，提供 APK 文件下载，常被用于下载地区限制应用或旧版本。虽然方便，但这类商店存在应用被篡改的风险。在 Android 中，大型应用使用多个 DEX 文件（如 classes.dex、classes2.dex）来绕过 64K 方法数限制；间谍软件就隐藏在 classes3.dex 中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/APKPure">APKPure</a></li>
<li><a href="https://www.nyxtbig.com/apkpure/">Unlocking Android's Hidden Gems: The Truth About APKPure in 2024</a></li>
<li><a href="https://developer.android.com/build/multidex">Enable multidex for apps with over 64K methods | Android Studio | Android Developers</a></li>

</ul>
</details>

**标签**: `#security`, `#spyware`, `#Telegram`, `#malware`, `#data breach`

---

<a id="item-3"></a>
## [加州拟豁免 Linux 免于年龄验证法律，此前遭强烈反对](https://www.tomshardware.com/software/linux/california-moves-to-exempt-linux-from-its-upcoming-age-verification-law-after-backlash-over-forcing-operating-systems-to-collect-users-ages-amendment-proposed-by-the-same-lawmaker-who-wrote-the-original-law) ⭐️ 8.0/10

加州议员提出对 AB 1856 法案的修正案，在技术社区的强烈反对后，拟豁免 Linux 发行版及其他开源操作系统免受该州年龄验证法律的约束。 这一豁免可能为年龄验证法律如何对待开源软件树立先例，但其他操作系统以及更广泛的言论自由影响仍令人担忧。 该豁免 specifically 针对 Linux 发行版，但可能不涵盖所有开源操作系统；例如，SteamOS 由于其与 Steam 的集成，可能仍需进行年龄验证。

hackernews · rbanffy · May 25, 18:19 · [社区讨论](https://news.ycombinator.com/item?id=48269961)

**背景**: 加州的年龄验证法律 AB 1856 最初要求所有操作系统在用户访问成人内容时验证其年龄。这引发了强烈反对，因为这将迫使像 Linux 这样的开源操作系统实施此类措施，许多人认为这违反了言论自由并施加了不合理的负担。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/California-AB-1856">California 's Age Verification Law May End Up Exempting... - Phoronix</a></li>
<li><a href="https://sesamedisk.com/california-age-verification-law-os-implications/">California ’s Age Verification Law : Impact on Operating Systems</a></li>

</ul>
</details>

**社区讨论**: 评论者对动机表示怀疑，一些人认为豁免是为了防止 Linux 开发者以第一修正案为由挑战该法律。其他人指出，该法律将负担转嫁给了消费者，并强调家长控制更为有效。

**标签**: `#policy`, `#linux`, `#age-verification`, `#open-source`, `#regulation`

---

<a id="item-4"></a>
## [C 语言扩展与编译器间可移植性](https://lemon.rip/w/6-c-extensions-compilers/) ⭐️ 8.0/10

一篇文章和社区讨论强调了将依赖于编译器特定扩展（如 GCC 的__attribute__）的 C 代码移植到 Clang、TCC 及业余编译器时面临的长期挑战。 这很重要，因为许多实际 C 项目使用了 GCC 特定扩展，限制了向其他编译器和平台的可移植性。讨论表明，即使是经验丰富的编译器实现者也难以找到变通方法，这表明需要更好的标准化或工具支持。 文章指出，就连 Clang 也必须对 GCC 的#include_next 扩展进行变通处理，项目经常使用 defined(__GNUC__)等条件宏来检测编译器特性。社区评论指出，这些检查往往不完整，在非 GCC 编译器上会失效。

hackernews · xngbuilds · May 25, 14:15 · [社区讨论](https://news.ycombinator.com/item?id=48267126)

**背景**: 像 GCC 和 Clang 这样的 C 编译器会添加非标准语言扩展以提高性能或便利性。这些扩展（例如__attribute__）不属于 ISO C 标准。当代码使用这些扩展时，可能无法在不支持它们的其他编译器上编译，从而需要通过特性检测宏或回退机制来变通。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lemon.rip/w/6-c-extensions-compilers/">On C extensions, portability, and alternative compilers</a></li>
<li><a href="https://en.wikipedia.org/wiki/GNU_Compiler_Collection">GNU Compiler Collection - Wikipedia</a></li>
<li><a href="https://clang.llvm.org/docs/LanguageExtensions.html">Clang Language Extensions — Clang 23.0.0git documentation</a></li>

</ul>
</details>

**社区讨论**: ImportC 实现者 WalterBright 描述他花了大量时间处理头文件中的各种'胡闹'。whizzter 批评了那些依赖于编译器检查而不考虑 Windows 和 FreeBSD 等平台的项目。fuhsnn 分享了帮助业余编译器处理主流代码库的资源。

**标签**: `#C programming`, `#portability`, `#compilers`, `#language extensions`, `#software engineering`

---

<a id="item-5"></a>
## [从 Go 迁移到 Rust：指南与权衡辩论](https://corrode.dev/learn/migration-guides/go-to-rust/) ⭐️ 8.0/10

一篇从 Go 迁移到 Rust 的详细指南发布，引发了关于两种语言之间权衡的细致讨论，特别是关于托管运行时和包管理方面的优劣。 这场讨论凸显了在后端开发中，托管运行时（Go）与系统级控制（Rust）之间的永恒选择，影响着开发者对每种语言最佳适用场景的判断。 该指南指出 Go 冗长的错误处理与 Rust 的'?'操作符之间的对比，同时社区评论提到 Go 的标准库涵盖了 Rust 需要依赖外部 crate 的许多需求。

hackernews · jabits · May 24, 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48259808)

**背景**: Go 使用垃圾回收器（托管运行时）实现内存安全，而 Rust 通过其所有权模型在没有 GC 的情况下实现内存安全。包管理也不同：Go 使用模块并注重标准库覆盖，而 Rust 依赖 Cargo 和 crates.io 管理依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Garbage_collection_(computer_science)">Garbage collection (computer science) - Wikipedia</a></li>
<li><a href="https://doc.rust-lang.org/book/ch04-00-understanding-ownership.html">Understanding Ownership - The Rust Programming Language</a></li>
<li><a href="https://app.studyraid.com/en/read/15009/518899/go-modules-vs-other-package-managers">Understand go Modules vs other package managers</a></li>

</ul>
</details>

**社区讨论**: 来自 Animats 和 tptacek 等专家的评论强调，选择通常归结为是否需要托管运行时。其他人指出 Rust 的依赖树可能更大，因为标准库功能较少。一些评论者怀疑原始文档的风格存在 AI 生成的痕迹。

**标签**: `#Go`, `#Rust`, `#language comparison`, `#migration`, `#web backends`

---

<a id="item-6"></a>
## [华为提出“韬定律”：时间缩微替代摩尔定律](https://www.peopleapp.com/column/30052220655-500007509895) ⭐️ 8.0/10

在 2026 年上海国际电路与系统研讨会上，华为发表了“韬定律”，这是一种用时间缩微替代传统几何缩微的半导体演进新原则。华为声称过去六年已据此设计量产了 381 款芯片，并计划今年秋季推出采用“逻辑折叠”技术的新麒麟手机芯片。 如果“韬定律”被验证有效，它将使半导体发展超越摩尔定律的物理极限，在不依赖纯粹晶体管缩小的情况下提供性能和密度提升的新路径。这对受制于先进制程工艺获取的华为及其他公司尤为重要，可能重塑芯片行业的竞争格局。 该定律使用统一优化目标——时间常数τ，涵盖从单个晶体管到数据中心工作负载的十二个数量级。关键使能技术包括“逻辑折叠”以及跨越器件、电路、芯片和系统的多层次协同优化机制，目标是在 2031 年实现相当于 1.4 纳米制程的晶体管密度。

telegram · zaihuapd · May 25, 01:35

**背景**: 传统半导体缩微遵循摩尔定律和 Dennard 缩微理论，主要通过缩小晶体管尺寸（几何缩微）来每 18-24 个月翻倍密度并提升性能。随着物理极限逼近，进一步几何缩微变得愈发困难且昂贵。“韬定律”提出另一种思路：通过逻辑折叠和系统级协同优化等创新，降低控制信号传播延迟的时间常数（τ），从而以“时间缩微”而非“尺寸缩微”的方式实现性能提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.futunn.com/en/post/73585128/huawei-has-unveiled-the-tao-s-law-what-technological-directions">Huawei has unveiled the 'Tao's Law'—what technological directions warrant attention?</a></li>
<li><a href="https://www.yicaiglobal.com/news/huawei-presents-tau-law-to-replace-geometric-scaling-with-time-scaling-in-semiconductor-industry">Huawei Presents Tau Law to Replace Geometric Scaling With Time Scaling in Semiconductor Industry</a></li>
<li><a href="https://www.gizmochina.com/2026/05/25/huawei-previews-kirin-2026-chip-with-higher-transistor-density-and-efficiency/">Huawei previews Kirin 2026 chip with higher transistor density and...</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#chip design`, `#Moore's Law`, `#Huawei`, `#innovation`

---

<a id="item-7"></a>
## [Epic 公布虚幻引擎 6，《火箭联盟》从 UE3 直接升级](https://www.pcgamer.com/gaming-industry/epic-reveals-first-unreal-engine-6-game-and-its-not-fortnite/) ⭐️ 8.0/10

这标志着虚幻引擎的一次重大代际跃升，可能解决 UE5 的优化批评，同时表明 Epic 通过《堡垒之夜》等游戏推动元宇宙的战略。《火箭联盟》从 UE3 跳到 UE6 展示了显著的技术革新。 《火箭联盟》自 Xbox 360 时代以来一直运行在 UE3 上，此次引擎升级堪比推出续作。UE6 预告片还包含了《堡垒之夜》等游戏的镜头，暗示一个统一平台。

telegram · zaihuapd · May 25, 02:20

**背景**: 虚幻引擎是 Epic Games 开发的游戏引擎，广泛应用于游戏和影视行业。四年前发布的 UE5 引入了 Nanite 和 Lumen 等先进技术，但在 PC 端因优化问题受到批评。2006 年发布的 UE3 是最早支持多线程和 DirectX 9 的引擎之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unreal_Engine_6">Unreal Engine 6</a></li>
<li><a href="https://en.wikipedia.org/wiki/Unreal_Engine_3">Unreal Engine 3</a></li>

</ul>
</details>

**标签**: `#Unreal Engine`, `#Epic Games`, `#Rocket League`, `#game development`, `#metaverse`

---

<a id="item-8"></a>
## [Mullvad 推出 VPN 出口 IP 指纹识别缓解措施](https://mullvad.net/en/help/exit-ip-vpn-servers-mitigation-rollout) ⭐️ 7.0/10

Mullvad 已推出缓解措施，通过改变出口 IP 地址的分配方式来防止出口 IP 指纹识别。 这一更新至关重要，因为出口 IP 指纹识别可能允许第三方跨网站追踪用户，从而削弱 VPN 的隐私保护。通过解决这一问题，Mullvad 增强了用户匿名性，并为其他 VPN 提供商树立了隐私标准。 该缓解措施可能涉及将用户分布到更多出口 IP 或随机化分配，从而打破此前可用于指纹识别的模式。Mullvad 的博客文章和服务器列表提供了该推出的技术细节。

hackernews · Cider9986 · May 25, 17:45 · [社区讨论](https://news.ycombinator.com/item?id=48269580)

**背景**: 出口 IP 指纹识别是一种利用一致的 VPN 出口 IP 地址来关联用户在不同服务上活动的技术，尽管真实 IP 被隐藏。与许多 VPN 在众多用户之间共享少量 IP 不同，Mullvad 此前为每个服务器分配多个出口 IP，这些 IP 可能随时间被指纹识别。此次缓解措施旨在防止这种关联。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberinsider.com/mullvad-vpn-exit-ip-patterns-could-enable-user-fingerprinting/">Mullvad VPN exit IP patterns could enable user fingerprinting</a></li>
<li><a href="https://swissvpn.pro/en/blog/browser-fingerprinting-protection">What Is Browser Fingerprinting & How to Stop It... | Swiss VPN Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者建议直接链接到 Mullvad 的博客文章以澄清，指出 Mullvad 浏览器的内置代理可避免此问题，并表达了在 LibreWolf 等浏览器中标准化伪造配置文件以进一步对抗指纹识别的愿望。

**标签**: `#VPN`, `#privacy`, `#IP fingerprinting`, `#Mullvad`, `#security`

---

<a id="item-9"></a>
## [荷兰查封 800 台服务器，逮捕 2 名网络犯罪帮凶](https://krebsonsecurity.com/2026/05/netherlands-seizes-800-servers-arrests-2-for-aiding-cyberattacks/) ⭐️ 7.0/10

荷兰当局查封了 800 台服务器，并逮捕了两名运营“防弹托管”服务的嫌疑人，该服务为网络犯罪分子（包括俄罗斯情报机构的幌子公司）提供基础设施。 此次行动捣毁了一个大型网络犯罪助纣为虐的机构，凸显出国际社会日益重视摧毁那些为非法活动提供庇护的防弹托管服务。 被查封的服务器被用于托管僵尸网络命令与控制服务器、恶意软件分发及其他非法操作，且该托管服务提供商涉嫌充当俄罗斯情报机构的幌子。

hackernews · jruohonen · May 25, 13:56 · [社区讨论](https://news.ycombinator.com/item?id=48266906)

**背景**: 防弹托管是指无视滥用投诉、继续提供非法内容的互联网托管服务，通常运营在法律规定较为宽松的地区。此类服务是网络犯罪基础设施的关键组成部分，为从垃圾邮件到勒索软件攻击等各种活动提供了支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bulletproof_hosting">Bulletproof hosting</a></li>
<li><a href="https://english.nv.ua/nation/russian-orthodox-church-used-as-kgb-front-for-decades-says-sbu-general-ukraine-news-50318187.html">Russian Orthodox Church used as KGB front for decades says SBU...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，这些托管公司不仅仅是态度宽松，而是直接作为俄罗斯情报机构的幌子运作；有用户声称它们专门为犯罪分子服务，合法客户无法使用。其他人对荷兰在网络攻击来源统计中的突出地位表示惊讶，并推测其与当地的数据隐私法律及托管环境有关。

**标签**: `#cybersecurity`, `#law enforcement`, `#Netherlands`, `#cyberattacks`, `#hosting`

---

<a id="item-10"></a>
## [IBM 剥离出首家纯代工量子芯片工厂](https://futurumgroup.com/insights/2-billion-chips-act-investment-in-quantum-bets-on-ibms-300mm-superconducting-silicon/) ⭐️ 7.0/10

IBM 将其量子芯片制造业务剥离，成立名为 Anderon 的独立纯代工厂，获得总计 20 亿美元投资，其中 10 亿美元来自《芯片法案》。这打造了首个不依附于整合器件制造商的专用量子芯片代工厂。 此举将量子硬件研发与 IBM 咨询主导的企业结构分离，有望加速创新。同时为其他量子公司提供共享的制造基础设施，降低门槛并加快行业发展。 该代工厂名为 Anderon，将位于纽约州，专注于使用 300 毫米硅晶圆制造超导量子芯片。作为纯代工厂，它将为其他公司制造芯片而不自行设计产品，遵循台积电的模式。

hackernews · rbanffy · May 25, 09:43 · [社区讨论](https://news.ycombinator.com/item?id=48265056)

**背景**: 量子计算芯片传统上需要专用实验室。纯代工厂为其他公司制造芯片而不自行设计，这一模式由台积电开创。《芯片法案》提供政府资金以促进国内半导体制造。IBM 此前在 Watson 项目上的困境凸显了在咨询主导的母公司内部商业化先进技术的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quantumzeitgeist.com/billion-chips-award-backs-ibms/">$1 Billion CHIPS Award Backs IBM’s Quantum Foundry Build</a></li>
<li><a href="https://cryptobriefing.com/us-government-2b-quantum-computing-ibm/">US government and IBM plan $2 billion quantum foundry in New York</a></li>
<li><a href="https://www.bipphoenix.com/ibm-plans-2b-quantum-chip-foundry-government-will-pay-half">IBM's $2B quantum chip foundry gets $1B US grant</a></li>

</ul>
</details>

**社区讨论**: 评论者对剥离普遍持积极态度，有人指出这使量子业务脱离了 IBM 的“审计与咨询”文化。他们赞赏独立代工厂可以为多家公司服务，惠及整个生态系统。也有人批评文章存在亲 IBM 倾向且可读性差。

**标签**: `#quantum computing`, `#IBM`, `#semiconductor foundry`, `#CHIPS Act`, `#spin-off`

---

<a id="item-11"></a>
## [Audiomass：免费开源的多轨网页音频编辑器](https://audiomass.co/?multitrack=1) ⭐️ 7.0/10

Audiomass 是一款免费开源的多轨音频编辑器，以渐进式 Web 应用 (PWA) 形式发布，支持离线使用，用户无需安装即可在浏览器中直接编辑音频。 该工具通过提供专业质量、免费替代付费软件的方式，实现了音频编辑的民主化，完全在浏览器中运行并支持离线。其 PWA 特性使其可在任何配备现代浏览器的设备上访问，降低了音乐制作和音频编辑的门槛。 该应用支持多轨编辑、采样导入和基本效果，使用标准 Web 技术（HTML、CSS、JavaScript）构建。它开源，允许社区贡献和代码审计。

hackernews · pantelisk · May 24, 15:25 · [社区讨论](https://news.ycombinator.com/item?id=48258015)

**背景**: 渐进式 Web 应用 (PWA) 是一种利用现代 Web 能力提供类原生应用体验的 Web 应用，包括可安装到主屏幕、离线功能和快速加载。PWA 使用标准 Web 技术（HTML、CSS、JavaScript）构建，并借助 Service Worker 实现离线缓存。这免去了为不同平台开发单独原生应用的需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Progressive_web_app">Progressive web app</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps">Progressive web apps | MDN</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，用户称赞其离线功能和复古的编码风格。有用户希望增加云端协作功能，也有用户报告了双击样本后卡顿等可用性问题。总体而言，该工具因其简洁和无强制广告而受到赞赏。

**标签**: `#audio editing`, `#open source`, `#web app`, `#PWA`, `#productivity`

---

<a id="item-12"></a>
## [DeepSeek Reasonix：原生编码智能体，高缓存低成本](https://esengine.github.io/DeepSeek-Reasonix/) ⭐️ 7.0/10

DeepSeek Reasonix 发布，这是一款开源的终端 AI 编码智能体，深度集成 DeepSeek 的前缀缓存机制，大幅降低 token 成本。 该智能体具有自定义单元格差异渲染器和一流的 MCP 支持，但一些用户质疑其必要性，因为通用桥接也可利用缓存优势。

hackernews · Alifatisk · May 24, 13:02 · [社区讨论](https://news.ycombinator.com/item?id=48256953)

**背景**: AI 编码智能体通过重复生成提示来执行任务，可能导致高昂的 token 成本。DeepSeek V4 Pro 提供 100 万 token 上下文窗口和混合专家架构，而提示缓存通过在不同请求间复用已缓存的前缀 token 来降低成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://esengine.github.io/DeepSeek-Reasonix/">Reasonix — DeepSeek - native AI coding agent</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek -ai/ DeepSeek - V 4 - Pro · Hugging Face</a></li>
<li><a href="https://rejoicehub.com/blogs/prompt-caching-llms-reduce-ai-api-costs">Prompt Caching in LLMs: Reduce AI API Costs by 81%</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：部分用户构建了简单桥接实现类似缓存效果，质疑专用智能体的必要性。另有用户批评网站用户体验，并建议用 Rust 或 Go 实现以提升性能。

**标签**: `#AI coding agent`, `#DeepSeek`, `#caching`, `#low cost`

---

<a id="item-13"></a>
## [微软因社区反对取消 244 英亩数据中心计划](https://www.tmj4.com/news/racine-county/microsoft-pulls-plug-on-plans-for-244-acre-data-center-in-caledonia-after-community-pushback) ⭐️ 7.0/10

微软已放弃在威斯康星州卡利多尼亚建造一个 244 英亩数据中心的计划，原因是遭到社区的强烈反对。这一取消标志着该公司在该地区云基础设施扩张的重大逆转。 这一事件凸显了科技公司对大型数据中心的需求与当地社区对土地使用和环境影响担忧之间日益加剧的紧张关系。它可能促使微软及其他云服务提供商重新评估选址策略和社区参与方式。 该 244 英亩的土地位于富士康此前计划建设大型工厂的附近，但该工厂未能建成，使居民对大型项目持怀疑态度。该数据中心将需要大量能源和水资源，加剧了环境担忧。

hackernews · cdrnsf · May 25, 13:09 · [社区讨论](https://news.ycombinator.com/item?id=48266422)

**背景**: 数据中心是容纳计算机服务器和网络设备的大型设施，对于云计算服务至关重要。它们消耗大量电力，并且通常需要大片土地和水源用于冷却。社区反对通常源于对噪音、环境影响以及破坏乡村风貌的担忧。

**社区讨论**: 社区评论突出了在富士康风波后的怀疑态度，一位用户指出该项目靠近失败的富士康项目，引发了当地的不信任。另一用户质疑 244 英亩数据中心的规模，而一位来自加拿大的评论者观察到，加拿大的反工业政策和邻避主义更为严重，解释了为何那里很少有此类项目。

**标签**: `#data centers`, `#Microsoft`, `#community opposition`, `#cloud infrastructure`, `#land use`

---

<a id="item-14"></a>
## [人工智能时代网络安全招聘激增](https://www.nytimes.com/2026/05/24/technology/one-job-that-is-growing-in-the-ai-era-cybersecurity-experts.html) ⭐️ 7.0/10

据《纽约时报》报道，人工智能时代对网络安全高管和工程师的需求激增，2026 年第一季度招聘量同比增长 11%，高管职位需求较去年秋季增加五到七倍。 这一趋势突显了来自人工智能模型（如 Anthropic 的 Mythos）的安全威胁日益复杂，这类模型能够发现软件漏洞，并强调了兼具安全专业知识与人工智能知识的专业人才的迫切需求。 高级安全岗位的薪酬包可达七八百万美元，安全工程师必须补充人工智能技能才能保持竞争力。部分猎头公司甚至因人手不足而拒绝客户。

telegram · zaihuapd · May 25, 06:21

**标签**: `#cybersecurity`, `#AI`, `#hiring`, `#security threats`

---

<a id="item-15"></a>
## [马斯克宣布 Grok V9-Medium 模型训练完成](https://x.com/elonmusk/status/2058787384364265734) ⭐️ 7.0/10

埃隆·马斯克宣布，拥有 1.5 万亿参数的 Grok V9-Medium 模型已完成训练，评估结果良好。经过微调和强化学习后，预计将在两到三周内向公众发布。 该新模型通过额外加入 Cursor 数据进行训练，相比当前在线的 Grok v8-small，在处理复杂编程任务时将有明显提升。这标志着 xAI 在大语言模型开发上的快速进展，可能挑战其他领先的 AI 模型。 Grok V9-Medium 基础模型拥有 1.5 万亿参数，并在训练中加入了大量 Cursor 数据。团队目前正在进行微调，几天后将启动强化学习，目标是在两到三周后向公众发布。

telegram · zaihuapd · May 25, 07:07

**背景**: Grok 是由埃隆·马斯克的 AI 公司 xAI 开发的大语言模型。模型规模通常用参数数量衡量，参数大致对应模型学习和存储信息的能力。之前的 Grok v8-small 版本有 0.5 万亿参数。Cursor 是一款 AI 驱动的代码编辑器，可提供编程辅助，其数据可能有助于提升模型的编码能力。

**标签**: `#AI`, `#Grok`, `#Elon Musk`, `#Large Language Models`, `#Machine Learning`

---

<a id="item-16"></a>
## [离体人脑用于药物测试](https://www.science.org/content/article/not-alive-not-dead-disembodied-human-brains-used-drug-testing) ⭐️ 7.0/10

美国生物科技公司 Bexorg 利用 BrainEx 灌流系统，在死亡数小时后恢复捐献大脑的部分代谢与细胞活动，用于测试阿尔茨海默病和帕金森病等神经疾病的药物。 这项技术挑战了当前对生死的定义，通过使用真实人脑组织而非动物模型，可能显著提高神经药物研发的成功率，同时引发关于意识与人类尊严的深刻伦理争论。 这些大脑并未恢复意识或完整神经活动，但研究引发担忧：现有伦理框架是否足以应对处于“半存活”状态的大脑，以及关于知情同意和生命边界的疑问。

telegram · zaihuapd · May 25, 14:57

**背景**: BrainEx 系统是一种灌流技术，通过输送营养和氧气来模拟自然血流，以维持细胞功能。传统上，脑灌流用于医学成像或研究循环，但将其应用于死亡后人脑是新颖的。这项研究基于早期的动物实验，旨在克服动物模型在神经疾病药物测试中的局限性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ventures.yale.edu/news/not-alive-not-dead-disembodied-human-brains-used-drug-testing">Not alive, but not dead: disembodied human brains used for drug ...</a></li>

</ul>
</details>

**标签**: `#neuroscience`, `#ethics`, `#drug testing`, `#consciousness`, `#biomedical research`

---