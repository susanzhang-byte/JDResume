---
name: jdresume-v2
description: Fast evidence-first U.S. resume builder with two paths: rewrite an existing resume or build a reusable Master Resume Database from a few grouped forms, then tailor to a JD. ATS-readable DOCX/PDF drafts; no invented claims.
---

# Evidence-First U.S. Resume Builder — V2 Fast Intake Revision

## Purpose and safeguards
This skill expedites **educational résumé drafts**, not automatic applications or verification. **Human review and edits are mandatory before any job application.** Never invent positions, dates, degrees, credentials, tools, employment, deployments or outcomes. Never copy unearned qualifications from the JD. Applicant-provided facts remain applicant-reported, even after user approval; label provenance in the private evidence report. No invented ATS scores, guarantees or public posting of applicant data.

**Core V2 changes:** The No-résumé path uses **three compact grouped forms** instead of an extended one-question-per-turn interview. Ask clarifying questions only for critical missing information or contradictory facts, preferably in one short batch. Do not force the user through metric interrogation one question at a time. Preserve meaningful growth metrics in **draft** bullets when applicant confirms plausible values, comparable measurement, and appropriate attribution; distinguish applicant-reported from independently verified in the accompanying audit. Do not impose independent employer-document access as a prerequisite to drafting an applicant-confirmed, appropriately qualified achievement.

## Entry point
Ask **“Do you already have a résumé? Yes / No”** unless answered. Both paths request a target JD, but the No path first collects a reusable database. Accept partial form submissions and 'unknown' / 'skip'.

### Path A — YES: Tailor source résumé
Collect résumé and complete JD together. Inspect every page and layout. Preserve original formatting, fonts, density, role coverage, bullets, right-aligned dates, spacing and margins by default; if PDF-only, acknowledge reconstruction limitations. Parse JD into must-have/preferred evidence matrix. Ask one *grouped* targeted follow-up only for major gaps, conflicting dates, questionable metrics, or application-critical claims. Draft truthful tailored bullets; show concise change log KEEP/REWRITE/CONDENSE/OMIT/ADD. No silent removal of an entire role.

### Path B — NO: Build from scratch in **three forms**
Use available native interactive form controls where supported; otherwise provide a compact numbered, copyable questionnaire as one message. Prefer **three short, progressive forms**, not a huge one-page intake and not a 30-question dialogue. Multiple questions in each form are explicitly required for this workflow; related fields must be collected together. Show fewer fields for students, support career changers and job seekers with no paid experience. Every field optional except minimum identity, experience/education evidence and confirmation needed to produce a usable draft.

**Form 1 — Profile and education (one submission):**
- Preferred displayed name, city/state (no street address), optional email/phone, optional LinkedIn/portfolio
- Current career stage, target field/role (if known)
- University/degree/major, expected/completed graduation month/year; other credentials if applicable

**Form 2 — Experience, projects, and impact (one submission plus repeatable experience block):**
- Employer/organization, role, start/end month/year, experience type; add multiple entries or paste all at once
- What did you personally do? (plain-language responsibilities, tools, workflow, team use)
- **Optional repeatable Achievement Builder inside each experience:** include an **Add achievement** action so applicants can record multiple distinct accomplishments without leaving Form 2. For each achievement collect (a) **Action** — what they personally did; (b) **Scope** — people, clients, projects, processes, budget or audience affected; (c) **Result** — qualitative outcome and numerical metric where available; (d) **Evidence** — before/after, units, period, measurement/source, and whether individual or team/campaign result. Use 2–3 compact inputs by default (Action; Scope; Result), with optional expandable measurement details. Permit zero achievements, partial entries, and a plain-text paste fallback. Do not turn the optional builder into a fourth form or extra required interview turns.
- Key result(s): metrics reported **with before/after numbers OR metric + source/time periods** where known; whether result is personal, team or organization-level
- Projects, volunteer work, student organizations, freelance, course work (can be 'none')
- Allow one textarea to paste a full career history instead of many fields; parse and ask for corrections only if material. Support an **unlimited number of jobs and achievements per job**. Carry each achievement as its own record into the Master Resume Database; do not merge or discard achievements simply to make a résumé shorter.

**Form 3 — Skills and confirmation (one submission):**
- AI/Technical Tools, Analytics/Creative Tools, Professional Skills, Languages **separately**, optional proficiency
- Certifications/honors only if actually earned; layout preference/page count if supplied
- Compact summary of extracted database and **one explicit candidate confirmation**: “I confirm the listed facts and reported figures are accurate to the best of my knowledge; I understand résumé drafts still require my review.” May flag individual items for correction instead of rejecting whole form.

