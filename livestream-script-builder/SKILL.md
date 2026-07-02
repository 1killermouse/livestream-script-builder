---
name: livestream-script-builder
description: Extract product facts from uploaded files, then generate, enrich, rewrite, standardize, or audit Chinese livestream sales scripts with coordinated host and control-room lines, especially timed 5-minute or 7-minute conversion loops. Use when the user uploads product pages, briefs, Word/PDF/table/image materials, or an existing script and asks for 直播话术、带货话术、主播话术、中控配合、憋单、塑品、破价、上车、逼单、返场、循环话术, a fixed-format run-of-show, or a compliance-safe adaptation for another product.
---

# Livestream Script Builder

Build speakable Chinese livestream scripts from uploaded or pasted product materials. Preserve the conversion rhythm of a live room while keeping claims truthful, separating evidence from copy, and returning a stable production-ready format.

## Workflow

1. Read every uploaded source using [references/upload-processing.md](references/upload-processing.md). Preserve source provenance.
2. Build the brief and claim ledger using [references/intake.md](references/intake.md).
3. Select `生成`, `丰富`, `改写`, or `审核` mode from the user's request; default to `生成` for raw product materials and `丰富` for an existing script.
4. Choose the 5-minute or 7-minute structure in [references/timing-frameworks.md](references/timing-frameworks.md).
5. Select only relevant blocks from [references/module-library.md](references/module-library.md).
6. Draft host, control-room, and demonstration lines as short spoken turns.
7. Audit every price, stock, identity, material, performance, warranty, and scarcity claim.
8. Deliver the fixed structure in [references/output-template.md](references/output-template.md).

Do not block on minor omissions. Use neutral language or explicit placeholders such as `【待确认：活动库存】`. Ask a question only when the missing fact would materially change the offer or create legal/compliance risk.

## Modes

- `生成`: create a full script from product materials.
- `丰富`: retain correct existing content, then add missing transitions, demonstrations, objections, control-room cues, and a return-loop handoff. Do not inflate it with repetitive hype.
- `改写`: adapt the structure to a new product, audience, tone, or runtime while re-verifying all facts.
- `审核`: return the annotated risk list and revised wording; do not rebuild the entire script unless requested.

If the request is ambiguous, state the chosen mode in one line and proceed.

## Drafting Rules

- Write natural spoken Mandarin, not brochure prose.
- Address the stated audience consistently; default to `大家` when unknown.
- Label roles as `主播` and `中控`. Add `动作` only where a demonstration, product close-up, price card, or link operation matters.
- Keep each turn easy to say in one breath. Vary sentence length and avoid mechanical repetition.
- Use interaction prompts sparingly and tie them to a real choice: use case, color, size, concern, or preference.
- Re-state only the top 2–3 selling points during the closing window.
- Give actual selection guidance when variants exist. Do not invent size, dosage, compatibility, or usage advice.
- Include a clean handoff into the next loop instead of ending abruptly.
- When rewriting an existing script, retain useful facts and rhythm but remove unsupported superlatives, coercion, and fake events.

## Truthfulness and Compliance Gate

Never fabricate or silently assume:

- stock counts, sold-out events, order counts, viewers, customer comments, or payment failures;
- original prices, future price increases, subsidies, lowest-price claims, or countdown deadlines;
- brand authorization, counter availability, inspection support, awards, certifications, or endorsements;
- ingredients, materials, origin, performance, safety, health effects, warranty, returns, or shipping insurance;
- demonstrations, test results, user experiences, or comparisons that did not occur.

Do not simulate fake viewer messages or instruct the host/control room to report invented sales. Phrase real operational branches conditionally, for example: `【若后台确认余量不足】主播：当前可售数量不多，请按实际需要选择。`

Avoid absolute or unverifiable wording such as `全网最低`, `百分百`, `绝对不会`, `闭眼入`, `错过再也没有`, or degrading competitor products. Replace it with specific, supportable value statements.

Do not pressure viewers to skip material information. Put essential restrictions, fit guidance, service terms, and risk information before the purchase prompt.

## Output Contract

Start with a compact header:

```markdown
# 【商品名】5分钟直播话术
- 目标：拉新 / 讲解 / 转化 / 返场
- 受众：【受众】
- 核心卖点：【卖点1】｜【卖点2】｜【卖点3】
- 活动机制：【已核验机制或待确认】
```

Then use a timed table:

```markdown
| 时间 | 角色 | 话术 / 动作 | 目的 |
|---|---|---|---|
| 00:00–00:20 | 主播 | …… | 暖场与定位 |
```

After the table, include only applicable appendices:

- `中控操作清单`: link, price card, variant, inventory, and visual cues.
- `事实核验清单`: unresolved claims and the evidence needed.
- `替换变量`: reusable placeholders for batch adaptation.
- `第二轮循环`: a shorter return loop when requested.
- `直播前核对卡`: facts and backend settings the team must confirm before going live.

Keep the estimated spoken length near 220–260 Chinese characters per minute, adjusted downward for demonstrations and audience interaction. Treat timing as a rehearsal estimate, not a guarantee.

## Final Audit

Before returning the script, confirm:

- total segment durations equal the requested runtime;
- every product fact comes from the brief or is marked pending;
- price and service terms are internally consistent;
- host and control-room lines do not contradict each other;
- the opening identifies the product quickly;
- the purchase prompt follows the key terms rather than hiding them;
- the script remains useful even if no one comments or if stock does not change.
- every claim copied from an upload can be traced to a source location or is marked pending.
