# RF 原理精读

本页按**收录时间倒序**归档值得精读的 RF / SDR 原理文章、论文、课程和演讲。每个条目直接链接到原文；需要查看同一期三个主题的完整上下文，可前往 [Weekly](../weekly/index.md)。

## 2026-08-01

### [Phase Sync in Digital Phased Arrays Through Direct RF Sampling — Part 1](https://www.analog.com/en/resources/technical-articles/phase-sync-digital-phased-arrays-part-1.html)

讨论直接 RF 采样阵列中的多通道相位同步，重点解释共享参考时钟、确定性延迟、SYSREF、JESD204、数字下变频器与 NCO 初始相位如何共同决定通道间相位可重复性。

适合从单通道 SDR 进一步进入 AoA、波束形成、多通道相干接收与阵列校准。

## 2026-07-31

### [IQ Sampling](https://pysdr.org/content/sampling.html)

从复数、混频、下变频和采样解释 SDR 为什么输出 IQ 数据，复基带带宽与采样率如何对应，以及负频率、I/Q 不平衡和镜像抑制的工程含义。

### [Digital Modulation](https://pysdr.org/content/digital_modulation.html)

通过星座图与 Python 示例解释 symbol、bit、PSK/QAM、噪声、频偏和定时偏差，是从观察频谱进入数字解调的基础材料。

### [The Fundamental Problem of Synchronization](https://wirelesspi.com/fundamental-problem-synchronization/)

解释接收机为何必须完成载波频率、载波相位和符号定时同步，以及频偏为何会表现为 IQ 平面中的持续旋转。

### [What Is a Symbol Timing Offset and How It Distorts the Rx Signal?](https://wirelesspi.com/what-is-a-symbol-timing-offset-and-how-it-distorts-the-rx-signal/)

解释采样点偏离最佳符号时刻后，如何造成幅度损失、ISI、星座扩散和判决裕量下降，并为 Gardner 等定时恢复算法建立直觉。
