# FirstDraft job agent

An open-source starter for a multi-user job-search assistant aimed at students and recent graduates. It keeps the useful core of the original dashboard—shortlisted roles, match scores, application tracking and tailored documents—while adding per-user CV-format and writing-style inputs.

## Included

- Responsive job-shortlist dashboard
- Local CV template and writing-sample pickers
- Expandable tailored-document cards
- Application status tracking
- Clear privacy guidance for future production use

This first public version is deliberately a front-end demo. It does not upload, store, parse or send personal documents to an AI provider. Open `index.html` in a browser to try it.

## Production roadmap

1. Add authentication and strict separation between users.
2. Encrypt documents in transit and at rest, with export and deletion controls.
3. Parse CV structure separately from personal details.
4. Create a writing-style profile from consented samples.
5. Add provider-neutral AI generation with human review before use.
6. Connect licensed job-data sources and respect their terms.
7. Add subscriptions only after privacy, security and quality checks.

## Responsible use

- Never invent qualifications, experience or references.
- Require users to review every generated document.
- Minimise personal data and never use customer files for training without explicit consent.
- Publish a privacy notice, retention policy and subprocessors list before accepting real documents.
- Do not automate final application submission without clear user confirmation.

## License

MIT
