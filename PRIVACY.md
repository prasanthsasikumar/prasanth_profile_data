# Privacy and Redaction Guidelines

This folder is intended for safe use with LLMs/agents. Apply the following:

1) Personal Identifiers
- Use professional email aliases or mask: prasanth[at]example[dot]com.
- Phone: last 4 digits only if needed. Avoid full numbers.

2) Compensation
- Prefer percentiles or ranges over exact amounts.
- Include benchmark source when claiming high remuneration.

3) Evidence
- Link to evidence stored elsewhere (e.g., EB1A_Application/02_Exhibit_Evidence/*).
- Avoid duplicating sensitive PDFs here.

4) Redaction Log
- Record any masking decisions in redactions.log with date, field, reason.

5) Access Control
- If you share this folder or put it under version control, ensure secrets are excluded by .gitignore and review files before publishing.

6) Data Hygiene
- Use schema_version for each YAML file.
- Keep items concise to ease chunking and retrieval.
