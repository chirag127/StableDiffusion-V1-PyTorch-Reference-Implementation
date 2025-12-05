# Security Policy

## Supported Versions

We are committed to maintaining a secure codebase. As this is a reference implementation and foundational AI model, we prioritize security for all actively maintained versions. Currently, we actively support:

*   The latest released version


## Reporting a Vulnerability

We appreciate your efforts to responsibly disclose security vulnerabilities. Please follow these steps to report a vulnerability:

1.  **Check for Public Disclosures:** First, check the project's [Issues](https://github.com/chirag127/StableDiffusion-V1-PyTorch-Reference-Implementation/issues) and [Pull Requests](https://github.com/chirag127/StableDiffusion-V1-PyTorch-Reference-Implementation/pulls) to see if the vulnerability has already been reported or addressed.

2.  **Private Disclosure:** If you believe you have found a new security vulnerability, please **DO NOT** open a public issue. Instead, send a detailed report to the maintainer via email at:
    *   `chirag.24.jain@gmail.com`

3.  **Report Content:** Your security report should include:
    *   A clear and concise description of the vulnerability.
    *   The affected version(s) of the software.
    *   Detailed steps to reproduce the vulnerability.
    *   Any relevant code snippets or environment details.
    *   Your suggested mitigation or fix, if any.

4.  **Response and Communication:** Upon receiving your report, we will:
    *   Acknowledge receipt of your email within **72 hours**.
    *   Triage the reported vulnerability and assess its impact.
    *   Keep you informed of our progress towards a fix.
    *   Coordinate with you on the disclosure timeline once a fix is available.

## Security Best Practices for Users

When using this reference implementation, please adhere to the following security best practices:

*   **Input Validation:** Always sanitize and validate any user-provided input before passing it to the model or its associated processing functions. This is especially critical if integrating this code into a larger application.
*   **Dependency Management:** Regularly update your dependencies (PyTorch, Python, and any other libraries) to their latest secure versions. This repository uses `uv` for dependency management, facilitating easier updates.
*   **Environment Security:** Ensure your development and deployment environments are secure. This includes restricting access to sensitive data and using secure network configurations.
*   **Model Loading:** Be cautious when loading models from untrusted sources. While this repository provides a reference implementation, real-world applications should implement robust checks for model integrity.

## Vulnerability Disclosure Timeline

We aim to follow a responsible disclosure process. Once a vulnerability is confirmed and a fix is developed, we will aim to release the fix promptly and publicly disclose the vulnerability and its resolution. The exact timeline will depend on the severity and complexity of the vulnerability.