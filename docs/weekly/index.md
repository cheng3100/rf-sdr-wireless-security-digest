# Weekly 简报归档

每期简报固定保留五个主题：软件项目、软硬件项目、RF / Wireless 动态、会议 / 活动高质量研究、RF 原理精读。动态栏目强调近期新闻与生态变化；会议研究栏目强调完整研究链路与高质量 slides/whitepaper/paper/tool；原理栏目强调长期学习价值。每期检索前会优先检查 [长期高价值信息源](../high-value-sources/index.md) 的增量，再扩展到更广泛来源。

## 2026-08-21

### [第 4 期：Radio-FM、Pocket SDR、BLERP 与 RDS 整链路](2026-08-21.md)

**原始文本：** [查看本次 ChatGPT 发布的完整原文](../raw/2026-08-21.md)

**主题入口：** [软件项目](2026-08-21.md#software) · [软硬件项目](2026-08-21.md#hardware-software) · [RF / Wireless 动态](2026-08-21.md#news) · [会议研究](2026-08-21.md#conference-research) · [RF 原理精读](2026-08-21.md#fundamentals)

本期软件方向重点看 radiom 的远程多 decoder SDR 工作台和 Radio-FM 的原始 I/Q foundation model；软硬件方向重点是 Pocket SDR v0.19 的多通道 GNSS RF frontend→tracking→PVT 完整链路，以及 HackRF Pro 主线配置能力。动态部分关注 Wi-Fi beamforming feedback 转化为隐私侧信道，以及 FCC 对 unlicensed D2D satellite 的推进。会议研究选择 BLERP，因为具备独立 research page、paper、slides、Black Hat Asia 研究条目和 nRF52 可复现实验链；原理精读选择 PySDR RDS end-to-end，把 IQ/filter/resample/sync/demod/protocol 串起来。

## 2026-08-14 · 五主题精确链接校正版

### [第 3 期修订：Black Hat 会议研究、MeshCore 与接收机同步](2026-08-14.md)

**原始文本：** [首次发布](../raw/2026-08-14.md) · [高价值来源测试](../raw/2026-08-14-02.md) · [五主题修订](../raw/2026-08-14-03.md) · [链接校正版](../raw/2026-08-14-04.md) · [精确锚点校正版](../raw/2026-08-14-05.md)

**主题入口：** [软件项目](2026-08-14.md#software) · [软硬件项目](2026-08-14.md#hardware-software) · [RF / Wireless 动态](2026-08-14.md#news) · [会议研究](2026-08-14.md#conference-research) · [RF 原理精读](2026-08-14.md#fundamentals)

本期正式采用五主题结构。软件方向重点是 SDRangel 的 MeshCore Rx/Tx 插件与 SatDump；软硬件方向继续跟踪 PortaPack Mayhem 与 Maia SDR。动态部分关注 Black Hat USA 2026 会后研究材料；会议研究栏目重点整理 6 GHz Wi-Fi AFC 与 Red Team SIGINT。此次精确链接校正后，AFC 条目直接使用 Black Hat 议题自身的 `#fragment`，点击即可定位到对应 session；对于尚未确认唯一 fragment 的 Red Team SIGINT，不再把 track 页面称为具体入口，而使用 Midnight Blue 的独立课程页作为主要入口。

## 2026-08-07

### [第 2 期：客户端演进、便携平台与 RF 安全研究](2026-08-07.md)

**原始文本：** [查看本次 ChatGPT 发布的完整原文](../raw/2026-08-07.md)

**主题入口：** [软件项目](2026-08-07.md#software) · [软硬件项目](2026-08-07.md#hardware-software) · [RF / Wireless 动态](2026-08-07.md#news) · [RF 原理精读](2026-08-07.md#fundamentals)

本期软件方向关注 AetherSDR、SDR++ Nightly 和 GNU Radio 4 的远程可观察性方向。软硬件方向关注 PortaPack Mayhem、Maia SDR 与 Pluto+。动态部分跟踪 GRCon26、EuGRD2026 与 RF 安全研究的新议题。原理精读选择 PySDR 的链路预算章节，建立从发射功率、传播损耗、天线和噪声到可解调 SNR 的系统视角。

## 2026-08-01

### [四主题测试发布](2026-08-01.md)

**主题入口：** [软件项目](2026-08-01.md#software) · [软硬件项目](2026-08-01.md#hardware-software) · [RF / Wireless 动态](2026-08-01.md#news) · [RF 原理精读](2026-08-01.md#fundamentals)

本期软件方向关注 SDRangel、QRadioLink 与 rtl_433。软硬件方向重点是 Maia SDR、PortaPack Mayhem 与 HackRF。动态部分关注频谱资产变化与便携 SDR 生态演进。原理精读选择 Wireless Pi 的同步总览文章。

## 2026-07-31

### [第 1 期](2026-07-31.md)

**主题入口：** [软件项目](2026-07-31.md#software) · [软硬件项目](2026-07-31.md#hardware-software) · [RF / Wireless 动态](2026-07-31.md#news) · [RF 原理精读](2026-07-31.md#fundamentals)

本期软件方向收录多类 SDR 工具与实验环境。软硬件方向关注便携 RF 采集节点、OpenWXSDR 与 Open.Space。该期尚未独立设置 RF / Wireless 动态栏目。原理部分围绕 IQ Sampling、数字调制与同步展开。
