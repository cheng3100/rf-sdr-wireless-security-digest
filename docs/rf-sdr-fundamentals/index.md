# RF 原理精读

本页按收录时间倒序归档长期高价值 RF / SDR 原理材料；完整历史上下文见 [Weekly](../weekly/index.md)。

## 2026-09-18

### [Wireless Pi：Design of a Low-SNR Receiver](https://wirelesspi.com/design-of-a-low-snr-receiver/)
用完整 OFDM receiver 串起 multipath、CFO、AWGN、coarse/fine synchronization、FFT、channel estimation/equalization、residual phase tracking 和 iterative decoding。核心工程直觉是：低 SNR 下同步误差会直接改变 channel estimator/equalizer/decoder 是否收敛，synchronization 不是孤立前处理步骤。

## 2026-09-11

### [PySDR：TDOA](https://pysdr.org/content/tdoa)
多 receiver cross-correlation/GCC delay estimation、range-difference geometry、同步和 measurement covariance。

## 2026-09-04

### [PySDR：Filters](https://pysdr.org/content/filters)
FIR/convolution 与实时 IQ chunk/filter-state 的连续性。

## 2026-08-28

### [PySDR：Pulse Shaping](https://pysdr.org/content/pulse_shaping)
RC/RRC、ISI、matched filter、eye diagram 与 timing recovery。

## 2026-08-21

### [PySDR：RDS End-to-End](https://pysdr.org/content/rds.html)
IQ → FM demod → filtering/resampling → synchronization → BPSK → RDS parsing。

## 2026-08-14

### [PySDR：Synchronization](https://pysdr.org/content/sync.html)
Symbol timing、coarse/fine frequency synchronization 与 Costas Loop。

### [PySDR：IQ Sampling](https://pysdr.org/content/sampling.html)
复基带、正负频率、IQ imbalance 与零中频工程直觉。

## 2026-08-07

### [PySDR：Link Budgets](https://pysdr.org/zh/content-zh/link_budgets.html)
发射功率、天线、传播损耗、噪声和 SNR 的系统链路。

## 2026-08-01

### [Wireless Pi：The Fundamental Problem of Synchronization](https://wirelesspi.com/fundamental-problem-synchronization/)
载波频率、相位和符号定时同步的总体模型。

### [Wireless Pi：FLL](https://wirelesspi.com/how-a-frequency-locked-loop-fll-works/)
频率误差检测与反馈跟踪。

### [Wireless Pi：Sampling Clock Offset in OFDM](https://wirelesspi.com/effect-of-a-sampling-clock-offset-on-an-ofdm-waveform/)
SCO 对 OFDM 子载波相位与 FFT 的影响。
