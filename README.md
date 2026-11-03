# JDResume — Evidence-First ATS Résumé Drafting Skill

> **Educational exercise tool. Drafts only. Human review is mandatory. Never fabricate information on a job application.**

JDResume is a reusable AI skill designed to **expedite U.S.-market résumé drafting and job-description tailoring for Applicant Tracking Systems (ATS)**. It helps users organize verified experience, translate job requirements into evidence-backed résumé bullets, and check formatting. It is **built for exercise and learning purposes**; it is not a credential-verification service, recruiter, employment adviser, guarantee of an interview, or automatic application tool.

## Essential notice

- **Every generated résumé is a DRAFT** and must be reviewed, corrected, and edited by a human before use.
- **Never invent, exaggerate, or misrepresent** jobs, dates, employers, degrees, responsibilities, technical proficiency, project deployment, certifications, outcomes, or metrics. Do not convert inferred capabilities into facts.
- Only include claims the applicant confirms and can substantiate. **Unverified metrics should be removed or marked for verification**, not silently retained.
- Preserve the original résumé's layout and work-history coverage by default. Propose deletions with a written rationale and obtain user agreement rather than silently removing relevant experience.
- ATS optimization means clear, parseable structure and relevant truthful terminology. **No universal ATS score, guaranteed pass, or guaranteed interview** exists.
- Respect privacy. Do not publish actual applicants' résumés or personal data in a public repository. This repository contains guidance, not an individual's résumé.

## What it does

1. Collects a résumé, complete job description, target market and formatting preferences.
2. Reviews credible current U.S. résumé guidance when browsing is available, noting source and access date.
3. Analyzes essential and preferred qualifications, separating exact requirements from nice-to-haves.
4. Builds a **claim-to-evidence matrix**: verified / applicant-reported / unverified / not demonstrated.
5. Conducts a concise, one-question-at-a-time interview to fill material evidence gaps.
6. Proposes a **keep / rewrite / condense / omit / add** change log *before* deleting content.
7. Drafts truthful, accomplishment-focused bullets and separates documented AI tools from verified implementation achievements.
8. Produces an editable Word draft and optionally a PDF; retains user-provided style by default.
9. Renders and audits both formats independently: page count, margins, font, line wrapping, dates right-aligned, section hierarchy, bullets, spacing, and bottom whitespace.
10. Returns the draft with a claim-verification checklist, change log, unresolved gaps, and a clear **human-review-required** warning.

## Installation / use

This repository follows the common ChatGPT/AI skill convention: instructions live in [`SKILL.md`](SKILL.md). Download the repository ZIP, then use the skill with an AI environment that supports importing custom skills or supplying skill instructions. **Adding a repository to GitHub does not install it into ChatGPT by itself**; the import mechanism depends on your ChatGPT configuration.

Suggested trigger: “Use JDResume to draft a U.S. ATS-readable résumé for this job description, using my existing résumé and preserving its formatting.”

## Files

- [`SKILL.md`](SKILL.md): operational instructions and guardrails
- [`references/quality-checklist.md`](references/quality-checklist.md): detailed content, layout, and evidence acceptance tests
- [`references/interview-guide.md`](references/interview-guide.md): evidence-gathering questions
- [`examples/illustrative-example.md`](examples/illustrative-example.md): fictional example (not an actual candidate résumé)

## Important limitations

- ATS vendors and employer configurations vary; a résumé can be readable without earning any specific score.
- One page may be appropriate for many candidates, but is **not a universal requirement**. Follow the applicant's stated preference and disclose material tradeoffs.
- A skill can assist with research and formatting, but must not imply it has used a renderer, reviewed a Word document, or verified an employer policy unless it actually has.
- This exercise tool does **not** submit applications or independently confirm the truth of an applicant's statements.

## Responsible use

The applicant owns the final résumé and is responsible for its accuracy. Review every bullet, date, title, claim, tool name, impact figure, and file layout before applying. **Do not fabricate a résumé to obtain a job.**

## References for further research

Consult official and reputable sources such as the [U.S. Department of Labor CareerOneStop](https://www.careeronestop.org/), [USC Career Center](https://careers.usc.edu/), and the [NACE career resources](https://www.naceweb.org/) when appropriate. These are starting points for checking current practices, not endorsements or proof of a universal ATS formula.
