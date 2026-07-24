
# Watermark-Free Studio / 无水印工作室

**零安装、纯浏览器端的水印去除与智能裁切工具。基于客户端 ONNX 模型进行局部修复（inpainting），无需服务器、无需上传——所有操作在本地浏览器完成。**

**Zero-install, browser-based watermark removal & smart cropping tool. Powered by client-side ONNX inpainting models. No server, no upload — everything runs locally in your browser.**

![scrennshot](https://github.com/CoiiChan/wasm_Watermark-Free-Studio/blob/main/screenshot1.png)
---

## Mouse & Scroll Wheel / 滚轮操作

| Action 操作 | Effect 效果 |
|---|---|
| Scroll wheel (image mode) | Adjust corner radius — scroll up to decrease, down to increase |
| 滚轮（图片模式） | 调节圆角半径 — 上滚减小，下滚增大 |
| Scroll wheel (hover on CRF slider) | Adjust video quality — scroll up to decrease CRF (better quality), down to increase |
| 滚轮（悬停 CRF 滑块） | 调节视频质量 — 上滚降低 CRF（更高质量），下滚提高 |
| Scroll wheel (smudge brush active) | Adjust brush size — scroll up to decrease, down to increase |
| 滚轮（涂抹笔刷激活时） | 调节笔刷大小 — 上滚减小，下滚增大 |

---
## Features / 特色

- **Zero install** — Open a link, works instantly. No download, no setup.
- **Fully local** — ONNX inpainting model runs on your GPU/CPU via WebAssembly. Performance depends entirely on your machine.
- **Image inpainting** — Mask watermarks, then AI fills naturally.
- **Smart crop & round corners** — Precise crop with real-time preview; adjustable corner radius for polished exports.


- **Video crop** — Trim watermark edges from video. *(Frame-by-frame inpainting is not supported for video — encoding large frames in memory easily triggers OOM.)*
- **视频裁切** — 切掉视频边缘水印。*(视频不支持逐帧修复——逐帧编码对内存要求极高，容易触发 OOM。)*
- **零安装** — 打开链接即用，无需下载安装。
- **完全本地运行** — ONNX 修复模型通过 WebAssembly 在你本机 GPU/CPU 上运行，性能完全取决于你的电脑配置。
- **图片修复** — 涂抹水印区域，AI 自动填补。
- **智能裁切与圆角** — 精准裁切实时预览，可调圆角半径。

---

## Disclaimer / 免责声明

**This tool runs entirely in your browser. No data is ever collected, uploaded, or transmitted. Your files stay on your machine.**

This tool is intended to assist in the creative process (e.g., removing unintended artifacts, pre-cropping to work around platform overlays). When publishing final content to social media or platforms, please comply with each platform's watermark and content policies.

