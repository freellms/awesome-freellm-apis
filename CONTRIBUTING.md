# Contributing to Freellms

First of all, thank you for considering contributing to this repository! We want to build a high-quality global resource for free LLMs APIs.

To ensure this list remains useful and high-quality, please review the following guidelines.

## Submission Guidelines

### 1. No Spam or Pure Advertising
This repository is dedicated to APIs that offer **genuine free tiers** for developers. 
- Do **NOT** submit PRs or Issues that are purely promotional for paid-only services.
- Submissions just asking for inclusion without clear details on the free tier limits will be rejected.
- We welcome services that have paid tiers, provided they have a distinct, usable free tier.

### 2. Formatting Your Contribution
When adding a new API to the list, please use the same table format as the provider tables in `README.md` (data is synced from freellms.org, so keep the entry in the same shape).

**Example Entry:**
```markdown
| Provider | Free Models | Credit Card? | Max Context | Modalities | Get API Key |
| --- | --- | --- | --- | --- | --- |
| [Provider Name](URL) | 3 | No | 128K | text | [Get Key →](key-url) |
```

**Config snippets** for AI tools (Claude Code, Cursor, Codex, etc.) belong in `code-examples/` as a separate Markdown file — include the exact `baseURL`, model IDs, and environment variables needed.

### 3. Global Project
This is a global project with READMEs in multiple languages (`README.md`, `README.zh-CN.md`, etc.).
- When adding an API, please add it to the primary `README.md` (English) at a minimum.
- If you can, we highly appreciate updates to the localized README files to keep them in sync.

## How to Submit

1. Fork the repository.
2. Create a new branch (`git checkout -b add-new-api`).
3. Add your changes following the formatting guidelines above.
4. Commit your changes (`git commit -m 'Add NewAPI to the list'`).
5. Push to the branch (`git push origin add-new-api`).
6. Open a Pull Request and complete the PR checklist.

Thank you for your contributions!
