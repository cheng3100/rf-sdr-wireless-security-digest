# 软件项目

本页按**收录时间倒序**归档以软件实现为主的 SDR / wireless 研究项目。每个条目直接链接到项目仓库或官方页面；需要查看同一期五个主题的完整上下文，可前往 [Weekly](../weekly/index.md)。

## 2026-09-04

### [FISSURE：分布式 RF operations / situational awareness](https://github.com/ainfosec/FISSURE)
FISSURE 当前主线已从单机 RF 工具集合继续扩展到分布式 sensor node、RF emitter geolocation、artifact/target/alert 管理和 TAK operator workflow。GRCon26 的 [FISSURE: Tactical RF Operations and Situational Awareness with GNU Radio](https://events.gnuradio.org/event/28/contributions/859/) 进一步展示其从 signal analysis framework 向多节点 RF operations 平台演进的方向。

## 2026-08-28

### [AetherSDR v26.8.4](https://github.com/aethersdr/AetherSDR/releases/tag/v26.8.4)
2026-08-23 发布，继续扩展 Icom 与 Hermes-Lite 2 backend 的 capability model、CI-V/CW/FM/IF filter 控制、恢复机制与 PSK Reporter/NR2 等功能。适合观察真实 SDR workstation 中多 radio backend、网络 transport、DSP/UI 和 authoritative state 的工程分层。

### [GNU Radio 4 官方仓库组织正式化](https://www.gnuradio.org/news/)
GNU Radio 官方于 2026-08-16 公布 GR4 仓库重构方向，将 runtime/core、可复用 DSP library、standard blocks 等拆成职责更明确的组件，并通过 builder/super-repo 组合。重点仓库包括 [gnuradio4-core](https://github.com/gnuradio/gnuradio4-core)、[gnuradio4-library](https://github.com/gnuradio/gnuradio4-library) 与 [gnuradio4-blocks](https://github.com/gnuradio/gnuradio4-blocks)。

## 2026-08-21

### [radiom](https://github.com/thepacket/radiom)
面向移动端/浏览器的 SDR 客户端，可连接 KiwiSDR、OpenWebRX 和 RTL_TCP，并把大量协议 decoder 集成到统一界面。适合研究远程 SDR source、网络访问、协议处理和移动 UI 的组合方式。

### [Radio-FM](https://arxiv.org/abs/2608.05793)
2026 年 8 月提交的 RF foundation model，直接从原始 I/Q 学习通用 radio representation，并覆盖调制识别、雷达、发射机识别、无线技术识别与干扰识别等任务。

## 2026-08-14 · 高价值来源测试修订版

### [SDRangel 7.27.1 / MeshCore 插件](https://github.com/f4exb/sdrangel/releases)
7.27.0/7.27.1 加入并修复 MeshCore Rx/Tx 插件。MeshCore 是基于 LoRa 的离网 mesh 系统，适合观察 SDRangel 如何把调制、解调、协议和 GUI/设备抽象组织进统一插件框架。

### [SatDump 2.0 Alpha](https://www.satdump.org/tags/release/)
继续把 SDR 输入、DSP、同步、FEC、framing、协议解析和图像/遥测恢复整合在同一 pipeline 中，适合作为“从 IQ 到业务数据”的完整软件架构样本。

### [Universal Radio Hacker v2.10.0](https://github.com/jopohl/urh/releases)
经典仓库已归档，但最终主版本仍适合作为成熟协议逆向工具基线。后续不再把它视为活跃动态源，而保留其 OOK/FSK/GFSK、多帧比较、编码和 CRC 分析方法论价值。

## 2026-08-14

### [SatDump 2.0 Alpha](https://www.satdump.org/tags/release/)
把卫星 SDR 采集、实时解调、纠错、协议解析、图像/遥测恢复和离线处理整合到一套工具链中，适合观察从 IQ 到最终业务数据的完整工程链路。

### [SDR++ Nightly 1.3.0](https://github.com/AlexandreRouma/SDRPlusPlus/releases)
跨平台通用 SDR 客户端，持续提供多 VFO、模块化 source/sink/decoder、SIMD DSP 与多硬件后端支持，适合作为用户态 SDR 数据通路代码阅读样本。

### [gr-satellites](https://github.com/daniestevez/gr-satellites)
当前 v5.x 主线面向 GNU Radio 3.10，覆盖 AX.25、GOMspace、CCSDS、AO-40 等协议，适合学习 OOT module 如何组织同步、解调、FEC、framing 与 telemetry。

## 2026-08-07

### [AetherSDR v26.7.4.1](https://github.com/aethersdr/AetherSDR/releases)
2026 年 7 月 27 日发布的热修复版本，恢复 WSJT-X 和控制面的 TCI rig control。项目近期还持续整合 D-STAR、MCP Server、3D FFT、降噪和语音处理，体现 SDR 客户端向综合工作台发展。

### [SDR++ Nightly 1.3.0](https://github.com/AlexandreRouma/SDRPlusPlus/releases)
采用 rolling/nightly 发布模式的跨平台 SDR 客户端，强调多 VFO、SIMD DSP、模块化 source/sink/decoder，以及原生硬件后端和 SoapySDR 兼容。

### [GNU Radio 4 Web 监控与 CyberEther 互操作](https://www.gnuradio.org/news/2026-05-26-gsoc26-started/)
GNU Radio 2026 GSoC 中的两个软件方向：为运行中的 GR4 flowgraph 提供 Web 监控 OOT 模块，以及实现 CyberEther 与 GNU Radio 的图形化互操作。适合远程实验平台和复杂流图可观察性建设。

## 2026-08-01 · 四主题测试发布

### [QRadioLink 0.10.2-1](https://github.com/qradiolink/qradiolink)
基于 GNU Radio 的 SDR 收发客户端，强调语音、数据和双向无线链路。适合研究 GNU Radio 应用如何组织收发状态、调制链、音频/数据接口和 GUI。

### [SDRangel 7.27.1](https://github.com/f4exb/sdrangel/blob/master/CHANGELOG)
综合 SDR 收发与分析工作台，覆盖多硬件后端、频谱和瀑布图、channelizer、信道插件及远程控制。适合从设备抽象、实时 IQ pipeline 和插件化解调角度阅读。

### [rtl_433](https://github.com/merbanan/rtl_433)
面向 ISM 频段传感器、遥控器和其他低功耗设备的解码工具与协议生态，支持结构化输出和多种 SDR 输入。

## 2026-08-01 · 初始测试

### [iq_tool 2.5](https://github.com/pclov3r/iq_resample_tool)
用于 IQ 数据重采样、滤波、频率平移和校正的命令行工具，适合构建可重复的离线处理流水线。

### [FISSURE](https://github.com/ainfosec/FISSURE)
面向 RF 研究的综合软件框架，整合信号检测、分类、IQ 操作、协议分析、测试和数据归档。

## 2026-07-31

### [RF-Swift](https://github.com/PentHertz/RF-Swift)
面向 RF 工具链的隔离部署环境，用于减少 GNU Radio、Python、SoapySDR 与设备驱动之间的依赖冲突。

### [Universal Radio Hacker](https://github.com/jopohl/urh)
面向 OOK、FSK、GFSK 和其他专有无线协议的交互式分析工具，其多帧比较、字段划分、编码推断与 CRC 分析思路具有参考价值。

### [SDROxide](https://github.com/sdroxide/sdroxide)
Rust 编写的 SDR 客户端方向，适合关注实时 IQ 缓冲、DSP pipeline、线程模型和 Rust 在 SDR 桌面软件中的工程实践。

### [Intercept](https://github.com/luigifcruz/intercept)
将多个 SDR decoder 与信号识别能力聚合到统一界面的项目方向，体现从单纯频谱显示向信号发现、分类和解码工作流整合的趋势。
