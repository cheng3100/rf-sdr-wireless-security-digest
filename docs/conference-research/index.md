# 会议 / 活动高质量研究

本页按**收录时间倒序**归档 Black Hat、DEF CON、USENIX Security、GRCon、European GNU Radio Days 等会议和活动中，与 RF / SDR / wireless hack 强相关、且具有完整研究链路的高质量材料。

这里关注的不是“会议新闻”，而是**研究本身**：例如发现某个 RF / wireless 漏洞，解释协议或物理层机制，使用 SDR / RF 硬件进行捕获、重放、注入、欺骗或验证，并公开 slides、whitepaper、paper、tool 或 demo。

## 收录标准

优先收录同时满足多项条件的材料：

- 有明确研究问题或真实漏洞，而不是泛泛介绍；
- 能解释 RF / PHY / MAC / protocol / hardware 中至少一个关键机制；
- 有可追溯的官方 slide、whitepaper、paper、video、tool 或代码；
- 使用 SDR、RF 测试设备、无线芯片、嵌入式硬件或电磁测量手段进行验证；
- 对复现实验、协议逆向、无线安全或系统设计具有长期参考价值。

## 与其他主题的区别

- **RF / Wireless 动态**：记录“最近发生了什么”，强调时效性；
- **RF 原理精读**：解释经典理论和成熟工程原理，强调学习价值；
- **会议 / 活动高质量研究**：围绕一个完整研究案例，把漏洞发现、机制分析、实验设备、攻击/验证方法和研究材料串起来，强调综合性。

## 优先检索的会议 / 活动

- [Black Hat Briefings / Trainings](https://blackhat.com/briefings/)
- [DEF CON](https://defcon.org/)
- [USENIX Security Symposium](https://www.usenix.org/conference/usenixsecurity26)
- [GNU Radio Conference / GRCon](https://events.gnuradio.org/)
- [European GNU Radio Days](https://gnuradiodays.sciencesconf.org/)

这些来源本身是否属于“长期高价值信息源”由 [高价值信息源](../high-value-sources/index.md) 单独维护；本页只记录其中真正值得长期归档的具体研究材料。

## 2026-08-14

### Black Hat USA 2026：6 GHz Wi-Fi AFC 安全研究

Black Hat USA 2026 的 **“Blind Trust in the 6 GHz Band: Weaponizing Wi-Fi Automated Frequency Coordination (AFC)”** 将 6 GHz Wi-Fi 的 Automated Frequency Coordination 控制机制作为攻击面研究对象。

**为什么值得归档：** 这类研究不是单纯的 Wi-Fi 协议漏洞，而是把无线设备、地理位置、频谱监管数据库、共享频谱规则和网络控制面连接成一个完整攻击面。适合用于学习 6 GHz Wi-Fi 在传统 PHY/MAC 之外新增的系统依赖。

**适合关注：** 6 GHz Wi-Fi、AFC、shared spectrum、监管控制面、无线基础设施安全。

**材料入口：** [Black Hat USA 2026 Briefings](https://blackhat.com/us-26/briefings.html)

### Black Hat USA 2026：Red Team SIGINT

Black Hat USA 2026 Wireless/Hardware Training 中的 **“Red Team SIGINT: Practical SDR hacking for mission-critical, automotive, aviation, and marine targets”** 覆盖 SDR、SIGINT、未知信号识别，以及 TETRA、DMR、P25、automotive、aviation、marine 等方向。

**为什么值得归档：** 其价值在于把无线原理、SDR 捕获与分析、真实行业协议和安全评估放在同一方法链中。后续如公开 slides、whitepaper、tool 或课程材料，应优先跟踪并更新到本条目。

**适合关注：** mission-critical radio、TETRA/DMR/P25、车载/航空/海事 RF、SDR/SIGINT 工作流。

**材料入口：** [Black Hat USA 2026 Training](https://blackhat.com/us-26/training/schedule/)
