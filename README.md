# RF / SDR / Wireless Security Digest

面向 RF、SDR 与无线安全研究的长期技术情报库。

内容分为两类开源项目：

1. **软件为主**：SDR 客户端、频谱/瀑布图、解调与协议分析、GNU Radio 模块、URH、rtl_433、FISSURE、SigMF 工具链等。
2. **软硬件一体**：HackRF 类开源 SDR、便携式 RF 平台、阵列、探针、扩展板，以及配套固件和主机软件。

同时持续收录无线协议安全研究、RF/SDR 原理文章、协议逆向案例和可执行实验。

## 本地预览

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

## 在线发布

仓库包含 GitHub Actions 工作流。启用 GitHub Pages 并将 Source 设为 **GitHub Actions** 后，推送到 `main` 会自动部署。
