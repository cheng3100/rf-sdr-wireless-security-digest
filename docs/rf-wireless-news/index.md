# RF / Wireless 动态

本页按更新时间倒序归档 RF、SDR 与 wireless 相关的近期动态和新闻，并直接附原始来源；完整历史上下文见 [Weekly](../weekly/index.md)。

## 2026-09-18

### [CVE-2026-16769：RS9116W/SiWx917 plaintext pause-encryption request DoS](https://symaro.com/cve/cve-2026-16769.html)
2026-09-08 公开，影响 Silicon Labs RS9116W/SiWx917。无线范围内未认证 peer 可发送未加密 pause-encryption request，设备错误处理本应受保护的状态消息并进入 DoS。该问题对应 [Proteus state-machine mutation testing 论文](https://arxiv.org/abs/2409.02905) 中的 B-E10，适合从“packet fuzzing → protocol state/property fuzzing”角度研究。

### [GRCon26 即将举行](https://events.gnuradio.org/event/28/)
会议 2026-09-21 开始。多个具体 contribution 目前仍显示 `There are no materials yet`；下一期优先检查 slides/paper/code/video 的实际发布，而非重复总日程。

## 2026-09-11

### [CVE-2026-5706](https://www.cve.org/CVERecord?id=CVE-2026-5706)
Silicon Labs Bluetooth Mesh extended advertisement OOB write/stack corruption。

## 2026-09-04

### [DJI Bluetooth DUML：CVE-2026-78306](https://github.com/advisories/ghsa-vq46-xr65-w8q7)
Bluetooth 控制面可修改 Wi-Fi 配置，体现跨无线链路 attack surface。

## 2026-08-28

### [BlueZ A2DP：CVE-2026-19774](https://www.zerodayinitiative.com/advisories/ZDI-26-589/)
A2DP stream endpoint 栈溢出。

### BlueZ EIR discovery：CVE-2026-80186
Discovery metadata 路径栈溢出。

## 2026-08-21

### Wi-Fi beamforming feedback 隐私侧信道
PHY feedback 被重新用于人体识别，提示 Wi-Fi sensing/CSI 的隐私边界。

### [FCC Unlicensed D2D](https://www.fcc.gov/document/fcc-looks-expand-d2d-satellite-connectivity-unlicensed-wireless)
探索 Part 15 设备与卫星直接通信。

## 2026-08-14

### [Black Hat USA 2026：Blind Trust in the 6 GHz Band](https://blackhat.com/us-26/briefings/schedule/#blind-trust-in-the-6-ghz-band-weaponizing-wi-fi-automated-frequency-coordination-afc-53998)
6 GHz Wi-Fi AFC 安全研究。

### [European GNU Radio Days 2026](https://gnuradiodays.sciencesconf.org/)
覆盖 SDR 网络安全、5G/6G、卫星、频谱监测、侧信道与 TEMPEST。
