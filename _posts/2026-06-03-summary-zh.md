---
layout: default
title: "Horizon Summary: 2026-06-03 (ZH)"
date: 2026-06-03
lang: zh
---

> From 38 items, 20 important content pieces were selected

---

1. [Let's Encrypt 将推出后量子证书](#item-1) ⭐️ 10.0/10
2. [Elixir v1.20 引入渐进式类型系统](#item-2) ⭐️ 9.0/10
3. [Google 发布 Gemma 4 12B：无编码器的多模态模型](#item-3) ⭐️ 9.0/10
4. [DaVinci Resolve 21 以照片和动态图形工具挑战 Adobe](#item-4) ⭐️ 8.0/10
5. [优步每月 1500 美元 AI 使用上限为 AI 工具定价提供参考](#item-5) ⭐️ 8.0/10
6. [Pwnd Blaster：通过蓝牙攻击电脑的音箱破解](#item-6) ⭐️ 8.0/10
7. [乐鑫科技推出搭载 RISC-V 和 SIMD 的 ESP32-S31](#item-7) ⭐️ 8.0/10
8. [Meta 允许员工 30 分钟内选择不被追踪](#item-8) ⭐️ 8.0/10
9. [数学家警告 AI 快速进军数学研究](#item-9) ⭐️ 8.0/10
10. [原版 PlayStation 硬件的深度逆向工程分析](#item-10) ⭐️ 8.0/10
11. [英伟达携 CPU 杀入 PC 赛道，支持笔记本运行 120B 大模型](#item-11) ⭐️ 8.0/10
12. [SpaceX 计划以每股 135 美元固定价 IPO，筹资 750 亿美元](#item-12) ⭐️ 8.0/10
13. [千问向第三方 Agent 和 Skill 全面开放](#item-13) ⭐️ 8.0/10
14. [HTTP/2 炸弹攻击远程拖垮主流服务器](#item-14) ⭐️ 8.0/10
15. [苹果因需求强劲将 MacBook Neo 产量翻倍](#item-15) ⭐️ 7.0/10
16. [对 Java 内存优化中'每字节都要计较'思维的批判](#item-16) ⭐️ 7.0/10
17. [大规模代理服务封锁波及 VLESS 和 AnyTLS 协议](#item-17) ⭐️ 7.0/10
18. [谷歌允许网站退出 AI 搜索结果](#item-18) ⭐️ 7.0/10
19. [测试显示 64GB 内存是专业创作用户的甜点配置](#item-19) ⭐️ 7.0/10
20. [美国教师工会呼吁限制小学 AI 使用及课堂屏幕](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Let's Encrypt 将推出后量子证书](https://letsencrypt.org/2026/06/03/pq-certs) ⭐️ 10.0/10

Let's Encrypt 于 2026 年 6 月 3 日宣布，计划使用 Merkle Tree 证书 (MTC) 过渡到后量子证书，以抵御量子计算机的威胁。 这对 Web PKI 来说是开创性的一步，因为量子计算机可能破解当前的公钥密码学；它为整个行业迁移到抗量子标准树立了先例。 Merkle Tree 证书将公共日志记录集成到证书本身，减少了开销并使透明度成为发行的内在属性；即使使用大型后量子签名，它们的设计也比传统证书更高效。

hackernews · SGran · Jun 3, 15:06 · [社区讨论](https://news.ycombinator.com/item?id=48385114)

**背景**: 后量子密码学 (PQC) 是指被认为能够抵御量子计算机攻击的密码算法，量子计算机可能利用 Shor 算法破解 RSA 和 ECDSA 等广泛使用的算法。美国国家标准与技术研究院 (NIST) 已开始标准化 PQC 算法。Merkle Tree 证书是一种新的证书格式，旨在与 PQC 配合使用，以减少握手数据量并提高性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ietf.org/archive/id/draft-davidben-tls-merkle-tree-certs-09.html">Merkle Tree Certificates</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>

</ul>
</details>

**社区讨论**: 评论者对生活在面临量子风险的科幻未来表示兴奋，但也担心 MTC 会失去数十年的实战检验和辅助工具。一些人建议使用混合构造，并链接了一篇详细讨论混合 PQC 方法误解的博客文章。

**标签**: `#post-quantum cryptography`, `#Let's Encrypt`, `#certificates`, `#quantum computing`, `#security`

---

<a id="item-2"></a>
## [Elixir v1.20 引入渐进式类型系统](https://elixir-lang.org/blog/2026/06/03/elixir-v1-20-0-released/) ⭐️ 9.0/10

Elixir v1.20 于 2026 年 6 月 3 日发布，引入了渐进式类型支持，允许开发者可选地添加可由编译器检查的类型注解。 这是 Elixir 的一个里程碑式特性，因为它将静态类型检查引入了一种常用于高并发系统的动态语言，从而提高了代码可靠性和开发者生产力。 Elixir v1.20 中的渐进式类型系统基于 Elixir 核心团队的工作，允许混合使用类型化和未类型化的代码，并且不会像其他一些渐进式类型系统那样渐进性地降低程序性能。

hackernews · cloud8421 · Jun 3, 19:02 · [社区讨论](https://news.ycombinator.com/item?id=48388324)

**背景**: 渐进式类型是一种允许在相同语言中进行静态类型和动态类型的类型系统，由 Jeremy Siek 和 Walid Taha 于 2006 年提出。它允许程序员在部分代码中添加类型注解，同时保持其他部分无类型，从而在灵活性和安全性之间取得平衡。Elixir 最初是一种基于 Erlang 虚拟机（BEAM）的动态类型语言，长期以来社区一直渴望获得这样的特性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gradual_typing">Gradual typing</a></li>
<li><a href="https://jsiek.github.io/home/WhatIsGradualTyping.html">What is Gradual Typing | Jeremy Siek</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论显示，长期使用 Elixir 的开发者对此感到兴奋，但也有人担心性能影响以及渐进式类型是否符合 Elixir 类似 Lisp 的哲学。一些用户报告说，类型系统在不引入破坏性变更的情况下发现了他们现有代码中的错误。

**标签**: `#Elixir`, `#gradual typing`, `#programming languages`, `#release`, `#type systems`

---

<a id="item-3"></a>
## [Google 发布 Gemma 4 12B：无编码器的多模态模型](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/) ⭐️ 9.0/10

Google DeepMind 发布了 Gemma 4 12B，这是一个密集的无编码器多模态模型，无需独立的专用编码器，直接通过 LLM 主干处理视觉和音频输入。该模型基于 Apache 2.0 许可证发布，可在 16 GB 内存的笔记本电脑上运行。 这种方法挑战了依赖大型外部编码器（如用于视觉的 SigLIP）的传统多模态架构，有望减小模型规模和推理成本。它可能使多模态 AI 更加普及，允许在消费级硬件上本地部署，并推动无编码器设计的进一步研究。 该模型用轻量级嵌入模块替代了视觉编码器，该模块仅由一次矩阵乘法、位置嵌入和归一化组成，参数总量仅 35M。社区测试使用 Q4 量化版本配合 llama.cpp 运行，发现性能尚可，但偶尔会出现多余的括号或逗号等琐碎语法错误。

hackernews · rvz · Jun 3, 16:04 · [社区讨论](https://news.ycombinator.com/item?id=48385906)

**背景**: 大多数多模态大语言模型（如 GPT-4V、Gemini）会使用独立的预训练编码器来处理视觉（如 SigLIP，550M 参数）和音频（如 Whisper，300M 参数），这些编码器庞大且需要额外算力。无编码器模型则将原始模态直接输入 LLM 主干，简化架构并通常减少内存占用。Gemma 4 12B 是 Google 首个开源的无编码器多模态模型，源自其之前的 Gemma 系列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemma/gemma-4/">Gemma 4 — Google DeepMind</a></li>
<li><a href="https://www.marktechpost.com/2026/06/03/google-deepmind-releases-gemma-4-12b-an-encoder-free-multimodal-model-with-native-audio-that-runs-on-a-16-gb-laptop/">Google DeepMind Releases Gemma 4 12B: An Encoder - Free ...</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人称赞这种高效的架构和 Google 的开源发布策略，也有人质疑其商业动机（“闭环”），并指出图像处理质量一般。一位运行 Q4 量化版本的用户报告说性能尚可，但需要手动修复琐碎的语法错误，表明该模型可能仍需进一步改进。

**标签**: `#AI`, `#multimodal`, `#Google`, `#model`, `#encoder-free`

---

<a id="item-4"></a>
## [DaVinci Resolve 21 以照片和动态图形工具挑战 Adobe](https://www.blackmagicdesign.com/products/davinciresolve/whatsnew) ⭐️ 8.0/10

Blackmagic Design 发布了 DaVinci Resolve 21，新增了照片管理功能和动态图形工具，使其成为 Adobe Lightroom 和 After Effects 的直接竞争对手。 此次更新显著扩展了 DaVinci Resolve 在视频编辑之外的功能，有可能用单个免费或低成本工具替代多个订阅，并为 Linux 用户提供了一个强有力的选择。 新的照片管理功能包括专门的导入、组织和编辑工作流程，而动态图形增强则包括基于 Fusion 的高级工具，可削弱 After Effects 的基本用途。

hackernews · pentagrama · Jun 3, 14:18 · [社区讨论](https://news.ycombinator.com/item?id=48384482)

**背景**: DaVinci Resolve 是一款专业的视频编辑、调色和音频后期制作套件。21 版本将其范围扩展到照片管理和动态图形，直接与 Adobe 的专业应用竞争。Blackmagic Design 提供了功能丰富的免费版本和付费的 Studio 版本。

**社区讨论**: 评论者称赞这次更新，指出它可能是 Linux 上最好的照片编辑器，也是 After Effects 在基本动态图形方面的可行替代品。一些人讨论了 AI 驱动工作流程改进的潜力，而另一些人则分享了 Linux 兼容性问题的经验。

**标签**: `#davinci resolve`, `#video editing`, `#photo management`, `#motion graphics`, `#blackmagic design`

---

<a id="item-5"></a>
## [优步每月 1500 美元 AI 使用上限为 AI 工具定价提供参考](https://simonwillison.net/2026/Jun/3/uber-caps-usage/) ⭐️ 8.0/10

据彭博社 2026 年 6 月 2 日报道，优步将每位员工每月的 AI 工具支出上限设为 1500 美元，涉及 Claude Code 等工具，以控制成本。 这为企业的 AI 工具定价提供了现实参考，可能影响其他公司对 AI 的预算分配以及供应商的定价策略。 该上限约为优步软件工程师中位薪资的 11%；若全球企业效仿，AI 公司月收入可能达到约 450 亿美元。

hackernews · pdyc · Jun 3, 12:25 · [社区讨论](https://news.ycombinator.com/item?id=48383056)

**背景**: 像 Claude 这样的大型语言模型正通过 Claude Code 等工具越来越多地用于企业软件开发。定价通常按 token 计费，随着成本攀升，企业开始尝试设置使用上限。优步此举是首批公开的案例之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者指出应避免像循环运行‘claude -p’这样浪费 token 的做法，争论考虑完全加载成本后 1500 美元是否显得合理，并质疑在 DeepSeek 等低价替代品的竞争下，AI 供应商能否维持当前定价。

**标签**: `#AI pricing`, `#enterprise AI`, `#AI tools`, `#cost management`, `#Uber`

---

<a id="item-6"></a>
## [Pwnd Blaster：通过蓝牙攻击电脑的音箱破解](https://blog.nns.ee/2026/06/03/katana-badusb/) ⭐️ 8.0/10

安全研究员 Rasmus Muratz 演示了 Pwnd Blaster 攻击，该攻击无需配对即可通过蓝牙远程向 Creative Sound Blaster Katana V2X 音箱写入任意固件，将其变成键盘向主机电脑发送按键。 此攻击凸显了物联网设备安全中严重的供应商疏忽，因为 Creative 表示不认为这是漏洞。该方法可能被武器化，制造通过音频外设感染计算机的自传播蠕虫。 攻击利用了 Creative 的 CTU（Creative 传输协议），该协议缺乏加密或认证，允许任何蓝牙设备发送固件更新命令。研究者还发布了第三方补丁以禁用通过蓝牙刷写固件的功能。

hackernews · xx_ns · Jun 3, 10:53 · [社区讨论](https://news.ycombinator.com/item?id=48382310)

**背景**: 许多现代音箱和扬声器包含蓝牙用于音频流，但还隐藏了用于固件更新或数据传输的 USB 接口。当通过 USB 连接到计算机时，这类设备可被重新编程，伪装成人机接口设备（HID），如键盘，从而实施类似 BadUSB 的按键注入攻击。缺乏安全的固件更新机制使它们容易受到远程劫持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://citforum.ru/news/46687/">Исследователь описал атаку на Creative Sound Blaster Katana...</a></li>
<li><a href="https://www.mulliner.org/bluetooth/hidattack.php">HID Attack</a></li>

</ul>
</details>

**社区讨论**: 评论者批评 Creative 尽管风险明显却否认该漏洞的安全性。一些人指出通过供应链攻击传播蠕虫的可能性，另一些人赞赏研究员的详尽披露和第三方补丁的发布。

**标签**: `#security`, `#vulnerability`, `#bluetooth`, `#firmware`, `#hardware hack`

---

<a id="item-7"></a>
## [乐鑫科技推出搭载 RISC-V 和 SIMD 的 ESP32-S31](https://www.espressif.com/en/products/socs/esp32-s31) ⭐️ 8.0/10

乐鑫科技发布了 ESP32-S31，这是一款搭载 SIMD 指令的双核 RISC-V 微控制器，最高运行频率 320 MHz，通过标准 RISC-V 工具链简化了基于 Rust 的开发。 在流行的嵌入式平台上集成 RISC-V 和 SIMD 降低了 Rust 开发的入门门槛，开发者只需使用 rustup target add riscv32imac-unknown-none-elf，无需依赖专有工具链，这可能加速 Rust 在物联网和嵌入式系统中的应用。 ESP32-S31 提供 60 个 GPIO，支持全面的多协议连接，由台积电制造。它是不断扩大的 ESP32 系列之一，但这导致了一些用户对命名感到困惑。

hackernews · volemo · Jun 3, 16:10 · [社区讨论](https://news.ycombinator.com/item?id=48385965)

**背景**: ESP32 是乐鑫科技推出的低成本、高能效微控制器系列，集成 Wi-Fi 和蓝牙。传统上使用 Tensilica Xtensa 内核，但最新型号采用了开放的 RISC-V 架构。SIMD（单指令多数据）指令可实现数据并行处理，对多媒体和数字信号处理任务非常有益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.espressif.com/en/products/socs/esp32-s31">ESP32-S31 Dual-Core RISC-V + Multi-Protocol SoC | Espressif Systems</a></li>
<li><a href="https://www.seeedstudio.com/blog/2026/04/14/esp32-s31-vs-esp32-s3-should-the-xiao-get-an-upgrade/">ESP32-S31 vs. ESP32-S3: Should Seeed Studio XIAO Upgrade?</a></li>

</ul>
</details>

**社区讨论**: 社区反馈总体积极：一位评论者赞扬乐鑫的进展，强调 RISC-V 简化了 Rust 开发；另一位则对 ESP32 家族命名日益混乱表示困惑。使用 WLED 的爱好者对此兴奋不已，也有人关注模组供货和定价情况。

**标签**: `#ESP32`, `#RISC-V`, `#Embedded Systems`, `#Rust`, `#SoC`

---

<a id="item-8"></a>
## [Meta 允许员工 30 分钟内选择不被追踪](https://www.bbc.com/news/articles/c93x0k194yno) ⭐️ 8.0/10

Meta 推出了一项政策，允许员工在工作场所监控中选择退出最多 30 分钟，让他们有一段短暂的不受追踪的时间。 这项政策突显了科技行业企业监控与员工隐私之间的持续紧张关系，并可能影响其他公司重新考虑其追踪做法。 选择退出时间限制为 30 分钟，并且可能仅适用于某些追踪机制，尽管具体细节尚未完全披露。

hackernews · reconnecting · Jun 3, 12:42 · [社区讨论](https://news.ycombinator.com/item?id=48383220)

**背景**: 工作场所监控在科技公司中很常见，雇主监控员工在设备上的活动以衡量生产力和防止数据泄露。Meta 与许多公司一样，使用追踪软件来监控其员工队伍。该政策提供了一个短暂的喘息机会，但并未消除整体监控。

**社区讨论**: 评论引用《雪崩》等反乌托邦小说来批评工作场所监控，一些用户质疑为什么有人会在 Meta 这样的政策下继续工作。其他人则讨论 IT 岗位中追踪的普遍性，并分享个人离开科技行业的计划。

**标签**: `#Meta`, `#workplace surveillance`, `#employee privacy`, `#tech ethics`, `#policy`

---

<a id="item-9"></a>
## [数学家警告 AI 快速进军数学研究](https://www.science.org/content/article/mathematicians-issue-warning-ai-rapidly-gains-ground) ⭐️ 8.0/10

一群数学家发出警告，反对 AI 在数学领域的快速进步，指出其可能对人类主导的研究和证明验证造成冲击。 这一警告标志着 AI 驱动的自动化与传统数学方法之间日益紧张的关系，可能重新定义数学研究的方式和验证过程。 数学家的担忧与艺术家和作家早期对生成式 AI 的反应类似，并强调 AI 在关键数学任务上的可靠性仍存疑。

hackernews · pseudolus · Jun 3, 10:05 · [社区讨论](https://news.ycombinator.com/item?id=48382052)

**背景**: 数学传统上是一门以人为本的学科，证明由同行严格验证。大型语言模型（LLM）的最新进展在生成猜想和辅助证明方面显示出潜力，但其输出可能毫无意义或错误。这引发了关于 AI 在数学研究中角色的辩论，尤其是针对如埃尔多斯问题这类出于好奇心的研究。

**社区讨论**: 评论者将 AI 的崛起与艺术和软件领域的早期颠覆相类比，指出 AI 的长期愚蠢尾巴可能永远无法完全解决。一些人认为 AI 更适合实用性问题，而好奇驱动的数学应保持人类主导。其他人则强调 AI 为数学带来的可及性，类似于开源软件的影响。

**标签**: `#AI`, `#mathematics`, `#research`, `#society`, `#disruption`

---

<a id="item-10"></a>
## [原版 PlayStation 硬件的深度逆向工程分析](https://www.copetti.org/writings/consoles/playstation/) ⭐️ 8.0/10

Rodrigo Copetti 发布了对原版 PlayStation 硬件架构的全面逆向工程分析，详细介绍了其 CPU、GPU、GTE、SPU 和内存系统。 该分析为复古计算爱好者、模拟器开发人员以及研究主机设计的工程师提供了宝贵的见解，有助于保存这一里程碑式游戏平台的技术遗产。 文章涵盖了 MIPS R3000A CPU、几何变换引擎（GTE）、图形处理单元（GPU）和声音处理单元（SPU），并配有详细的内存映射和数据路径图解说明。

hackernews · gregsadetsky · Jun 3, 10:24 · [社区讨论](https://news.ycombinator.com/item?id=48382142)

**背景**: 原版 PlayStation 于 1994 年发布，采用定制的 MIPS R3000A 兼容 CPU、独立的 GPU 以及专用的几何和声音处理芯片。理解其架构对于准确的游戏模拟和软件保存至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PlayStation_technical_specifications">PlayStation technical specifications - Wikipedia</a></li>
<li><a href="https://psx-spx.consoledev.net/geometrytransformationenginegte/">Geometry Transformation Engine ( GTE ) - PlayStation Specifications...</a></li>
<li><a href="https://psx-spx.consoledev.net/soundprocessingunitspu/">Sound Processing Unit (SPU) - PlayStation Specifications - psx-spx</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了技术见解，如《合金装备》中使用的内存映射技巧，并称赞了文章的表现形式。还有用户请求 PS1 网页模拟器推荐，有人推荐了 PCSX-Redux 和 DuckStation。

**标签**: `#PlayStation`, `#hardware architecture`, `#retro computing`, `#emulation`, `#console engineering`

---

<a id="item-11"></a>
## [英伟达携 CPU 杀入 PC 赛道，支持笔记本运行 120B 大模型](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247894165&idx=2&sn=0125e0e1973268ab6434b7a2664bcc8c) ⭐️ 8.0/10

英伟达宣布推出 PC 端 CPU，能将拥有百万上下文窗口、120B 参数的大模型完整塞入笔记本电脑，实现电脑、手机、桌面三端打通。 此举标志着英伟达正式进军 PC CPU 市场，可能挑战英特尔和 AMD 等老牌厂商，并将强大的 AI 能力直接带到消费设备上，无需依赖云端。 该 CPU 支持高达 120B 参数、百万级上下文窗口的模型，远超常见端侧模型规模。英伟达还表示构建了相应的数据集和评测基准。

rss · 量子位 · Jun 2, 04:05

**背景**: 拥有数千亿参数的大语言模型通常因内存限制而需要云服务器。端侧 AI 此前局限于较小模型（如 7B-13B），因为消费硬件缺乏足够 RAM。英伟达的新 CPU 旨在弥合这一差距，让超大规模模型能够在本地运行，可能改变 AI 的可访问性和隐私性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/大型语言模型">大型语言模型 - 维基百科，自由的百科全书</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1929217926403186704">你的百万级上下文窗口大模型，可能并没有你想象中那么强——为什么“工作记忆”比上下文窗口大小更关键 - 知乎</a></li>
<li><a href="https://blog.csdn.net/Dianajr/article/details/139564226">本 地部署AI大 模 型 —— Ollama文档中文翻译-CSDN博客</a></li>

</ul>
</details>

**标签**: `#英伟达`, `#CPU`, `#大模型`, `#PC`, `#AI`

---

<a id="item-12"></a>
## [SpaceX 计划以每股 135 美元固定价 IPO，筹资 750 亿美元](https://www.reuters.com/business/media-telecom/spacex-plans-raise-75-billion-ipo-135-per-share-source-says-2026-06-03/) ⭐️ 8.0/10

SpaceX 宣布计划以每股 135 美元的固定价格进行首次公开募股（IPO），通过发行 5.556 亿股筹集 750 亿美元，预计于 2026 年 6 月 12 日在纳斯达克以代码 SPCX 开始交易。 如果成功，这将是史上最大规模的 IPO，通过为 AI 计算和星链扩张提供资金，对航天、AI 和科技行业产生重大影响，并可能引发 OpenAI 和 Anthropic 等公司的巨型 IPO 浪潮。 在路演前锁定发行价的做法极为罕见；周四启动的路演上细节仍可能调整。SpaceX 去年营收 187 亿美元但净亏 49 亿，仅星链盈利。

telegram · zaihuapd · Jun 3, 09:01

**背景**: 固定价格 IPO 预先设定股价，而簿记建档 IPO 则根据投资者需求确定价格。SpaceX 是埃隆·马斯克创立的私营太空探索公司，以火箭和星链卫星互联网闻名。此次 IPO 将为公众提供投资机会，并为 AI 和卫星项目筹集资金。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fixed-price_contract">Fixed-price contract</a></li>
<li><a href="https://en.wikipedia.org/wiki/Initial_public_offering">Initial public offering - Wikipedia</a></li>

</ul>
</details>

**标签**: `#IPO`, `#SpaceX`, `#finance`, `#AI`, `#Starlink`

---

<a id="item-13"></a>
## [千问向第三方 Agent 和 Skill 全面开放](https://www.stcn.com/article/detail/3941333.html) ⭐️ 8.0/10

千问 APP 宣布向第三方 Agent 和 Skill 全面开放，所有企业均可在千问平台运营自己的品牌 Agent。瑞幸、肯德基、蜜雪冰城、东方航空等首批企业正在进行 Agent 服务测试，并将陆续上线。 这一举措将千问转变为一个 AI 平台生态系统，使企业能够通过 Agent 集成其服务，可能加速 AI 在面向客户角色中的应用。这标志着从独立聊天机器人向类似于 AI 应用商店的平台模式的战略转变。 开放范围包括第三方 Agent（自主 AI 实体）和 Skill（可重用能力）。具体上线时间和收入分成细节尚未公布。

telegram · zaihuapd · Jun 3, 12:15

**背景**: AI Agent 是能够追求目标、使用工具并自主采取行动的智能系统，通常在人类定义的目标和约束内运行。Skill 是可重用的能力模块，可以安装在 Agent 上以增强其功能，例如访问数据库或执行特定任务。千问是阿里巴巴开发的知名 AI 助手，开放平台允许第三方在其基础上构建。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>
<li><a href="https://www.skills.sh/">Discover and install skills for AI agents.</a></li>

</ul>
</details>

**标签**: `#AI platform`, `#third-party agents`, `#enterprise AI`, `#Qianwen`

---

<a id="item-14"></a>
## [HTTP/2 炸弹攻击远程拖垮主流服务器](https://blog.calif.io/p/codex-discovered-a-hidden-http2-bomb) ⭐️ 8.0/10

研究人员披露了一种名为 HTTP/2 Bomb 的新型远程拒绝服务攻击，该攻击利用 HPACK 压缩放大和类似 Slowloris 的连接保持，针对 NGINX、Apache HTTPD、Microsoft IIS、Envoy 和 Cloudflare Pingora 的默认 HTTP/2 配置，可使其崩溃。 该攻击意义重大，因为它能在几秒钟内通过 100 Mbps 家用网络瘫痪主流 Web 服务器，影响互联网基础设施的很大一部分。NGINX 和 Apache 已有部分补丁，但其他服务器仍存在漏洞，凸显了加强 HTTP/2 安全性的必要性。 单个客户端可在约 20 秒内占用 Apache httpd 和 Envoy 的 32 GB 内存。NGINX 在 1.29.8+ 版本中已修复，Apache 在 mod_http2 v2.0.41 中修复，而 IIS、Envoy 和 Pingora 尚无补丁。

telegram · zaihuapd · Jun 3, 15:00

**背景**: HPACK 是 HTTP/2 中使用的头部压缩方法，通过静态和动态表对头部进行编码来减少开销。Slowloris 是一种拒绝服务攻击，通过发送部分请求保持大量连接打开，耗尽服务器资源。HTTP/2 Bomb 结合了这些技术：它发送特制的压缩头部，解压时会急剧膨胀，同时保持慢速连接以占用内存。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://http2.github.io/compression-spec/compression-spec.html">HPACK</a></li>
<li><a href="https://blog.cloudflare.com/hpack-the-silent-killer-feature-of-http-2/">HPACK : the silent killer (feature) of HTTP/2</a></li>
<li><a href="https://en.wikipedia.org/wiki/Slowloris_(cyber_attack)">Slowloris (cyber attack ) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#HTTP/2`, `#DoS`, `#vulnerability`

---

<a id="item-15"></a>
## [苹果因需求强劲将 MacBook Neo 产量翻倍](https://www.macrumors.com/2026/06/03/macbook-neo-production-doubled-says-kuo/) ⭐️ 7.0/10

据分析师郭明錤透露，苹果因需求旺盛已将 MacBook Neo 的产量翻倍。 这表明消费者对更实惠的 MacBook 需求强劲，可能重塑苹果笔记本电脑产品线，并给竞争对手带来压力。 MacBook Neo 传闻价格更低，基础配置 8GB 内存，一些用户认为有限但尚可接受。

hackernews · tosh · Jun 3, 16:33 · [社区讨论](https://news.ycombinator.com/item?id=48386238)

**背景**: MacBook Neo 是苹果最新入门级笔记本电脑，旨在提供更亲民的价格，同时集成苹果自研芯片和生态系统优势。它与低端 Windows 笔记本电脑和 Chromebook 竞争。

**社区讨论**: 评论者称赞苹果的生态系统和成本效率，认为 MacBook Neo 适合作为家庭设备。一些人担心它会蚕食高端型号的销量，而另一些人则认为 8GB 内存足以满足日常使用。

**标签**: `#Apple`, `#MacBook`, `#Hardware`, `#Business`, `#Consumer Electronics`

---

<a id="item-16"></a>
## [对 Java 内存优化中'每字节都要计较'思维的批判](https://fzakaria.com/2026/06/01/every-byte-matters) ⭐️ 7.0/10

博客文章《每字节都要计较》批判了 Java/JVM 内存优化中流行的'每字节都要计较'思维，指出当真正的性能提升来自优化数据访问模式（如数组结构体与结构体数组的选择）时，关注单字节节省往往具有误导性。 这一讨论对 Java 开发者和性能工程师很重要，因为它揭示了内存优化中的常见误解，鼓励关注有影响的改动而非微优化。这也与即将推出的 JVM 改进（如 Project Valhalla 旨在减少对象头开销）相呼应。 文章指出，在 100 万个怪物中各读取 1 字节实际上是读取 100 万字节，说明孤立关注单字节的谬误。当前 JVM 每个对象头开销为 12 字节，下一版本将减少到 8 字节，而 Project Valhalla 可能在某些情况下完全消除对象头。

hackernews · ingve · Jun 3, 11:04 · [社区讨论](https://news.ycombinator.com/item?id=48382382)

**背景**: 在 Java 中，每个对象因 JVM 对象头而有额外开销，对象头存储类指针和锁信息等元数据。内存优化通常涉及对象数量与字段粒度的权衡，理解数据布局（如数组结构体与结构体数组）可显著影响缓存性能。该博客文章批评了不考虑这些更广泛模式的过于简单化的'每字节都要计较'方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baeldung.com/java-memory-layout">Memory Layout of Objects in Java | Baeldung</a></li>
<li><a href="https://docs.oracle.com/cd/E13222_01/wls/docs81/perform/JVMTuning.html">Tuning Java Virtual Machines (JVMs)</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意'每字节都要计较'思维常被误用，'moring'指出真正问题是数据布局而非单个字节。'pron'反驳说，在标准库的热点区域，布局优化确实重要。'ChrisMarshallNY'从嵌入式系统极端内存限制的历史角度提供了见解。

**标签**: `#Java`, `#JVM`, `#memory optimization`, `#data layout`, `#performance`

---

<a id="item-17"></a>
## [大规模代理服务封锁波及 VLESS 和 AnyTLS 协议](https://t.me/zaihuapd/41740) ⭐️ 7.0/10

2025 年 3 月 4 日，中国国家防火墙开始系统性地封禁热门代理服务商的 IP 段，严重影响 VLESS 协议及较新的 AnyTLS 协议。 此次审查升级干扰了大量用户对翻墙工具的使用，表明防火墙能够适应更新的加密协议，可能削弱现有代理技术的有效性。 此次封禁对非 TLS 加密类型影响相对较小，但缺乏官方统计数据，实际影响范围不明。以轻量无状态设计著称的 VLESS 协议受到严重影响，旨在缓解 TLS 嵌套指纹识别的新协议 AnyTLS 似乎也被大量阻断。

telegram · zaihuapd · Jun 3, 11:15

**背景**: VLESS 是一种无状态的轻量传输协议，常用于 V2Ray 或 Xray 等代理工具，设计上追求高性能且开销极小。AnyTLS 是由 sing-box 团队维护的较新 TLS 代理协议，通过填充机制混淆流量特征，缓解 TLS 嵌套指纹识别。GFW 历来通过分析协议指纹和流量模式来封禁代理 IP，此次事件表明它已能检测 VLESS 和 AnyTLS。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xtls.github.io/development/protocols/vless.html">VLESS 协议 | Project X</a></li>
<li><a href="https://www.ermao.net/article/anytls-guide/">AnyTLS 协 议 是 什 么 ？ AnyTLS 原理、sing-box... | 二毛</a></li>

</ul>
</details>

**标签**: `#GFW`, `#proxy`, `#censorship`, `#VLESS`, `#AnyTLS`

---

<a id="item-18"></a>
## [谷歌允许网站退出 AI 搜索结果](https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/) ⭐️ 7.0/10

谷歌在 Search Console 中新增了一项选项，允许网站所有者选择其内容是否出现在 AI 概览和 AI 模式中，且不影响常规搜索排名。同时，谷歌还推出了生成式 AI 搜索统计数据，帮助站长查看展示量和表现。 这赋予了站长对 AI 搜索功能中内容的更大控制权，可能减轻因 AI 摘要导致的流量损失。这为搜索引擎如何平衡 AI 创新与发布者权益树立了重要先例。 该退出选项目前在英国部分网站进行测试，并计划向全球推广。选择退出的网站将保留其常规排名和 Discover 信息流中的展现。此外，新的生成式 AI 搜索统计数据提供了展示量、页面级数据及地域信息。

telegram · zaihuapd · Jun 3, 12:00

**背景**: Google AI 概览是一种 AI 功能，会在搜索结果顶部生成摘要答案，常因不准确和减少源网站流量而受到批评。Google Search Console 是一个免费工具，帮助站长监控和优化其网站在 Google 搜索中的表现。这项新控制允许网站所有者退出 AI 生成的摘要，同时保持常规列表。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://search.google/ways-to-search/ai-overviews/">Google AI Overviews - Search anything, effortlessly</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Search_Console">Google Search Console</a></li>
<li><a href="https://search.google.com/search-console/about">Google Search Console</a></li>

</ul>
</details>

**标签**: `#Google`, `#AI search`, `#SEO`, `#Search Console`, `#AI Overviews`

---

<a id="item-19"></a>
## [测试显示 64GB 内存是专业创作用户的甜点配置](https://www.pugetsystems.com/labs/articles/when-does-ram-capacity-impact-performance/) ⭐️ 7.0/10

Puget Systems 测试了从 16GB 到 64GB 的内存配置在 Adobe 全家桶和 DaVinci Resolve 中的表现，发现 64GB 在复杂合成、AI 特效和 Fusion 节点工作流中持续优于更低容量。 对于升级工作站的专业人士来说，这提供了明确指导：32GB 足以应对轻量任务，但 64GB 是要求苛刻的创意工作负载的最佳投资，可能节省时间并提高生产力。 在 After Effects 2D 合成和 Lightroom 导出中，16GB 与 64GB 配置相比性能下降超过 40%，而 32GB 在 AI 特效和复杂 Fusion 场景中仍明显卡顿。

telegram · zaihuapd · Jun 3, 12:30

**背景**: Puget Systems 是一家位于华盛顿州奥本的定制工作站制造商，以严格的硬件测试闻名。诸如 Adobe After Effects 和 DaVinci Resolve 的 Fusion 页面等创意应用对内存需求很高，特别是在处理高分辨率素材、多层合成或 GPU 加速 AI 功能时。内存不足会迫使系统使用较慢的存储作为虚拟内存，导致性能瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Puget_Systems">Puget Systems</a></li>

</ul>
</details>

**标签**: `#memory`, `#creative software`, `#workstation`, `#Adobe`, `#DaVinci Resolve`

---

<a id="item-20"></a>
## [美国教师工会呼吁限制小学 AI 使用及课堂屏幕](https://www.aft.org/press-release/devices-down-eyes-hands-weingarten-calls-screen-bans-ai-limits-active-learning-major) ⭐️ 7.0/10

美国教师联合会（AFT）主席兰迪·温加滕提议在幼儿园至二年级禁止使用屏幕，在小学阶段停止面向学生的 AI 工具，并禁止 16 岁以下青少年使用社交聊天机器人。该计划还包括对科技公司征税以资助公共教育，并建立独立研究机构。 这是美国最大的教师工会的一项重要政策立场，可能影响地区和州对课堂技术的监管。如果被采纳，将重塑幼儿在教育环境中与 AI 和屏幕互动的方式，优先考虑主动学习和社交发展。 该提案特别针对 16 岁以下青少年使用模拟人类的社交聊天机器人，指出其对社交和心理健康的危害。温加滕还呼吁对大型科技公司征收“科技税”，以资助公共教育，并通过不受行业资助的独立研究机构对数字工具进行循证评估。

telegram · zaihuapd · Jun 3, 13:30

**背景**: 美国教师联合会（AFT）是美国最大的两个教师工会之一，代表约 170 万会员。该工会的立场反映了教育工作者对幼儿教育中过度依赖屏幕和 AI 的日益担忧，尤其是在疫情后远程学习激增的背景下。社交聊天机器人是旨在模拟人类对话的 AI 系统；支持者强调其陪伴潜力，但批评者警告这可能导致儿童情感依赖和隐私风险。

**标签**: `#education`, `#AI regulation`, `#screen time`, `#child development`, `#public policy`

---