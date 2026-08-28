# RF / Wireless 动态

本页按更新时间倒序归档 RF、SDR 与 wireless 相关的近期动态和新闻，并直接附上原始来源链接。

## 与 RF 原理精读的区别

- **RF / Wireless 动态**：看重时效性，回答“最近发生了什么、可能带来什么影响”。
- **RF 原理精读**：看重长期学习价值，回答“某个经典理论或成熟工程概念如何被解释清楚”。

## 2026-08-28

### [BlueZ A2DP stream endpoint 栈溢出：ZDI-26-589 / CVE-2026-19774](https://www.zerodayinitiative.com/advisories/ZDI-26-589/)
Zero Day Initiative 在 2026-08-24 公布该漏洞。BlueZ 对 A2DP stream endpoint 中用户可控长度缺少充分校验，复制到固定长度栈 buffer 时产生溢出；攻击者需要先让恶意 Bluetooth 设备完成 pairing，但成功后可能在 bluetoothd/root 上下文执行代码。

### [BlueZ EIR discovery 栈溢出：CVE-2026-80186](https://security.snyk.io/vuln/SNYK-DEBIAN11-BLUEZ-19268263)
2026-08-25 公开。攻击者处于 Bluetooth 无线范围内即可发送精心构造的 Extended Inquiry Response packet，触发 BlueZ discovery 路径 stack overflow，可导致 bluetoothd 崩溃并可能达到代码执行。与 A2DP 漏洞对比，它暴露的是 pairing/profile 建立之前的 discovery metadata attack surface。

## 2026-08-21

### Wi-Fi beamforming feedback 被用于无摄像头人体识别
8 月 18 日公开报道的一项研究显示，普通 Wi-Fi 基础设施中的 beamforming feedback 可以被用于人体识别；报道描述的实验在 197 名参与者上取得接近 100% 的识别率。值得关注的是原本用于链路优化的 PHY/CSI 类反馈正在成为隐私侧信道，后续 Wi-Fi sensing 标准的隐私边界值得持续跟踪。

### [FCC：Unleashing Unlicensed Spectrum for Direct-to-Device](https://www.fcc.gov/document/fcc-looks-expand-d2d-satellite-connectivity-unlicensed-wireless)
FCC 在 2026-08-06/07 推进 FCC-26-51 / ET Docket 26-169，探索允许部分 Part 15 非授权频段设备与获授权卫星直接通信，并讨论非授权设备在 spacecraft 中的使用。

## 2026-08-14 · 高价值来源测试修订版

### [Black Hat USA 2026：Blind Trust in the 6 GHz Band](https://blackhat.com/us-26/briefings/schedule/#blind-trust-in-the-6-ghz-band-weaponizing-wi-fi-automated-frequency-coordination-afc-53998)
Black Hat USA 2026 Briefings 出现针对 6 GHz Wi-Fi Automated Frequency Coordination（AFC）的安全研究，值得从共享频谱、监管数据库、无线控制面和安全边界的交叉视角持续关注。

### [Black Hat USA 2026：Red Team SIGINT Training](https://www.midnightblue.nl/explore/training/red-team-sigint-practical-sdr-hacking)
Wireless/Hardware Training 涵盖 RF/SDR/SIGINT、未知信号识别，以及 automotive、aviation、marine、TETRA、DMR、P25 等较少出现在普通 IoT SDR 教程中的场景。

### [Black Hat Briefings 会后材料](https://blackhat.com/us-26/briefings.html)
官方会在演讲者提供材料时把 slides、whitepapers 和 tools 放到对应 session page；2026 年 on-demand Briefings 从 8 月 14 日起开放给相应 pass 用户。Black Hat 因此被纳入长期高价值信息源列表。

## 2026-08-14

### [European GNU Radio Days 2026](https://gnuradiodays.sciencesconf.org/)
会议将于 2026 年 11 月 16–18 日在 Rennes 举办，8 月已进入注册和投稿阶段。本届明确关注 SDR 网络安全，同时覆盖 5G/6G、卫星通信、频谱监测、雷达感知、AI for Radio、侧信道与 TEMPEST。

### [FCC August 2026 Open Meeting Agenda](https://www.linkedin.com/posts/federal-communications-commission_august-2026-open-meeting-agenda-direct-to-device-activity-7483911319595925504-sUV2)
FCC 8 月公开会议议程包含 Direct-to-Device Spectrum，反映传统移动网络、卫星网络和终端直连能力正在进入更统一的频谱与监管讨论框架。

### [GRCon26](https://lists.gnu.org/archive/html/discuss-gnuradio/2026-05/msg00000.html)
GRCon26 将于 9 月 21–24 日在 Raleigh 举办，由 NC State/AERPAW 承办，议题覆盖 SDR 开发、无线系统、AI/ML、5G/6G、硬件集成、教育与实验平台。

## 2026-08-07

### [GRCon26 初步日程公布](https://events.gnuradio.org/event/28/overview)
GRCon26 将于 9 月在 Raleigh 举办，议题覆盖 FutureG、认知无线电、机器学习、Massive MIMO、同步、无线安全、SigMF 与硬件加速。

### [European GNU Radio Days 2026 聚焦 SDR 网络安全](https://www.gnuradio.org/news/2026-07-04-EuGRD26-announce/)
EuGRD2026 将于 11 月 16—18 日在 Rennes 举办，重点覆盖 SDR 网络安全、5G/6G、卫星通信、频谱监测、雷达感知、侧信道和 TEMPEST。

### [USENIX Security 2026 RF 安全研究](https://www.usenix.org/conference/usenixsecurity26)
本期关注会议中与非预期电磁辐射和无线安全相关的研究方向，适合作为 RF 安全研究新议题的观察窗口。

## 2026-08-01

### [AT&T 完成 EchoStar 频谱交易](https://www.reuters.com/business/media-telecom/att-closes-23-billion-deal-acquire-spectrum-echostar-2026-07-28/)
AT&T 获得约 50 MHz 的美国全国性频谱，包括约 30 MHz 的 3.45 GHz 中频段和约 20 MHz 的 600 MHz 低频段。该事件反映运营商仍同时强化低频覆盖资源与中频容量资源。

### [PortaPack Mayhem 持续发布 nightly 构建](https://github.com/portapack-mayhem/mayhem-firmware/releases)
Mayhem 社区在稳定版本之外保持高频迭代，近期变更继续改进协议接收、错误处理和现场可用性。
