

# Watermark-Free Studio / 无水印工作室

**Zero-install, browser-based watermark removal & smart cropping tool. Powered by client-side ONNX inpainting models. No server, no upload — everything runs locally in your browser.**

**零安装、纯浏览器端的水印去除与智能裁切工具。基于客户端 ONNX 模型进行局部修复（inpainting），无需服务器、无需上传——所有操作在本地浏览器完成。**
![scrennshot](https://github.com/CoiiChan/wasm_Watermark-Free-Studio/blob/main/screenshot1.png)
---

## Why / 为什么做

Many AI image/video generation platforms (Midjourney, Runway, Kling, etc.) embed watermarks into outputs, making downstream creative reuse difficult.

许多 AI 生图/生视频平台会在输出结果中附带水印，直接用于下游创作受限。

This tool provides two practical workflows:

本工具提供两种实用工作流：

| Scenario 场景 | Solution 方案 |
|---|---|
| **Remove existing watermarks** — Draw a mask over the watermark area, and the ONNX inpainting model fills it naturally. | **消除已有水印** — 在水印区域涂抹遮罩，ONNX 修复模型自动填补。 |
| **Pre-crop to avoid watermarks** — Before generating, expand your source canvas by ~10% to reserve space for platform watermarks. After generation, use the crop tool to precisely trim them off. | **预扩展裁切规避水印** — 生成前将素材尺寸扩展约 10% 预留给平台水印区，生成后用裁切工具精准切掉。 |

---

## Features / 特色

- **Zero install** — Open a link, works instantly. No download, no setup.
- **零安装** — 打开链接即用，无需下载安装。

- **Fully local** — ONNX inpainting model runs on your GPU/CPU via WebAssembly. Performance depends entirely on your machine.
- **完全本地运行** — ONNX 修复模型通过 WebAssembly 在你本机 GPU/CPU 上运行，性能完全取决于你的电脑配置。

- **Image inpainting** — Mask watermarks, then AI fills naturally.
- **图片修复** — 涂抹水印区域，AI 自动填补。

- **Smart crop & round corners** — Precise crop with real-time preview; adjustable corner radius for polished exports.
- **智能裁切与圆角** — 精准裁切实时预览，可调圆角半径。

- **Video crop** — Trim watermark edges from video. *(Frame-by-frame inpainting is not supported for video — encoding large frames in memory easily triggers OOM.)*
- **视频裁切** — 切掉视频边缘水印。*(视频不支持逐帧修复——逐帧编码对内存要求极高，容易触发 OOM。)*

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

## Privacy / 隐私

**This tool runs entirely in your browser. No data is ever collected, uploaded, or transmitted. Your files stay on your machine.**

**本工具完全在浏览器本地运行，不会收集、上传或传输任何用户数据。你的文件始终留在你的电脑上。**

---

## Disclaimer / 免责声明

This tool is intended to assist in the creative process (e.g., removing unintended artifacts, pre-cropping to work around platform overlays). When publishing final content to social media or platforms, please comply with each platform's watermark and content policies.

本工具旨在辅助创作过程（如去除意外瑕疵、预裁切规避平台叠加层）。在社交媒体或平台发布最终内容时，请遵守各平台的水印与内容规则。
*（内容由AI生成，仅供参考）*
