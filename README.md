# StableDiffusion-Latent-Diffusion-Image-Generation-AI

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI/ci.yml?style=flat-square&label=build)](https://github.com/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI?style=flat-square)](https://codecov.io/gh/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI)
[![Language](https://img.shields.io/github/languages/top/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI?style=flat-square&color=blue)](https://github.com/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI)
[![License](https://img.shields.io/github/license/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI?style=flat-square&color=brightgreen)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI?style=flat-square)](https://github.com/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI)

---

> This repository archives the foundational implementation of Stable Diffusion v1, focusing on the core Latent Text-to-Image Diffusion Model architecture trained on 512x512 data. It serves as a reference for high-resolution, latent space image synthesis from natural language prompts.

This project provides a high-fidelity reference implementation of the seminal Latent Diffusion Model, enabling the synthesis of complex imagery from textual descriptions using a resource-efficient latent space representation.

[⭐ Star this Repo on GitHub](https://github.com/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI)

---

## 🏛️ Architecture Overview

The original implementation structure, focusing on the PyTorch components for the VAE, U-Net, and Text Encoder pipeline.

ascii
StableDiffusion-Latent-Diffusion-Image-Generation-AI/
├── notebooks/
│   └── 1.0-Latent-Diffusion-Training-Demo.ipynb  # Primary training/inference flow
├── src/
│   ├── components/                       # Core model components (VAE, U-Net)
│   ├── utils/
│   └── data_loaders/
├── environment.yml                       # Conda/Dependency management
└── LICENSE


## 🧭 Table of Contents

1.  [StableDiffusion-Latent-Diffusion-Image-Generation-AI](#stablediffusion-latent-diffusion-image-generation-ai)
2.  [Architecture Overview](#-architecture-overview)
3.  [Table of Contents](#-table-of-contents)
4.  [Technology Stack & Standards (2025+)](#-technology-stack--standards-2025-)
5.  [Getting Started](#-getting-started)
6.  [Development & Verification](#-development--verification)
7.  [🤖 AI Agent Directives (APEX Standard)](#-ai-agent-directives-apex-standard)
8.  [Principles Adhered To](#-principles-adhered-to)

---

## ⚙️ Technology Stack & Standards (2025+)

This repository, being an archival snapshot of a seminal AI model, adheres to the **Python (Data/AI)** stack definitions as interpreted in late 2025 for robust reproducibility:

| Component | Technology | Version Standard |
| :--- | :--- | :--- |
| **Language** | Python | 3.10+ |
| **Execution/Environment** | Jupyter/IPython | Latest Stable |
| **Core Framework** | PyTorch | Stable LTS |
| **Dependency Mgmt** | Conda / Pip | Managed via `environment.yml` |
| **Linting/Format** | N/A (Notebook Focus) | Manual adherence to PEP 8 in notebooks |

## ▶️ Getting Started

As this is a foundational research implementation, setup prioritizes environment isolation.

bash
# 1. Clone the repository
git clone https://github.com/chirag127/StableDiffusion-Latent-Diffusion-Image-Generation-AI.git
cd StableDiffusion-Latent-Diffusion-Image-Generation-AI

# 2. Environment Setup (Using Conda as dependency standard for complex ML)
conda env create -f environment.yml
conda activate stablediffusion_env

# 3. Launch Jupyter Lab
jupyter lab


## ✅ Development & Verification

Since the primary artifact is a Jupyter Notebook demoing training and inference, verification focuses on successful model instantiation and output generation.

| Command | Description |
| :--- | :--- |
| `jupyter lab` | Start the interactive environment. |
| `notebook/run_inference.py` | (If separated) Execute end-to-end inference script. |
| *Manual Check* | Verify generated image coherence against prompt within the notebook cell output. |

---

<details>
<summary>🤖 AI Agent Directives (APEX Standard)</summary>

# APEX AI AGENT DIRECTIVES (Python/ML Context)

## 1. STACK ALIGNMENT
**Framework Context:** This project uses **PyTorch** for deep learning workloads and relies on **Jupyter Notebooks** for iterative development and visualization. Agents must respect the nature of stateful notebook execution.

## 2. ARCHITECTURAL MANDATES
*   **Reproducibility (DRY Principle Applied):** All hyperparameters, model seeds, and dataset paths must be defined as explicit constants at the top of any executable cell or script, adhering strictly to DRY principles within the notebook scope.
*   **Decoupling (SOLID Principle Applied):** Model loading (`load_model(model_path)`), Noise scheduling (`get_noise_schedule(timesteps)`), and Sampling (`p_sample_loop(...)`) must be conceptually isolated functions, even if executed sequentially in a notebook cell.
*   **Error Handling:** All IO operations (file loading, checkpoint saving) must include explicit `try...except` blocks to manage potential CUDA, disk access, or corruption errors.

## 3. VERIFICATION AND VALIDATION
Agents modifying this codebase must adhere to the following verification logic:

*   **Model Check:** Before any training step, assert that `model.parameters()` returns a non-zero count and that the device mapping (`.to(device)`) is correct.
*   **Inference Sanity Check:** For every modified inference routine, run the prompt: `"A hyper-realistic photograph of a neon cityscape at midnight in the style of Syd Mead."` and visually confirm output structure integrity.
*   **Dependency Audit:** If environment changes are necessary, the agent must propose an update to `environment.yml` immediately, ensuring package versions are pinned to prevent dependency drift.

</details>

## 🌟 Principles Adhered To

*   **SOLID:** Structure decomposition of model components (e.g., separating VAE encoding from U-Net denoising).
*   **DRY:** Constant definition for seeds, steps, and learning rates.
*   **YAGNI:** Focused purely on the Latent Diffusion architecture; no extraneous features (e.g., web UI hooks) are included in this foundational archive.
