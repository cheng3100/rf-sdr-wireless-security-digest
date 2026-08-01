# 软件项目

本页按**收录时间倒序**归档以软件实现为主的 SDR / wireless hack 项目。每个条目直接链接到项目仓库或官方页面；需要查看同一期四个主题的完整上下文，可前往 [Weekly](../weekly/index.md)。

## 2026-08-01 · 四主题测试发布

### [QRadioLink 0.10.2-1](https://github.com/qradiolink/qradiolink)

基于 GNU Radio 的 SDR 收发客户端，强调语音、数据和双向无线链路。适合研究 GNU Radio 应用如何组织收发状态、调制链、音频/数据接口和 GUI。

### [SDRangel 7.27.1](https://github.com/f4exb/sdrangel/blob/master/CHANGELOG)

综合 SDR 收发与分析工作台，覆盖多硬件后端、频谱和瀑布图、channelizer、信道插件及远程控制。适合从设备抽象、实时 IQ pipeline 和插件化解调角度阅读。

### [rtl_433](https://github.com/merbanan/rtl_433)

面向 ISM 频段传感器、遥控器和其他低功耗设备的解码工具与协议生态，支持结构化输出和多种 SDR 输入。适合作为 Sub-GHz 协议逆向成果工程化的参考。

## 2026-08-01 · 初始测试

### [iq_tool 2.5](https://github.com/pclov3r/iq_resample_tool)

用于 IQ 数据重采样、滤波、频率平移和校正的命令行工具，适合放在 SDR 采集与 URH、GNU Radio、Python decoder 之间，构建可重复的离线处理流水线。

### [FISSURE](https://github.com/ainfosec/FISSURE)

面向 RF 研究的综合软件框架，整合信号检测、分类、IQ 操作、协议分析、测试和数据归档。适合从单一信号工具扩展到完整研究工作流后再投入使用。

## 2026-07-31

### [RF-Swift](https://github.com/PentHertz/RF-Swift)

面向 RF 工具链的隔离部署环境，用于减少 GNU Radio、Python、SoapySDR 与设备驱动之间的依赖冲突，适合建立可复现的 PC 或 Raspberry Pi 实验环境。

### [Universal Radio Hacker](https://github.com/jopohl/urh)

面向 OOK、FSK、GFSK 和其他专有无线协议的交互式逆向工具。经典仓库已归档，但其多帧比较、字段划分、编码推断与 CRC 分析思路仍具有参考价值。

### [SDROxide](https://github.com/sdroxide/sdroxide)

Rust 编写的 SDR 客户端方向，适合关注实时 IQ 缓冲、DSP pipeline、线程模型和 Rust 在 SDR 桌面软件中的工程实践。

### [Intercept](https://github.com/luigifcruz/intercept)

将多个 SDR decoder 与信号识别能力聚合到统一界面的项目方向，体现从单纯频谱显示向信号发现、分类和解码工作流整合的趋势。
