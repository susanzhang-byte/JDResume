# JDResume V2 — Fast Evidence-First U.S. Resume Builder

> **Experimental review branch only: `v2-master-resume-builder`. The original `main` branch stays unchanged. No merge without owner approval.**

Create **ATS-readable, truthful educational résumé drafts** for two applicant types:

| Route | Intake | Output |
|---|---|---|
| **Already have a résumé** | Upload résumé + JD together; 1 concise evidence check only if needed | Tailored editable **DOCX + PDF**, original style preserved by default |
| **No résumé** | **3 grouped forms**: Profile/Education → Experience/Projects/Metrics → Skills/Review; then request JD | Reusable Master Resume Database + tailored **DOCX + PDF** |

### Why this revision?
The first V2 interview took too many turns and omitted applicant-supplied growth statistics merely because the assistant had not independently accessed internal records. This version reduces intake friction while retaining evidence-first precision.

### Metrics: truthful, useful, and correctly scoped
- **Do not fabricate or distort figures.** User-confirmed, coherent metrics from a described report **can appear in the résumé draft**, with a *separate* verification checklist. An internal report mentioned by the applicant is still **not independently verified** by the tool.
- Convert reported data correctly: follower **growth rate** 10% → 15% is **+5 percentage points / +50% relative growth-rate increase**, not +200%; ticket purchases 5 → 30 is **+500%**, if periods/units are comparable.
- Distinguish *supported campaign-level performance* from *individual causation*. Do not say an intern “drove” team ticket-sales growth without a defensible basis.
- When numbers are contradictory, periods aren't comparable, or candidate refuses to affirm source/accuracy, omit specific figure or flag it outside the résumé; never invent proof.
- This is an **educational exercise tool**, not independent employment verification. **Human review and edits are mandatory** before real application. No ATS pass/interview guarantees.

### Quality retained
- Original résumé layout and role coverage preserved (Path A), including right-aligned job dates and page density.
- Single-column ATS-readable U.S. layout (Path B); AI/technical and language skills separate.
- Independently inspect both created Word and PDF drafts; no invented links, file claims or testing statements.
- Database stays separate from per-JD versions. No public upload of candidate data.

## Files
- [SKILL.md](SKILL.md) — two routes, short grouped forms, metric policy and delivery
- [references/interview-guide.md](references/interview-guide.md) — three-form intake
- [references/master-database-schema.md](references/master-database-schema.md) — portable evidence model
- [references/quality-checklist.md](references/quality-checklist.md) — acceptance tests
- [examples/illustrative-example.md](examples/illustrative-example.md) — fictional examples

GitHub hosting does not install the skill into ChatGPT automatically. This branch can be tested without merging.
