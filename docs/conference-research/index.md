# 会议 / 活动高质量研究

本页按**收录时间倒序**归档 Black Hat、DEF CON、USENIX Security、GRCon、European GNU Radio Days 等会议和活动中，与 RF / SDR / wireless hack 强相关、且具有完整研究链路的高质量材料。

这里关注的不是“会议新闻”，而是**研究本身**：发现某个 RF / wireless 漏洞或系统问题，解释协议/物理层/硬件机制，使用 SDR 或 RF 测试手段进行捕获、重放、注入、欺骗或验证，并尽量追踪 slides、whitepaper、paper、tool、video 或 demo。

## 收录标准

- 有明确研究问题或真实漏洞；
- 能解释 RF / PHY / MAC / protocol / hardware 中至少一个关键机制；
- 优先有官方 slide、whitepaper、paper、video、tool 或代码；
- 使用 SDR、RF 测试设备、无线芯片、嵌入式硬件或电磁测量手段进行验证；
- 对复现实验、协议逆向、无线安全或系统设计具有长期参考价值。

## 链接规则

- 会议研究条目必须优先给出**能直接定位到具体议题/课程/材料的链接**，不能只链接会议首页、总日程或筛选后的 track 页面；
- 对 Black Hat 这类单页 schedule，如果具体条目有 fragment ID，必须保留完整 `#fragment`；
- 若官方 slides / whitepaper / tool 已公开，直接链接材料；
- 若尚未找到可验证的公开材料链接，必须明确写“当前未找到可验证公开 slides/whitepaper/tool”，不得把会议主页或总日程冒充材料链接；
- 若无法确认官方唯一 fragment，不猜测 URL；改用作者/研究团队的独立具体技术页面作为主要入口，同时把官方 track/list 页面仅作为会议归属证明。

## 2026-08-28

### [USENIX Security ’26：Injected and Leaked — Actively Inducing Side-Channel Leakage Using Electromagnetic Injection and Hardware Nonlinearity](https://www.usenix.org/conference/usenixsecurity26/presentation/yan-haoran)

