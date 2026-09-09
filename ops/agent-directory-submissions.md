# Agent directory submission audit

Last attempted: 2026-09-09T15:34:02Z

These submissions use public, no-auth endpoints and no paid placement.

## Agent Directory API

HTTP status: 409

```json
{"success":false,"error":"An agent with this handle already exists"}
```

## agents-launch

HTTP status: 409

```json
{"error":"Agent with this website_url already exists","agent":{"id":"a008eded-bb45-470b-b0d1-8f8a63372b46","slug":"opc-clinic","name":"OPC Clinic","tagline":"Evidence-first founder diagnosis for launched products that are not converting.","description":"Open-source AI diagnostician for solo founders. It uses multi-turn evidence interrogation to identify the most plausible post-launch bottleneck and define a measurable 7-day test instead of returning generic advice.","website_url":"https://qrex102300-ui.github.io/opc-clinic/","api_docs_url":null,"logo_url":null,"category":"productivity","pricing":"freemium","submitter_name":null,"vote_count":0,"created_at":"2026-09-09T15:28:06.411313+00:00","instructions_url":null}}
```

## OpenAgentSkill

HTTP status: 202

The receipt below is sanitized: submission tokens/status URLs are removed before anything is written to the public repository.

```json
{"success":true,"accepted":true,"message":"Submission saved. Automated review continues in the background.","submission":{"id":"bf365a0b-ada2-44e8-ad44-380ce25bda26","status":"submitted","skill":{"name":"opc-clinic","description":"一个会拷问创业者的 AI 业务诊断官。当用户想诊断自己的创业项目、一人公司或小微业务卡在哪里时使用——尤其是用户描述了某个具体卡点(没人付费、卡住了、涨不上去、不知道方向对不对、转化低、留不住用户等)并想找到真正的病因和行动项时。触发场景包括:'诊断我的项目''我的产品卡住了''帮我看看问题在哪''为什么没人买''我该不该继续做''分析一下我的业务'等。它不给放之四海皆准的通用建议,而是像一个不留情面的诊断官,一层层追问,把症状追到病因。An AI diagnostician for solo founders and small businesses (OPC) stuck at any stage.","path":"skill/SKILL.md","sourceUrl":"https://github.com/qrex102300-ui/opc-clinic/tree/782e43ba0495dcf95c7ecbb856cea2a2120eeee4/skill"}}}
```
