# 协议逆向

整理从 IQ 捕获到独立 decoder 的完整方法：

1. 记录中心频率、采样率、增益和时间元数据；
2. 判断调制方式与占用带宽；
3. 估计 symbol rate 与帧边界；
4. 判断 line coding、bit order、whitening 与 scrambling；
5. 比较多帧并识别地址、计数器和 payload；
6. 推导 checksum / CRC；
7. 使用 Python 或 GNU Radio 独立复现 decoder。
