# Upwork Prompt Flows – ai-prompts-library

## Decision Tree – From Job Post to Proposal

1. **Intake the Job Post**
   - Run `en/client_fit_red_flag_analyzer.txt` with description, budget, timeline, and your gut-check.
   - If "No" → archive. If "Conditional" → gather missing info. If "Yes" → continue.

2. **Scope from Initial Notes**
   - Feed post + call notes into `en/discovery_notes_to_scope.txt` to get goals, constraints, phased deliverables, and timeline.
   - For discovery-heavy jobs, run `automation_discovery_call` or `chatbot_discovery_call` first for agenda.

3. **Draft Proposal**
   - Use `en/upwork_job_response_helper.txt` (or `upwork_proposal_general` for longer-form) with the scope output.

4. **Delivery & Retrospective Hooks**
   - Note relevant delivery prompts (e.g., `automation_discovery_call`, `podcast_to_blog`).
   - After delivery, run `en/post_project_retrospective.txt` to capture wins and tee up testimonials.

---

## Job Type → Prompt Chain

| Job Type                  | Recommended Prompt Chain                                      |
|---------------------------|---------------------------------------------------------------|
| Automation                | client_fit_red_flag_analyzer → automation_discovery_call* → discovery_notes_to_scope → upwork_job_response_helper → post_project_retrospective |
| Chatbot                   | client_fit_red_flag_analyzer → chatbot_discovery_call* → discovery_notes_to_scope → upwork_job_response_helper or upwork_proposal_general → post_project_retrospective |
| Scraping / Data Extraction| client_fit_red_flag_analyzer → discovery_notes_to_scope → upwork_job_response_helper → weekly_review_planning → post_project_retrospective |
| AI Security / Audit       | client_fit_red_flag_analyzer (compliance focus) → discovery_notes_to_scope → upwork_proposal_general → post_project_retrospective |

\*Discovery call prompts are optional but useful if a call is scheduled.

---

## Checklist – "Job → Proposal in 20 Minutes"

- [ ] Run `client_fit_red_flag_analyzer`; decide go/no-go.
- [ ] If go, run `discovery_notes_to_scope` to capture goals & constraints.
- [ ] If needed, triage with `upwork_job_triage_plan`.
- [ ] Generate response with `upwork_job_response_helper` or `upwork_proposal_general`.
- [ ] Submit proposal and log follow-up timing with `weekly_review_planning`.
- [ ] After delivery, run `post_project_retrospective`.

---

## Meta-Prompt – Multi-Prompt Workflow

> You are my AI proposal partner with access to the **ai-prompts-library** (English prompts).
> Given the job description:
>
> `<JOB_DESCRIPTION>`
>
> 1. Choose which prompts to run (e.g., `client_fit_red_flag_analyzer` → `discovery_notes_to_scope` → `upwork_job_response_helper`) and explain why.
> 2. For each prompt, show the filled-in template (variables populated from job info).
> 3. Produce the outputs in order and finish with a ready-to-send Upwork proposal text.
> 4. End with follow-up recommendations and any missing info to confirm on a call.
