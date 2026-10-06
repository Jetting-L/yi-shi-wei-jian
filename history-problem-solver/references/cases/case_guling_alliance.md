# 固陵会兵：联盟承诺与行动协调

## 目录

- 案例定位
- 决策分析速览
- 结构化案例卡

## 案例定位

边界为汉军在固陵未等到韩信、彭越而败，至刘邦遣使提出具体封地条件、诸军会于垓下。《史记》卷七叙述建议与使者往返，卷八仅简述固陵失约及后来会兵。两篇同属一书，不是独立双证。能核对的是叙事中的行动先后；韩信、彭越未赴约的真实理由、承诺后来如何履行，不能由此段确定。

## 决策分析速览

| 路径 | 证据地位 | 当时可能获得 | 当时须承担 |
|---|---|---|---|
| 按原约等待会兵 | recorded_action（较早阶段） | 若盟军按期来到，可合力作战 | 盟军不至时汉军单独受击；原约具体条件不详 |
| 遣使提出具体封地条件 | recorded_action（败后阶段） | 可能让共同进兵的收益更清楚 | 让出土地及事后履约、分配的成本 |
| 败后继续催促而不改条件 | counterfactual | 不增加分地承诺 | 若不至的原因未变，仍可能等不到援军 |

## 结构化案例卡

