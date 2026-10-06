# 文种称病不朝：减少参与未能避免政治迫害

## 目录

- 案例定位
- 决策分析速览
- 结构化案例卡

## 案例定位

v0.2：核对《史记》与较晚《吴越春秋》，新增动机假说、四条路径的取舍及实施边界；后者不作为独立心理实录。

## 决策分析速览

下表是条件分析，潜在收益与代价不等于已经发生的事实。完整理由、证据等级与未知见 decision_reconstruction。

| 路径 | 证据地位 | 潜在收益 | 潜在代价 |
|---|---|---|---|
| 继续上朝并参与政务 | analytical_alternative | 如果仍能有效参与，可保持信息渠道、履职与表达机会 | 若危险来自君主猜忌，直接接触和持续权力地位可能增加暴露 |
| 称病不朝 | recorded_action | 若对方接受疾病理由，可减少当面参与而不直接声明政治决裂 | 减少接触也可能减少信息和澄清机会 |
| 明确请求辞官或减轻职责 | counterfactual | 若被接受，可使角色边界比单纯缺席更明确 | 可能被拒绝或被理解为不满、疏离 |
| 离越，在别处重建生活 | counterfactual | 若可安全实施，可能比留在当地更大程度改变依附关系 | 可能有迁移、家庭安排、生计和追究风险 |

## 结构化案例卡

