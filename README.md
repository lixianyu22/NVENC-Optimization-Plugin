# NVENC Optimization Engine

Hardware video encoding & decoding SDK built on NVIDIA GPUs. Wraps native NVENC / NVDEC with Visionular's proprietary perceptual encoding technology.

---

## Overview

- **20%+ bitrate savings** over native NVENC at equal or better VMAF quality
- **High concurrency & low latency** — retains native NVENC's performance characteristics
- **Drop-in integration** — no changes to your existing transcoding pipeline

---

## Use Cases

| Scenario                   | Benefit                                                      |
| :------------------------- | :----------------------------------------------------------- |
| Live streaming platforms   | Cut bandwidth costs while sustaining low end-to-end latency  |
| Cloud video & CDN services | Improve compression efficiency for offline batch transcoding |
| Cloud gaming               | Real-time, high-fidelity encoding at constrained bitrates    |
| UGC short-video platforms  | Optimize encoding for large-scale video processing           |

---

## Benchmark Data

> Test hardware: NVIDIA GeForce RTX 4060 Ti
> Test clips: publicly available standard test sequences

| Encoder                       | Standard | Average Bitrate | Bitrate Savings |  VMAF | GPU Usage | Max FPS |
| :---------------------------- | :------: | --------------: | --------------: | ----: | --------: | ------: |
| Native NVENC                  |  H.264   |    2469.11 kbps |               — | 74.84 |        3% | 555 fps |
| **NVENC Optimization Engine** |  H.264   |    1732.22 kbps |      **29.84%** | 75.05 |        9% | 552 fps |
| Native NVENC                  |  H.265   |    2466.30 kbps |               — | 81.49 |        3% | 495 fps |
| **NVENC Optimization Engine** |  H.265   |    1642.37 kbps |      **33.41%** | 81.95 |        9% | 494 fps |

---

## Demo Video

Side-by-side comparison of NVENC Optimization Engine vs native NVENC:

> [Watch comparison video](https://evaluation-results.visionular.com/external/260729/video_compare_3840x1080_dynamic.mp4)

---

## Integration

No overhaul required — simply replace your current encoder:

1. **FFmpeg integration** — drop-in custom encoder plugin
2. **Direct API** — C / C++ API for custom pipelines

---

## Contact

The SDK is currently in final validation and available through our early access program.

For a free trial or technical evaluation: **mkt@visionular.com**
