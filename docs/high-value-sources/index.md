# 长期高价值信息源

本页维护一组**稳定、小而精**的 RF / SDR / wireless hack 长期信息源。它不是链接大全，也不要求每次 Weekly 更新都新增来源。

维护原则：

- 优先保留能够持续、系统性地产出高质量内容的来源；
- 每期检索时优先检查这些来源是否有新材料，再进行更广泛搜索；
- 某来源只有在多个更新周期中反复证明有价值时才加入；
- 来源短期没有更新是正常的，不因“保持新鲜”而替换；
- 原理学习与最新动态分开评价：经典文章可以长期保留，会议/项目站点则重点检查增量。

## PySDR

**入口：** [PySDR: A Guide to SDR and DSP using Python](https://pysdr.org/)

**是什么：** Marc Lichtman 编写的免费在线 SDR / DSP 教材，以图示、Python 示例和工程直觉解释无线通信与软件无线电。

**长期价值：** 内容结构系统，覆盖 IQ、采样、FFT、滤波、数字调制、链路预算、信道编码、SigMF、同步等核心主题；历史 Weekly 已多次从这里选出高价值原理文章。

**适合关注：**

- IQ / complex baseband；
- sampling / aliasing / FFT；
- filtering / pulse shaping；
- digital modulation；
- link budget / noise / SNR；
- IQ file / SigMF；
- carrier、timing、frame synchronization。

**使用注意：** 更适合作为原理学习主线，而不是追求新闻时效性。后续优先检查章节新增、重大修订以及与当前学习主题直接相关的章节，不必每期重复收录。

**代表内容：** [IQ Sampling](https://pysdr.org/content/sampling.html) · [Link Budgets](https://pysdr.org/content/link_budgets.html) · [Synchronization](https://pysdr.org/content/sync.html)

## Black Hat Briefings / Trainings

**入口：** [Black Hat Briefings](https://blackhat.com/briefings/)

**是什么：** Black Hat 官方会议内容库。Briefings 会公开会议议程，并在演讲者提供材料时发布 slides、whitepapers 和 tools；Training 中也会出现较系统的硬件、无线和 SDR 课程。

**长期价值：** 对 wireless hack 而言，其价值不只在“安全新闻”，而在于经常出现将 RF 原理、真实硬件、协议、攻击面和实验方法结合起来的材料，尤其适合寻找软硬结合的 SDR/RF slides 与安全研究案例。

**适合关注：**

- Wireless / Network Security；
- Hardware / Embedded；
- Cyber-Physical Systems & IoT；
- RF / SDR / SIGINT；
- Wi-Fi / Bluetooth / cellular / mission-critical radio；
- electromagnetic side channel / TEMPEST；
- automotive、aviation、marine 与 physical access RF。

**使用注意：** Black Hat 内容质量和与 RF 的相关性差异较大，后续只筛选真正涉及无线物理层、频谱、射频硬件、协议空口或电磁侧信道的内容，不因为会议热度而泛化收录。优先链接官方 session page 和官方 Presentation Material。

**代表内容：** [Black Hat USA 2026 Briefings](https://blackhat.com/us-26/briefings.html) · [Black Hat USA 2026 Schedule](https://blackhat.com/us-26/briefings/schedule/) · [Red Team SIGINT Training](https://blackhat.com/us-26/training/schedule/index.html?track%5B%5D=wireless)

## Wireless Pi

**入口：** [Wireless Pi](https://wirelesspi.com/)

**是什么：** Qasim Chaudhari 长期维护的无线通信、DSP 与 SDR 技术站点，以直觉化方式深入解释同步、调制、PLL/FLL、定时恢复等接收机核心问题。

**长期价值：** 历史 Weekly 已反复引用其同步系列；相比单篇教程，它的优势是多个文章之间能组成连续学习路径。

**适合关注：** carrier/timing synchronization、Costas loop、FLL、PLL、Gardner/Mueller and Muller、MSK/CPFSK、OFDM impairment。

**使用注意：** 很多文章并非最新发布，但原理长期有效，因此评价重点是解释质量和学习路径，而不是发布日期。

**代表内容：** [The Fundamental Problem of Synchronization](https://wirelesspi.com/fundamental-problem-synchronization/) · [Mueller and Muller Timing Synchronization](https://wirelesspi.com/mueller-and-muller-timing-synchronization-algorithm/) · [Costas Loop](https://wirelesspi.com/costas-loop-for-carrier-phase-synchronization/)

## GNU Radio 官方站点 / GRCon

**入口：** [GNU Radio](https://www.gnuradio.org/) · [GNU Radio Events](https://events.gnuradio.org/)

**是什么：** GNU Radio 项目官方新闻、教程、版本方向和 GRCon/European GNU Radio Days 等社区会议入口。

**长期价值：** 同时覆盖 SDR 软件框架演进和真实应用方向。会议内容经常涉及无线安全、Massive MIMO、同步、FutureG、卫星、雷达、SigMF、硬件加速与实验平台，适合作为“开源 SDR 社区正在做什么”的长期观察源。

**适合关注：** GNU Radio 4、OOT modules、硬件接入、HIL、无线安全、频谱监测、雷达/定位、5G/6G、SATCOM、SigMF。

**使用注意：** 官方新闻适合动态栏目；教程和高质量会议技术材料可进入原理精读或软件/软硬件项目栏目。避免只因会议公布日程就重复收录相同信息。
