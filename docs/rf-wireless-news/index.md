# RF / Wireless 动态

本页按更新时间倒序归档 RF、SDR 与 wireless hack 相关的近期动态和新闻，并直接附上原始来源链接。

## 与 RF 原理精读的区别

- **RF / Wireless 动态**：看重时效性，回答“最近发生了什么、可能带来什么影响”。新闻可以偏行业、社区、产品、监管或安全事件，不要求都深入技术细节。
- **RF 原理精读**：看重长期学习价值，回答“某个经典理论或成熟工程概念如何被解释清楚”。内容不以最新为必要条件。

## 2026-08-07

### [GRCon26 初步日程公布](https://events.gnuradio.org/event/28/overview)

GRCon26 将于 9 月 21—25 日在 Raleigh 举办，主会场初步日程已公布，最后一天安排 AERPAW 室外无线实验平台演示。会议覆盖 FutureG、认知无线电、机器学习、Massive MIMO、同步、无线安全、SigMF 与硬件加速。

### [European GNU Radio Days 2026 聚焦 SDR 网络安全](https://www.gnuradio.org/news/2026-07-04-EuGRD26-announce/)

EuGRD2026 将于 11 月 16—18 日在 Rennes 举办，重点覆盖 SDR 网络安全、5G/6G、卫星通信、频谱监测、雷达感知、侧信道和 TEMPEST。

### [TrojPix：数字视频线缆电磁隐蔽信道](https://www.usenix.org/conference/usenixsecurity26/presentation/zhang-guoming)

研究通过不可见像素调制控制视频线缆的电磁辐射，在多种商用显示器和线缆上报告最高 8.1 Mbps、最远 208 米的实验结果。它把 RF 安全研究扩展到非无线设备的非预期电磁发射。

## 2026-08-01

### [AT&T 完成 230 亿美元 EchoStar 频谱交易](https://www.reuters.com/business/media-telecom/att-closes-23-billion-deal-acquire-spectrum-echostar-2026-07-28/)

AT&T 获得约 50 MHz 的美国全国性频谱，包括约 30 MHz 的 3.45 GHz 中频段和约 20 MHz 的 600 MHz 低频段。该事件反映运营商仍同时强化低频覆盖资源与中频容量资源。

对 SDR 和无线研究而言，商业频谱资产变化会影响未来网络部署、频段利用密度和可观测的空口环境，也提醒实验者将频谱政策和产业部署纳入技术观察。

### [PortaPack Mayhem 持续发布 nightly 构建](https://github.com/portapack-mayhem/mayhem-firmware/releases)

Mayhem 社区在稳定版本之外保持高频迭代，近期变更继续改进 FLEX、POCSAG 等协议的接收、纠错结果呈现和消息格式。

这说明便携 SDR 生态的重点正从单纯增加功能，逐渐扩展到协议细节、错误处理和现场可用性。