```yaml
schema_version: '0.2'
case_id: case_guling_alliance
title: 固陵会兵：联盟承诺与行动协调
status: reviewed
review:
  reviewed_by: Codex：在线录文及本地 DOCX/Markdown 对照，非史学鉴定
  reviewed_at: '2026-10-01'
  notes: 卷七、卷八同书互参；卷七的分地解释属于张良的归因，不作韩信、彭越真实心理或承诺兑现的证据。
scope:
  period: 楚汉战争末期
  date_range: 汉五年前后；不据本卡确定精确日月
  date_precision: approximate
  event_boundary: 固陵约兵未会、汉军失利，至遣使提出封地条件后诸军会于垓下
  people: [刘邦, 张良, 韩信, 彭越, 项羽]
  organizations: [汉军, 韩信所部, 彭越所部, 楚军]
classification:
  primary_category: competition_negotiation
  secondary_categories: [cooperation_trust, timing]
  tags: [incentives, dependencies, information_quality, power_balance, time_window]
  classification_note: 聚焦联盟成员的承诺与协调；古代战争结果不能直接作为现代谈判效果证据。
sources:
- source_id: src_shiji7
  work_title: 史记
  author_or_compiler: 司马迁
  source_type: later_compilation
  chapter_or_volume: 卷七·项羽本纪
  edition_or_translator: 维基文库简体在线录文；本地 DOCX/Markdown 底本未说明，未作纸本校勘
  locator: 汉欲西归至垓下会兵段，特别是固陵失利、张良建议、使者往返
  url: https://zh.wikisource.org/zh-hans/史記/卷007
  accessed_on: '2026-10-01'
  verification: checked
  temporal_relation: 西汉编纂楚汉战争叙事，非会兵现场记录。
  dependence_on_other_sources: 与本卡卷八同属《史记》，不计独立证据。
  limitations: 人物对话与未赴约理由由史书转述；在线录文与本地转录有个别字形差异。
- source_id: src_shiji8
  work_title: 史记
  author_or_compiler: 司马迁
  source_type: later_compilation
  chapter_or_volume: 卷八·高祖本纪
  edition_or_translator: 维基文库简体在线录文；本地 DOCX/Markdown 底本未说明，未作纸本校勘
  locator: 鸿沟议和后汉王追项羽、固陵失利至诸军会垓下段
  url: https://zh.wikisource.org/zh-hans/史記/卷008
  accessed_on: '2026-10-01'
  verification: checked
  temporal_relation: 西汉编纂楚汉战争叙事，非会兵现场记录。
  dependence_on_other_sources: 与卷七同书互参；此处省略了具体分地建议，不能把省略当否定。
  limitations: 只支持会兵前后顺序，不独立支持封地理由或承诺实际兑现。
claims:
- claim_id: clm_01
  statement: 《史记》卷七、卷八均记汉王与韩信、彭越约会攻楚，二人军队未按所记时点会合，汉军在固陵失利。
  claim_type: recorded_event
  source_refs: [src_shiji7, src_shiji8]
  source_locators: [卷七“至固陵”段, 卷八“至固陵，不会”段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 同书两篇可核，具体约定与不至原因缺少独立现场材料。
  exact_quote: null
  quote_checked: false
- claim_id: clm_02
  statement: 卷七把韩信、彭越未至与尚未分得土地相联系，作为张良向汉王提出的解释，并记其建议给出具体封地。
  claim_type: attributed_speech
  source_refs: [src_shiji7]
  source_locators: [卷七“诸侯不从约，为之奈何”至“与共分天下”段]
  support: supported
  historicity_confidence: low
  confidence_reason: 可核对史书如何归属张良之言，不能确证盟军真实动机或对话原貌。
  exact_quote: null
  quote_checked: false
- claim_id: clm_03
  statement: 卷七记汉王接受建议，遣使分别向韩信、彭越提出楚破后给予指定土地的条件。
  claim_type: recorded_event
  source_refs: [src_shiji7]
  source_locators: [卷七“于是乃发使者告韩信、彭越”段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 行动见史书叙述；承诺是否充分传达及以后如何履行另待核查。
  exact_quote: null
  quote_checked: false
- claim_id: clm_04
  statement: 卷七记使者到达后二人表示进兵，随后韩信、彭越等军会于垓下；卷八简述采用张良计后会兵。
  claim_type: recorded_event
  source_refs: [src_shiji7, src_shiji8]
  source_locators: [卷七“使者至”至“皆会垓下”段, 卷八“用张良计”至“大会垓下”段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 同书两篇记行动顺序，不能隔离其他使军队会合的因素。
  exact_quote: null
  quote_checked: false
- claim_id: clm_05
  statement: 卷八接着记诸侯联军在垓下击败项羽军，并记汉王随后夺取齐王韩信的军队。
  claim_type: recorded_event
  source_refs: [src_shiji8]
  source_locators: [卷八“与诸侯兵共击楚军”至“夺其军”段]
  support: supported
  historicity_confidence: medium
  confidence_reason: 是史书对后续结果的记载，不能用战胜倒推全部盟约已公平履行。
  exact_quote: null
  quote_checked: false
source_assessment:
  conflicts: []
  single_source_limit: 卷七和卷八同属《史记》；后一篇略去土地条件，不是独立印证或明确反证。此次未核能独立解释盟军心理、使者沟通和分地执行的材料。
  later_embellishments:
  - 不使用“分地一许即人人诚信合作”的后见概括替代承诺履行记录。
situation:
  summary: 约兵未会后汉军在固陵受挫，汉王需重新协调盟军以继续攻楚。
  claim_refs: [clm_01]
  decision_maker: 刘邦；盟军是否出兵另由韩信、彭越决定
  affected_parties: [韩信及其所部, 彭越及其所部, 汉军, 楚军, 战区民众]
  desired_outcome_at_the_time: 依约合兵击楚；其他参与者的目标和各自底线未完整记载。
  constraints: [单独作战刚遭失败, 联盟各方有独立兵力, 分地承诺将影响之后的权力与资源分配]
  information_available_then: [汉王知约兵未会及固陵败局, 张良提出未分地的解释, 盟军各自真实理由未知]
  decision_problem: 原约未能协调行动时，怎样重新提出足以促成会兵的条件并承担后续承诺？
options_available:
- option: 提出具体封地条件并遣使
  availability_basis: 卷七记张良建议、汉王采纳和使者传达。
  claim_refs: [clm_02, clm_03]
  constraints: [土地须可授予, 盟军须接收且愿意进兵, 日后兑现方式未见本段]
decision_taken:
  action: 汉王遣使提出战后封地条件；传文随后记盟军进兵会合。
  claim_refs: [clm_03, clm_04]
counterfactual_options:
- option: 败后仍按原约催促而不改变条件
  feasibility_assumptions: [仍能接触盟军, 原约仍对各方有约束力]
  uncertainty: 史书未记败后采用此路，也不知原约的具体内容和可执行性。
- option: 暂停攻势重新查明未至原因
  feasibility_assumptions: [军情允许等待, 能取得可靠解释]
  uncertainty: 未见此选择的提出与可行性；等待亦有楚军变化和补给成本。
key_variables:
- variable_id: var_incentives
  tag: incentives
  historical_observation: 张良将未分地作为盟军未至的解释，汉王随后给出封地条件。
  claim_refs: [clm_02, clm_03]
  modern_equivalent: 合作方对贡献和回报的预期是否一致
  observable_indicator: 各方明确提出的条件、责任分配和可核的承诺文本
- variable_id: var_dependencies
  tag: dependencies
  historical_observation: 原约未会，汉军单独作战失利；后续会兵改变兵力组合。
  claim_refs: [clm_01, clm_04]
  modern_equivalent: 一个伙伴不到位时总体计划是否仍可执行
  observable_indicator: 关键任务依赖图、到位确认、替代安排和截止时点
- variable_id: var_information
  tag: information_quality
  historical_observation: 未至原因在材料中主要由张良解释，未见韩信、彭越的独立理由记录。
  claim_refs: [clm_02]
  modern_equivalent: 决策者是否直接核实伙伴的障碍与条件
  observable_indicator: 各方直接反馈、资源和权限证据、相互确认的时间表
outcomes:
- perspective: 汉军及联盟
  criterion: 是否在本次战役会兵
  horizon: 固陵失利后至垓下
  observed_result: 《史记》记韩信、彭越等军到达并共同作战。
  claim_refs: [clm_04]
  assessment: success
  uncertainty: 无法把会兵单独归因于封地承诺，也未证承诺实际兑现。
- perspective: 韩信与彭越
  criterion: 所获土地和地位是否按约实现
  horizon: 垓下以后
  observed_result: 本卡所核段落没有足够材料判断两项承诺如何履行。
  claim_refs: [clm_03, clm_05]
  assessment: ambiguous
  uncertainty: 卷八另记夺韩信之军，说明战后权力变化，不能直接等同于封地承诺未兑现。
- perspective: 战区民众
  criterion: 会战造成的生命与生活损失
  horizon: 当次战役
  observed_result: 所核段落叙述战争，但不足以核算各路径对民众的代价。
  claim_refs: [clm_04, clm_05]
  assessment: ambiguous
  uncertainty: 军事会合对联盟有利，不自动等于民众受益。
overall_assessment:
  label: mixed
  rationale: 会兵在所核叙事中实现；盟约履行、个人收益及民众代价未能由该结果确定。
causal_analysis:
  proposed_mechanisms:
  - mechanism: 明确共同作战的回报可能促进盟军行动协调。
    variable_refs: [var_incentives, var_dependencies]
    supporting_claim_refs: [clm_01, clm_02, clm_03, clm_04]
    inference_strength: hypothesis
    inference_reason: 史书记载条件提出在会兵之前，但未提供各盟军的独立决策过程。
    competing_explanations: [楚军局势变化, 其他使者或军事压力, 盟军原本就在行进而只是迟到]
    evidence_that_would_weaken_it: [可靠材料显示盟军进兵决定早于封地承诺，或主要受其他条件驱动]
  selection_and_outcome_bias: 因最终合兵获胜就推定张良对未至原因的解释必然准确，属于结果倒推。
  unresolved_factors: [原约内容和会兵期限, 韩信与彭越未至的真实原因, 封地承诺的具体履行, 各军成本与民众损失]
warning_signs:
- signal: 联合作战的关键参与方未按约到位，计划仍依赖其军力。
  available_to_actor_then: true
  claim_refs: [clm_01]
transferable_mechanisms:
- mechanism: 在合作落空时直接核查各方条件，并把承诺、依赖和履行责任说清。
  conditions_required: [合作方可自由表达条件, 承诺合法且有权限兑现, 各方有确认与纠错渠道]
  modern_evidence_needed: [各方实际障碍和目标, 可兑现资源, 责任和期限, 未到位时的替代计划]
  what_not_to_infer: 不能认定给更大利益必然换来合作，也不能因短期到场就认定长期信任或公平履约。
analogy_limits:
- historical_condition: 君主之间在战争中谈封地并以军队施压
  modern_difference: 当代合作受合同、劳动及第三方权益约束；人身暴力与封地不能转作谈判手段。
  effect_on_recommendation: 只借用核查条件和明确可兑现承诺的方法，不照搬军事竞争或权力分配。
modern_problem_examples:
- 多方项目的伙伴未按原约投入，是否应先核实障碍并调整责任或回报？
- 联盟成员口头同意，却在关键节点未到位，怎样设置可执行的确认和替代方案？
comparison_ids: []
missing_information: [原约内容, 各盟军的独立心理与命令记录, 承诺履行材料, 能隔离分地条件作用的比较资料]
decision_reconstruction:
  decision_stages:
  - stage: 原约未会与固陵失利
    evidence: clm_01
    interpretation: 到场依赖失效已成为汉王可见的问题，原因仍未证实。
  - stage: 张良解释与建议
    evidence: clm_02
    interpretation: 未分地是史书归属张良的解释，不是盟军自述。
  - stage: 汉王遣使改提条件
    evidence: clm_03
    interpretation: 可确定传文记了条件变化；其传达效果与可兑现性未明。
  - stage: 盟军会合
    evidence: clm_04、clm_05
    interpretation: 行动顺序相符，但战胜不能证明唯一因果或公平履约。
  goal_hypotheses:
  - goal: 集结足够兵力击败楚军
    evidence_level: plausible_inference
    basis: clm_01、clm_03、clm_04 的战事叙述
    limit: 刘邦如何在胜负、土地与盟友关系之间加权，材料未完整说明。
  - goal: 在会兵同时保留战后的主导地位
    evidence_level: speculative
    basis: 封地承诺影响未来分配，卷八另记战后夺韩信之军
    limit: 不能凭后事认定作承诺时已有违约计划。
  option_tradeoffs:
  - option_id: opt_original
    option: 按原约等待会兵
    availability: recorded_action
    claim_refs: [clm_01]
    basis: 较早阶段确有约兵及未会；败后继续等待并非已记录决策。
    expected_benefits: [若按期会合，可避免重新谈条件]
    expected_costs: [不能及时会合时，单独作战可能再次受挫]
    conditions: [原约内容和期限对盟军足够清楚, 到场安排可行]
    possible_reactions: [盟军可能按约到场，也可能继续受未知障碍影响]
    future_options: 原约若可执行，可保留原有分配安排；若不可执行，须重新协调。
    uncertainty: 原约具体条件和盟军未至原因未知。
  - option_id: opt_offer
    option: 遣使提出战后封地条件
    availability: recorded_action
    claim_refs: [clm_02, clm_03]
    basis: 卷七明确记载建议、采纳和使者出发。
    expected_benefits: [若分配是实际障碍，可增加会兵的可预期收益]
    expected_costs: [未来须承担土地与权力分配的履约成本, 若承诺模糊或落空将损害关系]
    conditions: [有权作出且有能力履行, 使者能准确传达, 对方愿意接受]
    possible_reactions: [卷七记使者到后两方答应进兵；真实权衡与其他促因未知]
    future_options: 短期可能取得协作，长期会形成兑现与治理问题。
    uncertainty: 所核段落不能确认具体履约情况或封地是唯一原因。
  - option_id: opt_nochange
    option: 败后只催促，不改变合作条件
    availability: counterfactual
    claim_refs: []
    basis: 为比较而提出；史书未记此败后方案被采纳。
    expected_benefits: [暂不增加土地承诺]
    expected_costs: [若原先条件不足，可能再次无法会合]
    conditions: [仍有军情时间, 原约仍足以约束各方]
    possible_reactions: [盟军反应不可从此段判断]
    future_options: 可保留后续谈判空间，也可能错过当次作战窗口。
    uncertainty: 不可把它写成汉王曾认真考虑的选项。
  motive_hypotheses:
  - hypothesis_id: hyp_share
    question: 韩信、彭越为什么未按约会兵？
    explanation: 张良将未分地视为可能原因。
    evidence_level: source_attribution
    claim_refs: [clm_02]
    support: 传文明确归属张良此解释，随后记汉王改变条件。
    alternatives: [行军和通信延迟, 各军自身战场判断, 对既有承诺或风险的不同理解]
    what_is_missing: 两人各自的同期命令、通信及对原约的理解。
  - hypothesis_id: hyp_risk
    question: 韩信、彭越为什么未按约会兵？
    explanation: 也可能因军情、风险或到场能力而迟延，与土地条件不完全相同。
    evidence_level: speculative
    claim_refs: [clm_01]
    support: 多军协调存在此类可能，但本卡没有直接记录其权衡。
    alternatives: [张良提出的分地解释]
    what_is_missing: 行军时间、补给、对楚军的情报及两军各自指令。
  implementation:
    recorded_steps: [clm_03：汉王遣使提出具体战后封地条件, clm_04：传文记答复与后来会兵]
    necessary_questions: [原约是否写明期限和责任？, 使者如何确认双方接受？, 战后封地如何执行与解决争议？]
    unknown_procedures: [使者传话原貌, 双方军令及行军安排, 土地实际交割与持续时间]
    do_not_invent: 不补造书面盟约、签署程序或“承诺立即兑现”的情节。
  choice_explanation:
    best_supported: 史书记汉王在原约失效后采用张良的分地建议，后来盟军会兵；原因链仍是有竞争解释的假说。
    confidence: 对行动顺序的把握高于对未至动机、分地因果作用与履约状况的把握。
    counterfactual_limit: 未观察败后不改条件的结果，不能算出分地方案必然最优。
  life_course:
    short_term: 传文记会兵并获军事胜利；各方即时代价未完整量化。
    medium_term: 战后土地与权力安排可能改变联盟关系，但本卡所核段落不足以评价两项承诺的履行。
    long_term: 不以垓下一战给韩信、彭越或民众的全部人生结局贴成功标签。
    values_limit: 不把君主的扩张目标当成现代项目的价值目标。
    modern_bridge: 先问现代各方真正的共同目标和合法权限，再核实未到位的原因、可兑现承诺与下一次确认节点。
```
