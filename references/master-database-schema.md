# Master Resume Database — Structure and Rules

## Purpose
A portable, reusable **career evidence inventory**, *not* a finished résumé or an invented employment history. Keep this broad master separate from all JD-targeted drafts; never overwrite facts during tailoring. Use private local files with user permission; do not publish applicants' personal data to GitHub.

## Suggested JSON-compatible structure

```json
{
  "schema_version": "1.0",
  "candidate": {
    "preferred_name": "",
    "city_state": "",
    "email": "",
    "phone": "",
    "linkedin": "",
    "portfolio": ""
  },
  "career_direction": [],
  "experiences": [
    {
      "id": "exp-001",
      "type": "employment | internship | volunteer | research | freelance | leadership | project",
      "organization": "",
      "role": "",
      "location": "",
      "start_date": "YYYY-MM or unknown",
      "end_date": "YYYY-MM | present | unknown",
      "date_precision": "month | year | unknown",
      "responsibilities": [],
      "achievements": [
        {
          "problem": "",
          "personal_action": "",
          "tools_methods": [],
          "deliverable": "",
          "stage": "learned | practiced | prototyped | tested | piloted | deployed | adopted | other",
          "stakeholders": "",
          "outcome": "",
          "metric": null,
          "metric_source_method": null,
          "permitted_claim": "",
          "source": "resume | document | applicant interview",
          "evidence_status": "documented | applicant-reported | unverified | not-demonstrated",
          "candidate_confirmed": false
        }
      ],
      "source": "",
      "evidence_status": "applicant-reported",
      "candidate_confirmed": false,
      "verification_questions": []
    }
  ],
  "education": [],
  "certifications": [],
  "skills": {
    "ai_technical": [],
    "professional_domain": [],
    "languages": []
  },
  "open_questions": [],
  "candidate_reviewed": false,
  "last_review_date": null
}
```

## Rules
- Null/unknown means **not known**, not permission to infer. Never fill blank fields with plausible examples.
- Document source and whether the candidate has confirmed each claim; supporting files and applicant reports do not imply independent authentication.
- Use real metric calculations only when the user can substantiate source, baseline, time period and attribution.
- Keep languages distinct from AI tools and technical competencies; list proficiency only when user has stated it.
- Ask one adaptive question at a time and periodically recap for corrections. Allow legitimate student projects and unpaid experience with accurate labels.
- When a new JD arrives, create a separate targeted résumé version. Save the master inventory unchanged unless the applicant deliberately corrects/adds evidence.
- The skill **cannot guarantee persistence**. Export portable JSON or Markdown and let user retain it; use connected private storage only with explicit approval.
