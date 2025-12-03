# Contributing to StableDiffusion-Latent-Diffusion-AI-Image-Generator-Python-Notebook

Thank you for considering contributing to this project. We aim to maintain a high standard of quality, velocity, and future-proofing, aligning with the Apex Technical Authority's principles.

## 1. Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to the maintainer at [chirag127@example.com](mailto:chirag127@example.com).

## 2. How to Contribute

We welcome contributions of all forms, including bug reports, feature requests, documentation improvements, and code contributions. All contributions should be made via pull requests.

### 2.1. Getting Started

1.  **Fork the repository:** Create your own copy of the repository on GitHub.
2.  **Clone your fork:** `git clone https://github.com/chirag127/StableDiffusion-Latent-Diffusion-AI-Image-Generator-Python-Notebook.git`
3.  **Set up your development environment:**
    *   Ensure you have Python 3.10+ installed.
    *   Use `uv` for package management:
        bash
        uv venv .venv
        source .venv/bin/activate
        uv pip install -r requirements.txt
        
    *   Verify environment setup and linting:
        bash
        ruff check .
        pytest tests/
        

### 2.2. Development Workflow

1.  **Create a new branch:** For each new feature or bug fix, create a dedicated branch from the `main` branch:
    bash
    git checkout -b feature/your-feature-name
    
    or
    bash
    git checkout -b bugfix/your-bug-fix-name
    
2.  **Make your changes:** Implement your feature or fix the bug.
3.  **Write tests:** Ensure your changes are covered by appropriate tests. New features should have corresponding tests, and bug fixes should ideally have tests that reproduce the bug before the fix.
4.  **Lint and format:** Run the linter and formatter to ensure code consistency:
    bash
    ruff format .
    ruff check .
    
5.  **Run tests:** Execute the test suite to ensure everything works as expected:
    bash
    pytest
    
6.  **Commit your changes:** Use clear and concise commit messages. Follow conventional commit message guidelines if possible.
    bash
    git commit -m "feat: Add support for conditional image generation"
    
7.  **Push your branch:** Push your changes to your fork on GitHub:
    bash
    git push origin feature/your-feature-name
    
8.  **Open a Pull Request:** Create a pull request from your branch to the `main` branch of the original repository (`chirag127/StableDiffusion-Latent-Diffusion-AI-Image-Generator-Python-Notebook`).

### 2.3. Contribution Guidelines

*   **Code Quality:** Adhere to the principles of SOLID, DRY, and YAGNI. Write clean, readable, and maintainable code.
*   **Testing:** All code contributions must include comprehensive tests. Aim for high code coverage.
*   **Documentation:** Keep documentation up-to-date, including READMEs, docstrings, and any other relevant files.
*   **AI Agent Directives:** Ensure any new AI-related logic aligns with the directives specified in `AGENTS.md` and maintains robust error handling.

## 3. Submitting a Pull Request

When submitting a pull request, please:

*   Describe your changes clearly in the pull request description.
*   Reference any relevant issues using keywords (e.g., `Fixes #123`, `Closes #456`).
*   Ensure your pull request passes all automated checks (CI/CD).

## 4. Reporting Bugs

If you find a bug, please open an issue on GitHub. Provide as much detail as possible:

*   **Version:** The version of the software you are using.
*   **Environment:** Your operating system, Python version, and any relevant dependencies.
*   **Steps to Reproduce:** Clear, step-by-step instructions to reproduce the bug.
*   **Expected Behavior:** What you expected to happen.
*   **Actual Behavior:** What actually happened.
*   **Screenshots/Logs:** Any relevant screenshots or error logs.

## 5. Feature Requests

If you have an idea for a new feature, please open an issue on GitHub to discuss it before implementing it. This helps ensure that the feature aligns with the project's goals and direction.

## 6. Project Standards

This project follows the Apex Technical Authority's guidelines, emphasizing:

*   **Zero-Defect:** Strive for bug-free code.
*   **High-Velocity:** Efficient development and contribution process.
*   **Future-Proof:** Utilizing modern standards and maintainable architecture.

We are using the following technologies and principles:

*   **Python 3.10+**
*   **uv:** Package management and dependency resolution.
*   **Ruff:** Linting and formatting.
*   **Pytest:** Testing framework.
*   **Jupyter Notebooks:** For experimentation and demonstration.
*   **Architecture:** Modular Monolith principles applied within the notebook context.
*   **AI Integration:** Clear contracts and error handling for any model interactions.

By contributing, you agree to abide by these standards and guidelines.
