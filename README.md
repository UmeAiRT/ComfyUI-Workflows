# UmeAiRT's ComfyUI Workflows

![ComfyUI](https://img.shields.io/badge/ComfyUI-Workflow%20Collection-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
[![Auto-Sync](https://img.shields.io/badge/Auto--Sync-Supported-cyan)](https://github.com/UmeAiRT/ComfyUI-UmeAiRT-Sync)

Welcome to this collection of workflows for ComfyUI, designed and optimized to work with various models and techniques. This repository is the ideal companion to the UmeAiRT ecosystem.

---

## Prerequisites

**IMPORTANT:** These workflows are designed to work with the specific ecosystem and custom nodes installed by the **[UmeAiRT ComfyUI Auto-Installer](https://github.com/UmeAiRT/ComfyUI-Auto_installer)**. If you are using a standard ComfyUI installation, you might encounter missing node errors.

---

## How to Use

### 🥇 Method 1: Auto-Sync (Recommended)
**Forget manual downloads.** Use my custom loader node to keep your workflows automatically updated every time you start ComfyUI.

1. Open **ComfyUI Manager**.
2. Search for and install **`ComfyUI-UmeAiRT-Sync`**.
3. Restart ComfyUI.
4. Your workflows will appear automatically in `ComfyUI/user/default/workflows/UmeAiRT`.

### 🥈 Method 2: The Auto-Installer
If you are setting up ComfyUI from scratch, the UmeAiRT installer automatically clones this entire repository into the correct folder during the installation process.

### 🥉 Method 3: Manual Method
1.  Go to the `ComfyUI/user/default/workflows` directory.
2.  Execute the command `git clone https://github.com/UmeAiRT/ComfyUI-Workflows`.

---

## 📂 Naming Convention

To make finding files easier, workflows now follow a strict naming convention: `Model_Function_Variant.json`.

* **Standard:** `Flux_Txt2Img.json` (Base version)
* **GGUF:** `Flux_Txt2Img_GGUF.json` (Optimized for low VRAM)
* **Nunchaku:** `Flux_Txt2Img_Nunchaku.json` (Specific backend)

---

## Workflow Catalog

Here is the list of available workflows, categorized by model family.

### ⚡ FLUX
Workflows optimized for models in the FLUX family.

#### Generation
* **`Flux_Txt2Img.json`**: Basic text-to-image generation.
* **`Flux_Img2Img.json`**: Transform an existing image.
* **`Flux_Kontext.json`**: Advanced contextual generation.

#### Editing
* **`Flux_Inpaint.json`**: Modify or replace specific areas of an image.
* **`Flux_Outpaint.json`**: Extend an image beyond its original borders.

#### Tools & ControlNet
* **`Flux_ControlNet_*.json`**: Precise control using Canny, Depth, HED, or OpenPose.
* **`Flux_LoRA.json`**: How to implement LoRA adapters.
* **`Flux_Upscale.json`**: High-fidelity upscaling.

---

### 🎨 SDXL
Robust workflows for Stable Diffusion XL.

#### Generation
* **`SDXL_Txt2Img.json`**: High-quality generation from prompt.
* **`SDXL_Img2Img.json`**: Image variation and restyling.

#### Editing
* **`SDXL_Inpaint.json`**: Seamless object removal or addition.
* **`SDXL_Outpaint.json`**: Canvas expansion.

#### Tools
* **`SDXL_ControlNet.json`**: Structure guidance.
* **`SDXL_LoraTester.json`**: Utility to quickly test LoRA weights.

---

### 🖌️ Z-IMAGE
Workflows for the Z-Image generation model.

* **`Z-Image_Txt2Img.json`**: Standard generation.
* **`Z-Image_Img2Img.json`**: Image-to-image transformation.
* **`Z-Image_Inpaint.json`**: Native inpainting capabilities.

---

### 🖼️ HIDREAM
Workflows designed for the HiDream model.

* **`HiDream_Txt2Img.json`**: Text-to-image generation.
* **`HiDream_Img2Img.json`**: Image transformation.
* **`HiDream_Inpaint.json`**: Native inpainting capabilities.

---

### 🎬 LTXV
Workflows for the LTX-Video model.

* **`LTXV_Txt2Video.json`**: Create short clips from text.
* **`LTXV_Img2Video.json`**: Animate static images.

---

### 🎥 WAN
Workflows for models in the WAN family.

#### WAN 2.1
* **`Wan_Txt2Video.json`**: Standard text-to-video.
* **`Wan_Img2Video.json`**: Standard image-to-video.
* **`Wan_Face2Video.json`**: Character consistency in video.
* **`Wan_Video_Extension.json`**: Extend clip duration.
* **`Wan_Video2Loop.json`**: Create seamless loops.
* **`Wan_VACE.json`**: Advanced Video Composition/Editing.

#### WAN 2.2
* **`Wan2.2_Txt2Video.json`**: High-quality 720p text-to-video generation.
* **`Wan2.2_Img2Video.json`**: Image animation with the new 2.2 model.
* **`Wan2.2_Txt2Img.json`**: Still image generation capabilities.
* **`Wan2.2_Img2Img.json`**: Image-to-image transformation.
* **`Wan2.2_StartEndFrame.json`**: Generate video bridging a start and end image.
* **`Wan2.2_FunControl.json`**: Advanced control features for video generation.

---

### 🛠️ General Tools
Utility tasks compatible with multiple models.

* **`Img2Txt_Caption.json`**: Extract prompts from images (JoyTag/WD14).
* **`Video_Interpolation.json`**: Smooth out frame rates.
* **`Video_Upscaler.json`**: Simple upscaling for any video.
* **`Video_Merge.json`**: Stitch multiple video clips together.

---

## Contributing

Suggestions and contributions are welcome. If you have improvements for a workflow or have created a new one that could benefit the community, feel free to open an "Issue" or a "Pull Request".

## License

This project is under the MIT License.
