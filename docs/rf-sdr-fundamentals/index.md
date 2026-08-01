# RF 原理精读

本页按**收录时间倒序**归档值得精读的 RF / SDR 原理文章、论文、课程和演讲。每个条目直接链接到原文；需要查看同一期四个主题的完整上下文，可前往 [Weekly](../weekly/index.md)。

本页强调经典理论、基础概念和成熟工程原理的长期学习价值，不以新闻时效性为主要标准。

## 2026-08-01 · 四主题测试发布

### [The Fundamental Problem of Synchronization](https://wirelesspi.com/fundamental-problem-synchronization/)

系统解释数字接收机为何必须分别处理载波频率、载波相位和符号定时同步，并建立“频偏导致 IQ 平面持续旋转”的工程直觉。

适合作为后续学习 FLL、PLL、Gardner、Mueller and Müller、Costas loop 和 OFDM 同步的总入口。

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
