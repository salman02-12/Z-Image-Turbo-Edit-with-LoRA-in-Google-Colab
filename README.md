# ⚡ Z-Image-Turbo Edit with LoRA in Google Colab

This repository contains an easy-to-use Google Colab notebook designed for **Z-Image-Turbo Edit**. Powered by ComfyUI, this tool allows you to upload an existing image and use AI to edit, modify, or reimagine it using lightning-fast GGUF models and custom LoRAs.

**🎥 Watch the Tutorial:** [Edit Images Using AI for FREE | Image to Image AI | Setup Z Image Edit with LoRA in Google Colab](https://www.youtube.com/watch?v=766BBB-sqvg)

**🚀 Run in Colab:** [Open Google Colab Notebook](https://colab.research.google.com/drive/1nKkpuLbq_hjOH3_LkVO8UvR-iBtnbvwV?usp=sharing)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salman02-12/Z-Image-Turbo-Edit-with-LoRA-in-Google-Colab/blob/main/Z_Image_Edit_CoinNoin.ipynb)

---

## ✨ Features Supported in this Notebook

This notebook automates the setup process into 3 simple steps:

1. **⚙️ Initialize Core Environment**: Sets up ComfyUI and installs the necessary GGUF processing nodes for Z-Image-Turbo.
2. **📥 High-Speed Asset Downloader & LoRA Setup**: Automatically fetches the required models (`z-image-turbo-Q8_0.gguf`, Qwen text encoders, and VAE) using Aria2c for maximum speed. It also provides tools to easily upload or download custom LoRAs.
3. **🎨 Z-Image-Turbo Edit Generation**: The core editing engine. Features include:
   * **Source Image Upload**: Easily upload the image you want to edit directly within the notebook.
   * **Prompts**: Enter your editing instructions (e.g., "Woman holding a brick") and negative prompts.
   * **Edit Controls**: Adjust the `MAX_DIMENSION` for resolution scaling and fine-tune the `DENOISE` slider to control how much the original image changes.
   * **LoRA Integration**: Apply stylistic changes using your uploaded LoRAs.
   * **Advanced Settings**: Customize Steps, CFG, Samplers, and Schedulers.

## 🛠️ How to Use

1. Click the "Open in Colab" badge above.
2. Go to **Runtime > Change runtime type** and ensure a **T4 GPU** is selected.
3. Run **Cell 1** to initialize the ComfyUI core engine.
4. Go to **Cell 2**. Select your `LORA_SOURCE` (None, Download from URL, or Upload from Computer), paste the URL if applicable, and run the cell to download all assets. 
5. Go to **Cell 3**. 
   * Ensure `UPLOAD_SOURCE_IMAGE` is checked on your first run.
   * Type your editing prompt, configure your Denoise strength, and hit Play. 
   * When prompted, upload your source image.
   * The ComfyUI server will process the edit in the background, and your new image will appear below the cell!

## 🤝 Credits
* **Notebook Creator:** [@CoinNoin](https://www.youtube.com/@CoinNoin)
* **Base Model (GGUF):** [Unsloth / Z-Image-Turbo-GGUF](https://huggingface.co/unsloth/Z-Image-Turbo-GGUF)
