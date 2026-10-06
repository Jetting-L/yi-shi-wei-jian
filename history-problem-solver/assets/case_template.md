# 历史案例卡模板

## 目录

- 使用与字段约定
- 决策重建字段规则
- 可复制的 YAML 模板
- 核验与入库标准

## 使用与字段约定

复制下面的 YAML 块，一卡描述一个边界明确的事件或决策阶段，不用一张卡概括人物的一生。字段说明保留在本模板，案例文件无需重复。

- 使用 UTF-8 与两空格缩进；`schema_version` 固定写成字符串（当前为 0.2）。稳定的 `case_id` 使用小写字母、数字和下划线，例如 `case_<event>_<stage>`；正式记录时替换占位符。
- 在主文件所链接的分类表中选择类别与标签。`secondary_categories` 最多两个；已审阅案例的 `tags` 通常三至六个。
- 未知标量用 `null`，无条目用 `[]`，另在 `missing_information` 解释重要缺失。不要把“未知”填成 false 或零。填写时删除未使用的空白列表对象。
- `source_id`、`claim_id` 及 `variable_id` 在卡内必须唯一，所有引用必须指向实际条目。
- 区分记录事实、言论、评论与现代分析；同一史书可以包含多种内容类型，应逐项标注。
- 记录来源差异时，区分明确矛盾、叙述详略不同与尚未查到材料；缺载不等于否定，同一作品的多个数字版本不等于多份独立证据。
- 正文和摘要均将缺载表述为“所核材料未记载／无法确认”，不得先写“没有做、没有完成或没有获准”，再在后文补不确定性。
- `options_available` 仅记录有依据的当时选项；现代提出的替代做法写入 `counterfactual_options` 并标注假设，不能假称古人曾考虑过。
- 对照关系使用 `comparison_ids` 留接口；没有对照卡时保持空列表，不编造 ID，也不要求每例必配成败对照。

## 决策重建字段规则

版本 0.2 在原字段上增加 decision_reconstruction；旧卡的事实引用与 ID 保持稳定。不要用更丰富的推理掩盖证据不足。

- goal_hypotheses 与 motive_hypotheses 的 evidence_level 取 source_attribution（史书归属的心理）、plausible_inference（有依据但未证实的推断）、speculative（机制假设）或 unknown（缺乏依据）。史书写了某种动机不等于真实心理已经确证。
- option_tradeoffs 的 availability 取 recorded_action、recorded_offer、analytical_alternative 或 counterfactual；后二者不可混入 options_available。逐项记录潜在收益、代价、实施条件、他人反应与对未来选择的影响，均按当时信息评估，不用最终结局反推。
- implementation 分开记录已知动作和未知程序；没有流程记录时，说明需要知道什么，不能虚构请假、辞官或批准制度。
- choice_explanation 说明哪种解释较受支持、为什么仍有疑问，以及什么无法由材料回答。多个假说不等于同样可信。
- life_course 分析短、中、长期的路径变化，区分所载后续与事前计划；不得替历史人物或现代用户设定价值目标。

## 可复制的 YAML 模板

