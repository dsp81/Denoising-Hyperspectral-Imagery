# Hyperspectral Image Denoising



This project focuses on **hyperspectral image (HSI) denoising** using a diffusion-based generative framework. Building upon the **Diff-Unmix** architecture, we enhance spectral-spatial restoration through two major contributions:
- A **custom loss function** combining perceptual loss and SVD-based thresholding.
- Ongoing work on **CLIP-guided conditioning** and **spatial transformer units** to further improve semantic understanding and structure retention.


## What's New / Ongoing Work

###  Current Extensions (Work in Progress)
- **CLIP-Guided Conditioning**: Leverages OpenAI's CLIP to extract global semantic context and guide diffusion sampling.
- **Spatial Transformer Units**: Integrating spatial attention mechanisms to better capture global structural dependencies during restoration.

---

## Original Architecture: Diff-Unmix

> *Reference Paper: "Unmixing Diffusion for Self-Supervised Hyperspectral Image Denoising" (Zeng et al., 2023)*


## Our Key Modifications

### 1.  Custom Loss Function
We redefine the training objective by combining:
- **Perceptual Loss**: Captures high-level semantic fidelity using features from a pre-trained VGG-like encoder. This helps the model retain perceptual quality beyond pixel-wise accuracy.
### 2.  SVD Thresholding
- SVD thresholding was applied during the unmixing stage to filter out spectral noise and enhance convergence stability during training.

