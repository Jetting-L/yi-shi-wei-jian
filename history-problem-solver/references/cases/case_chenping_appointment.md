# 陈平受任：能力、指控与组织信任

## 目录

- 案例定位
- 决策分析速览
- 结构化案例卡

## 案例定位

事件边界为陈平经魏无知引见、获汉王任用，至周勃与灌婴等提出指控后，汉王询问魏无知和陈平并继续任用。不能把指控当事实，也不能从日后破楚倒推当时所有任用风险都已排除。

## 决策分析速览

以下为汉王在收到异议后的条件分析；《史记》未留下完整招聘制度或候选名单。

| 路径 | 证据地位 | 潜在收益 | 潜在代价 |
|---|---|---|---|
| 听取指控后直接撤换 | analytical_alternative | 若指控属实，可迅速限制风险 | 若指控失实，可能失去可用人才并损害举荐渠道 |
| 询问举荐人及当事人后继续任用 | recorded_action | 保留其谋划能力并回应争议 | 若未核实财物与权责，组织疑虑仍可能存在 |
| 暂时限权并核查资金和职责 | counterfactual | 若可执行，可减少任用与监督之间的二选一 | 所核材料未记载此程序，也不知当时能否实行 |

## 结构化案例卡

```yaml
schema_version: '0.2'
case_id: case_chenping_appointment
title: 陈平受任：能力、指控与组织信任
status: reviewed
review:
  reviewed_by: Codex：在线文本与结构审阅，非历史学专家鉴定
  reviewed_at: '2026-10-01'
  notes: 复核《史记》卷五十六、《汉书》卷四十在线录文与本地 DOCX/Markdown 同段；指控不作事实判定，《汉书》相似叙事不算独立证据。底本未确认。
scope:
  period: 楚汉战争
  date_range: 陈平归汉后、荥阳受困前；不定公历年月
  date_precision: approximate
  event_boundary: 陈平获任护军至汉王闻指控、询问并继续任用
  people: [刘邦, 陈平, 魏无知, 周勃, 灌婴]
  organizations: [汉军, 楚军]
classification:
  primary_category: organization_people
  secondary_categories: [cooperation_trust, risk_uncertainty]
  tags: [competence, integrity, information_quality, accountability, incentives, power_balance]
  classification_note: 聚焦组织如何处理新人能力、举荐与未经核实的指控，不把汉王做法设为现代聘用标准。
sources:
- source_id: src_shiji56
  work_title: 史记
  author_or_compiler: 司马迁
  source_type: later_compilation
  chapter_or_volume: 卷五十六·陈丞相世家
  edition_or_translator: 维基文库当前在线录文；旧审阅记录 oldid=1961615，本轮未复查该固定版本；未核纸本底本
  locator: “平遂至修武降汉”至“诸将乃不敢复言”段；后续荥阳用计段仅作结果边界
  url: https://zh.wikisource.org/zh-hant/史記/卷056
  accessed_on: '2026-10-01'
  verification: checked
  temporal_relation: 西汉编纂楚汉之际事件，非任用现场记录。
  dependence_on_other_sources: 与《汉书》相似段落有承袭关系；具体文本链条本次未校勘。
  limitations: 传文内对话、指控内容和人物心理不可直接当逐字实录或司法调查结论。
- source_id: src_hanshu40
  work_title: 汉书
  author_or_compiler: 班固等
  source_type: later_compilation
  chapter_or_volume: 卷四十·陈平传
  edition_or_translator: 维基文库在线录文；未核纸本底本
  locator: “平遂至修武降汉”至“诸将乃不敢复言”段
  url: https://zh.wikisource.org/zh-hans/漢書/卷040
  accessed_on: '2026-10-01'
  verification: checked
  temporal_relation: 后汉编纂，晚于事件及《史记》。
  dependence_on_other_sources: 与《史记》叙事和措辞高度相似，不计为独立确证。
  limitations: 引见人数《史记》作七人，《汉书》作十人；该差异不影响本卡决策问题，但不能强行统一。
claims:
- claim_id: clm_01
  statement: 两书都叙述陈平经魏无知引见，汉王交谈后授都尉、参乘及护军职责，诸将当时反对迅速重用。
  claim_type: recorded_event
  source_refs: [src_shiji56, src_hanshu40]
  source_locators: [史记卷56修武引见段, 汉书卷40修武引见段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 两书文本可核，但叙事相近且并非独立双重证明。
  exact_quote: null
  quote_checked: false
- claim_id: clm_02
  statement: 周勃、灌婴等在传文中指控陈平旧有不端、反复易主及收金影响军职安排；这些是他们提出的指控，不是本卡确认的事实。
  claim_type: attributed_speech
  source_refs: [src_shiji56, src_hanshu40]
  source_locators: [史记卷56绛侯灌婴进言段, 汉书卷40绛灌进言段]
  support: supported
  historicity_confidence: low
  confidence_reason: 可确认史书这样归属指控，无法据此核实各项指控真伪。
  exact_quote: null
  quote_checked: false
- claim_id: clm_03
  statement: 汉王听后询问魏无知与陈平；传文记魏无知强调才用，陈平解释转投经历及受金用途，并提出若谋划无用可退还金、请求离开。
  claim_type: attributed_speech
  source_refs: [src_shiji56, src_hanshu40]
  source_locators: [史记卷56汉王召让段, 汉书卷40汉王召问段]
  support: supported
  historicity_confidence: low
  confidence_reason: 问答可追溯为史书叙事；陈平的自我辩解不能单独证实资金去向与清白。
  exact_quote: null
  quote_checked: false
- claim_id: clm_04
  statement: 传文记汉王此后向陈平致歉、厚赐，任其为护军中尉；在这一叙事段落中，诸将不敢再言。
  claim_type: recorded_event
  source_refs: [src_shiji56, src_hanshu40]
  source_locators: [史记卷56“汉王乃谢”段, 汉书卷40“汉王乃谢”段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 两书有相近记载，但是否所有疑虑消除、是否另作审计未见材料。
  exact_quote: null
  quote_checked: false
- claim_id: clm_05
  statement: 《史记》《汉书》均叙述陈平后来为汉王献策、参与荥阳应对；这只是后续能力表现线索。
  claim_type: recorded_event
  source_refs: [src_shiji56, src_hanshu40]
  source_locators: [史记卷56荥阳受围后段, 汉书卷40荥阳受围后段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 传文有后续叙事，不能倒推早期财物指控已查清或任用决定必然最优。
  exact_quote: null
  quote_checked: false
source_assessment:
  conflicts:
  - claim_refs: [clm_01]
    source_refs: [src_shiji56, src_hanshu40]
    disagreement: 《史记》称同进七人，《汉书》称十人；与本卡任用争议的核心无关。
    handling: 保留数字差异，不用统一人数论证汉王选人质量。
  single_source_limit: 核心叙事来自《史记》传统，《汉书》的相近叙述不按独立史料计数。
  later_embellishments:
  - 不采用演义式“刘邦完全不问品行，只看才能”的绝对化概括。
situation:
  summary: 汉王在战争中迅速任用新来的陈平，既有将领质疑能力和可信度。
  claim_refs: [clm_01, clm_02]
  decision_maker: 刘邦
  affected_parties: [陈平, 举荐人魏无知, 既有将领, 汉军]
  desired_outcome_at_the_time: 可推测需要能帮助对楚作战的人；是否另有用人原则与个人信任标准，材料未完整交代。
  constraints:
  - 战争中人才与决策时间都有限，护军职位涉及既有将领。
  - 指控中混有可核的转投经历与尚未核实的不端行为。
  information_available_then:
  - 刘邦可听到魏无知举荐、既有将领异议及陈平辩解。
  - 完整资金记录、各项指控的调查结果，所核材料未记载。
  decision_problem: 对有潜在能力但受严重指控的新任人员，应如何判断是否继续授予护军权力？
options_available:
- option: 询问举荐人和当事人后继续任用
  availability_basis: 史书记录的问答与任命。
  claim_refs: [clm_03, clm_04]
  constraints: [现存材料不显示指控已被独立核实]
- option: 接受陈平请求离开的提议
  availability_basis: 传文中的当事人提议。
  claim_refs: [clm_03]
  constraints: [会失去其可能能力, 提议真实性与条件由史书转述]
decision_taken:
  action: 汉王询问后继续任用陈平，授护军中尉。
  claim_refs: [clm_03, clm_04]
counterfactual_options:
- option: 暂限权并独立核查资金与任职表现
  feasibility_assumptions: [能设定职责边界, 能取得可核的财物与绩效记录]
  uncertainty: 所核史料未记此做法或当时组织是否具备条件。
key_variables:
- variable_id: var_evidence
  tag: information_quality
  historical_observation: 指控、举荐与当事人辩解同时出现，真伪并未逐项核实。
  claim_refs: [clm_01, clm_02, clm_03]
  modern_equivalent: 人员评价中的证据质量
  observable_indicator: 具体行为记录、独立核验和可申辩材料
- variable_id: var_competence
  tag: competence
  historical_observation: 魏无知称陈平有用，后续传文记其献策。
  claim_refs: [clm_03, clm_05]
  modern_equivalent: 与岗位直接相关的能力
  observable_indicator: 可复核的任务样本、试用表现与同行反馈
- variable_id: var_accountability
  tag: accountability
  historical_observation: 护军职责影响诸将，受金指控触及资源分配。
  claim_refs: [clm_01, clm_02]
  modern_equivalent: 授权、资金使用与监督是否匹配
  observable_indicator: 权限范围、财务记录、复核和申诉程序
outcomes:
- perspective: 刘邦与汉军
  criterion: 是否保留陈平担任护军
  horizon: 指控处理的当次决策
  observed_result: 传文记继续任用，并写诸将在该段落中不敢再言。
  claim_refs: [clm_04]
  assessment: success
  uncertainty: 留任是可观察决定，不代表疑虑消失或资金指控被证伪。
- perspective: 既有将领与组织治理
  criterion: 资金与权责问题是否获得可核查处理
  horizon: 重新任命之后
  observed_result: 所核段落未记独立调查或长期监督结果。
  claim_refs: [clm_02, clm_03, clm_04]
  assessment: ambiguous
  uncertainty: 缺载不能写作完全没有监督。
overall_assessment:
  label: mixed
  rationale: 传文显示留任及后续贡献，诚信指控的核实与组织成本仍未知。
causal_analysis:
  proposed_mechanisms:
  - mechanism: 汉王兼听举荐、异议与辩解，可能避免仅凭流言失去人才。
    variable_refs: [var_evidence, var_competence]
    supporting_claim_refs: [clm_01, clm_02, clm_03, clm_04]
    inference_strength: plausible_contribution
    inference_reason: 问答在任命前出现，但后续成果不能证明当时完成了充分调查。
    competing_explanations: [战争压力促使汉王承担较高风险, 史家可能突出识才叙事, 魏无知的关系影响判断]
    evidence_that_would_weaken_it: [可靠材料显示任命主要由别的政治交易决定或指控已被另外核清]
  selection_and_outcome_bias: 因陈平后来的计策而认定所有旧指控失实，是结果偏差；未被采纳的人才无从在此叙事中比较。
  unresolved_factors: [资金数额与用途的独立记录, 各项指控真伪, 原有将领后来是否仍有异议]
warning_signs:
- signal: 迅速授予影响他人的权力，同时出现具体资金分配指控。
  available_to_actor_then: true
  claim_refs: [clm_01, clm_02]
transferable_mechanisms:
- mechanism: 将能力判断与可信度核查分别进行，并使授权、监督与风险相称。
  conditions_required: [可核实行为证据, 当事人有解释机会, 指控涉及的权责可界定]
  modern_evidence_needed: [具体绩效样本, 财务和利益冲突记录, 合法公平的调查程序]
  what_not_to_infer: 不能以“有才”允许骚扰、贪污或其他严重不端；也不能把匿名传闻直接当事实。
analogy_limits:
- historical_condition: 战争中君主可立即授予或撤销军职
  modern_difference: 当代招聘与纪律处分有法律、隐私、劳动保障和正当程序要求。
  effect_on_recommendation: 应核查当地规则并保障调查公平，不能复制君主个人裁断。
modern_problem_examples:
- 新合作者能力强，但有未经核实的失信指控，怎样决定权限与核查步骤？
- 团队因新任主管影响资源分配而不满，如何分别处理能力与监督？
comparison_ids: []
missing_information: [指控真伪的独立材料, 汉王与既有将领后续关系, 授权监督的实际制度]
decision_reconstruction:
  decision_stages:
  - stage: 引见与快速任用
    evidence: clm_01
    interpretation: 战时识才收益与组织接受成本同时出现。
  - stage: 指控与答辩
    evidence: clm_02、clm_03
    interpretation: 指控只能作为核查起点，答辩也非无罪证明。
  - stage: 继续任用
    evidence: clm_04
    interpretation: 决策被记载，完整调查过程未明。
  goal_hypotheses:
  - goal: 为汉军获得可用谋士
    evidence_level: plausible_inference
    basis: 战争背景与 clm_01、clm_05
    limit: 未见刘邦自述所有任用目标。
  - goal: 在不失去既有将领支持的情况下使用新人
    evidence_level: plausible_inference
    basis: clm_01、clm_02及询问举荐人与陈平的行为
    limit: 是否把安抚诸将作为明确目标无法确认。
  option_tradeoffs:
  - option_id: opt_dismiss
    option: 听取指控后撤换陈平
    availability: analytical_alternative
    claim_refs: [clm_02]
    basis: 根据异议提出的分析备选，史书未记汉王考虑或执行。
    expected_benefits: [若指控属实，可立即限制相关风险, 可能回应将领不满]
    expected_costs: [若指控失实，失去可能的人才, 可能打击外来者与举荐者]
    conditions: [可替代人选, 指控足以支持相应处置]
    possible_reactions: [既有将领可能接受，陈平与举荐者可能受损；均不确定]
    future_options: 保留其他用人方式，却可能关闭陈平的参与机会。
    uncertainty: 不把后续战果当作此路必错的证据。
  - option_id: opt_retain
    option: 询问后继续任用
    availability: recorded_action
    claim_refs: [clm_03, clm_04]
    basis: 两书记录的决定。
    expected_benefits: [保留可能有用的才能, 给举荐与申辩以机会]
    expected_costs: [若指控属实，护军权力可造成进一步伤害, 组织信任可能受损]
    conditions: [汉王有权任命, 陈平愿留任]
    possible_reactions: [传文记诸将在该段落中不敢再言；内心信任或长期反应未知]
    future_options: 可观察后续表现，也可能形成难纠正的授权问题。
    uncertainty: 史书未详财物核查与长期监督。
  - option_id: opt_limit
    option: 暂限权并核查
    availability: counterfactual
    claim_refs: []
    basis: 现代分析提出，未见当时采用或可行的证据。
    expected_benefits: [保留能力评估机会, 控制财物与人事风险]
    expected_costs: [调查需要时间与可信人员, 战时可能损失速度]
    conditions: [能够界定权限并取得记录]
    possible_reactions: [诸将、陈平或魏无知的反应均未知]
    future_options: 在现代条件下可能保留后续增权或撤换空间。
    uncertainty: 不是史书记载的第三方案。
  motive_hypotheses:
  - hypothesis_id: hyp_ability
    question: 为什么汉王继续任用？
    explanation: 可能更看重陈平提供的谋划能力。
    evidence_level: plausible_inference
    claim_refs: [clm_03, clm_04]
    support: 传文安排了能力辩护与随后任命。
    alternatives: [战争紧迫, 个人与举荐关系, 后世识才叙事]
    what_is_missing: 刘邦权衡指控时的真实标准与信息。
  - hypothesis_id: hyp_risk
    question: 为什么汉王继续任用？
    explanation: 也可能认为在当时战争压力下，等待更多核查的成本更高。
    evidence_level: speculative
    claim_refs: [clm_01, clm_04]
    support: 战争背景可见，但汉王并未留下该理由的可信直接记录。
    alternatives: [相信陈平辩解, 对将领指控本就怀疑]
    what_is_missing: 可替代谋士、决策时间与核查能力。
  implementation:
    recorded_steps: [clm_01记引见与任命, clm_02记指控, clm_03记两次问答, clm_04记继续任用]
    necessary_questions: [各项指控有何独立证据？, 金的用途和护军权限如何记录？]
    unknown_procedures: [是否调查资金或证人, 是否限制权限, 如何监督与复核]
    do_not_invent: 不补写现代背景调查、审计或试用期；不将被指控改写为已犯错。
  choice_explanation:
    best_supported: 文本明确记问答后继续任用，能力考量是有依据的解释，但不能证明汉王已查清品行。
    confidence: 行动可追溯，问答细节与真实动机较不确定。
    counterfactual_limit: 无法用后来战果计算撤换或限权的替代结局。
  life_course:
    short_term: 陈平获更高护军职权；传文写诸将在该段落中不敢再言。
    medium_term: 史书记其后献策；不等于资金指控已获证伪。
    long_term: 此卡不以陈平日后地位评价整套组织治理方式。
    values_limit: 战时胜利、程序公正与个体权益并非同一指标。
    modern_bridge: 先问用户要解决用人、合作信任还是组织公平，再决定查什么证据、给何种权限及何时复盘。
```
