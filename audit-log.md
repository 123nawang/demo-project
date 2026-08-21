# AI 使用记录与审计日志

## 1. 任务概览
- 工具：GitHub Copilot / VS Code / Python / LaTeX / Git
- 任务：基于 demo-project 的 DID 与稳健性研究工作流，生成 assignment 要求的文件与文档。

## 2. 接受的输出
- output/estimand.md：识别目标与研究边界说明。
- prompts/robustness/*.md：R1–R7 与 T1–T4 的独立稳健性检验 Prompt。
- output/robustness_summary.md：对所有稳健性检验的总体判定。
- .claude/skills/robustness-check/SKILL.md：通用 DID 稳健性 Skill。
- .claude/agents/eval-did-robustness.md：综合评估 Agent。
- output/eval_robustness_report.md：综合评估报告。
- output/iteration_reflection.md：两轮迭代反思。

## 3. 拒绝或修改的输出
- 拒绝了直接把“显著性”解释为“真实因果证据”的表述。
- 修改了 AI 早期输出中缺乏边界声明和迁移性说明的问题。
- 强调在合成数据中使用“统计上稳定”而不是“真实因果已证明”。

## 4. 验证方式
- 核对文件是否存在并位于要求位置。
- 检查 Prompt 是否包含四要素：目标、边界、验证、汇报。
- 检查 Skill 是否覆盖六模块：触发条件、背景知识、工作步骤、检查清单、边界条件、验证方式。
- 检查 Agent 是否覆盖 S1–S6 综合评估流程。
- 对文件内容进行人工审查，确认无越界、无虚构文献、无对真实世界的夸大结论。

## 5. 研究者判断
- 当前输出满足作业要求中的文档与流程要求。
- 若需进一步落实真实研究，下一步应在真实数据上重复执行同一套流程，并补全统计检验与因果识别论证。
