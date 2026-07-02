#上传材料处理

##来源优先级

在起草之前，请阅读所有提供的文件。支持产品简介、现有脚本、产品细节截图、Word/PDF文档、电子表格、纯文本和在环境可以访问时粘贴的链接。

在来源冲突时使用此证据优先级：

1. 当前活动设置或签署的服务条款
2. 当前官方产品规格和包装
3. 测试报告、证书或生产厂家文件
4. 用户提供的简介
5. 现有脚本或促销文案

不得将促销文案视为其自身主张的证明。

##提取程序

1. 为每个来源分配一个ID，例如`S1`、`S2`，并记录其文件名或标题。
2. 提取产品身份、规格、变体、受众、使用案例、价格、活动规则、物流、退货、保修、演示和禁用措辞。
3. 记录确切单位和限定词。保留`高达`、测试条件、型号、日期及地区限制。
4. 去除重复的等价主张，而不合并不兼容的值。
5. 为不同的价格、材料、容量、服务周期或变体规则建立冲突列表。
6. 标记无法阅读的图片区域和缺失的页面，而不是猜测。

##固定上传摘要

Before the script, produce this compact block when files were uploaded:

```markdown"
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
