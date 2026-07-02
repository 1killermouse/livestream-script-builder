# Livestream Script Builder

一个面向 Codex / Agent 的中文直播话术 Skill。上传商品资料、现有话术、Word、PDF、表格或图片，即可提取事实并生成带时间轴的 5 分钟或 7 分钟“主播＋中控”协同话术。

它提炼了直播间常见的暖场、互动、塑品、选择建议、优惠说明、保障说明、上车与返场节奏，同时明确禁止编造库存、销量、评论、材质、功效、原价、补贴和售后承诺。

## 安装

将 `livestream-script-builder` 文件夹复制到 Codex skills 目录：

```bash
cp -R livestream-script-builder "${CODEX_HOME:-$HOME/.codex}/skills/"
```

重新启动 Codex，或刷新可用 Skills。

## 使用示例

```text
使用 $livestream-script-builder，根据下面的商品资料生成一套 5 分钟直播话术。
商品：……
受众：……
已核验卖点：……
价格和活动：……
售后：……
```

也可以要求它：

- 把现有话术改成 7 分钟主播＋中控版本；
- 为同一商品生成第二轮返场循环；
- 审核话术中的虚假稀缺、绝对化用语和未核验承诺；
- 按新的商品资料迁移原有话术节奏。
- 上传多份资料后，汇总事实、发现冲突并标记来源；
- 在不改变真实信息的前提下丰富现有话术；
- 固定输出资料摘要、直播设定、时间轴、中控清单、备用分支、返场、核对卡和事实核验表。

##目录

```text
livestream-script-builder/
├── SKILL.md
├── agents/openai.yaml
└── references/
├── intake.md
├── module-library.md
├── output-template.md
├── timing-frameworks.md
└── upload-processing.md
```

##设计说明

本仓库复用的是话术结构和工作流，不收录来源文档的逐字稿。生成内容仍需由使用者根据商品证据、平台规则和适用法律复核后再播出。
