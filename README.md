# UmeAiRT's ComfyUI Workflows

![ComfyUI](https://img.shields.io/badge/ComfyUI-Workflow%20Collection-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

Welcome to this collection of workflows for ComfyUI, designed and optimized to work with various models and techniques. This repository is the ideal companion to the UmeAiRT Auto-Installer.

---

## Prerequisites

**IMPORTANT:** These workflows are designed to work with the specific ecosystem and custom nodes installed by the **[UmeAiRT ComfyUI Auto-Installer](https://github.com/UmeAiRT/ComfyUI-Auto_installer)**. If you are using a standard ComfyUI installation, you will likely encounter missing node errors.

## How to Use

### Recommended Method: The Auto-Installer
The easiest way to use these workflows is through the UmeAiRT installer. It automatically clones this entire repository into the correct folder (`ComfyUI/user/default/workflows/`), giving you access to all workflows directly within the ComfyUI interface.

### Manual Method (via Release)
1.  Go to the [**Releases**](https://github.com/UmeAiRT/ComfyUI-Workflows/releases) page of this repository.
2.  Download the source code `.zip` file from the latest release.
3.  Extract the contents of the zip file into your `ComfyUI/user/default/workflows` directory.
4.  You may need to rename the extracted folder to something simple, like `UmeAiRT-Workflows`. Your final path should look like this: `ComfyUI\user\default\workflows\UmeAiRT-Workflows\FLUX...`

---

## Workflow Catalog

Here is the list of available workflows, categorized by model family.

### FLUX
Workflows optimized for models in the FLUX family.

#### Base (fp16 / fp8)
* **`TXT to IMG.json`**: Basic text-to-image generation.
* **`IMG to IMG.json`**: Basic image-to-image generation.
* **`INPAINT.json`**: For modifying or replacing part of an image (inpainting).
* **`OUTPAINT.json`**: For extending an image beyond its original borders (outpainting).
* **ControlNet**
    * `CtrlNet Canny.json`: Guides generation using Canny edges.
    * `CtrlNet Depth.json`: Guides generation using a depth map.
    * `CtrlNet HED.json`: Guides generation using soft edges (HED).
    * `CtrlNet Openpose.json`: Guides generation from a skeletal pose.
* **Tools**
    * `Background changer.json`: Workflow to change the background of an image.
    * `LoRA.json`: Example of how to use a LoRA with FLUX models.
    * `PuLID_Redux.json`: Using PuLID and Redux for face enhancement.
    * `Upscale.json`: Upscales the resolution of a generated image.

#### GGUF
Versions optimized for VRAM using quantized GGUF models. The workflows are identical to the base versions.

---

### HIDREAM
Workflows designed for the HiDream (image) model.

#### Base & GGUF
* **`HiDream - TXT to IMG.json`**: Text-to-image generation with HiDream.
* **`HiDream - IMG to IMG.json`**: Image-to-image generation with HiDream.
* **`HiDream - INPAINT.json`**: Inpainting with the specific capabilities of HiDream.

---

### LTXV
Workflows for the LTX-Video model (video generation).

#### Base & GGUF
* **`LTXV - TXT to VIDEO (base/gguf).json`**: Text-to-video generation.
* **`LTXV - IMG to VIDEO (base/gguf).json`**: Animates a starting image to create a video.

---

### WAN
Workflows for models in the WAN 2.1 family (video generation).

#### Base & GGUF
* **`TXT to VIDEO.json`**: Text-to-video generation.
* **`IMG to VIDEO.json`**: Animates an image to create a video.
* **`Face to VIDEO.json`** (GGUF): Applies an identity (face) to a video.
* **`VIDEO EXTENSION.json`**: Extends the duration of an existing video.
* **`VIDEO to LOOP.json`**: Transforms a short video into a seamless loop.
* **`StartEndFrames.json`**: Generates a video by specifying a start and an end frame.
* **Tools**
    * `Frames interpolations.json`: Increases the smoothness of a video by creating intermediate frames.
    * `Upscaler.json`: Increases the resolution of a video.
    * `Video merge.json`: Merges several video clips.

---

## Contributing

Suggestions and contributions are welcome. If you have improvements for a workflow or have created a new one that could benefit the community, feel free to open an "Issue" or a "Pull Request".

## License

This project is under the MIT License.