**论文 PDF：** [usenixsecurity26-yan-haoran.pdf](https://www.usenix.org/system/files/usenixsecurity26-yan-haoran.pdf)

研究把 EM injection 与 EM side-channel leakage 连接起来：攻击者主动注入 RF，让放大器、ADC、电源转换器等非线性器件把低频 secret signal 与注入 carrier 混频/调制，从而把原本难以观测的低频秘密搬移到更容易远距离接收的电磁频段。

作者设计 InjectEave，并展示使用可获得 RF equipment 对有线/无线耳机播放音频进行约 30 m 远距离窃听及穿墙实验；同时分析智能家居功耗、模拟传感器输入等低频秘密的 injection-induced leakage，以及固定电话闭环窃听/操纵案例。

**研究链路：** RF injection → hardware nonlinearity → low-frequency secret 上变频/调制到泄漏载波 → RF receiver 捕获 → signal processing/recovery → eavesdropping 或 closed-loop manipulation。

**长期价值：** 这是非常典型的“非协议型 wireless hack”：漏洞根因位于 mixed-signal hardware，SDR/RF equipment 用于频谱观察、捕获、扫描与恢复，适合扩展传统协议逆向之外的 RF 安全视角。

**slides 状态：当前未找到可验证的独立公开 slides URL。** USENIX 已公开具体 session 与论文 PDF；后续若补充 slides/video，应更新本条目。

### 本期最值得精读的会议 / 活动研究

**Injected and Leaked。**

## 2026-08-21

### BLERP：BLE Re-Pairing Attacks and Defenses

**具体研究页：** [NDSS — BLERP: BLE Re-Pairing Attacks and Defenses](https://www.ndss-symposium.org/ndss-paper/blerp-ble-re-pairing-attacks-and-defenses/)

**论文 PDF：** [2026-f121-paper.pdf](https://www.ndss-symposium.org/wp-content/uploads/2026-f121-paper.pdf)

**Slides PDF：** [f0121-sacchetti-slides.pdf](https://www.ndss-symposium.org/wp-content/uploads/f0121-sacchetti-slides.pdf)

**Black Hat Asia 2026 研究团队条目：** [EURECOM — Exploiting BLE re-pairing with the BLERP attacks](https://www.eurecom.fr/en/publication/8697?slug=exploiting-ble-re-pairing-with-the-blerp-attacks)

BLERP 研究 BLE re-pairing 的信任边界。BLE 允许已配对设备重新协商并替换安全状态/密钥，作者分析出多项设计层漏洞，包括 unauthenticated re-pairing 与 security-level downgrade，并构造 Central/Peripheral impersonation、single-channel MitM 和 double-channel MitM 等攻击。

作者还实现了 BLERP toolkit，使用低成本 **nRF52** 与 **Mynewt / NimBLE / Scapy** 做 OTA pairing/re-pairing 测试和端到端 MitM，并在 22 个目标上评估。

**研究链路：** BLE pairing/session establishment → re-pairing trust boundary → key/security-level overwrite or downgrade → nRF52 OTA tool → impersonation/MitM → mitigation。

**长期价值：** 这是很适合 wireless hack 学习的方法论样本：从规范/状态机入手，寻找 trust boundary，再用低成本无线硬件构造可复现实验，最后回到协议修复。

### 本期最值得精读的会议 / 活动研究

**BLERP。** 它的材料链非常完整：独立 research page、paper、slides、Black Hat Asia 研究条目和可复现实验工具都能串起来。

## 2026-08-14

### [Black Hat USA 2026：Blind Trust in the 6 GHz Band — Weaponizing Wi-Fi AFC](https://blackhat.com/us-26/briefings/schedule/#blind-trust-in-the-6-ghz-band-weaponizing-wi-fi-automated-frequency-coordination-afc-53998)

研究对象是 6 GHz 标准功率 Wi-Fi 使用的 Automated Frequency Coordination。Black Hat 官方日程确认该议题于 2026-08-06 11:05 举行，讲者为 Yilu Dong、Tianchang Yang，contributors 为 Arupjyoti Bhuyan、Syed Rafiul Hussain。

**Black Hat 具体议题入口：** [Blind Trust in the 6 GHz Band — Weaponizing Wi-Fi AFC](https://blackhat.com/us-26/briefings/schedule/#blind-trust-in-the-6-ghz-band-weaponizing-wi-fi-automated-frequency-coordination-afc-53998)

**具体技术背景/研究报道：** [Dark Reading — 6 GHz Wi-Fi Flaws Could Disrupt Critical Systems](https://www.darkreading.com/perimeter/6-ghz-wi-fi-flaws-disrupt-critical-systems)

**研究链路：** 6 GHz shared spectrum 规则 → AFC 输入与信任边界 → 位置/设备参数等输入被错误信任或伪造 → 频谱授权决策异常 → 潜在 RF 干扰与共存风险。

**slides / whitepaper / tool 状态：** 当前未找到可验证的独立公开 slides / whitepaper / tool URL。

### Red Team SIGINT — Practical SDR hacking for mission-critical, automotive, aviation, and marine targets

**主要具体入口：** [Midnight Blue — Red Team SIGINT: Practical SDR hacking](https://www.midnightblue.nl/explore/training/red-team-sigint-practical-sdr-hacking)

**Black Hat 官方归属/课程列表证明：** [Black Hat USA 2026 Wireless Training](https://blackhat.com/us-26/training/schedule/index.html?track%5B%5D=wireless)

**相关具体案例材料：** [Midnight Blue — Analyzing the Taiwan High-Speed Rail (THSR) TETRA cyber incident, part 1](https://www.midnightblue.nl/blog/analyzing-the-taiwan-high-speed-rail-thsr-tetra-cyber-incident-part-1)

课程覆盖 RF、SDR、SIGINT、未知信号识别，以及 automotive、aviation、marine、physical access、TETRA、DMR、P25 等 mission-critical radio。

**slides / lab / tool 状态：** 当前未找到可验证的 Black Hat 公开 slide deck URL。
