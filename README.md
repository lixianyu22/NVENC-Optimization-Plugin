## 产品介绍

Nvenc Optimization Engine 是一款基于 NVIDIA GPU 的硬件视频编解码 SDK。它封装 NVENC / NVDEC，并融合自研视频感知编码技术，其优势在于：

- 在相同画质下，相较原生 NVENC 可节省 **20% 以上**码率
- 保留 GPU 已有的**高并发**和**低延迟**编码特性
- 接入便捷，在不改变已有转码流程的前提下，可快速接入并使用

---
### 适用场景

- 直播平台 — 降低带宽成本，保持低延迟
- 视频云 / CDN — 离线转码，提升压缩效率
- 云游戏 — 高画质低码率实时编码
- UGC 短视频 — 海量视频处理的编码优化

### 数据展示

| 编码器                        | 编码标准 | 视频平均码率 |   码率节省 | VMAF 值 | GPU 占用率 | 编码最大 FPS |
| :---------------------------- | :------: | -----------: | ---------: | ------: | ---------: | -----------: |
| NVENC                         |  H.264   | 2469.11 kbps |          — |   74.84 |         3% |      555 fps |
| **Nvenc-Optimization-Engine** |  H.264   | 1732.22 kbps | **29.84%** |   75.05 |         9% |      552 fps |
| NVENC                         |  H.265   | 2466.30 kbps |          — |   81.49 |         3% |      495 fps |
| **Nvenc-Optimization-Engine** |  H.265   | 1642.37 kbps | **33.41%** |   81.95 |         9% |      494 fps |

> 测试机型：NVIDIA GeForce RTX 4060Ti
> 测试视频来自开源视频集
### 展示视频
https://evaluation-results.visionular.com/external/260729/video_compare_3840x1080_dynamic.mp4

---
### 接入流程
<img width="774" height="297" alt="截屏2026-07-29 19 56 13" src="https://github.com/user-attachments/assets/142b8deb-9ac4-43bd-a199-1a931fa69a5a" />

- 调用Nvenc Optimization Engine进行编码时不需要改变已有的转码流程，只需要替换当前的编码器即可
- Nvenc Optimization Engine支持集成至FFmpeg中

### 联系我们
- 当前SDK还在最后测试阶段，因此在github上暂时未提供。
- 如需免费试用/技术评估，请联系mkt@visionular.com	