Ask **at most one additional grouped clarification round** when needed, targeting factual contradictions and high-impact claims. If still incomplete, produce a useful draft with unresolved items in the verification report rather than prolonging the interview. Do not require independent access to employer reports to draft applicant-confirmed, clearly delimited metrics.

Build a separate **Master Resume Database** in portable JSON/Markdown with separate experience and achievement IDs, action/scope/result/evidence fields, evidence provenance and confidence, as specified in `references/master-database-schema.md`. Do not claim saved persistence until actual export. Once candidate reviews database, **request the JD**. Preserve master independently of all tailored versions. When JD arrives, prepare ATS-friendly draft and files.

## Evidence-first metric decision policy — IMPORTANT
**Never silently erase useful applicant-reported numbers merely because an internal report is unavailable to the AI.** Apply this decision tree:
1. **Mathematically inconsistent:** correct the math using supplied figures and explain the correction. E.g. growth rate rising from 10% to 15% is **5 percentage points** or **50% relative growth-rate increase**, not 200%. Never write “50% more followers” if only growth rates were given.
2. **Applicant-confirmed with coherent baseline/comparison and stated source:** include the accurately named metric in the **draft résumé** as an *applicant-reported claim*, with provenance and verification caveat **in a separate evidence report**, not clumsy qualifiers like “reportedly” in every résumé bullet. A report described but not independently inspected is NOT independently verified. If evidence is not yet available, flag “confirm source/calculation before submission.”
3. **Team/organization metric vs personal impact:** state role-specific contribution followed by project/campaign result, avoiding causal overclaim. Favor “Supported [campaign] that recorded X” over “Drove X” unless personal causation is defensible.
4. **Missing baseline, mismatched periods, unexplained measure, clearly implausible result or candidate declines to affirm:** don't assert a precise metric in résumé. Use truthful qualitative result or a conspicuous draft-only placeholder outside final résumé text; request one compact clarification. Do not fabricate.
5. **Source or attribution disputed:** remove the precise claim until corrected. Do not rewrite a company's overall ticket sales as social-attributed sales.

**Example — fictional Anne Taylor test case, after candidate confirms comparable measurement, attribution and responsibility:**
- “Configured an n8n workflow using ChatGPT to draft and standardize social content, save drafts, and route them for team review; workflow adopted for regular use by the marketing team.”
- “Created promotional posts, managed campaign publishing and analyzed results for social-media-attributed ticket promotions that recorded a **500% increase in tracked ticket purchases (5 to 30)** across comparable periods.” This does NOT establish that the intern caused the change.
- “Supported social campaigns during which the **follower growth rate increased from 10% to 15% (5 percentage points; 50% relative increase)** across comparable three-month reporting periods.” Only after candidate affirms the periods and source reflect the same metric.
These are examples of *draft-level, applicant-confirmed* claims, not independent proof about the real Dodgers. If the two periods are not confirmed comparable, leave that precision outside the résumé and flag it.

### Shared tailoring process
Parse JD into role requirements and truthful evidence. Map each requirement to `documented / applicant-reported confirmed / unresolved / not demonstrated`. Use accurate JD keywords only if covered by applicant evidence. Prefer concise accomplishment bullets with confirmed outcomes; keep resume readable rather than applying rigid maximal compression. Deliver a draft promptly instead of repeatedly circling one figure.

### Layout and deliverables
**Path A:** Preserve original template as closely as possible, including correct far-right job-date tab stops, formatting and bottom whitespace. **Path B:** clean single-column reverse-chronological U.S. résumé, conventional headings, readable fonts, no decorative tables/icons/text boxes, ATS-readable text. Keep AI/Technical Skills distinct from Language Skills; one-page preference is not universal.
When tools support it, create actual **editable DOCX and matching selectable-text PDF**; independently render/inspect both, including page count, fonts, clipping, bullet indentation, text extraction, alignment, date positions and blank bottom space. Provide links only to verified files. Deliver (a) tailored resume, (b) compact change/ATS notes, (c) **separate evidence & verification report** identifying applicant-reported metrics and what needs to be substantiated, and (d) optional reusable master JSON/Markdown export. If file tools unavailable, state this truthfully; do not pretend.
No posting of private records to public GitHub; no merging with main without explicit owner authorization.

## Mandatory closing notice
**EDUCATIONAL EXERCISE — DRAFT ONLY. Applicant must check all facts, source metrics, claims, and layout before applying. Never fabricate or exaggerate. ATS readability is not a hiring guarantee.**

## References
Read `references/interview-guide.md`, `references/master-database-schema.md`, `references/quality-checklist.md`, `examples/illustrative-example.md`.
