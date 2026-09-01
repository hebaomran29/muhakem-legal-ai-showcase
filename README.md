# Muhakem Legal AI · مُحكِّم

<p align="center">
  <img src="./assets/favicon.png" alt="Muhakem logo" width="110" />
</p>

<h3 align="center">Arabic-first legal intelligence for Egyptian legal workflows.</h3>

<p align="center">
  <a href="https://hebaomran29.github.io/muhakem-legal-ai-showcase/">Live Website</a> ·
  <a href="./docs/Muhakem_Project_Summary.pdf">Project Summary</a> ·
  <a href="https://github.com/hebaomran29/muhakem-legal-ai">Private Source Repository</a>
</p>

> **Muhakem is a public product showcase, not the application source code.** The complete backend, legal corpus, databases, credentials, model files, and private runtime remain outside this repository.

---

## Product overview

**Muhakem** is a research and software prototype that brings four legal workflows into one Arabic-first workspace: legal consultation, contract generation, defense-memorandum preparation, and contract review. The product is designed around a simple principle: AI should make legal work faster and more organized while keeping evidence inspection and professional judgment visible.

The showcase is intentionally static. It presents the product concept, the working prototype through short recordings, the system architecture, and the project summary without connecting to a production backend or exposing private user data.

## Why Muhakem?

Legal professionals may need to move between statutory texts, judicial rulings, commentary, previous memoranda, and contract documents before preparing a useful answer or draft. General-purpose AI can produce fluent text, but fluency alone does not guarantee a relevant Egyptian-law source, a complete contract clause, or a case-specific defense argument.

Muhakem addresses this workflow gap through specialized routing, retrieval-grounded generation, structured document pipelines, clause-level interaction, and validation before the result reaches the legal professional. The system assists the professional; it does not replace legal advice, review, or decision-making.

## Core workflows

| Workflow | Product value |
| --- | --- |
| **Legal consultation** | Arabic questions answered through a retrieval-grounded research workflow with relevant legal material. |
| **Contract generation** | Structured drafting with clause-level addition, editing, and deletion. |
| **Defense memoranda** | Case-fact structuring, crime-aware retrieval, and generation of a reviewable defense memorandum. |
| **Contract review** | OCR-assisted extraction, clause-level analysis, risk signals, and legal-basis inspection. |
| **Usage analytics** | Token, latency, operation, and estimated-cost tracking for technical and academic comparison. |

## Product walkthroughs

The [live website](https://hebaomran29.github.io/muhakem-legal-ai-showcase/) contains the four recordings below in an interactive video section. The files are kept under `assets/screenshots/` to preserve the existing public showcase structure.

| Walkthrough | File |
| --- | --- |
| Legal consultation | [`consultation.mp4`](./assets/screenshots/consultation.mp4) |
| Contract generation | [`contract-generation.mp4`](./assets/screenshots/contract-generation.mp4) |
| Defense memorandum | [`defense-memo.mp4`](./assets/screenshots/defense-memo.mp4) |
| Contract review and OCR | [`contract-review.mp4`](./assets/screenshots/contract-review.mp4) |

## Technical architecture

Muhakem separates the user interface from orchestration, retrieval, generation, document processing, and validation. This separation supports online, hybrid, and local deployment modes without changing the product surface.

```text
React / Vite workspace
        ↓
FastAPI orchestration and session services
        ↓
Specialized legal workflows
        ↓
Qdrant hybrid retrieval + embeddings + legal metadata
        ↓
LLM generation + validation + editable document output
```

### Technology map

| Layer | Technologies and responsibilities |
| --- | --- |
| Frontend | React, Vite, responsive workspace, workflow screens, usage dashboard. |
| Backend | FastAPI, session management, specialized legal pipelines, document services. |
| Retrieval | Qdrant, semantic embeddings, lexical/BM25 retrieval, legal metadata, optional graph relations. |
| AI runtime | Qwen/Ollama for local or hybrid generation, with compatible online providers when required. |
| Documents | OCR, Arabic text processing, smart chunking, clause analysis, validation, and DOCX export. |
| Evaluation | Token tracking, latency measurement, operation counts, and estimated cloud-cost comparison. |

## Repository structure

```text
.
├── assets/
│   ├── favicon.png
│   └── screenshots/
│       ├── consultation.mp4
│       ├── contract-generation.mp4
│       ├── defense-memo.mp4
│       └── contract-review.mp4
├── docs/
│   └── Muhakem_Project_Summary.pdf
├── index.html
├── style.css
└── README.md
```

## Run the showcase locally

The public showcase requires no Python environment, backend, database, API key, or model download. Open `index.html` directly in a browser, or serve the repository with any static HTTP server. The deployed website is available at:

**[hebaomran29.github.io/muhakem-legal-ai-showcase](https://hebaomran29.github.io/muhakem-legal-ai-showcase/)**

## Project team

Muhakem was developed as a graduation project by **Heba Reda Mohamed Omran, Manal Gamil Hassan Alaaeldin, Omnia Mahfouz Abdellatif Mostafa, Nehal Hammam Hassan Abdelhamed, and Mariam Magdy Abdo Mohamed Elatbany**, under the supervision of **Prof. Ghazal Abdelaty Fahmy**, within the Digilians 9 Months Diploma in AI and Data Science.

## Responsible-use boundaries

Muhakem is a research and software prototype. It is not a substitute for advice from a qualified lawyer. Generated content must be checked against applicable legislation, official sources, and the facts of the individual matter. The public repository intentionally excludes API keys, `.env` files, legal documents, user records, SQLite databases, Qdrant collections, OCR caches, model weights, and private source code.

## Portfolio links

| Resource | Link |
| --- | --- |
| Live Website | [Open the showcase](https://hebaomran29.github.io/muhakem-legal-ai-showcase/) |
| Public Repository | [Open on GitHub](https://github.com/hebaomran29/muhakem-legal-ai-showcase) |
| Project Summary | [Read the four-page PDF](./docs/Muhakem_Project_Summary.pdf) |
| Private Application Source | [Open the private repository](https://github.com/hebaomran29/muhakem-legal-ai) |

---

<p align="center"><sub>© Muhakem team · Public showcase · August 2026</sub></p>
