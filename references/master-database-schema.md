# Master Resume Database — Portable Evidence Schema (v2 fast intake)

Keep source inventory independent from job-specific résumé versions. Never infer facts from the JD. Fictional tests must be explicitly marked fictional.

```json
{
  "schema_version": "2.0",
  "test_data": false,
  "candidate": {"preferred_name": "", "city_state": "", "email": null, "phone": null, "linkedin": null, "portfolio": null},
  "career_stage": null,
  "career_direction": [],
  "education": [],
  "experiences": [
    {
      "id": "exp-001",
      "type": "employment",
      "organization": "",
      "title": "",
      "start": null,
      "end": null,
      "responsibilities": [],
      "tools_used": [],
      "projects": [],
      "achievements": [
        {
          "id": "exp-001-ach-001",
          "action": "",
          "scope_details": "",
          "result": "",
          "evidence_notes": "",
          "scope": "individual | team | campaign | organization | unknown",
          "result_wording": "",
          "measurement": "",
          "baseline": null,
          "final": null,
          "unit": null,
          "comparison_periods": null,
          "periods_comparable": null,
          "attribution_method": null,
          "reported_source": null,
          "source_inspected": false,
          "mathematics_checked": false,
          "applicant_confirmed": false,
          "evidence_status": "applicant-reported",
          "draft_resumable": false,
          "verification_note": ""
        }
      ]
    }
  ],
  "projects_volunteering_leadership": [],
  "skills": {"ai_technical": [], "analytics_creative": [], "professional": [], "languages": []},
  "unresolved_questions": [],
  "applicant_reviewed": false
}
```

**Repeatability:** Each experience can have zero, one, or many separately identified achievements. Form 2's optional Achievement Builder supplies action, scope, result and evidence for each. Never merge away source achievements or require all four fields to be filled. A result may be qualitative; numbers are optional. Store each metric's provenance and confirmation individually.

**Evidence status is not binary:** applicant-reported and candidate-confirmed metrics may appear in an **educational draft** when coherent, source-described and accurately scoped, without falsely claiming independent verification. Track verification status in a separate report. A documented source that has merely been named is **not** a document that was inspected.

**Decisions:** if baseline/period/attribution is missing, do not imply precision or causality. If inconsistent, calculate correctly, ask one grouped follow-up. Keep original reported claims and corrections in the database. Do not publish private candidate records. Export JSON/Markdown on request; do not claim persistence until actually saved.
