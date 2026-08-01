# 软硬件项目

本页按**收录时间倒序**归档软硬件结合的 SDR / wireless hack 开源项目。每个条目直接链接到项目仓库、论文或官方页面；需要查看同一期四个主题的完整上下文，可前往 [Weekly](../weekly/index.md)。

## 2026-08-01 · 四主题测试发布

### [Maia SDR v0.12.0](https://github.com/maia-sdr/maia-sdr/releases)

面向 ADALM-Pluto 的开源 FPGA SDR 系统，由 Amaranth HDL、Rust 嵌入式服务、内核模块和 WebAssembly UI 组成，支持高采样率实时瀑布图和 SigMF IQ 录制。

### [PortaPack Mayhem 2.4.0](https://github.com/portapack-mayhem/mayhem-firmware)

运行在 HackRF + PortaPack 上的社区固件，把 USB SDR 扩展为带显示、存储和设备端应用的便携 RF 平台，适合研究有限算力下的 UI、DSP 与硬件控制协同。

### [HackRF 2026.01.3](https://github.com/greatscottgadgets/hackrf)

从 RF 硬件、CPLD、MCU 固件到 libhackrf 和主机工具均开放的完整 SDR 平台，适合从 USB streaming、buffer 生命周期和软硬件边界角度系统学习。

## 2026-07-31

### [Field-Deployable RF Capture System](https://arxiv.org/abs/2607.01368)

由 HackRF One、Raspberry Pi 5、GNSS 与高速 SSD 组成的便携 IQ 采集节点，重点涉及 USB streaming、持续写盘、时间与位置元数据及 SigMF 归档。

### [OpenWXSDR](https://github.com/dl2sba/openwxsd)

将 RTL-SDR 或 Airspy 与 Linux 主机组合成长期无人值守的探空气球接收平台，适合观察多 SDR 管理、自动扫描、任务调度与持续解码。

### [Open.Space](https://github.com/open-space-foundation)

面向低成本可拼接 SDR 阵列的开源方向，适合学习多通道时钟、相位同步、阵元校准和数字波束形成。
