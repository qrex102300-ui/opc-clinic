# TrustedSkills discovery audit

Last attempted: **2026-09-10 18:53 CST**

Goal: enroll the public OPC Clinic skill in TrustedSkills through its documented zero-cost auto-discovery route, without using owner identity, email, private credentials, paid placement, or unsolicited community promotion.

## Registry compatibility prepared

`skill/SKILL.md` was normalized only for cross-registry interoperability, not landing-page or funnel polish:

- semantic version: `1.0.0`
- declared platforms: `openclaw`, `claude`, `openai`
- description reduced to the registry's documented metadata length range
- repository remains public and MIT licensed

TrustedSkills documents that a public GitHub repository can be auto-discovered after adding the `openclaw-skill` repository topic, with discovery running periodically.

## Topic enrollment result

A one-shot GitHub Actions workflow attempted to preserve all existing repository topics and add only `openclaw-skill` through GitHub's repository-topics API.

Observed result:

- workflow: `Enable TrustedSkills discovery`
- run ID: `34468391731`
- repository read succeeded
- topic update API returned: **HTTP 403**
- `GITHUB_TOKEN` permissions visible in the run: `Contents: write`, `Metadata: read`
- no topic was changed
- no owner identity, personal token, private credential, or paid workaround was used

## Classification

**Not counted as a confirmed listing or pending review.** The external submission gate was not reached because this GitHub connection cannot mutate repository topics. No blind retry will be made with the same permission set.

The skill remains registry-compatible for other public intake routes that accept a direct GitHub folder URL.
