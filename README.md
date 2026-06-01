# E&L Scientific Copilot - Regulatory Workflow Cockpit

An interactive demonstration cockpit for an **Extractables & Leachables (E&L)**
scientific and regulatory review workflow, built around a fictional case study
(**NovaTera NVT-217**). It shows how an AI copilot can support toxicologists,
analytical chemists, and QA/RA teams across a connected set of deliverables.

> **AI output requires QA / Toxicology review.** The case is fictional and for
> demonstration and educational purposes only. Nothing here is regulatory,
> toxicological, or legal advice.

## Live site

If GitHub Pages is enabled for this repository, the cockpit is available at:

```
https://<your-username>.github.io/<repository-name>/
```

The entry point is `index.html`. Use the sidebar or the clickable workflow map
to open each deliverable.

## What is included

| File | Deliverable |
|------|-------------|
| `index.html` | Cockpit shell - navigation, workflow map, artifact viewer |
| `artifact1_risk_register.html` | E&L Risk Register |
| `artifact2_gap_assessment.html` | Regulatory Gap Assessment |
| `artifact3_decision_brief.html` | Risk Summary + Decision Brief |
| `artifact4_supplier_change.html` | Supplier Change Impact |
| `artifact5_readiness.html` | Regulatory Readiness |
| `workflow_diagram.html` | Standalone workflow diagram |
| `skill/el-scientific-reviewer/SKILL.md` | The E&L reviewer skill definition |

## What is intentionally NOT included

This repository does **not** contain any third-party standards or guidance
documents (ISO, USP, ICH, PQRI, FDA, EMA). Those are copyrighted by their
respective owners and cannot be redistributed. The artifacts reference the
standards by name only and do not reproduce their text. A `.gitignore` blocks
these file types from ever being committed.

## Standards referenced (by name only)

ICH Q3D (R2), ICH Q3E (draft), ICH M7 (R2); USP <661>, <1663>, <1664>;
ISO 10993-17 / -18, ISO/TS 21726; PQRI E&L recommendations; FDA and EMA
packaging and nitrosamine guidance. Obtain these from their official sources.

## Running locally

No build step. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000/
```

## License

Original works by Gaetano Bonifacio are licensed under
**CC BY-NC 4.0** (see `LICENSE`). Third-party standards are excluded and remain
under their own terms.

---

Prepared by Gaetano Bonifacio PhD, MBA | © 2026
