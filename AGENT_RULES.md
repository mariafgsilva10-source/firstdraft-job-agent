# FirstDraft agent rules

Adapted from the original workflow with all personal data and credentials removed.

## Job discovery
- Use licensed APIs such as Reed and Adzuna.
- Never scrape LinkedIn, Indeed or services that prohibit automated collection.
- Let users configure titles, locations, radius, result limits and daily limits.
- Deduplicate by source and job ID. Mark a job seen only after processing.
- Keep unprocessed jobs eligible for a later run.

## Tailored writing
- Treat each user's CV and consented writing samples as the source of truth.
- Never invent experience, qualifications, dates, employers, achievements or references.
- Write directly and confidently without exaggeration or generic corporate clichés.
- Build each letter around the job description and the strongest two or three relevant examples.
- Prefer evidence to unsupported adjectives: experience, action, outcome, skill and relevance.
- Keep cover letters concise and require user review before use.
- Preserve the user's preferred CV structure while reordering truthful content for relevance.
- Return structured output that can be validated before document generation.

## Multi-user privacy
- Scope identity, contact details, CVs, samples, preferences and generated files to the authenticated user.
- Store API credentials only as encrypted deployment secrets, never in source control or browser code.
- Encrypt private documents, minimise retention, and provide export and permanent deletion.
- Never train on customer material without separate explicit consent.
- Never submit an application automatically. Require clear user confirmation.

## Required environment variables
- REED_API_KEY
- ADZUNA_APP_ID
- ADZUNA_APP_KEY
- AI_PROVIDER_API_KEY

Every deployment must use its own credentials. Never reuse another user's accounts or the original project's secrets.
