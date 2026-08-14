# 会议 / 活动高质量研究

本页按**收录时间倒序**归档 Black Hat、DEF CON、USENIX Security、GRCon、European GNU Radio Days 等会议和活动中，与 RF / SDR / wireless hack 强相关、且具有完整研究链路的高质量材料。

这里关注的不是“会议新闻”，而是**研究本身**：发现某个 RF / wireless 漏洞或系统问题，解释协议/物理层/硬件机制，使用 SDR 或 RF 测试手段进行捕获、重放、注入、欺骗或验证，并尽量追踪 slides、whitepaper、paper、tool、video 或 demo。

## 收录标准

- 有明确研究问题或真实漏洞；
- 能解释 RF / PHY / MAC / protocol / hardware 中至少一个关键机制；
- 优先有官方 slide、whitepaper、paper、video、tool 或代码；
- 使用 SDR、RF 测试设备、无线芯片、嵌入式硬件或电磁测量手段进行验证；
- 对复现实验、协议逆向、无线安全或系统设计具有长期参考价值。

## 链接规则

- 会议研究条目必须优先给出**具体议题/课程/材料链接**，不能用会议首页代替；
- 若官方 slides / whitepaper / tool 已公开，直接链接材料；
- 若尚未找到可验证的公开材料链接，必须明确写“当前未找到可验证公开 slides/whitepaper/tool”，不得把会议主页或总日程冒充材料链接；
- 可额外给出作者/研究团队的具体技术页面作为补充，但要与官方会议入口区分。

## 2026-08-14

### Black Hat USA 2026：Blind Trust in the 6 GHz Band — Weaponizing Wi-Fi AFC

研究对象是 6 GHz 标准功率 Wi-Fi 使用的 Automated Frequency Coordination。Black Hat 官方日程确认该议题于 2026-08-06 11:05 举行，讲者为 Yilu Dong、Tianchang Yang，contributors 为 Arupjyoti Bhuyan、Syed Rafiul Hussain。

**具体议题入口：** [Black Hat USA 2026 Briefings Schedule — 该页面中可直接定位该标题、时间和讲者](https://blackhat.com/us-26/briefings/schedule/)

**具体技术背景/研究报道：** [Dark Reading — 6 GHz Wi-Fi Flaws Could Disrupt Critical Systems](https://www.darkreading.com/perimeter/6-ghz-wi-fi-flaws-disrupt-critical-systems)

**研究链路：** 6 GHz shared spectrum 规则 → AFC 输入与信任边界 → 位置/设备参数等输入被错误信任或伪造 → 频谱授权决策异常 → 潜在 RF 干扰与共存风险。

**长期价值：** 适合学习 Wi-Fi PHY/MAC 之外的频谱管理依赖，以及 RF 规则、位置、监管数据库与网络安全如何组成新的系统攻击面。

**slides / whitepaper / tool 状态：** Black Hat 官方说明材料若由演讲者提交，会出现在具体 session 页面底部的 `Presentation Material`。截至本次修订，公开检索可以确认议题、时间、讲者和研究主题，但**尚未找到可验证的独立公开 slides / whitepaper / tool URL**。后续只在找到确切材料 URL 后补入，不再使用 Briefings 首页代替。

### Black Hat USA 2026 Training：Red Team SIGINT — Practical SDR hacking for mission-critical, automotive, aviation, and marine targets

课程覆盖 RF、SDR、SIGINT、未知信号识别，以及 automotive、aviation、marine、physical access、TETRA、DMR、P25 等 mission-critical radio。Black Hat 官方课程描述还包括拦截/解密手持无线通信、汽车安全系统测试，以及铁路、水务、无人机和警务/军用无线电攻击案例。

**Black Hat 具体课程入口：** [Black Hat USA 2026 Training Schedule — Wireless track / Red Team SIGINT](https://blackhat.com/us-26/training/schedule/index.html?track%5B%5D=wireless)

**讲师团队具体课程页：** [Midnight Blue — Red Team SIGINT: Practical SDR hacking](https://www.midnightblue.nl/explore/training/red-team-sigint-practical-sdr-hacking)

**相关具体案例材料：** [Midnight Blue — Analyzing the Taiwan High-Speed Rail (THSR) TETRA cyber incident, part 1](https://www.midnightblue.nl/blog/analyzing-the-taiwan-high-speed-rail-thsr-tetra-cyber-incident-part-1)

**研究/方法链：** RF 基础 → 信号发现与识别 → SDR capture / analysis → 协议与系统安全弱点 → 真实行业无线系统验证。

**长期价值：** 适合作为综合 RF security methodology 入口，尤其补足普通 SDR 教程较少覆盖的 mission-critical、交通和基础设施无线系统。

**slides / lab / tool 状态：** Black Hat 该项属于 Training，不是 Briefing；当前可验证的公开资料以 Black Hat 课程说明、Midnight Blue 课程页和其公开案例文章为主，**未找到可验证的 Black Hat 公开 slide deck URL**。后续若讲师公开 slides、lab 或 tooling，再追加直接链接。

### 本期最值得精读的会议 / 活动研究

**Blind Trust in the 6 GHz Band。** 它最能体现本页定位：从频谱规则与系统架构找到新的信任边界，再把控制面问题落回真实 RF 干扰和频谱共存；同时本次修订明确区分“具体议题入口”和“实际 slides/whitepaper/tool 是否已经公开”。