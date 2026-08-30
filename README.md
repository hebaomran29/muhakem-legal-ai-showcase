# Muhakem Legal AI — Public Showcase

Muhakem is an Arabic legal-AI workspace designed to help legal professionals research Egyptian law, draft contracts and defense memoranda, and review legal documents with traceable references.

> This repository is a presentation-only showcase. The full application source, backend, legal corpus, user data, model files, credentials, and private implementation are intentionally excluded.

## What the project demonstrates

| Capability | Demonstration |
| --- | --- |
| Arabic legal consultation | Conversational legal research grounded in retrieved legal material. |
| Contract generation | Structured drafting with clause-level refinement. |
| Defense-memo drafting | Organized memoranda built from facts, defenses, evidence, and requests. |
| Contract review | OCR-assisted extraction, clause analysis, legal references, and confidence indicators. |
| Usage analytics | Token counts, latency, operation breakdown, and estimated cloud-cost comparison. |

## Research and engineering focus

The project explores a privacy-conscious architecture for legal AI. It separates retrieval, generation, document processing, and presentation so that deployment can move between online, hybrid, and local environments without redesigning the user experience.

## Demo

Open [`index.html`](./index.html) locally, or use the GitHub Pages deployment when enabled. The demo is intentionally static and uses fictional examples. It does not connect to a production backend and does not process confidential legal documents.

## Privacy

Do not upload or commit API keys, `.env` files, legal documents, user records, SQLite databases, vector databases, OCR caches, model weights, or private source code to this showcase repository.

## Private source repository

The full implementation is maintained separately in a private repository. Access is intentionally restricted while the project is under development and evaluation.

## Disclaimer

Muhakem is a research and software prototype. Its outputs are not a substitute for advice from a qualified lawyer and should be reviewed against the applicable legislation and official sources.
