"# Uploaded Material Processing

## Source priority

Read all supplied files before drafting. Support product briefs, existing scripts, product-detail screenshots, Word/PDF documents, spreadsheets, plain text, and pasted links when the environment can access them.

Use this evidence priority when sources conflict:

1. Current campaign setup or signed service terms
2. Current official product specification and packaging
3. Test report, certificate, or manufacturer documentation
4. User-provided brief
5. Existing script or promotional copy

Do not treat promotional copy as proof of its own claims.

## Extraction procedure

1. Assign each source an ID such as `S1`, `S2`, and record its filename or title.
2. Extract product identity, specifications, variants, audience, use cases, price, campaign rules, logistics, returns, warranty, demonstrations, and prohibited wording.
3. Record exact units and qualifiers. Preserve `up to`, test conditions, model numbers, dates, and regional limits.
4. Deduplicate equivalent claims without merging incompatible values.
5. Build a conflict list for different prices, materials, capacities, service periods, or variant rules.
6. Mark unreadable image regions and missing pages instead of guessing.

## Fixed upload summary

Before the script, produce this compact block when files were uploaded:

```markdown
## 资料提取摘要
- 已读取：S1《文件名》；S2《文件名》
- 商品：……
- 可直接使用的事实：……
- 冲突信息：……
- 待确认信息：……
- 本次模式：生成 / 丰富 / 改写 / 审核
```

For each high-risk claim in the fact-check list, cite its source as `[S1，第3页]`, `[S2，规格表]`, or another available locator. Do not invent page or cell locations.

## Existing-script preservation

When enriching an uploaded script:

- Keep verified product facts and distinctive, natural host phrasing.
- Remove duplicates before adding new content.
- Replace fake audience, stock, order, countdown, and control-room events with conditional branches.
- Preserve the requested runtime by trading repetition for proof, guidance, or objection handling.
- Show a concise `保留 / 新增 / 修正` summary before the revised script.
