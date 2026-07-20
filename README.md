# FlaxseedsPro Documentation

Everything exists for the main website.

## Quick Start

```bash
pip install -r requirements.txt
mkdocs serve     # http://localhost:8000
mkdocs build     # site/ directory for deployment
```

## Deployment

This repository deploys to **Cloudflare Pages**. The production branch is `main`.

Every push to `main` triggers an automatic build and deploy. Preview deployments are created for all pull requests.

## Structure

```
flaxseedspro-docs/
├── docs/                      # Documentation source
│   ├── index.md              # Homepage
│   ├── products/             # Product technical specs (5)
│   ├── production-equipment/ # Equipment specs (7)
│   ├── technical-documents/  # Process tech + QC (2)
│   ├── faq/                  # Technical FAQ
│   ├── glossary/             # Industry terminology
│   ├── guides/               # Technical guides
│   ├── research/             # Research overview
│   ├── white-papers/         # White paper index
│   ├── certificates/         # Certification listing
│   ├── resources/            # External links
│   └── about/                # Company info
├── overrides/                # Theme overrides (JSON-LD)
└── .github/workflows/        # CI/CD pipeline
```

## Principles

- **Production First** — Stable plugins only. No experimental dependencies.
- **Zero Error** — CommonMark compliant. All links relative. No broken references.
- **Main Website First** — Every document page links back to the main website.
- **Human Expert Writing** — Technical documentation style. No AI writing patterns.
- **Professional Depth** — Information density. Real parameters and data.
- **Authority Flow** — JSON-LD Schema guides search authority from docs back to main website.
- **Stable > Simple > Features** — Choose stability over minimalism over feature quantity.