```yaml
schema_version: '0.2'
case_id: case_wenzhong_withdrawal
title: 文种称病不朝：减少参与未能避免政治迫害
status: reviewed
review:
  reviewed_by: Codex：在线文本与结构审阅，非历史学专家鉴定
  reviewed_at: '2026-09-28'
  notes: v0.2：核对《史记》与较晚《吴越春秋》，新增动机假说、四条路径的取舍及实施边界；后者不作为独立心理实录。
scope:
  period: 春秋末
  date_range: 越灭吴后、勾践去世前；具体年份不作断定
  date_precision: approximate
  event_boundary: 范蠡致书劝离至文种称病不朝并最终遭赐剑
  people:
  - 文种（所核段落称大夫种）
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
  - power_balance
  - information_quality
  - downside
  classification_note: 用于区分减少参与与实际降低风险；不能据此诊断用户的处境。
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
- source_id: src_wuyue10
  work_title: 吴越春秋
  author_or_compiler: 赵晔（东汉，作品目录署名）
  source_type: later_compilation
  chapter_or_volume: 勾践伐吴外传第十
  edition_or_translator: 维基文库在线录文；未核影印底本
  locator: 范蠡既去之后的内忧不朝段；勾践二十五年段
  url: https://zh.wikisource.org/zh-hans/吳越春秋/勾踐伐吳外傳
  accessed_on: '2026-09-28'
  verification: checked
  temporal_relation: 晚于西汉《史记》的传世叙述，非文种同期记录。
  dependence_on_other_sources: 与《史记》等的具体材料关系本次未考定，不计为独立心理证据。
  limitations: 正文混有术数解释和死后化潮等叙事；只记录其如何讲述事件，不将相关对话或心理直接当实录。
claims:
- claim_id: clm_01
  statement: 《史记》记范蠡离越后致书劝大夫种离去。
  claim_type: attributed_speech
  source_refs:
  - src_shiji41
  - src_shiji41_check
  source_locators:
  - 卷41越王句践节末，范蠡遂去段
  support: supported
  historicity_confidence: low
  confidence_reason: 传世文本有此叙述，但人物心理、话语与细节缺乏同时代独立核验。
  exact_quote: null
  quote_checked: false
- claim_id: clm_02
  statement: 该段记大夫种见信后称病不朝。
  claim_type: recorded_event
  source_refs:
  - src_shiji41
  - src_shiji41_check
  source_locators:
  - 卷41种见书之后
  support: supported
  historicity_confidence: medium
  confidence_reason: 已核对传世记载；非同时代独立记录，不能把文本一致等同于事件完全确证。
  exact_quote: null
  quote_checked: false
- claim_id: clm_03
  statement: 该段继而记有人谗称大夫种将作乱。
  claim_type: recorded_event
  source_refs:
  - src_shiji41
  - src_shiji41_check
  source_locators:
  - 卷41称病不朝之后
  support: supported
  historicity_confidence: medium
  confidence_reason: 已核对传世记载；非同时代独立记录，不能把文本一致等同于事件完全确证。
  exact_quote: null
  quote_checked: false
- claim_id: clm_04
  statement: 该段记勾践赐剑，大夫种随后自杀。
  claim_type: recorded_event
  source_refs:
  - src_shiji41
  - src_shiji41_check
  source_locators:
  - 卷41越王乃赐种剑至种遂自杀
  support: supported
  historicity_confidence: medium
  confidence_reason: 已核对传世记载；非同时代独立记录，不能把文本一致等同于事件完全确证。
  exact_quote: null
  quote_checked: false
- claim_id: clm_05
  statement: 《史记》在早先复国叙事中记勾践将国政交给大夫种。
  claim_type: recorded_event
  source_refs:
  - src_shiji41
  source_locators:
  - 卷41吴既赦越之后，举国政属大夫种段
  support: supported
  historicity_confidence: medium
  confidence_reason: 已核对传世记载，不能据此恢复某一时刻全部职责。
  exact_quote: null
  quote_checked: false
- claim_id: clm_06
  statement: 《吴越春秋》以大夫种内忧不朝描写其状态。
  claim_type: source_commentary
  source_refs:
  - src_wuyue10
  source_locators:
  - 范蠡既去之后的内忧不朝段
  support: supported
  historicity_confidence: low
  confidence_reason: 文本可核对，但较晚材料中的心理、指控和对话不能当独立事实；也不据篇幅丰富提升可信度。
  exact_quote: null
  quote_checked: false
- claim_id: clm_07
  statement: 《吴越春秋》叙述有人把缺席归因于未获增官加封而心怀怨望；这是谗者的说法。
  claim_type: attributed_speech
  source_refs:
  - src_wuyue10
  source_locators:
  - 内忧不朝之后的谗言段
  support: supported
  historicity_confidence: low
  confidence_reason: 文本可核对，但较晚材料中的心理、指控和对话不能当独立事实；也不据篇幅丰富提升可信度。
  exact_quote: null
  quote_checked: false
- claim_id: clm_08
  statement: 《吴越春秋》在缺席段后仍写文种向勾践进言及受召的对话。
  claim_type: recorded_event
  source_refs:
  - src_wuyue10
  source_locators:
  - 异日种谏及勾践二十五年召相国段
  support: supported
  historicity_confidence: low
  confidence_reason: 文本可核对，但较晚材料中的心理、指控和对话不能当独立事实；也不据篇幅丰富提升可信度。
  exact_quote: null
  quote_checked: false
source_assessment:
  conflicts:
  - claim_refs:
    - clm_02
    - clm_06
    - clm_07
    - clm_08
    source_refs:
    - src_shiji41
    - src_wuyue10
    disagreement: 《史记》简记称病不朝；《吴越春秋》补叙内忧、怨望指控与后续对话。属于不同叙事层次，不能无缝合并为完整心理与行动实录。
    handling: 逐书归属；内忧是后世解释，怨望是被记载的指控；不能判定真病、装病、永久缺席或完整退出程序。
  single_source_limit: 核心行动主要依据《史记》；新增《吴越春秋》补充叙事角度，材料独立性未证。其较详细的心理与对话不能消除动机不确定性。
  later_embellishments:
  - 所核段落不证明文种贪恋权位。
  - 史书记录的谗言不能改写成已证实的谋反。
  - 从收到劝告到称病的叙事顺序，不能证明其全部心理与计划。
situation:
  summary: 见 clm_01—clm_04。对风险警告有所行动，却仍受到君主的致命处置。
  claim_refs:
  - clm_01
  - clm_02
  - clm_03
  - clm_04
  decision_maker: 大夫种（文种）；最终惩罚由勾践施加
  affected_parties:
  - 文种
  - 勾践
  desired_outcome_at_the_time: 具体目标未知；称病可能意在避祸，但不能当作已证实心理。
  constraints:
  - 没有可确认的离境条件记录
  - 是否有有效申辩或保护渠道未知
  information_available_then:
  - 书中叙述其收到劝离信
  - 是否预先知道谗言及后续处置未知
  decision_problem: 面对劝离警告采取何种响应；所核记载不能重建他的完整可选方案。
options_available:
- option: 称病不朝
  availability_basis: 史料记载的实际行动
  claim_refs:
  - clm_02
  constraints:
  - 不等于已经离境或解除君主控制
decision_taken:
  action: 称病不朝；不能擅自改写为毫无行动或已完成正式辞官。
  claim_refs:
  - clm_02
counterfactual_options:
- option: 像范蠡一样离越
  feasibility_assumptions:
  - 有交通与可支配资源
  - 存在允许离开的时间与条件
  - 能够处理随行家属等约束
  uncertainty: 范蠡曾离开不证明文种同样能离开，更不证明离开一定安全。
key_variables:
- variable_id: var_exit
  tag: exit_options
  historical_observation: 记载中的响应为称病不朝，非记载已完成的离越。
  claim_refs:
  - clm_02
  modern_equivalent: 减少工作参与是否真正解除责任和风险
  observable_indicator: 权限、责任、交接与退出安排是否实际改变
- variable_id: var_power
  tag: power_balance
  historical_observation: 君主仍能施加致命处置。
  claim_refs:
  - clm_04
  modern_equivalent: 他方实际能够施加的后果与外部制约
  observable_indicator: 可核实的处罚权限、程序、申诉与外部帮助
- variable_id: var_info
  tag: information_quality
  historical_observation: 警告与谗言分属不同信息，其真实性和可得性不能混同。
  claim_refs:
  - clm_01
  - clm_03
  modern_equivalent: 风险信号与猜测的区分
  observable_indicator: 信息来源、可验证行为及当事人能否及时知道
- variable_id: var_downside
  tag: downside
  historical_observation: 叙事结果是死亡，代价不可逆。
  claim_refs:
  - clm_04
  modern_equivalent: 现实中最严重且可信的不利后果
  observable_indicator: 损失性质、承担者、可逆性；不能拿历史死亡直接放大现代小冲突
outcomes:
- perspective: 文种
  criterion: 个人生命安全
  horizon: 收到警告至赐剑后的阶段
  observed_result: 见 clm_04。
  claim_refs:
  - clm_04
  assessment: failure
  uncertainty: 仅指安全结果失败，不判定其道德、能力或全部人生失败。
overall_assessment:
  label: failure
  rationale: 只评价此阶段个人安全结果；不意味着称病导致死亡，或受迫害者应为迫害负责。
causal_analysis:
  proposed_mechanisms:
  - mechanism: 减少参与并不一定消除对方施加伤害的能力。
    variable_refs:
    - var_exit
    - var_power
    supporting_claim_refs:
    - clm_02
    - clm_04
    inference_strength: plausible_contribution
    inference_reason: 结果说明称病未充分保护他；不能据此确定称病是否增加或减少了风险。
    competing_explanations:
    - 谗言及勾践的决定可能独立于称病行动
    - 未被记载的政治纠葛可能改变结局
    - 文本组织可能服务于功成退隐的叙事主题
    evidence_that_would_weaken_it:
    - 可信材料显示他已获得有效外部保护，死亡源于另一独立事件
    - 证据显示现有情节的时序或身份有实质错误
  selection_and_outcome_bias: 不得把范蠡和文种当作随机分配退出与留下的实验；二人资源与可行选项未知。避免用遇害结果倒推其贪婪或愚蠢。
  unresolved_factors:
  - 称病的具体目的
  - 离境机会与可行性
  - 谗言是谁提出及其背景
  - 各环节间隔多久
warning_signs:
- signal: 收到劝离信（按《史记》叙述）。
  available_to_actor_then: true
  claim_refs:
  - clm_01
- signal: 有人以作乱相谗；文种当时能否知道未知。
  available_to_actor_then: null
  claim_refs:
  - clm_03
transferable_mechanisms:
- mechanism: 检查风险来源是否因减少参与而真实改变，而非只检查自己是否减少露面。
  conditions_required:
  - 确有可核验的现实风险
  - 减少参与与风险暴露之间存在可分析的关系
  modern_evidence_needed:
  - 仍承担的责任
  - 实际控制权
  - 退出与求助渠道
  what_not_to_infer: 不能推出请假或低调必然危险、应立即辞职，或受害是自身不够聪明造成的。
analogy_limits:
- historical_condition: 君主赐剑的政治暴力
  modern_difference: 普通工作冲突通常不具有相同的权力性质与后果；具体法律及保障须另行核对。
  effect_on_recommendation: 不能把同事争功或领导不满等同生命威胁。
- historical_condition: 所核记载缺少文种可选行动的详细信息
  modern_difference: 现实咨询可追问资源、约束与选择。
  effect_on_recommendation: 先补齐关键现实信息，不用历史人物结局替用户决定。
modern_problem_examples:
- 我已经减少参与一个有风险的合作，但仍承担责任，应该核查什么？
- 收到退出建议后，怎样判断警告是否可信且退出是否可行？
comparison_ids:
- comparison_exit_response
missing_information:
- 称病是否出于避祸的心理证据不足
- 不能由材料缺载断定从未尝试其他退出行动
- 已读较晚材料但未完成独立史源考证；病情、正式许可与缺席持续时间未知。
decision_reconstruction:
  decision_stages:
  - stage: 风险提示
    evidence: clm_01：史书记述收到范蠡劝离；不是自动证明书信原貌。
    interpretation: 可能改变他对继续任职的预期，但无法测量他信了多少。
  - stage: 行动
    evidence: clm_02：以疾病为由不朝；clm_06：较晚叙事用内忧解释。
    interpretation: 行动形态有据；动机与制度细节没有同等证据。
  - stage: 他人解释
    evidence: clm_03、clm_07：出现针对他的指控。
    interpretation: 缺席可能被赋予政治意义；不能认定缺席制造了指控。
  - stage: 结果
    evidence: clm_04：赐剑与死亡的记载。
    interpretation: 结果不可逆，但不能因此认定他当时有更优且可行的安全选项。
  goal_hypotheses:
  - goal: 避免政治危险、暂缓直接接触
    evidence_level: plausible_inference
    basis: clm_01、clm_02 的先后及 clm_06 的较晚解释
    limit: 可作为较贴合文本的解释，但不是文种亲自陈述并独立核实的目标。
  - goal: 同时保留身份、影响力或以后调整的空间
    evidence_level: speculative
    basis: 行动未等于已完成辞官或离境
    limit: 保留身份可能来自约束，也可能出于计划；不能据此称其贪恋权位。
  - goal: 因身体或情绪负担暂时无法履职
    evidence_level: unknown
    basis: 称病不提供诊断；内忧也不是医学记录
    limit: 无法断定真病或装病，更不能追认具体精神疾病。
  option_tradeoffs:
  - option_id: opt_attend
    option: 继续上朝并参与政务
    availability: analytical_alternative
    claim_refs:
    - clm_05
    basis: 曾任国政职务提供背景，但警告发生时恢复或持续参与是否可行未知。
    expected_benefits:
    - 如果仍能有效参与，可保持信息渠道、履职与表达机会
    - 可能有机会澄清立场、维持已有政治关系
    expected_costs:
    - 若危险来自君主猜忌，直接接触和持续权力地位可能增加暴露
    - 履职会继续消耗精力，也可能延续自己不愿承担的责任
    conditions:
    - 仍获准参与且有表达空间
    - 履职机会实际有益而非单纯受控
    possible_reactions:
    - 可能被理解为继续忠诚，也可能被理解为不愿放权；两种均属假设
    future_options: 可能保留在朝行动空间，也可能进一步绑定原关系。
    uncertainty: 没有材料证明上朝会比不上朝安全，也不知文种是否认真考虑此项。
  - option_id: opt_illness
    option: 称病不朝
    availability: recorded_action
    claim_refs:
    - clm_02
    basis: 史料明确记录这一行动形态，真实病情与批准过程未明。
    expected_benefits:
    - 若对方接受疾病理由，可减少当面参与而不直接声明政治决裂
    - 可能取得喘息或观察时间；这些收益并未在史料中被验证
    expected_costs:
    - 减少接触也可能减少信息和澄清机会
    - 不自动撤销既有身份、责任和他人处置能力
    - 理由可能被他人重新解释为不满或回避
    conditions:
    - 事实上能够缺席
    - 理由是否被接受、持续多久、再被召见如何处理均未知
    possible_reactions:
    - clm_07 中有人将缺席解释为怨望；这只是被记录的指控，不是客观动机
    future_options: 可能保留返回的余地，却未必形成新的独立生活路径。
    uncertainty: 不能证明他以此设计了长期退出计划，也不能断言该策略完全无效或导致死亡。
  - option_id: opt_resign
    option: 明确请求辞官或减轻职责
    availability: counterfactual
    claim_refs: []
    basis: 现代分析提出的替代方案，未核到文种当时采用或可获批准的记录。
    expected_benefits:
    - 若被接受，可使角色边界比单纯缺席更明确
    expected_costs:
    - 可能被拒绝或被理解为不满、疏离
    - 即使解除职务，也未必脱离人身控制
    conditions:
    - 能提出请求
    - 对方愿意接受且实施安排有效
    possible_reactions:
    - 可能理解为退让，也可能视作拒绝继续效力；不确定
    future_options: 可能开启不任职生活，也可能失去表达渠道而仍受原权力约束。
    uncertainty: 无法把现代自愿离职制度套入，也不能假称只差一封辞呈。
  - option_id: opt_depart
    option: 离越，在别处重建生活
    availability: counterfactual
    claim_refs: []
    basis: 范蠡的记载仅证明范蠡曾这样做，不证明文种可复制。
    expected_benefits:
    - 若可安全实施，可能比留在当地更大程度改变依附关系
    expected_costs:
    - 可能有迁移、家庭安排、生计和追究风险
    - 原有身份、关系与事业可能中断
    conditions:
    - 交通、资源、目的地、时机与同行安排
    - 对方追索能力及外部接纳条件
    possible_reactions:
    - 可能被允许、忽略或阻拦；没有材料确定
    future_options: 可能打开新路径，也可能因失去支持使选择更少。
    uncertainty: 离开不是保证生存的处方；不能凭失败结局责怪未离开者。
  motive_hypotheses:
  - hypothesis_id: hyp_avoid
    question: 为什么不想上朝？
    explanation: 收到警告后，可能希望减少与危险来源的接触，或暂时降低参与程度。
    evidence_level: plausible_inference
    claim_refs:
    - clm_01
    - clm_02
    - clm_06
    support: 与记载顺序及较晚文本的忧惧解释相容。
    alternatives:
    - 真实患病或身心负担
    - 尚在犹豫或受限而未能采取其他行动
    what_is_missing: 没有同时代私人记录，不能确知权衡过程。
  - hypothesis_id: hyp_reason
    question: 为什么选择称病，而不是直接说不愿继续任职？
    explanation: 从交流机制推测，疾病理由可能把缺席解释为无法履职，减少直接评价君主或公开决裂的意味。
    evidence_level: speculative
    claim_refs:
    - clm_02
    support: 这是针对该理由可能发挥作用的现代解释，史书没有解释为何偏偏选它。
    alternatives:
    - 确有病情
    - 这只是史家概括行动的用语，未保留其他沟通
    - 可能还采取过未被记录的动作
    what_is_missing: 不知道他是否比较过其他理由，也不知道当时的认可规则、沟通方式或长期计划。
  - hypothesis_id: hyp_hold
    question: 为什么没有立即离越？
    explanation: 可能是成本、约束、目标冲突或对风险的不同判断；目前无法在这些解释中作可靠选择。
    evidence_level: unknown
    claim_refs: []
    support: 所核材料没有充分描述文种的退出资源与选择过程。
    alternatives:
    - 没有安全离境机会
    - 仍重视未完成的责任
    - 判断短期缺席已经足够
    - 并未形成完整计划
    what_is_missing: 各假说均需新增证据；不能以材料沉默证明某一种。
  implementation:
    recorded_steps:
    - clm_02：称病不朝这一行动被记载
    necessary_questions:
    - 谁向谁传达缺席理由？
    - 是否获准，或只是发生了缺席？
    - 持续多久，是否仍处理政务？
    - 有无交接、代办、再次召见的安排？
    unknown_procedures:
    - 不能确认书面申请、使者、医者证明或固定病假规则
    - 不能确定是否完全不上朝或从此停止全部政治接触；clm_08 的较晚叙事还写到此后对话
    do_not_invent: 称病不朝不是现代请病假制度的同义词；不补造流程，也不把叙事当成现代装病的操作指南。
  choice_explanation:
    best_supported: 能确定的是文本所记行动，较贴合材料的动机解释是忧虑或避险；为何最终排除其他选项仍不能确定。
    confidence: 对行动记载的把握高于对动机、效果与制度的把握。
    counterfactual_limit: 只能说不同假设下各选项有何取舍，不能声称算出了文种当时的最优策略。
  life_course:
    short_term: 称病可能改变参与节奏，但是否得到休息、改善安全或保留影响力均未被直接证实。
    medium_term: 继续保有何种身份、关系与生计依赖不详；留在原环境并不自动决定最终命运。
    long_term: 所载死亡终结了后续机会；这是结果，不是证明所有留下者命运相同。
    values_limit: 不能把现代安稳生活、创业或收入目标投射给文种。
    modern_bridge: 先了解现实用户想获得哪一种下一阶段，再比较减少参与、调整关系与真正退出分别会带来怎样的生活和责任。
```
