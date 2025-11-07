# Prasanth Profile Data

This repository stores structured profile data (YAML/JSON) and short narratives (Markdown) for generating bios, CVs, timelines, and evidence-backed summaries. It’s designed to be consumed by a companion app (frontend + backend) for Q&A and automation.

## What’s inside

- `identity.yml` — Core profile facts (contacts, links, metrics, memberships)
- `index.json` — Simple index for tools/agents
- `timeline/` — Positions and roles (one file per role)
- `awards/` — Awards and recognitions
- `publications/` — Papers/articles/preprints with DOIs and citation metadata
- `claims/eb1a_criteria.yml` — EB1A criteria → evidence mapping
- `narratives/bio_short.md` — Short bio referencing item ids
- `PRIVACY.md` — Redaction and PII handling guidelines

Conventions
- ISO dates (YYYY-MM-DD), stable ids, currency codes (USD/INR), and explicit units
- Cross-reference by ids (e.g., `evidence_refs: ["pub:pub_2020_chi_gaze_hand"]`)
- Keep large PDFs and private documents outside this repo; link to them instead

## Using this with a UI (profile-app)

The companion UI can read data directly from this repo using raw GitHub URLs (read-only) or by cloning as a submodule.

Recommended (simple, read-only):
- Fetch files via `https://raw.githubusercontent.com/<user>/prasanth_profile_data/<branch>/<path>`
- Cache responses in the app for performance

Alternative (local dev or advanced):
- Add this repo as a git submodule in the app and read files from disk
- Or sync a copy at build time

## Roadmap (next)

- Complete 2024 publication metadata (authors, DOIs, venue counts)
- Add JMUI 2020 citation metrics (Springer)
- Verify IEEE VR 2024 metadata and ISMAR 2019 author list
- Optional: Add `trips/` for travel documents with `meta.yml` per trip

## Privacy

Do not store sensitive PII here. For private documents (e.g., IDs, tickets, letters), use a private storage (e.g., Google Drive) and link references only.

