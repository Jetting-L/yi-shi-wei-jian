# 历史对照卡模板

先明确比较问题，再选择案例；不能从一胜一败反推两者处境相同。对照用于生成待检验的问题，不自动建立因果关系。

证据引用统一写为 `case_id#claim_id`，必须存在于对应案例卡。史料缺载一律记 unknown，不能填“没有”。实际案例文件由 SKILL.md 直接链接。

`status` 取 draft / reviewed；`pairing_quality` 取 strong / limited / unsuitable，指结构可比性而非因果确证。核心目标不同或证据太薄时可判 unsuitable，不强行完成对照。

```yaml
schema_version: "0.1"
comparison_id: null
title: null
status: draft
review:
  reviewed_by: null
  reviewed_at: null
  notes: null
question: null
case_ids: []
historical_goal_comparability: null
shared_structure:
  - statement: null
    evidence_refs: []
outcome_axes:
  - criterion: null
    horizon: null
    case_observations: []
    comparability_limit: null
candidate_variables:
  - variable: null
    case_observations: []
    evidence_refs: []
    inference: null
    unknowns: []
    modern_question: null
    why_answer_changes_next_step: null
pairing_quality: limited
confounders: []
source_dependence: null
provisional_lessons:
  - lesson: null
    conditions: []
    rival_explanations: []
    evidence_that_would_weaken_it: []
    forbidden_inference: null
modern_goal_gate:
  first_question: null
  if_unknown: null
  if_known: null
goal_dependent_paths:
  - provisional_goal: null
    candidate_paths: []
    life_impacts: null
    next_step: null
    review_trigger: null
analogy_limits: []
open_questions: []
```

填写规则：

- case_observations 中每项写 `case_id`、`observation` 与 `evidence_refs`；缺证据时保留空引用并明说未知，不引用无关事实补洞。
- outcome_axes 为两例采用同一指标、时间视角与评价主体；资料不能满足时说明有限可比。不能用甲完成行动、乙生命结局强配一成一败。
- candidate_variables 只是待检验变量；只有一侧有资源记载时，不能断定另一侧没有资源。解释何种现实答案会怎样改变下一步。
- goal_dependent_paths 是现代条件分析，不是古代案例结论。示例目标可以并存；不要把用户强制归类，也不默认某目标更好。
- 审阅前核对案例引用、反向 comparison_ids、两例的目标与结果口径、替代解释、古今差异及目标未知时的交互方式。
