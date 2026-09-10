# MCP.Directory Agent Skill submission

Last attempted: 2026-09-10T09:59:19Z
Audit corrected: 2026-09-10

Goal: add OPC Clinic to a high-fit agent-skill discovery surface using the directory’s designated public submission form.
Only the public SKILL.md URL and public project metadata were supplied. Email/person identity fields were intentionally left blank. No payment, private credential, CAPTCHA bypass, or unrelated community promotion was used.

## Verdict

**UNVERIFIED — DO NOT COUNT AS A LISTING OR PENDING REVIEW.**

The browser successfully opened the public skill-submission route and attempted the form, but after clicking submit it landed on `https://mcp.directory/submit`, whose rendered page was the generic **Submit a Server** form. There was no skill-specific acknowledgement, receipt, submission ID, or explicit confirmation that OPC Clinic entered the review queue. The original workflow's broad `successSignal` matched generic words such as “review” on that unrelated page and was therefore a false positive.

Because the sprint scorecard only moves on observable evidence, this route remains uncounted unless a later public listing or explicit skill-submission acknowledgement is independently verified. The form is not blindly retried in order to avoid duplicate submissions.

## Sanitized attempt evidence

```json
{
  "surface": "https://mcp.directory/submit-skill",
  "skillSource": "https://github.com/qrex102300-ui/opc-clinic/blob/main/skill/SKILL.md",
  "attempted": true,
  "submittedEmail": false,
  "submittedIdentity": false,
  "verifiedSubmission": false,
  "blockedByCaptcha": false,
  "finalUrl": "https://mcp.directory/submit",
  "observedPage": "Generic 'Submit a Server' page; no skill-specific acknowledgement or receipt",
  "countOnScorecard": false
}
```
