# API Keys with Free Tiers — Starter Index

This repository is intended to become a field-organized guide to legitimate APIs that offer a free tier, with official signup links and practical setup notes.

**Current repository status:** the tracked root currently contains this README, the MIT license, a file named download, and free-api-keys-guide-report.docx. The category folders listed below are **planned, not present in the current tree**. There is not yet a working, field-organized API catalogue in the repository.

Free tiers change often. Rate limits, billing requirements, regional availability, and access policies can change without notice. Confirm the provider's official pricing and terms before depending on any listed limit.

## Planned categories

| Category | Intended coverage | Current status |
|---|---|---|
| Weather | Weather and climate data | Folder/entries not yet added |
| Maps and geolocation | Maps, geocoding, and location APIs | Folder/entries not yet added |
| AI and LLM | Model inference and AI services | Folder/entries not yet added |
| IoT cloud | Device-to-cloud APIs and dashboards | Folder/entries not yet added |
| General and miscellaneous | News, currency, source control, and other APIs | Folder/entries not yet added |

These are roadmap categories, not links to existing files. Add a category directory and its README before linking it from this page.

## Standard format for future entries

Each provider entry should include:

- **Provider and purpose** — what the service does.
- **Official documentation and signup** — links to the provider's own website.
- **Free-tier limits** — exact limits, with a date checked and a link to the official pricing/terms page.
- **Setup steps** — the actual path to create or obtain a credential, based on the provider's current UI.
- **Authentication and rate limits** — relevant headers, quotas, reset windows, and restrictions.
- **Billing and regional caveats** — including any card requirement, trial expiration, or geographic limitation.
- **Data handling and attribution** — where relevant to the API.

Do not label a service “free” based only on a blog post or third-party list. Free access may require billing details and may be subject to fair-use restrictions.

## Safe credential handling

- Never commit API keys, access tokens, passwords, or private client secrets.
- Store local credentials in environment variables or an ignored .env file.
- Commit only a .env.example file containing placeholder values.
- If a secret is exposed, revoke or rotate it with the provider. Removing it from the latest commit alone does not invalidate it.
- Do not paste working keys into issues, pull requests, screenshots, or documentation.

Example local configuration:

~~~bash
# Example only — use a locally stored credential
export SERVICE_API_KEY="your_key_here"
~~~

Application code should read the environment variable rather than embedding the value in source code.

## Current files

~~~text
.
├── README.md
├── LICENSE
├── download
└── free-api-keys-guide-report.docx
~~~

The file named download currently contains only these ignore patterns:

~~~text
.DS_Store
*.log
~~~

It is **not** a download script. It has been left in place to avoid a potentially risky rename without checking all references. The DOCX is present, but this README does not independently validate its contents, provider links, or stated limits.

## Contributing

Before adding or updating a provider:

1. Check the provider's official documentation, pricing, and terms.
2. Use direct official signup/documentation links.
3. Record the date on which the limits were checked.
4. Explain authentication, quotas, billing requirements, and important restrictions.
5. Verify that the entry contains no real credentials.
6. Check every relative Markdown link against a file that actually exists in the repository.

## License

MIT — see LICENSE.

---

## Maintenance & Audit

- **Audit date:** 23 November 2026
- **Documentation status:** README reviewed and audit record added on this date.
- **Scope and evidence:** This is a documentation-level maintenance pass. It does not establish that source code compiles, dependencies are current, security has been tested, or runtime behavior has been verified.
- **Code and tests:** No new functional code changes or test results are claimed by this README update. Run project-specific build, test, and security checks before relying on the project.
- **Maintenance baseline:** Documentation status recorded through 23 November 2026; revisit setup instructions, dependencies, security, known limitations, and tests when the project changes.

## Contact

Maintained up to 25 November 2026.

If you encounter any problems, please contact [carmodbhai@gmail.com](mailto:carmodbhai@gmail.com).
