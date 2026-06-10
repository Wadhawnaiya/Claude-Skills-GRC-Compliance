# Contributing to Claude Skills for GRC

Thank you for your interest in contributing. This document explains how to submit improvements while keeping this repository aligned with applicable data-protection obligations, especially **India’s Digital Personal Data Protection Act, 2023 (DPDPA) and DPDP Rules, 2025**.

## Code of Conduct

- Be respectful and constructive.
- Focus on factual, regulatory-cited improvements.
- Do not submit personal data about yourself or others.

## How to Contribute

1. **Fork** the repository and create a feature branch (`git checkout -b feature/short-name`).
2. Make your changes. Keep them scoped to the framework you are updating.
3. Include **regulatory citations** (section, article, rule, or clause numbers) where guidance is amended.
4. Add or update tests/eval cases if you change behaviour.
5. **Commit** with a clear message: `type(scope): description`.
   - Examples: `fix(DPDPA): correct Rule 6 breach timeline`, `docs(ISO27001): add 2022 transition note`
6. **Push** to your fork and open a **Pull Request** against `main`.
7. Fill in the PR template. Link any related issue.

## DPDPA-Specific Contribution Rules

When updating the **DPDPA skill** (or adding India-related content):

- Cite the **Digital Personal Data Protection Act, 2023** and/or **DPDP Rules, 2025**.
- Use DPDPA terminology: **Data Fiduciary**, **Data Principal**, **Significant Data Fiduciary**, **Data Protection Board of India**.
- Flag any guidance depending on future Central Government notifications as **provisional**.
- Do not substitute GDPR concepts unless explicitly mapped and labelled as GDPR equivalents.

## Style

- Markdown: use ATX headings (`##`), fenced code blocks, and tables for requirements.
- Keep lines under ~120 chars.
- Add a short description to new files at the top in a blockquote or comment.

## Security

See [SECURITY.md](SECURITY.md) for how to report vulnerabilities.

## License

By contributing, you agree that your contributions will be licensed under the project’s **MIT License**.
