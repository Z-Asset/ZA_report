---
name: za-report
description: 报告阶段（文稿）—— 论文写作。当用户要「写论文」「起草章节」「提取写作风格」「去 AI 味」时使用。
whenToUse: 论文写作、章节起草、写作风格提取、humanize。
---

# 报告阶段（文稿）

派发 Writer（`references/agents/writer.md`）与 writer-critic（`references/agents/writer-critic.md`），读取并**完整采纳其角色设定**。

## 工作流

1. **收集上下文**：现有草稿、research spec、lit review、`references/domain/domain-profile.md`、Bibliography_base.bib、results_summary.md
2. **检测论文类型**：reduced-form / structural / theory+empirics / descriptive
3. **按章节路由**：intro / strategy / results / conclusion / abstract / data / model / full
4. **派发 Writer**：段落级 argument moves 起草，存 `paper/sections/[section].tex`
5. **质量自检**：每段有明确目的、findings 领句、方程编号、cite key 存在、效应量带单位、无禁忌 hedging、记号一致（见 `references/rules/working-paper-format.md`、`references/rules/content-invariants.md`）
6. 呈现给用户，标 TBD / VERIFY / PLACEHOLDER 项

## 附加模式

**humanize**：去 24 类 AI 写作痕迹（structural/lexical/rhetorical/formatting）。
**style-guide**：从用户既往论文提取写作风格到 `personal-style-guide.md`（每断言须有语料引用，无证据写 `[insufficient corpus evidence]`）。

## 原则
- 这是用户的论文，匹配其 voice；绝不编造结果（用 TBD 占位）
- 引用可验证；argument moves 先行、cleanup 后置
