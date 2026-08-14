# 会议 / 活动高质量研究

本页按**收录时间倒序**归档 Black Hat、DEF CON、USENIX Security、GRCon、European GNU Radio Days 等会议和活动中，与 RF / SDR / wireless hack 强相关、且具有完整研究链路的高质量材料。

这里关注的不是“会议新闻”，而是**研究本身**：发现某个 RF / wireless 漏洞或系统问题，解释协议/物理层/硬件机制，使用 SDR 或 RF 测试手段进行捕获、重放、注入、欺骗或验证，并尽量追踪 slides、whitepaper、paper、tool、video 或 demo。

## 收录标准

- 有明确研究问题或真实漏洞；
- 能解释 RF / PHY / MAC / protocol / hardware 中至少一个关键机制；
- 优先有官方 slide、whitepaper、paper、video、tool 或代码；
- 使用 SDR、RF 测试设备、无线芯片、嵌入式硬件或电磁测量手段进行验证；
- 对复现实验、协议逆向、无线安全或系统设计具有长期参考价值。

## 与其他主题的区别

- **RF / Wireless 动态**：最近发生了什么；
- **会议 / 活动高质量研究**：一个研究如何从问题发现走到机制分析和实验验证；
- **RF 原理精读**：经典理论如何被系统讲清楚。

## 2026-08-14

### [Black Hat USA 2026：Blind Trust in the 6 GHz Band — Weaponizing Wi-Fi AFC](https://blackhat.com/us-26/briefings/schedule/)

研究对象是 6 GHz 标准功率 Wi-Fi 使用的 Automated Frequency Coordination。AFC 为避免 Wi-Fi 干扰既有 6 GHz incumbent 系统，需要根据设备位置等信息决定可用信道和功率，因此传统无线系统新增了外部数据库/网络控制面。

**研究链路：** 6 GHz shared spectrum 规则 → AFC 输入与信任边界 → 错误/伪造信息影响频谱授权 → 潜在 RF 干扰与共存风险。

**长期价值：** 适合学习 Wi-Fi PHY/MAC 之外的频谱管理依赖，以及 RF 规则、位置、监管数据库与网络安全如何组成新的系统攻击面。

**材料状态：** Black Hat 官方 session 已确认；后续持续检查该 session 的 Presentation Material。如公开 slides、whitepaper 或 tool，则优先替换/补充为直接材料链接。

### [Black Hat USA 2026 Training：Red Team SIGINT](https://blackhat.com/us-26/training/schedule/index.html?track%5B%5D=wireless)

课程覆盖 RF、SDR、SIGINT、未知信号识别，以及 automotive、aviation、marine、physical access、TETRA、DMR、P25 等 mission-critical radio。官方课程说明还包含拦截/解密手持无线通信、汽车安全测试，以及铁路、水务、无人机和警务/军用无线电攻击案例。

**研究/方法链：** RF 基础 → 信号发现与识别 → SDR capture / analysis → 协议与系统安全弱点 → 真实行业无线系统验证。

**长期价值：** 非常适合作为“综合 RF security methodology”入口，尤其补足普通 SDR 教程较少覆盖的 mission-critical、交通和基础设施无线系统。

**材料状态：** 当前主要是官方 Training 描述；若讲师后续公开 slides、lab、tool 或案例文档，应优先补入。

### 本期最值得精读的会议 / 活动研究

**Blind Trust in the 6 GHz Band。** 它最能体现本页定位：从频谱规则与系统架构找到新的信任边界，再把控制面问题落回真实 RF 干扰和频谱共存。