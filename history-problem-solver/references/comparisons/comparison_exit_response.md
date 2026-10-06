# 从完成旧任务到选择下一阶段：范蠡与文种

## 目录

- 对照结论与证据边界
- 结构化对照卡

## 对照结论与证据边界

这是一组**有限可比**的正式对照，用于提出更好的问题：下一阶段想保留什么、改变什么，所选行动能否实现它？不能据此证明离开优于留下。

| 比较项 | 范蠡 | 文种 | 可以得出的结论 |
|---|---|---|---|
| 行动 | 记载中实际离越 | 记载中称病不朝 | 动作改变的范围不同，但效果不能只由动作名称确定 |
| 主观目标 | 史书赋予忧虑解释 | 有较晚的内忧叙事，完整目标未知 | 不能假定二人都只求安稳，也不能把其中一人定义为贪恋地位 |
| 退出条件 | 有携资、随行与乘舟记载 | 可用资源与离境条件不详 | 未知不等于没有，不能把资源差异当成已证实的决定因素 |
| 人生影响 | 旧角色改变；后续经历主要见《史记》 | 记载中最终遭赐剑 | 生存结果、职业结果与生活满意度不能互相替代 |

详细历史依据继承两张案例卡，不把重复转述计算为新增证据。现代路径必须从用户回答出发；以下目标示例不意味着推荐其中一种生活。

## 结构化对照卡

