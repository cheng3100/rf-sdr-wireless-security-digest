# 软硬件项目

本页按**收录时间倒序**归档软硬件结合的 SDR / wireless 开源项目。每个条目直接链接到项目仓库、论文或官方页面；需要查看同一期四个主题的完整上下文，可前往 [Weekly](../weekly/index.md)。

## 2026-08-14 · 高价值来源测试修订版

### [PortaPack Mayhem Nightly 2026-07-26](https://github.com/portapack-mayhem/mayhem-firmware/releases)
7 月 nightly 中出现 TETRA RX、VOR Navigation、EPIRB TX SGB 等无线应用相关变化。它持续体现 HackRF + PortaPack 这种受限嵌入式 RF 平台如何在 UI、DSP、存储和协议应用之间做资源取舍。

### [Maia SDR](https://maia-sdr.org/)
继续作为“RFIC + FPGA + Linux + Web UI”架构代表：AD936x 负责 RF 收发，FPGA 承担高带宽频谱/DSP 数据面，ARM/Linux 运行设备服务并导出 SigMF 数据。

## 2026-08-14

### [PortaRF](https://www.cnx-software.com/2026/05/14/portarf-single-board-sdr-mixes-hackrf-one-and-portapack-h4m-hardware-adds-ai-voice-control/)
2026 年出现的开源单板便携 SDR，尝试把 HackRF One 与 PortaPack H4M 的能力整合到一块 PCB 上，适合研究成熟 SDR 生态如何从板卡组合向完整设备演进。

### [PortaPack Mayhem](https://github.com/portapack-mayhem/mayhem-firmware)
稳定版为 2.4.0，同时保持大量 nightly 构建。项目持续展示受限 CPU/内存条件下 UI、DSP、存储和 RF 控制的协同问题。

### [Maia SDR](https://maia-sdr.org/)
以 ADALM-Pluto/Pluto+ 为主要平台，把高带宽 FFT/频谱处理放到 FPGA，ARM 侧运行 Rust 服务，并通过浏览器展示瀑布图和导出 SigMF IQ。

## 2026-08-07

### [PortaPack Mayhem Nightly 2026-07-26](https://github.com/portapack-mayhem/mayhem-firmware/releases)
7 月继续保持 nightly 构建。项目把 HackRF、显示、按键、存储和设备端 RF 应用组合为便携平台，近期演进持续聚焦协议细节、UI 和现场稳定性。

### [Maia SDR v0.12.0](https://github.com/maia-sdr/maia-sdr/releases)
基于 ADALM-Pluto 的 FPGA SDR 项目，v0.12.0 更新 Rust 2024 生态及多个内部组件，继续提供高采样率瀑布图、Web UI 和 SigMF IQ 录制。

### [Pluto+](https://github.com/plutoplus/plutoplus)
在 PlutoSDR 架构上扩展 Ethernet、外部参考时钟和 SD 卡等能力，并开放原理图与固件构建方法。适合研究 Zynq、AD936x、IIO、FPGA HDL 与 Linux 固件的完整边界。

## 2026-08-01 · 四主题测试发布

### [Maia SDR v0.12.0](https://github.com/maia-sdr/maia-sdr/releases)
面向 ADALM-Pluto 的开源 FPGA SDR 系统，由 Amaranth HDL、Rust 嵌入式服务、内核模块和 WebAssembly UI 组成，支持高采样率实时瀑布图和 SigMF IQ 录制。

### [PortaPack Mayhem 2.4.0](https://github.com/portapack-mayhem/mayhem-firmware)
运行在 HackRF + PortaPack 上的社区固件，把 USB SDR 扩展为带显示、存储和设备端应用的便携 RF 平台。

### [HackRF 2026.01.3](https://github.com/greatscottgadgets/hackrf)
从 RF 硬件、CPLD、MCU 固件到 libhackrf 和主机工具均开放的完整 SDR 平台，适合从 USB streaming、buffer 生命周期和软硬件边界角度系统学习。

## 2026-07-31

### [Field-Deployable RF Capture System](https://arxiv.org/abs/2607.01368)
由 HackRF One、Raspberry Pi 5、GNSS 与高速 SSD 组成的便携 IQ 采集节点，重点涉及 USB streaming、持续写盘、时间与位置元数据及 SigMF 归档。

### [OpenWXSDR](https://github.com/dl2sba/openwxsd)
将 RTL-SDR 或 Airspy 与 Linux 主机组合成长期无人值守的探空气球接收平台，适合观察多 SDR 管理、自动扫描、任务调度与持续解码。

### [Open.Space](https://github.com/open-space-foundation)
面向低成本可拼接 SDR 阵列的开源方向，适合学习多通道时钟、相位同步、阵元校准和数字波束形成。