```yaml
schema_version: "0.2"
case_id: null
title: null
status: draft  # draft / reviewed；reviewed 仅代表完成下列审阅要求
review:
  reviewed_by: null
  reviewed_at: null  # YYYY-MM-DD
  notes: null

scope:
  period: null
  date_range: null  # 可写约数、纪年；勿伪造精确日期
  date_precision: unknown  # exact / approximate / disputed / unknown
  event_boundary: null  # 从哪个决定到哪个观察节点
  people: []
  organizations: []

classification:
  primary_category: unmapped
  secondary_categories: []
  tags: []
  classification_note: null

sources:
  - source_id: src_01
    work_title: null
    author_or_compiler: null
    source_type: null  # near_contemporary / later_compilation / modern_research / literary / other
    chapter_or_volume: null
    edition_or_translator: null
    locator: null  # 页码、段落或可唯一定位的文本线索
    url: null  # 只填真实查阅的地址；纸本可留空
    accessed_on: null
    verification: not_checked  # checked / partial / not_checked
    temporal_relation: null  # 成书与事件的时间距离；未知则说明
    dependence_on_other_sources: null  # 转抄或共同来源；未调查不得称独立
    limitations: null

claims:
  - claim_id: clm_01
    statement: null
    claim_type: recorded_event  # recorded_event / attributed_speech / source_commentary / modern_interpretation
    source_refs: []
    source_locators: []  # 与此主张直接相关的定位信息
    support: unverified  # supported / partial / contested / unverified
    historicity_confidence: unknown  # high / medium / low / unknown
    confidence_reason: null  # 为什么记载可信或存疑；不等于网页是否可访问
    exact_quote: null  # 非必填；仅保留已核对的短引文
    quote_checked: false

source_assessment:
  conflicts:
    - claim_refs: []
      source_refs: []
      disagreement: null
      handling: null  # 保留分歧或说明采用依据，不能直接多数表决
  single_source_limit: null
  later_embellishments: []  # 后世附会、演义或常见误传

situation:
  summary: null
  claim_refs: []
  decision_maker: null
  affected_parties: []
  desired_outcome_at_the_time: null
  constraints: []
  information_available_then: []
  decision_problem: null

options_available:
  - option: null
    availability_basis: null
    claim_refs: []
    constraints: []
decision_taken:
  action: null
  claim_refs: []
counterfactual_options:
  - option: null
    feasibility_assumptions: []
    uncertainty: null

key_variables:
  - variable_id: var_01
    tag: null  # 使用受控标签
    historical_observation: null
    claim_refs: []
    modern_equivalent: null
    observable_indicator: null  # 今天如何验证它，而不是只写“信任”

outcomes:
  - perspective: null  # 谁的成败，谁承担代价
    criterion: null  # 具体目标或指标
    horizon: null  # 短期/长期及具体观察区间
    observed_result: null
    claim_refs: []
    assessment: ambiguous  # success / failure / mixed / ambiguous
    uncertainty: null
overall_assessment:
  label: ambiguous  # success / failure / mixed / ambiguous
  rationale: null  # 多方或长短期冲突时不能机械压成成功/失败

causal_analysis:
  proposed_mechanisms:
    - mechanism: null
      variable_refs: []
      supporting_claim_refs: []
      inference_strength: hypothesis  # hypothesis / plausible_contribution / well_supported
      inference_reason: null
      competing_explanations: []
      evidence_that_would_weaken_it: []
  selection_and_outcome_bias: null
  unresolved_factors: []
warning_signs:
  - signal: null
    available_to_actor_then: null  # true / false / null
    claim_refs: []

transferable_mechanisms:
  - mechanism: null
    conditions_required: []
    modern_evidence_needed: []
    what_not_to_infer: null
analogy_limits:
  - historical_condition: null
    modern_difference: null
    effect_on_recommendation: null  # 缩小适用范围，还是足以否定类比？
modern_problem_examples: []  # 具体问题，不给未经现实信息支持的答案
comparison_ids: []
missing_information: []

decision_reconstruction:
  decision_stages:
  - stage: null
    evidence: null
    interpretation: null
  goal_hypotheses:
  - goal: null
    evidence_level: unknown
    basis: null
    limit: null
  option_tradeoffs:
  - option_id: null
    option: null
    availability: counterfactual
    claim_refs: []
    basis: null
    expected_benefits: []
    expected_costs: []
    conditions: []
    possible_reactions: []
    future_options: null
    uncertainty: null
  motive_hypotheses:
  - hypothesis_id: null
    question: null
    explanation: null
    evidence_level: unknown
    claim_refs: []
    support: null
    alternatives: []
    what_is_missing: null
  implementation:
    recorded_steps: []
    necessary_questions: []
    unknown_procedures: []
    do_not_invent: null
  choice_explanation:
    best_supported: null
    confidence: null
    counterfactual_limit: null
  life_course:
    short_term: null
    medium_term: null
    long_term: null
    values_limit: null
    modern_bridge: null
```

## 核验与入库标准

把 `status` 改为 `reviewed` 前逐项审阅；填写审阅者、日期及遗留限制。初始空白模板必须保持 `draft`。

1. 身份与范围：填写稳定 ID、标题、事件边界、决策者、待决问题与分类。至少记录一个关键变量、一项明确结果、一条可迁移机制和一项重要类比限制。
2. 出处：至少一项实际核验的史料，并提供书名、篇章/卷次和可定位线索；若无法定位到篇章则在 locator 中提供充分位置与原因。来源难以追溯的故事保留为 draft，不进入建议依据。
3. 主张：处境、实际行动与结果中的核心断言均能经 `claim_refs` 追溯到来源。`supported` 只表示材料支持该说法，不自动证明史实无误。引文与历史人物原话特别谨慎。
4. 不确定性：每项关键主张填写置信理由；存在冲突时记录不同说法、来源关系及处理方式。已审阅案例仍可保留争议，使用时必须带上限制。
5. 推理：因果分析至少提出一项竞争解释及可削弱它的证据。将未证实动机、反事实和后世推断明确隔离；不把最终胜负当成机制证明。
6. 成败：填写评价主体、指标、时间跨度及代价。个人收益不能自动代表组织、家属或社会收益。
7. 迁移：现代对应必须有可观察指标；说明制度、权利、暴力环境等差异怎样改变建议。不能只写笼统的“古今不同”。
8. 一致性：类别、标签与枚举合法，所有内部引用存在；没有尚未创建的对照卡引用。审阅通过不等于证明该案例适合所有同类问题。

单一来源不必自动否决；明确其局限。多个来源也不必自动提升置信度；先核查它们是否相互依赖。一个强叙事案例不能替代关于现代问题的系统证据。

9. 深度：完成至少两种可能动机与三条待比较路径；若材料不足或事件不适合此数量，明确说明，不能凑数。记录为什么选该行动、替代方式可能有何取舍、实施需要什么与史料尚不能回答什么。
10. 目标：区分事件结果、当事人当时目标与后续人生轨迹，不以事业成败代替生活评价。