```yaml
schema_version: "0.1"
comparison_id: comparison_exit_response
title: 从完成旧任务到选择下一阶段：范蠡与文种
status: reviewed
review:
  reviewed_by: Codex，结构与引用审阅，非因果鉴定
  reviewed_at: "2026-09-28"
  notes: 依据两张 0.2 案例卡；只有有限结构可比性，不是控制实验。
question: 阶段性任务结束后，如何依据下一阶段目标评估继续参与、调整参与与实际退出？
case_ids: [case_fanli_departure, case_wenzhong_withdrawal]
historical_goal_comparability: 两人完整目标与主观权重均不可确知，不假设目标相同；现代用户目标必须另行询问。
shared_structure:
  - statement: 两人的相关行动均被置于越灭吴后的政治叙事中，涉及与同一君主的关系。
    evidence_refs: [case_fanli_departure#clm_01, case_wenzhong_withdrawal#clm_01]
  - statement: 行动需要面对他人的解释与处置，不能只由本人意愿决定后果。
    evidence_refs: [case_fanli_departure#clm_02, case_wenzhong_withdrawal#clm_03, case_wenzhong_withdrawal#clm_04]
outcome_axes:
  - criterion: 是否完成离越
    horizon: 各案例所界定的行动阶段
    case_observations:
      - case_id: case_fanli_departure
        observation: 记载已离越。
        evidence_refs: [case_fanli_departure#clm_03]
      - case_id: case_wenzhong_withdrawal
        observation: 记载称病不朝，不是已完成离越；未知他是否曾尝试离境。
        evidence_refs: [case_wenzhong_withdrawal#clm_02]
    comparability_limit: 文种是否以离越为目标未知，不能按未离越认定其决策失败。
  - criterion: 个人生命安全
    horizon: 行动之后；两例的记载时间跨度不完全一致
    case_observations:
      - case_id: case_fanli_departure
        observation: 《史记》另叙后续经历及晚年；其史实置信度受限。
        evidence_refs: [case_fanli_departure#clm_04]
      - case_id: case_wenzhong_withdrawal
        observation: 记载最终遭赐剑而死。
        evidence_refs: [case_wenzhong_withdrawal#clm_04]
    comparability_limit: 结果不同不能排除权力关系、资源、时机与叙事选择等因素。
candidate_variables:
  - variable: 行动改变的范围
    case_observations:
      - case_id: case_fanli_departure
        observation: 改变所在环境及原任职关系。
        evidence_refs: [case_fanli_departure#clm_03]
      - case_id: case_wenzhong_withdrawal
        observation: 减少朝见，不证明已解除其他关系或责任。
        evidence_refs: [case_wenzhong_withdrawal#clm_02]
    evidence_refs: [case_fanli_departure#clm_03, case_wenzhong_withdrawal#clm_02]
    inference: 改变参与程度与改变依附结构可能不是同一件事；是分析命题而非已证实定律。
    unknowns: [两人的完整职责及行动过程, 不同行动各自产生多大效果]
    modern_question: 你希望下一阶段改变的是工作节奏、收入、角色、关系，还是方向本身？
    why_answer_changes_next_step: 若只想恢复个人时间，可比较任务调整与换环境；若想改变职业内容，则需检验新路径而不只减轻现岗位负担。
  - variable: 退出的现实可行性
    case_observations:
      - case_id: case_fanli_departure
        observation: 有可携物品、随行与交通记载，但准备过程未知。
        evidence_refs: [case_fanli_departure#clm_03]
      - case_id: case_wenzhong_withdrawal
        observation: 同类条件未知；缺载不证明没有。
        evidence_refs: []
    evidence_refs: [case_fanli_departure#clm_03]
    inference: 目标相同也可能需要不同过渡方式，但不能断言文种缺资源。
    unknowns: [资产可用程度, 家属安排, 保护和接纳条件]
    modern_question: 为实现你确认的阶段目标，哪些过渡条件必须先成立？
    why_answer_changes_next_step: 条件已具备可以评估直接转换；条件不足则比较分阶段准备、降低规模或调整路径，而非自动放弃目标。
  - variable: 行动表达与他人解释
    case_observations:
      - case_id: case_fanli_departure
        observation: 辞别叙事包括挽留与威胁。
        evidence_refs: [case_fanli_departure#clm_02]
      - case_id: case_wenzhong_withdrawal
        observation: 较晚记载把缺席解释为怨望的指控。
        evidence_refs: [case_wenzhong_withdrawal#clm_07]
    evidence_refs: [case_fanli_departure#clm_02, case_wenzhong_withdrawal#clm_07]
    inference: 理由的本意、接收方解释与实际效果需要分别检查；不能预设某种话术必然有效。
    unknowns: [当事人的真实意图, 对话原貌, 对方原有意图]
    modern_question: 对方实际说过或做过什么？哪些只是我们猜测的反应？
    why_answer_changes_next_step: 有明确约定时可核实与落实；只有猜测时先取得信息，不因历史故事升级冲突。
pairing_quality: limited
confounders: [目标与主观权重不同或未知, 资源和退出机会未知, 与君主关系不同或未知, 观察跨度不同, 后世叙事选择]
source_dependence: 同书不同网站不独立；《史记》《国语》《吴越春秋》之间的具体材料关系未完成考证。
provisional_lessons:
  - lesson: 完成旧目标不自动决定下一阶段，应把目标、动作、执行条件与结果分开。
    conditions: [现实用户正在选择下一阶段, 有空间澄清目标或进行小规模探索]
    rival_explanations: [现实问题可能只是临时疲惫或局部安排，而非方向转换]
    evidence_that_would_weaken_it: [用户已明确目标且只需执行细节时，不应再做完整价值探索]
    forbidden_inference: 一有成绩就应离开；留下者目光短浅；安稳优于进取或反之。
  - lesson: 减少参与是否有用取决于希望改变什么，以及实际改变了什么。
    conditions: [已明确希望改变的内容, 能核实责任和关系是否发生变化]
    rival_explanations: [部分参与本身可能足以实现恢复时间等目标, 危险可能来自与参与程度无关的因素]
    evidence_that_would_weaken_it: [现实中减少任务已稳定实现目标且未留下关键风险]
    forbidden_inference: 只有彻底退出才有效；文种遇害是自己的选择应得。
modern_goal_gate:
  first_question: 这次改变如果值得，你希望下一阶段的日常具体有什么不同？最想保留什么？
  if_unknown: 先从最近想减少和增加的体验谈起；仍不明确则约定一个能检验偏好的小体验，再谈方向。
  if_known: 引用用户已经表达的目标、期限与底线，直接比较路径；不重复盘问人生意义。
goal_dependent_paths:
  - provisional_goal: 更可预测的生活与更多关系或个人时间
    candidate_paths: [调整任务或工作边界, 换更符合日常要求的岗位, 有准备的恢复或照料阶段]
    life_impacts: 比较日常节奏与精力、收入变化、关系投入及未来重返工作的条件；留任未必稳定，辞职也未必安稳。
    next_step: 选一项最想改变的日常体验，核实哪条路径真能改善，并明确其代价。
    review_trigger: 实际安排与承诺持续不符，或另一项重要目标被明显损害。
  - provisional_goal: 尝试自己的项目或创造更大的自主空间
    candidate_paths: [在可行约束下验证想法, 分阶段转换, 条件成熟后的全职投入]
    life_impacts: 可能增加创造和决策权，也可能增加经营、客户与协作责任；需区分喜欢创造与喜欢经营。
    next_step: 选择能验证核心需求或自己对真实工作内容偏好的最小行动，规模由用户约定。
    review_trigger: 得到真实反馈后，需求、个人意愿、代价或资源条件明显不同于预期。
  - provisional_goal: 先完成一个阶段收入目标
    candidate_paths: [以当前岗位达到目标, 比较更匹配的岗位, 调整收入目标或阶段期限]
    life_impacts: 收入与学习、关系、健康和个人时间存在取舍；达到金额也不能保证生活满意。
    next_step: 明确目标、缺口与期限，再比较达到目标所需的时间和代价，而非默认收入越高越好。
    review_trigger: 达到目标、所付代价超过用户底线，或用户对下一阶段的偏好发生变化。
  - provisional_goal: 尚未确定方向，或存在上述之外的目标
    candidate_paths: [探索具体日常偏好, 体验候选工作的真实内容, 围绕用户自述另建路径]
    life_impacts: 探索也有时间与精力成本，但可减少被抽象头衔和故事牵引；不要求立刻永久定向。
    next_step: 共同选一个可在约定期限内带来新信息的体验，事先说明希望区分的偏好。
    review_trigger: 得到足以调整目标的新体验，或探索持续无新增信息，需要改换方式。
analogy_limits: [君主政治暴力不能等同普通雇佣关系, 不把称病不朝当现代病假程序, 不把后续经商倒推为事前创业目标, 古代结果不替现代用户排序价值]
open_questions: [两人的真实目标和可选空间, 文种缺席的完整程序和时长, 范蠡离越过程中是否实际遭阻拦及离去后是否被追索, 来源独立性与叙事形成过程]
```
