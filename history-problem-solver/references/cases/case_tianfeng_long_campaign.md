# 田丰劝袁绍久持：窗口变化与进攻时机

## 目录

- 案例定位
- 决策分析速览
- 结构化案例卡

## 案例定位

事件边界为建安五年曹操击刘备时田丰劝袁绍袭其后方，至刘备败后田丰改劝久持、袁绍南下并于官渡失利。《三国志》与《后汉书》都记前后两次建议，因此不能把田丰写成任何时候都主张等待。久持战略没有在这次战役中实施，不能因官渡失利就说它必胜。

## 决策分析速览

| 路径 | 证据地位 | 潜在收益 | 潜在代价 |
|---|---|---|---|
| 曹操东征刘备时袭其后 | recorded_offer（较早阶段） | 若后方空虚，可争取阶段优势 | 情报、行军与其他战线风险未知；未实施，效果不可证 |
| 刘备败后立即南下决战 | recorded_action（较晚阶段） | 若速胜，可尽快达成军事目标 | 对手已回防，集中决战的损失风险较大 |
| 刘备败后持久准备、分兵牵制 | recorded_offer（较晚阶段） | 可利用资源、准备与消耗争取主动 | 时间、粮食、民众负担及敌方变化会反噬；不能保证获胜 |

## 结构化案例卡

