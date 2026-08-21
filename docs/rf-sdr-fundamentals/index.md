# RF 原理精读

本页按**收录时间倒序**归档值得精读的 RF / SDR 原理文章、论文、课程和演讲。每个条目直接链接到原文；需要查看同一期五个主题的完整上下文，可前往 [Weekly](../weekly/index.md)。

本页强调经典理论、基础概念和成熟工程原理的长期学习价值，不以新闻时效性为主要标准。长期优先来源见 [高价值信息源](../high-value-sources/index.md)。

## 2026-08-21

### [PySDR：End-to-End Example with RDS](https://pysdr.org/content/rds.html)
使用真实 FM 广播中的 Radio Data System（RDS）把多个 SDR/DSP 环节串成完整 receiver：IQ acquisition → FM demod → frequency shift → filtering → decimation/resampling → symbol timing → fine frequency synchronization → BPSK demod → bit/byte parsing。

适合作为 IQ Sampling、Link Budget、Synchronization 之后的整链路练习。重点不是单个算法，而是观察采样率转换、滤波、频偏和同步状态如何层层影响最终 protocol decode。

## 2026-08-14 · 高价值来源测试修订版

### [PySDR：Synchronization](https://pysdr.org/content/sync.html)
把 symbol timing、coarse frequency synchronization、fine frequency synchronization 与 Costas Loop 放进同一接收链路中解释。适合建立“先处理大频偏与采样时刻，再由细跟踪环持续收敛残余 CFO/phase”的整体模型。

PySDR 以 Pluto 在 2.4 GHz、25 ppm 条件下可能对应约 ±60 kHz CFO 为例，直观说明本振 ppm 误差如何映射为复基带中的实际频偏。

## 2026-08-14

### [PySDR：IQ Sampling](https://pysdr.org/content/sampling.html)
从复数、正负频率、混频和采样解释 SDR 为什么通常输出 I/Q 两路构成的复基带信号。建议重点理解复采样带宽、负频率、频偏导致的 IQ 平面旋转、IQ imbalance 镜像以及零中频 DC offset/LO leakage。

可配合真实 IQ 文件做三个离线实验：FFT 观察正负频率；人为加入频偏观察频谱平移和星座旋转；人为修改 I/Q 幅度或相位观察镜像 spur。

## 2026-08-07

### [PySDR：Link Budgets](https://pysdr.org/zh/content-zh/link_budgets.html)
从系统视角解释发射功率、天线增益、自由空间路径损耗、噪声带宽与 SNR 如何组成链路预算，并用 ADS-B 给出完整示例。

适合把天线、传播、前端、噪声和解调所需 SNR 连接起来，帮助从“软件看频谱”进入完整无线链路的系统思维。

## 2026-08-01 · 四主题测试发布

### [The Fundamental Problem of Synchronization](https://wirelesspi.com/fundamental-problem-synchronization/)
系统解释数字接收机为何必须分别处理载波频率、载波相位和符号定时同步，并建立“频偏导致 IQ 平面持续旋转”的工程直觉。

### [How a Frequency Locked Loop Works](https://wirelesspi.com/how-a-frequency-locked-loop-fll-works/)
从频率误差检测和反馈环路角度解释 FLL 如何跟踪载波频偏，适合在理解同步总体问题后继续阅读。

### [Effect of a Sampling Clock Offset on an OFDM Waveform](https://wirelesspi.com/effect-of-a-sampling-clock-offset-on-an-ofdm-waveform/)
解释采样时钟偏差如何在 OFDM 系统中逐步累积，并与残余 CFO、FFT 输入和子载波相位变化产生联系。

## 2026-08-01 · 初始测试

### [Phase Sync in Digital Phased Arrays Through Direct RF Sampling — Part 1](https://www.analog.com/en/resources/technical-articles/phase-sync-digital-phased-arrays-part-1.html)
讨论直接 RF 采样阵列中的多通道相位同步，重点解释共享参考时钟、确定性延迟、SYSREF、JESD204、数字下变频器与 NCO 初始相位如何共同决定通道间相位可重复性。

## 2026-07-31

### [IQ Sampling](https://pysdr.org/content/sampling.html)
从复数、混频、下变频和采样解释 SDR 为什么输出 IQ 数据，复基带带宽与采样率如何对应，以及负频率、I/Q 不平衡和镜像抑制的工程含义。

### [Digital Modulation](https://pysdr.org/content/digital_modulation.html)
通过星座图与 Python 示例解释 symbol、bit、PSK/QAM、噪声、频偏和定时偏差，是从观察频谱进入数字解调的基础材料。

### [What Is a Symbol Timing Offset and How It Distorts the Rx Signal?](https://wirelesspi.com/what-is-a-symbol-timing-offset-and-how-it-distorts-the-rx-signal/)
解释采样点偏离最佳符号时刻后，如何造成幅度损失、ISI、星座扩散和判决裕量下降，并为定时恢复算法建立直觉。
