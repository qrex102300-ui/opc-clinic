# Free directory acquisition round 2

Last attempted: 2026-09-09T23:14:38Z

Goal: expand legitimate zero-cost external discovery without unsolicited comments, paid spend, private credentials, or owner identity.
The workflow used only designated public submission forms and intentionally left email/person identity fields blank. It does not bypass CAPTCHA or other human-verification gates.

```json
[
  {
    "id": "aitoolsindex",
    "surface": "https://aitoolsindex.org/submit",
    "attempted": true,
    "submittedEmail": false,
    "submittedIdentity": false,
    "categorySelected": null,
    "pricingSelected": null,
    "finalUrl": "about:blank",
    "successSignal": false,
    "blockedByCaptcha": false,
    "bodyText": "This site can’t be reached\n\nCheck if there is a typo in aitoolsindex.org.\n\nDNS_PROBE_FINISHED_NXDOMAIN\nReload",
    "error": "page.goto: net::ERR_NAME_NOT_RESOLVED at https://aitoolsindex.org/submit\nCall log:\n  - navigating to \"https://aitoolsindex.org/submit\", waiting until \"domcontentloaded\"\n"
  },
  {
    "id": "launchkittools",
    "surface": "https://launchkittools.com/submit",
    "attempted": true,
    "submittedEmail": false,
    "submittedIdentity": false,
    "categorySelected": "Productivity",
    "pricingSelected": "Freemium",
    "finalUrl": "https://launchkittools.com/submit",
    "successSignal": true,
    "blockedByCaptcha": false,
    "bodyText": "LaunchKit\nTools\nBrowse\nAbout\nContact\nSubmit a Tool\n\nKnow an AI tool that should be listed? Tell us about it and we'll review it for inclusion.\n\nTool Name *\nWebsite URL *\nCategory *\nSelect a category\nWriting\nDesign\nCoding\nMarketing\nVideo\nAudio\nProductivity\nData\nPricing\nSelect pricing model\nFree\nFreemium\nPaid\nEnterprise\nShort Description\nYour Email (optional)\nSubmit Tool\nThanks! We'll review your submission and add it if it's a good fit.\nHome\nContact\nPrivacy\n\n© 2026 LaunchKit Tools. All rights reserved.",
    "error": null
  },
  {
    "id": "curatahub",
    "surface": "https://curatahub.com/submit",
    "attempted": true,
    "submittedEmail": false,
    "submittedIdentity": false,
    "categorySelected": "Business",
    "pricingSelected": null,
    "finalUrl": "https://curatahub.com/submit",
    "successSignal": true,
    "blockedByCaptcha": false,
    "bodyText": "Tools\nCategories\nStacks\nBlog\nGraveyard\nSubmit Tool\nSubscribe\nSubmit an AI tool\n\nKnow a great AI tool that isn't in the database? Tell us about it. We review every submission.\n\nThanks — submission received\n\nWe'll review the tool and get back to you if we add it.\n\nA curated database of AI tools that are actually useful, actively maintained and worth your time.\n\nSITE\nTools\nCategories\nBlog\nDeals\nSubmit a Tool\nBEST OF 2026\n★ Curata Picks\nBest Writing\nBest Coding\nBest Image\nBest Video\nBest Research\nRESOURCES\nNewsletter\nFAQ\nPublish Guide\nPrivacy Policy\nTerms\nAffiliate Disclosure\n\n© 2026 Curata AI. All rights reserved.\n\nCurated for creators, builders & teams.\n\nEdit with",
    "error": null
  },
  {
    "id": "findaitools",
    "surface": "https://findaitools.app/submit",
    "attempted": true,
    "submittedEmail": false,
    "submittedIdentity": false,
    "categorySelected": null,
    "pricingSelected": null,
    "finalUrl": "about:blank",
    "successSignal": false,
    "blockedByCaptcha": false,
    "bodyText": "Access to findaitools.app was denied\n\nYou don't have authorization to view this page.\n\nHTTP ERROR 403\nReload",
    "error": "page.goto: net::ERR_HTTP_RESPONSE_CODE_FAILURE at https://findaitools.app/submit\nCall log:\n  - navigating to \"https://findaitools.app/submit\", waiting until \"domcontentloaded\"\n"
  },
  {
    "id": "alieradox",
    "surface": "https://alieradox.com/submit",
    "attempted": true,
    "submittedEmail": false,
    "submittedIdentity": false,
    "categorySelected": null,
    "pricingSelected": null,
    "finalUrl": "https://alieradox.com/submit",
    "successSignal": false,
    "blockedByCaptcha": false,
    "bodyText": "Checking your browser before accessing\nalieradox.com\n\nPlease wait for up to 5 seconds...",
    "error": "Required product fields not found (name=false, url=false, description=false)"
  }
]
```
