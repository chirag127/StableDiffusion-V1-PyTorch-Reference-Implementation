---
name: Bug Report
about: "Report a bug in the implementation of the Stable Diffusion latent diffusion model."
title: "[Bug] - Describe the issue concisely"
labels: "bug"
assignees:

body:
  - type: markdown
    attributes:
      value: | # Use this template to report bugs. Provide as much detail as possible.
        # **1. Project Context**
        *   **Repository:** [`StableDiffusion-Latent-Diffusion-AI-Image-Generator-Python-Notebook`](https://github.com/chirag127/StableDiffusion-Latent-Diffusion-AI-Image-Generator-Python-Notebook)
        *   **AI Agent Directives Reference:** [AGENTS.md](https://github.com/chirag127/StableDiffusion-Latent-Diffusion-AI-Image-Generator-Python-Notebook/blob/main/AGENTS.md)
        *   **Issue Reporter:** @${github.actor}

        ## :bug: Bug Description
        Please provide a clear and detailed description of the bug you encountered. What did you expect to happen, and what actually happened?

  - type: markdown
    attributes:
      value: | # **2. Steps to Reproduce**
        Please provide the exact steps to reproduce the bug. If possible, include code snippets or notebook cell outputs.

        1.  Go to '...' steps
        2.  Click on '....'
        3.  Scroll down to '....'
        4.  See error

  - type: markdown
    attributes:
      value: | # **3. Environment Details**
        Specify the environment where the bug occurred. This is crucial for debugging.

        *   **Operating System:** (e.g., Windows 11, macOS Sonoma, Ubuntu 22.04)
        *   **Python Version:** (e.g., Python 3.10.12)
        *   **PyTorch Version:** (e.g., PyTorch 2.1.0)
        *   **Dependencies:** (List key installed libraries and their versions, e.g., `diffusers==0.20.0`, `transformers==4.33.0`)
        *   **Notebook Environment:** (e.g., JupyterLab 3.6.5, VS Code Notebooks)
        *   **Hardware:** (e.g., NVIDIA RTX 4090 with 24GB VRAM, Google Colab GPU, CPU)

  - type: markdown
    attributes:
      value: | # **4. Expected Behavior vs. Actual Behavior**

        **Expected Behavior:**
        [Describe what you expected to happen.]

        **Actual Behavior:**
        [Describe what actually happened.]

  - type: markdown
    attributes:
      value: | # **5. Screenshots / Logs (Optional)**
        If applicable, add screenshots to help explain the problem. You can attach files by dragging and dropping them into the comment area.

        log
        [Paste relevant log snippets here.]
        

  - type: markdown
    attributes:
      value: | # **6. Additional Information (Optional)**
        Any other context about the problem. You can provide additional information or suggestions here.