```yaml
schema_version: '0.2'
case_id: case_tianfeng_long_campaign
title: 田丰劝袁绍久持：窗口变化与进攻时机
status: reviewed
review:
  reviewed_by: Codex：在线文本与结构审阅，非历史学专家鉴定
  reviewed_at: '2026-10-01'
  notes: 复核《三国志》卷六、《后汉书》卷七十四上在线录文与本地 DOCX/Markdown 同段；袭后与久持分属不同窗口，裴注引文不等于正文。底本未确认。
scope:
  period: 东汉末建安五年官渡战役前后
  date_range: 建安五年（约公元200年）；具体日月不定
  date_precision: approximate
  event_boundary: 曹操东征刘备时的时机建议，至袁绍南下、官渡败后田丰遇害
  people: [袁绍, 田丰, 曹操, 刘备, 沮授, 郭图]
  organizations: [袁绍军, 曹操军]
classification:
  primary_category: timing
  secondary_categories: [risk_uncertainty, organization_people]
  tags: [time_window, readiness, information_quality, resources, downside, option_value]
  classification_note: 核心是机会窗口变化后的战略调整；组织采纳异议为次要主题。
sources:
- source_id: src_sgz6
  work_title: 三国志
  author_or_compiler: 陈寿；所核页面亦含裴松之注引后出材料
  source_type: later_compilation
  chapter_or_volume: 卷六·袁绍传及裴松之注
  edition_or_translator: 维基文库在线录文；未核纸本底本
  locator: 袁绍传“建安五年，太祖自东征备”段与“初，绍之南也”田丰劝久持段
  url: https://zh.wikisource.org/wiki/三國志/卷06
  accessed_on: '2026-10-01'
  verification: checked
  temporal_relation: 西晋史书叙述东汉末事件；裴注所引材料更晚汇入此传。
  dependence_on_other_sources: 与《后汉书》相关段落可能共享早期材料，不能按两份独立现场记录计。
  limitations: 注引《先贤行状》含更详细的田丰心理与旁人话语，不与陈寿正文混为同级证据。
- source_id: src_hhs74
  work_title: 后汉书
  author_or_compiler: 范晔等
  source_type: later_compilation
  chapter_or_volume: 卷七十四上·袁绍刘表列传
  edition_or_translator: 维基文库在线录文；未核纸本底本
  locator: 沮授与郭图议南下段、建安五年曹操东征刘备至田丰被系段
  url: https://zh.wikisource.org/zh-hant/後漢書/卷74上
  accessed_on: '2026-10-01'
  verification: checked
  temporal_relation: 南朝刘宋编纂，晚于事件及《三国志》。
  dependence_on_other_sources: 与《三国志》相关叙述相似；具体承袭链未在本次考定。
  limitations: 添述沮授、郭图等论辩，不等于能复原袁绍全部会议过程。
claims:
- claim_id: clm_01
  statement: 两书均叙述曹操东征刘备时，田丰劝袁绍袭其后方，袁绍以儿子患病为由未行；曹操随后击败刘备。
  claim_type: recorded_event
  source_refs: [src_sgz6, src_hhs74]
  source_locators: [三国志卷6“太祖自东征备”段, 后汉书卷74上建安五年段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 史书可核，但具体病情、袁绍真正权衡与袭后效果无法由叙事确证。
  exact_quote: null
  quote_checked: false
- claim_id: clm_02
  statement: 曹操击败刘备后，田丰在两书中建议袁绍转为久持、修农战、分兵牵制，反对立即用一战定成败。
  claim_type: attributed_speech
  source_refs: [src_sgz6, src_hhs74]
  source_locators: [三国志卷6“初，绍之南也”段, 后汉书卷74上“田丰以既失前几”段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 战略方向在两书相近；具体话语与预测期限不能当逐字或可靠战果预测。
  exact_quote: null
  quote_checked: false
- claim_id: clm_03
  statement: 两书叙述袁绍未采纳久持建议，田丰反复进谏后被以扰乱军心之由拘禁。
  claim_type: recorded_event
  source_refs: [src_sgz6, src_hhs74]
  source_locators: [三国志卷6“绍不从”段, 后汉书卷74上“绍以为沮众”段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 事件由后世史书记载，处罚理由为史书归属，不等于袁绍全部心理已知。
  exact_quote: null
  quote_checked: false
- claim_id: clm_04
  statement: 《后汉书》另记沮授提出先休养、渐进牵制，郭图与审配主张趁早进攻，袁绍采纳后者。
  claim_type: attributed_speech
  source_refs: [src_hhs74]
  source_locators: [卷74上“沮授进说”至“绍纳图言”段]
  support: supported
  historicity_confidence: low
  confidence_reason: 较晚传书提供论辩叙事，未查到独立会议记录。
  exact_quote: null
  quote_checked: false
- claim_id: clm_05
  statement: 《三国志》记袁绍军在官渡失利，随后田丰被杀。
  claim_type: recorded_event
  source_refs: [src_sgz6]
  source_locators: [卷6官渡败后“绍军既败”段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 败局与被杀可核为史书记载，杀人动机仍需谨慎。
  exact_quote: null
  quote_checked: false
- claim_id: clm_06
  statement: 《三国志》归属袁绍败后因未采纳田丰意见而自认受嘲的话语；这不能独立证明田丰实际讥笑过他。
  claim_type: attributed_speech
  source_refs: [src_sgz6]
  source_locators: [卷6“绍还，谓左右曰”段]
  support: supported
  historicity_confidence: low
  confidence_reason: 是史书归属的言论，袁绍心理和田丰实际反应未获独立核查。
  exact_quote: null
  quote_checked: false
source_assessment:
  conflicts:
  - claim_refs: [clm_02]
    source_refs: [src_sgz6, src_hhs74]
    disagreement: 《三国志》记久持计划“不及二年”可克，《后汉书》作“不及三年”；都是传文中被归属的预测。
    handling: 不选一个作准确期限，不据这两个数字承诺久持必胜。
  single_source_limit: 《三国志》《后汉书》并非独立同期作战档案；更细的处罚动机主要来自《三国志》正文与裴注引述，不能相互简单累加可信度。
  later_embellishments:
  - 不采用《三国演义》的官渡人物对话与兵力数字来填补当时信息。
situation:
  summary: 袁绍掌北方资源、准备南下；曹操先东征刘备，后回防。田丰在前后不同信息条件下提出不同建议。
  claim_refs: [clm_01, clm_02, clm_04]
  decision_maker: 袁绍
  affected_parties: [田丰, 袁绍军, 曹操军, 战区民众]
  desired_outcome_at_the_time: 可推测袁绍想在与曹操的竞争中取得优势；速决、声望、合法性等目标的具体权重未知。
  constraints:
  - 对手位置和守备随曹操东征、回防而变化。
  - 持久与速战都需承担军需、人员及民众成本。
  information_available_then:
  - 田丰据曹操东征与回防分别判断窗口，袁绍可听到不同谋士意见。
  - 袁绍对敌军准确兵力、粮食、政治变化的掌握程度未由本卡复原。
  decision_problem: 机会窗口变化后，应立即集中南下还是转向准备与牵制？
options_available:
- option: 趁曹操东征刘备时袭其后方
  availability_basis: 较早阶段田丰的记载中建议。
  claim_refs: [clm_01]
  constraints: [窗口短暂, 行军与情报条件未知]
- option: 刘备败后立即南下决战
  availability_basis: 袁绍实际选择与郭图等人的记载中主张。
  claim_refs: [clm_03, clm_04]
  constraints: [曹操已可回防, 决战输赢代价高]
- option: 刘备败后久持并分兵牵制
  availability_basis: 田丰明确建议，沮授另有相近而非完全相同的渐进方案。
  claim_refs: [clm_02, clm_04]
  constraints: [需要补给、组织纪律与时间, 敌方反制未知]
decision_taken:
  action: 袁绍未在曹操东征时袭后，后来南下对曹操用兵；田丰因进谏被拘禁。
  claim_refs: [clm_01, clm_03]
counterfactual_options: []
key_variables:
- variable_id: var_window
  tag: time_window
  historical_observation: 田丰前后建议不同，区别在曹操东征与回防。
  claim_refs: [clm_01, clm_02]
  modern_equivalent: 机会是否随外部状态变化
  observable_indicator: 对手或市场的实际行动、截止条件及窗口关闭信号
- variable_id: var_readiness
  tag: readiness
  historical_observation: 久持方案要求农战准备与分兵，速战派主张尽早把握优势。
  claim_refs: [clm_02, clm_04]
  modern_equivalent: 准备带来的收益与延误代价
  observable_indicator: 资源消耗速度、需要补齐的能力、等待期间对方的变化
- variable_id: var_dissent
  tag: information_quality
  historical_observation: 记录有互相冲突的谋士意见，田丰被拘禁。
  claim_refs: [clm_02, clm_03, clm_04]
  modern_equivalent: 决策组织能否审查逆耳意见
  observable_indicator: 反对意见的证据、回应方式及允许修正决策的渠道
outcomes:
- perspective: 袁绍军
  criterion: 当次南下是否击败曹操
  horizon: 官渡战役阶段
  observed_result: 《三国志》记袁绍军败。
  claim_refs: [clm_05]
  assessment: failure
  uncertainty: 失败不能隔离时机、补给、战场处置与偶然性各自贡献。
- perspective: 田丰
  criterion: 建议是否被采纳与自身安全
  horizon: 南下至败后
  observed_result: 建议未获采纳，史书记其遭拘禁并被杀。
  claim_refs: [clm_03, clm_05]
  assessment: failure
  uncertainty: 杀人决策的完整心理过程未获独立验证。
- perspective: 战区民众
  criterion: 持久或速战带来的损害
  horizon: 战役及替代路线
  observed_result: 本卡无足够材料比较两路对民众的实际总体损害。
  claim_refs: []
  assessment: ambiguous
  uncertainty: 田丰方案的袭扰本身也可能伤害民众，不能只评价军事胜负。
overall_assessment:
  label: mixed
  rationale: 袁绍的当次军事目标失败且田丰遇害；替代战略及民众损害无法由结局求出。
causal_analysis:
  proposed_mechanisms:
  - mechanism: 机会窗口变化后仍以集中的速决方式行动，可能增加对手回防时的决战风险。
    variable_refs: [var_window, var_readiness]
    supporting_claim_refs: [clm_01, clm_02, clm_03, clm_05]
    inference_strength: hypothesis
    inference_reason: 文本给出先后与后果，却不能隔离其他战场因素，更未观察久持的真实结果。
    competing_explanations: [曹操的指挥与袁军补给问题, 部下选择与战场偶然性, 久持也可能因资源消耗而失败]
    evidence_that_would_weaken_it: [可靠资料表明曹操回防并未改变关键机会，或官渡失败与进攻时点无关]
  selection_and_outcome_bias: 因袁绍失败而把所有谋士反对意见视为必然正确，是结果偏差；田丰预测的二或三年胜利未被实际验证。
  unresolved_factors: [袁军实际资源与持续作战能力, 速战和久持对民众的代价, 决战失败各原因的相对权重]
warning_signs:
- signal: 原定袭后目标已经回防，原方案的前提变化。
  available_to_actor_then: true
  claim_refs: [clm_01, clm_02]
transferable_mechanisms:
- mechanism: 根据机会窗口和准备条件的变化重评行动时点，保留异议渠道。
  conditions_required: [能辨认关键外部变化, 等待与立即行动的成本均可估计, 可安全讨论反对意见]
  modern_evidence_needed: [真实截止条件, 资源消耗与准备进度, 对方行动变化, 利害相关者的影响]
  what_not_to_infer: 不可推断“早攻必胜”“等待必胜”，更不能把军事袭扰转化为现代欺骗或伤害建议。
analogy_limits:
- historical_condition: 古代战争可用分兵袭扰消耗对手与民众
  modern_difference: 现代个人、组织决策有法律、伦理及第三方权益约束。
  effect_on_recommendation: 只迁移重新评估窗口的思路，不迁移暴力与袭扰手段。
modern_problem_examples:
- 原本适合立刻推出的项目，关键对手条件变化后，是否应调整时点？
- 团队对现在上线与继续准备有争论，如何核对窗口和等待成本？
comparison_ids: []
missing_information: [独立的战时记录, 两种未实施战略的真实效果, 袁绍目标与信息的完整记录]
decision_reconstruction:
  decision_stages:
  - stage: 曹操东征刘备
    evidence: clm_01
    interpretation: 田丰建议立即利用相对空虚的后方；不是始终主张等待。
  - stage: 曹操胜刘备后
    evidence: clm_02、clm_04
    interpretation: 情势变化，久持与速战的收益代价需重新计算。
  - stage: 袁绍南下与田丰被拘
    evidence: clm_03
    interpretation: 采纳了速战方向，惩罚异议可见；内部完整理由未知。
  - stage: 官渡败后
    evidence: clm_05、clm_06
    interpretation: 观察到失败与田丰遇害，不能验证久持的反事实结果。
  goal_hypotheses:
  - goal: 在竞争中击败曹操
    evidence_level: plausible_inference
    basis: clm_01、clm_02与实际南下
    limit: 胜利之外的袁绍目标及权重不可确证。
  - goal: 尽早利用北方优势完成战役
    evidence_level: source_attribution
    basis: clm_04中郭图等的劝进理由及袁绍采纳叙事
    limit: 这是谋士言论与史书叙事，不能当袁绍内心独白。
  option_tradeoffs:
  - option_id: opt_early
    option: 曹操东征时袭其后
    availability: recorded_offer
    claim_refs: [clm_01]
    basis: 田丰在较早时点的记载中建议。
    expected_benefits: [若曹操后方空虚，可能取得阶段优势]
    expected_costs: [行军、情报及其他战线风险, 军民损害]
    conditions: [确有空虚且来得及行动, 袁军可组织袭击]
    possible_reactions: [曹操可能回援或另行应对，结果未知]
    future_options: 可能改变后续谈判和作战空间，也可能陷入新风险。
    uncertainty: 未实施，不能断言必胜；时间窗口大小未经本卡量化。
  - option_id: opt_attack
    option: 刘备败后集中南下
    availability: recorded_action
    claim_refs: [clm_03, clm_04]
    basis: 袁绍实际南下，郭图等较晚叙事主张速战。
    expected_benefits: [若速胜，可较快实现军事目标, 避免持久战消耗]
    expected_costs: [在对手回防后承担集中决战损失, 失利会削弱后续选择]
    conditions: [军粮、指挥与补给能支持决战, 对手防御可以突破]
    possible_reactions: [曹操回防并交战，具体战场应对不是本卡完整重建]
    future_options: 速胜可扩张，失败则压缩后续战略空间。
    uncertainty: 已知失败不证明决策时胜算为零。
  - option_id: opt_hold
    option: 刘备败后久持、农战准备与分兵牵制
    availability: recorded_offer
    claim_refs: [clm_02, clm_04]
    basis: 田丰与沮授均提出渐进方案，细节并不完全相同。
    expected_benefits: [可能利用资源优势与准备时间, 保留选择进攻时点的余地]
    expected_costs: [长期军需与民众负担, 对手也可能变强或改变联盟]
    conditions: [后勤可持续, 军队能执行分兵方案, 目标允许推迟]
    possible_reactions: [曹操可能防御、出击或结盟，实际未观察]
    future_options: 保留部分行动空间，也可能错失速战机会。
    uncertainty: 二年或三年的胜利预测是史书归属的意见，不是被验证的期限。
  motive_hypotheses:
  - hypothesis_id: hyp_speed
    question: 为什么袁绍仍选择南下？
    explanation: 郭图等强调优势与早取之机，袁绍可能认为速战收益更高。
    evidence_level: plausible_inference
    claim_refs: [clm_04, clm_03]
    support: 《后汉书》记谋士争论和采纳结果。
    alternatives: [政治合法性, 军队整合, 其他情报影响]
    what_is_missing: 袁绍自己的完整权衡与可信战前资源记录。
  - hypothesis_id: hyp_face
    question: 为什么袁绍拘禁田丰？
    explanation: 传文归属扰乱军心的理由；也可能涉及权威或内部派系，但后者只是推测。
    evidence_level: source_attribution
    claim_refs: [clm_03, clm_06]
    support: 史书写以沮众为由拘禁，并归属败后担忧被笑的话语；均非完整心理记录。
    alternatives: [派系矛盾, 战时纪律考虑, 史家叙事偏向]
    what_is_missing: 决策过程、田丰言行的独立记录。
  implementation:
    recorded_steps: [clm_01记早期建议未行, clm_02记后期久持建议, clm_03记南下与拘禁, clm_05记败局和遇害]
    necessary_questions: [两次建议之间发生哪些可核实的军事变化？, 袁军久持资源是否够用？]
    unknown_procedures: [内部会议与情报流程, 两种战略详细后勤计划, 拘禁与处死的完整程序]
    do_not_invent: 不把袁绍儿子病情、心理、具体兵力和久持胜率补成确定事实。
  choice_explanation:
    best_supported: 袁绍先拒袭后，后拒久持而南下；《后汉书》还呈现速战意见，但其真实权重不明。
    confidence: 选择方向与败局可追溯到后世史书，反事实胜负与心理解释更不确定。
    counterfactual_limit: 官渡败局不能证明田丰任一未采纳建议必然成功。
  life_course:
    short_term: 南下前田丰遭拘禁，军队进入高代价战役。
    medium_term: 《三国志》记官渡失利与田丰被杀。
    long_term: 本卡不从此一战推定袁绍政权全部历史必然性或民众总体福祉。
    values_limit: 军事胜败不是评价所有当事人与民众代价的唯一指标。
    modern_bridge: 对用户已确认的目标，核实真实窗口、准备成本和可保留选项；不要把“时机”变成永远冲刺或永远等待的口号。
```
