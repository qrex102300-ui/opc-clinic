# AllToolsDirectory submission audit

Last attempted: 2026-09-10T13:54:57Z

Surface: https://www.alltoolsdirectory.com/submit

The public page advertises free submission with no login. A guarded browser attempt used only public OPC Clinic project information and left contact email/social fields blank. No personal identity, owner email, private credential, payment, CAPTCHA bypass, or unrelated-community promotion was used.

## Result

**NOT SUBMITTED / DO NOT COUNT.**

The browser reached the designated submit action, but the form then displayed **“Please enter a valid email address”** while remaining on the submission page. That validation is stronger evidence than the first-pass automation heuristic that had marked `acceptedSignal: true` merely because static page copy contained words such as “review”. There was no success/thank-you state, no redirect, and no live OPC Clinic directory entry.

Classification:

```json
{
  "attempted": true,
  "submissionAccepted": false,
  "live": false,
  "blockedByRequiredEmail": true,
  "usedIdentity": false,
  "usedEmail": false,
  "usedPayment": false,
  "countAsConfirmedListing": false,
  "countAsPendingReview": false
}
```

This surface should not be retried during the sprint unless the owner explicitly supplies/authorizes an email identity for directory submissions.