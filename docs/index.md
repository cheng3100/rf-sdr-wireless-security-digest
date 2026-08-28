# RF / SDR / Wireless Hack Digest

这是一个持续更新的 RF、SDR 与 wireless hack 技术情报库。每期简报先在 ChatGPT 对话中完整发送，再同步归档到本仓库，便于历史查询、分类整理和长期阅读。

## 站点结构

本站保留八个顶层入口：

1. **Home**：项目定位、范围与使用方式；
2. **Weekly**：每周完整简报归档；
3. **软件项目**：以软件实现为主的 SDR / wireless hack 动向与新项目；
4. **软硬件项目**：硬件与软件栈结合的开源 SDR / wireless hack 项目；
5. **RF / Wireless 动态**：近期行业新闻、社区事件、会议发布、监管变化、产品发布、频谱政策、安全事件与生态变化；
6. **会议研究**：Black Hat、DEF CON、USENIX Security、GRCon 等会议/活动中，以完整研究为单位的高质量 slides、whitepaper、paper、tool 与 demo；
7. **RF 原理精读**：对经典理论、基础概念和成熟工程原理进行高质量阐释的学习材料；
8. **高价值信息源**：长期维护少量稳定、高质量的 RF / SDR / wireless hack 信息来源，后续每期优先检查这些来源的增量。

## 五个长期主题

### 软件项目

覆盖 SDR 客户端、频谱与瀑布图工具、IQ 处理、解调与协议分析、GNU Radio / gr-* 模块、SoapySDR、rtl_433、URH、FISSURE、SigMF、驱动和固件工具。

### 软硬件项目

覆盖 HackRF 类开源 SDR、便携式 RF 平台、开源收发机、多通道阵列、扩展板，以及配套固件、FPGA gateware、驱动和主机软件。

### RF / Wireless 动态

按时间倒序整理近期新闻与事件，强调时效性和影响范围。内容可以包括行业、社区、会议、产品、监管、频谱政策、无线安全事件和项目生态变化，不要求每条都深入技术细节。

### 会议 / 活动高质量研究

以一个完整研究案例为单位，收录 Black Hat、DEF CON、USENIX Security、GRCon、European GNU Radio Days 等会议/活动中的 RF / SDR / wireless hack 高质量材料。典型条目会串起“发现漏洞或研究问题 → 解释 RF/协议/硬件机制 → 使用 SDR/RF 设备验证、注入、欺骗或攻击 → 给出 slides/whitepaper/paper/tool”。它不同于新闻，也不同于纯原理教程，强调综合性和长期研究参考价值。

### RF 原理精读

只收录具有长期学习价值的原理性材料，覆盖 IQ、采样、混频、滤波、调制解调、频偏、载波与符号同步、链路预算、天线、射频前端、信道和协议物理层。

**三个内容层次的区别：** RF / Wireless 动态关注“最近发生了什么”；会议研究关注“一个具体研究如何发现、解释并验证问题”；RF 原理精读关注“经典概念如何被解释清楚”。

## 高价值信息源

[长期高价值信息源](high-value-sources/index.md) 不是链接大全，而是一组经过多期验证的稳定来源。当前优先包括 PySDR、Black Hat Briefings / Trainings、Wireless Pi 与 GNU Radio 官方站点 / GRCon。列表强调质量与长期价值，不要求每期新增来源。

## 最新一期

[2026-08-28 · 第 5 期：AetherSDR、H4M Pro 开源、BlueZ 与主动电磁侧信道](weekly/2026-08-28.md)
