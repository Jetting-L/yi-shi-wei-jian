# 范蠡离越：退出行动与退出条件

## 目录

- 案例定位
- 决策分析速览
- 结构化案例卡

## 案例定位

v0.2：沿用已核《史记》《国语》，新增目标假说、三条路径与实施条件；区分离越前意图和后来经历。

## 决策分析速览

下表是条件分析，潜在收益与代价不等于已经发生的事实。完整理由、证据等级与未知见 decision_reconstruction。

| 路径 | 证据地位 | 潜在收益 | 潜在代价 |
|---|---|---|---|
| 接受挽留、继续任职 | recorded_offer | 若兑现，可能保留地位、政治影响和既有资源 | 继续依赖同一权力关系 |
| 暂时退居或减少参与 | counterfactual | 若被允许，可能留出考虑时间并保留关系 | 可能不改变依附与风险 |
| 离越并重新安置生活 | recorded_action | 若能完成且不被追究，可能摆脱部分原有依附 | 放弃或改变既有角色与关系 |

## 结构化案例卡

```yaml
schema_version: '0.2'
case_id: case_fanli_departure
title: 范蠡离越：退出行动与退出条件
status: reviewed
review:
  reviewed_by: Codex：在线文本与结构审阅，非历史学专家鉴定
  reviewed_at: '2026-09-28'
  notes: v0.2：沿用已核《史记》《国语》，新增目标假说、三条路径与实施条件；区分离越前意图和后来经历。
scope:
  period: 春秋末
  date_range: 越灭吴之后；本卡不定离越的公历年月
  date_precision: approximate
  event_boundary: 灭吴后范蠡辞别勾践至离越；后续去向仅作证据边界说明
  people:
  - 范蠡
  - 勾践
  organizations:
  - 越国
classification:
  primary_category: stay_leave
  secondary_categories:
  - risk_uncertainty
  tags:
  - exit_options
  - resources
  - power_balance
  - information_quality
  - alternatives
  classification_note: 适合探讨权力不对等下的退出条件；不是一般离职建议的默认案例。
sources:
- source_id: src_shiji41
  work_title: 史记
  author_or_compiler: 司马迁
  source_type: later_compilation
  chapter_or_volume: 卷四十一·越王勾践世家
  edition_or_translator: 维基文库在线录文，页面固定版本 oldid=2018395；未核验纸本底本
  locator: 越王句践节末范蠡致书与文种之死；范蠡节离越、迁齐及迁陶段
  url: https://zh.wikisource.org/zh-hans/史記/卷041
  accessed_on: '2026-09-28'
  verification: checked
  temporal_relation: 西汉编纂，叙述春秋末事件；非当事人同步记录。
  dependence_on_other_sources: 与《国语》相似段落可能具有材料承袭关系，本次未证明来源独立。
  limitations: 只核对相关在线录文；对话、书信与人物内心不能视为逐字实录。
- source_id: src_shiji41_check
  work_title: 史记
  author_or_compiler: 司马迁
  source_type: later_compilation
  chapter_or_volume: 卷四十一·越王勾践世家
  edition_or_translator: 识典古籍 HY2295 在线录文；页面标示司马迁撰、裴骃集解、司马贞索隐；未核影印底本
  locator: 范蠡遂去至种遂自杀段；范蠡事越王勾践至卒老死于陶段
  url: https://www.shidianguji.com/book/HY2295/chapter/1kw42qbybwgsp
  accessed_on: '2026-09-28'
  verification: checked
  temporal_relation: 西汉编纂，叙述春秋末事件；非当事人同步记录。
  dependence_on_other_sources: 同一《史记》篇章的另一数字呈现，仅用于文本对照，不是独立史料。
  limitations: 页面存在明显录文讹字、缺字图像；本次只交叉核对关键情节，不据此建立校勘结论。
- source_id: src_guoyu21
  work_title: 国语
  author_or_compiler: 传统题左丘明；本卡不以传统署名确认作者或成书年代
  source_type: later_compilation
  chapter_or_volume: 卷二十一·越语下
  edition_or_translator: 维基文库在线注释本，固定版本 oldid=1968473；正文与夹注分别阅读，未核纸本底本
  locator: 末节“范蠡乘轻舟以浮于五湖”
  url: https://zh.wikisource.org/zh-hans/國語/卷21
  accessed_on: '2026-09-28'
  verification: checked
  temporal_relation: 传世叙事，不作为事件现场记录；本次不对具体成书年代作鉴定。
  dependence_on_other_sources: 与《史记》离越段有相似叙事，未证明独立。
  limitations: 只支持本节所述离越及去向不明，不支持后续经商、寿终的断言。
claims:
- claim_id: clm_01
  statement: 《史记》在灭吴后的叙事中写范蠡辞越；《国语》也载事成后辞别。
  claim_type: recorded_event
  source_refs:
  - src_shiji41
  - src_guoyu21
  source_locators:
  - 卷41范蠡节首段
  - 卷21末节
  support: supported
  historicity_confidence: medium
  confidence_reason: 已核对传世记载；非同时代独立记录，不能把文本一致等同于事件完全确证。
  exact_quote: null
  quote_checked: false
- claim_id: clm_02
  statement: 两书均以许诺分国和惩罚威胁叙述勾践挽留，范蠡仍决定离去。
  claim_type: attributed_speech
  source_refs:
  - src_shiji41
  - src_guoyu21
  source_locators:
  - 卷41辞别对话
  - 卷21末节辞别对话
  support: supported
  historicity_confidence: low
  confidence_reason: 传世文本有此叙述，但人物心理、话语与细节缺乏同时代独立核验。
  exact_quote: null
  quote_checked: false
- claim_id: clm_03
  statement: 《史记》记范蠡携珠玉与私属乘舟离去；《国语》记乘舟泛五湖，不明其最终去向。
  claim_type: recorded_event
  source_refs:
  - src_shiji41
  - src_guoyu21
  source_locators:
  - 卷41范蠡节离越段
  - 卷21末节乘舟段
  support: supported
  historicity_confidence: medium
  confidence_reason: 已核对传世记载；非同时代独立记录，不能把文本一致等同于事件完全确证。
  exact_quote: null
  quote_checked: false
- claim_id: clm_04
  statement: 《史记》另叙范蠡赴齐、迁陶、经营及老死于陶。
  claim_type: recorded_event
  source_refs:
  - src_shiji41
  source_locators:
  - 卷41范蠡节迁齐迁陶段及末段
  support: supported
  historicity_confidence: low
  confidence_reason: 传世文本有此叙述，但人物心理、话语与细节缺乏同时代独立核验。
  exact_quote: null
  quote_checked: false
- claim_id: clm_05
  statement: 《史记》把离越决定解释为范蠡担忧盛名难久与勾践难共安乐。
  claim_type: source_commentary
  source_refs:
  - src_shiji41
  source_locators:
  - 卷41范蠡节辞越前叙述
  support: supported
  historicity_confidence: low
  confidence_reason: 传世文本有此叙述，但人物心理、话语与细节缺乏同时代独立核验。
  exact_quote: null
  quote_checked: false
source_assessment:
  conflicts:
  - claim_refs:
    - clm_03
    - clm_04
    source_refs:
    - src_shiji41
    - src_shiji41_check
    - src_guoyu21
    disagreement: 《国语》止于去向不明；《史记》有迁齐、迁陶和晚年叙事。叙述详略及离开路线表述不同，不等于前者明确否认后者。两处《史记》在线录文财富数字亦不同。
    handling: 不合成唯一已证实行程，不使用精确财富数字；将后续经历明确归于《史记》，不作为退出机制已证实的依据。
  single_source_limit: 退出阶段虽有两部传世文本，来源独立性未证；携资与后续经历主要依赖《史记》。
  later_embellishments:
  - 本卡不采用未经此次核验的西施同行叙事。
situation:
  summary: 见 clm_01—clm_05。任务告一段落后，个人是否继续依附原权力关系成为新问题。
  claim_refs:
  - clm_01
  - clm_02
  - clm_05
  decision_maker: 范蠡
  affected_parties:
  - 范蠡
  - 随行者
  - 勾践
  desired_outcome_at_the_time: 按传世叙事：离开越国；自保为合理解释，不冒充本人可核验的完整目标。
  constraints:
  - 挽留叙事中存在惩罚威胁
  - 退出不是现代契约下的普通辞职
  information_available_then:
  - 记载中的辞别互动；其实际掌握的其他危险情报未知
  decision_problem: 面对挽留与威胁，是否离开，以及是否有实际离开的条件？
options_available:
- option: 留下
  availability_basis: 记载中的分国挽留
  claim_refs:
  - clm_02
  constraints:
  - 许诺能否兑现未知
  - 长期安全无从由此确定
- option: 离开
  availability_basis: 记载中实际采取的行动
  claim_refs:
  - clm_03
  constraints:
  - 有携资、随行与交通条件的记载
  - 不等于其他人也有这些条件
decision_taken:
  action: 采取离越行动。
  claim_refs:
  - clm_03
counterfactual_options: []
key_variables:
- variable_id: var_exit
  tag: exit_options
  historical_observation: 发生了实际离开的行动。
  claim_refs:
  - clm_03
  modern_equivalent: 能否执行退出而非只有退出意愿
  observable_indicator: 可行时间、履约安排、居所及接续方案
- variable_id: var_resources
  tag: resources
  historical_observation: 有携带资产与随行者的记载。
  claim_refs:
  - clm_03
  modern_equivalent: 可支配储备与可求助支持
  observable_indicator: 个人可支配资源及使用限制；不能将古代私属关系等同现代支持网络
- variable_id: var_power
  tag: power_balance
  historical_observation: 辞别叙事包含惩罚威胁。
  claim_refs:
  - clm_02
  modern_equivalent: 对方限制行动的实际能力
  observable_indicator: 真实发生的威胁、控制权限、有效保障与求助渠道
- variable_id: var_info
  tag: information_quality
  historical_observation: 动机和结局均由后世文本呈现。
  claim_refs:
  - clm_04
  - clm_05
  modern_equivalent: 现实担忧是否有可核查证据
  observable_indicator: 具体行为与记录，区分观察、传闻和猜测
outcomes:
- perspective: 范蠡
  criterion: 是否离开越国原任职关系
  horizon: 辞别与离去阶段
  observed_result: 传世叙事中的离去见 clm_03。
  claim_refs:
  - clm_03
  assessment: success
  uncertainty: 这是事件范围内的相对成功，不证明退出普遍安全。
- perspective: 范蠡及家属
  criterion: 长期安全与整体福祉
  horizon: 退出之后
  observed_result: 《史记》提供后续经历，《国语》不作同样说明。
  claim_refs:
  - clm_04
  assessment: ambiguous
  uncertainty: 不凭其中的富贵结局判定完整人生与所有家属的福祉。
overall_assessment:
  label: success
  rationale: 仅对“完成离越”这一限定目标评价；其他目标另列，不把成功扩展到全部人生。
causal_analysis:
  proposed_mechanisms:
  - mechanism: 可携资源与行动条件可能使退出意愿转为现实。
    variable_refs:
    - var_exit
    - var_resources
    supporting_claim_refs:
    - clm_03
    inference_strength: plausible_contribution
    inference_reason: 材料同段出现携资、随行、交通与离去，但没有隔离各因素的作用。
    competing_explanations:
    - 勾践的后续反应及执行条件可能影响结果；是否追索、是否曾尝试而未奏效，所核材料不足以确认，均只能作为待检验假说。
    - 叙事选择与后世塑造可能夸大主动规划的作用
    evidence_that_would_weaken_it:
    - 显示资产并非本人可用，或退出完全取决于另有保护的可靠材料
  selection_and_outcome_bias: 因后来离开而回推其事前必然聪明，是结果偏差；没有选择过退出却失败的同类总体资料。
  unresolved_factors:
  - 离越前准备程度
  - 挽留对话的真实性
  - 其他未记载的保护因素
  - 离去过程中是否实际遭到阻拦，以及离去后是否被追索；完成离越不能排除这些过程发生过。
warning_signs:
- signal: 挽留与惩罚威胁同时出现（记载中的话语）。
  available_to_actor_then: true
  claim_refs:
  - clm_02
transferable_mechanisms:
- mechanism: 将退出意愿与退出能力分开评估。
  conditions_required:
  - 当前关系确实产生需考虑退出的问题
  - 存在可合法、可安全实施的路径
  modern_evidence_needed:
  - 具体风险事实
  - 可支配资源
  - 替代安排与履约约束
  what_not_to_infer: 不能由范蠡离去断定用户应立即离职，或能力强的人不需要准备。
analogy_limits:
- historical_condition: 君主权力下的惩罚威胁
  modern_difference: 现代具体情境可能具有契约、申诉与外部保护机制，实际可用程度须查证。
  effect_on_recommendation: 优先核实实际约束与保障，不能把上级等同于君主。
- historical_condition: 史料记载范蠡具备可携资源
  modern_difference: 用户的经济与家庭约束可能完全不同。
  effect_on_recommendation: 需要准备过渡条件；不能只复制离开这一动作。
modern_problem_examples:
- 主要项目结束后，是否退出一个权力高度不对等的合作？
- 已决定离开，怎样核实自己是否具备行动条件？
comparison_ids:
- comparison_exit_response
missing_information:
- 无同时代独立记录与现代学术专题考证
- 未核纸本或影印版本
- 真实退出成本和完整时间线未知
decision_reconstruction:
  decision_stages:
  - stage: 阶段任务结束
    evidence: clm_01：灭吴后辞别
    interpretation: 任务完成可引出下一阶段选择，但并不使退出必然合理。
  - stage: 挽留与威胁
    evidence: clm_02：两书中的辞别对话
    interpretation: 留下的潜在收益与权力风险同时出现；对话真实性有限。
  - stage: 实际离越
    evidence: clm_03：携资、随行、乘舟的记载
    interpretation: 可描述动作和条件，不能补写全部准备过程。
  - stage: 后来生活
    evidence: clm_04：后续经历主要见《史记》
    interpretation: 后来经商不等于辞越前已制定创业计划。
  goal_hypotheses:
  - goal: 结束在越任职并避开不安的权力关系
    evidence_level: source_attribution
    basis: clm_05：史书赋予的判断；clm_01：辞别行为
    limit: 后世归属的心理不是独立核实的本人自述。
  - goal: 转向可自主安排的生活
    evidence_level: plausible_inference
    basis: 实际改变依附关系的动作
    limit: 不等于完全自由、追求隐居或当时已决定经商。
  - goal: 辞越前已经计划商业成功
    evidence_level: unknown
    basis: 只有后续经商叙述
    limit: 不得从后来结局倒推事前人生规划。
  option_tradeoffs:
  - option_id: opt_stay
    option: 接受挽留、继续任职
    availability: recorded_offer
    claim_refs:
    - clm_02
    basis: 记载中的分国许诺提供选项线索，不证明许诺可兑现。
    expected_benefits:
    - 若兑现，可能保留地位、政治影响和既有资源
    expected_costs:
    - 继续依赖同一权力关系
    - 伴随威胁的挽留可能压缩自主空间
    conditions:
    - 承诺可信且能兑现
    - 本人仍愿意承担相应责任
    possible_reactions:
    - 可能强化合作，也可能延续疑忌；均不确定
    future_options: 保留政治路径，但可能提高以后退出成本。
    uncertainty: 不能由离去后的结局证明留下必死。
  - option_id: opt_partial
    option: 暂时退居或减少参与
    availability: counterfactual
    claim_refs: []
    basis: 分析提出的中间方案；未核到范蠡当时采用或获准的证据。
    expected_benefits:
    - 若被允许，可能留出考虑时间并保留关系
    expected_costs:
    - 可能不改变依附与风险
    - 角色模糊可能招致不同解释
    conditions:
    - 能减轻职责且边界被接受
    possible_reactions:
    - 可能被理解为休息、退让或拒绝；无法确知
    future_options: 可能保留转向余地，也可能拖延必要改变。
    uncertainty: 不是证明范蠡有过此备选，更不是文种与范蠡具有相同选项。
  - option_id: opt_leave
    option: 离越并重新安置生活
    availability: recorded_action
    claim_refs:
    - clm_03
    basis: 有实际动作与部分物质条件的记载。
    expected_benefits:
    - 若能完成且不被追究，可能摆脱部分原有依附
    expected_costs:
    - 放弃或改变既有角色与关系
    - 迁移、生计以及可能追究的不确定性
    conditions:
    - 交通、可携资源及随行安排
    - 离开后能建立可持续生活
    possible_reactions:
    - 记载有挽留威胁并记离去；是否发生实际阻拦或后续追索、如何应对，所核材料未详。
    future_options: 可能打开新生活路径；后续经商并非唯一可能方向。
    uncertainty: 成功离去不证明所有准备、保护与动机都已被记录。
  motive_hypotheses:
  - hypothesis_id: hyp_safety
    question: 为什么不接受更高的地位或赏赐？
    explanation: 依《史记》赋予的动机，可能认为留下的不安超过了许诺的吸引力。
    evidence_level: source_attribution
    claim_refs:
    - clm_02
    - clm_05
    support: 这是史书提供的解释，而非只由结果猜测。
    alternatives:
    - 其他未被记载的关系与个人目标也可能影响选择
    what_is_missing: 他如何估计风险、重视哪些目标、是否相信许诺，缺少直接记录。
  - hypothesis_id: hyp_action
    question: 为什么选择实际离开而不是仅减少参与？
    explanation: 可能希望改变依附结构，而不仅改变日常参与程度。
    evidence_level: plausible_inference
    claim_refs:
    - clm_03
    support: 实际行动改变了所在环境；其主观设计仍是推断。
    alternatives:
    - 可能有其他个人或家庭考虑
    - 叙事可能简化了多阶段过程
    what_is_missing: 没有完整备选方案清单与决策过程。
  implementation:
    recorded_steps:
    - clm_01、clm_02：辞别及互动
    - clm_03：携资、与私属乘舟离去
    necessary_questions:
    - 何时准备交通与资产？
    - 谁参与安排，是否受到阻拦？
    - 离开后靠什么安置并持续生活？
    unknown_procedures:
    - 没有可靠的完整操作清单
    - 资产数量、来源、随行者具体职责与路线不明
    do_not_invent: 不能把几句叙事扩展成秘密撤离攻略；现代行动应依据当下合法责任与真实条件。
  choice_explanation:
    best_supported: 文本提供了离越动作及其赋予的忧虑解释；可分析收益与代价，但不能重建精确的主观权重。
    confidence: 部分行动可追溯，意图和每个条件的因果贡献更不确定。
    counterfactual_limit: 留下、部分退出或离开是否更好，取决于未完全掌握的目标与约束。
  life_course:
    short_term: 离开改变角色、关系与环境，并伴随迁移和生计不确定性；具体体验未明。
    medium_term: 《史记》叙述迁齐、迁陶与经营，《国语》没有相同完整轨迹。
    long_term: 后世成功叙事不能证明其生活始终安稳，也不能保证模仿者会成功。
    values_limit: 不能把范蠡固定塑造成喜欢安稳的人或天生创业者；后来的经历不能替他确认事前目标。
    modern_bridge: 用此例区分完成旧目标、想要的新阶段与可实施的过渡，不把离职本身当作人生目标。
```
