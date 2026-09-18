# 会议 / 活动高质量研究

按收录时间倒序归档 RF / SDR / wireless hack 的完整会议研究链；具体材料优先于会议首页，无法验证 slides/whitepaper/tool 时明确标注。

## 2026-09-18

### [USENIX Security ’26：PrivacyShield — Relaying BLE Beacons to Counter Unsolicited Tracking](https://www.usenix.org/conference/usenixsecurity26/presentation/hofhammer)

**论文：** https://francozappa.github.io/publication/2026/pshield/paper.pdf  
**Artifact：** https://github.com/HexHive/privacyshield

研究利用 offline finding BLE beacon 缺少足够位置真实性认证这一点，把 beacon 捕获后经网络分发到远端 ESP32 relay 重放，让第三方手机在错误地点上报 beacon，从而混淆 stalking tag 的位置。Artifact 包含 Flask relay server、AirGuard Android 修改、ESP32 relay firmware、Sniffle 相关代码和 Find My location-report 工具。

**研究链：** BLE beacon → capture → network relay → ESP32 RF retransmission → crowdsourced geolocation backend → privacy effect。

**Slides 状态：当前未找到可验证的独立公开 slides URL。**

## 2026-09-11

### [GRCon26：Remote ID Spoofing Detection](https://events.gnuradio.org/event/28/contributions/887/)
用 RSSI、Doppler、AoA 等 RF 物理证据与 UAV 广播 telemetry 交叉验证。当前无 materials。

## 2026-09-04

### [USENIX Security ’26：TrojPix](https://www.usenix.org/conference/usenixsecurity26/presentation/zhang-guoming)
不可见 pixel modulation → video cable EM emission → RF capture → covert channel；论文已公开，slides 未找到。

## 2026-08-28

### [USENIX Security ’26：Injected and Leaked](https://www.usenix.org/conference/usenixsecurity26/presentation/yan-haoran)
RF injection → hardware nonlinearity → secret up-conversion → RF capture；InjectEave 展示约 30 m 音频窃听等实验。

## 2026-08-21

### [NDSS：BLERP — BLE Re-Pairing Attacks and Defenses](https://www.ndss-symposium.org/ndss-paper/blerp-ble-re-pairing-attacks-and-defenses/)
具备 paper、slides、nRF52/Mynewt/NimBLE/Scapy 工具链与真实设备验证。

## 2026-08-14

### [Black Hat USA 2026：Blind Trust in the 6 GHz Band — Weaponizing Wi-Fi AFC](https://blackhat.com/us-26/briefings/schedule/#blind-trust-in-the-6-ghz-band-weaponizing-wi-fi-automated-frequency-coordination-afc-53998)
使用具体 session fragment。当前未找到可验证独立 slides/whitepaper/tool URL。

### [Red Team SIGINT](https://www.midnightblue.nl/explore/training/red-team-sigint-practical-sdr-hacking)
覆盖 TETRA/DMR/P25、automotive、aviation、marine 等 SDR/SIGINT 场景；当前未找到 Black Hat 公开 slide deck。
