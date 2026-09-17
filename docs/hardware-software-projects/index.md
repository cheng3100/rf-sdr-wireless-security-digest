# 软硬件项目

本页按**收录时间倒序**归档软硬件结合的 SDR / wireless 开源项目；完整历史上下文见 [Weekly](../weekly/index.md)。

## 2026-09-18

### [gr-autopilot：Closed-Loop GNU Radio Flowgraph Synthesis with SDR HIL](https://events.gnuradio.org/event/28/contributions/867/)
GRCon26 项目把 LLM/MCP flowgraph generation 闭环到 USRP/ADALM-Pluto：生成 Tx/Rx flowgraph → 部署真实 SDR → 受控 RF path 测试 → 根据真实 RF feedback 迭代。长期价值在于把时钟、CFO、gain、noise、channel impairment 等真实硬件因素纳入自动 SDR 开发/回归闭环。当前 contribution 页面尚无 presentation materials。

## 2026-09-11

### [RFSoC4x2 + GNU Radio 高带宽 SDR](https://events.gnuradio.org/event/28/contributions/870/)
公开代码 [strath-sdr/rfsoc_qsfp_offload](https://github.com/strath-sdr/rfsoc_qsfp_offload)，覆盖 100GbE streaming、PYNQ.remote/gRPC、运行时 DUC/DDC 和 PL DDR burst capture。

## 2026-09-04

### [Meshtastic 2.8.0 Alpha](https://github.com/meshtastic/firmware)
LoRa mesh 引入 public-key node identity、XEdDSA packet signing 等身份/认证方向。

## 2026-08-28

### [PortaPack H4M Pro 开源硬件](https://github.com/portapack-mayhem/mayhem-firmware/pull/3298)
PCB、Gerber 和 schematic 文件合入 Mayhem。

## 2026-08-21

### [Pocket SDR v0.19](https://github.com/tomojitakasu/PocketSDR)
多通道 GNSS RF frontend、IF 采集与完整接收机。

### [HackRF](https://github.com/greatscottgadgets/hackrf)
持续演进 HackRF Pro radio configuration 能力。

## 2026-08-14

### [PortaPack Mayhem](https://github.com/portapack-mayhem/mayhem-firmware)
HackRF + PortaPack 便携 RF 平台。

### [Maia SDR](https://maia-sdr.org/)
AD936x + FPGA + Linux + Web UI 的完整 SDR 系统样本。

### [Pluto+](https://github.com/plutoplus/plutoplus)
PlutoSDR 扩展 Ethernet、外部参考时钟与 SD 卡。

## 2026-07-31

### [Field-Deployable RF Capture System](https://arxiv.org/abs/2607.01368)
HackRF One + Raspberry Pi 5 + GNSS + SSD 的便携 IQ 采集节点。

### [Open.Space](https://github.com/open-space-foundation)
低成本可拼接 SDR 阵列与多通道同步方向。
