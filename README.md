# E&L Scientific Copilot - A Regulatory Workflow Cockpit
<img width="1319" height="535" alt="E L preview" src="https://github.com/user-attachments/assets/66e58bdc-e544-4c95-8453-1915ad5cad0f" />

An interactive cockpit for an **Extractables & Leachables (E&L)** scientific and
regulatory review workflow, built around a fictional case study
(**NovaTera NVT-217**). It shows how an AI copilot can support toxicologists,
analytical chemists, and QA/RA teams across a connected set of deliverables -
from risk register to regulatory readiness.

Repository: https://github.com/gaetanobonifacio-ux/Extractables-Leachables-cockpit

> **AI output requires QA / Toxicology review.** The case is fictional and for
> demonstration purposes only. You can r-use this tool with your drug-related documentation. Nothing here is regulatory, toxicological, or legal advice.

---

## View the cockpit

**Online (live site):**

```
https://gaetanobonifacio-ux.github.io/Extractables-Leachables-cockpit/
```

Open the link, then use the sidebar or the workflow map to move between the
five deliverables.

**On your own computer:**

1. Download this repository (green **Code** button -> **Download ZIP**) and unzip it.
2. Open `index.html` in any modern web browser.

That is all - there is no build step and nothing to install.

---

## The deliverables

| # | Deliverable | What it shows |
|---|-------------|---------------|
| 01 | E&L Risk Register | Identified extractables/leachables, scored by risk |
| 02 | Regulatory Gap Assessment | Compliance by dimension; cross-source inconsistencies |
| 03 | Risk Summary + Decision Brief | Go / no-go reasoning for reviewers |
| 04 | Supplier Change Impact | Effect of a material change on the risk picture |
| 05 | Regulatory Readiness | Submission-readiness snapshot |

A standalone workflow diagram is also included in `artifacts/workflow_diagram.html`.

---

## Install the skill

The `el-scientific-reviewer` skill teaches an AI assistant how to reason about
E&L scientific and regulatory review. To use it with Claude:

1. Locate (or create) your skills directory:
   - macOS / Linux: `~/.claude/skills/`
   - Windows: `%USERPROFILE%\.claude\skills\`
2. Copy the skill folder from this repository into it, keeping the folder name:

   ```bash
   cp -r skills/el-scientific-reviewer ~/.claude/skills/
   ```

   On Windows, copy the `skills/el-scientific-reviewer` folder into
   `%USERPROFILE%\.claude\skills\` using File Explorer.
3. Restart your assistant. The skill activates automatically when you ask about
   E&L, extractables, leachables, or related regulatory review tasks.

To remove it, delete the `el-scientific-reviewer` folder from your skills directory.

---

## Repository layout

```
.
├── index.html                       Cockpit entry point (open this)
├── artifacts/                       The five deliverables + workflow diagram
│   ├── artifact1_risk_register.html
│   ├── artifact2_gap_assessment.html
│   ├── artifact3_decision_brief.html
│   ├── artifact4_supplier_change.html
│   ├── artifact5_readiness.html
│   └── workflow_diagram.html
├── skills/
│   └── el-scientific-reviewer/      The installable skill
│       └── SKILL.md
├── README.md
└── LICENSE
```

---

## Standards referenced (by name only)

The artifacts reference these standards by name; they do **not** reproduce the
text of any standard. Obtain the documents from their official sources:

ICH Q3D (R2), ICH Q3E (draft), ICH M7 (R2); USP <661>, <1663>, <1664>;
ISO 10993-17 / -18, ISO/TS 21726; PQRI E&L recommendations; FDA and EMA
packaging and nitrosamine guidance.

---

## License

Licensed under **CC BY-NC 4.0** (see `LICENSE`). You may share and adapt the
material for non-commercial purposes with attribution to
Gaetano Bonifacio, PhD, MBA. Third-party standards are not included and remain
under their own terms.

---

Prepared by Gaetano Bonifacio PhD, MBA | © 2026
