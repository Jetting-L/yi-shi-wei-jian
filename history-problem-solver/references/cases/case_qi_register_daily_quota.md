# HC-014｜南齐检籍：核验责任、查错日额与纠偏诏

## 案例定位

候选编号 HC-014；稳定 ID 为 `case_qi_register_daily_quota`。本卡按 Astra 2026-10-01 模板证据审阅于 2026-10-06 有限登记为 reviewed；保留 U-014 及原证据限制。边界从建元二年诏议及虞玩之检籍表，到太祖采表后另加日额、传文所叙强退，再到世祖永明八年纠偏诏；跨两帝，不概括南齐全部户籍史。

本轮实际回读《南齐书》卷三十四 L5101–5117，完整读取检籍表和 L5113 的安排、后果、纠偏。L5105 是此前财库表，不作检籍核心出处。见 [建元二年诏议](../../source-md/7.南齐书.md:5109)、[检籍表](../../source-md/7.南齐书.md:5111)、[日额与纠偏](../../source-md/7.南齐书.md:5113)。所核为本地转录，底本与诏表原件未确认。

## 决策分析速览

| 路径 | 证据地位 | 预期收益 | 主要代价／缺口 |
|---|---|---|---|
| 按虞表落实县审、上州、虚昧同咎及首悔 | recorded_offer | 可能减少推诿、使审核责任明确 | 同含严刑和募役要求；纯提案的独立效果未知 |
| 采表后另设板籍官并加每日查错额 | recorded_action | 文本归属意图是防懈怠 | 传文记正籍强退充限；不知统一日额数和错误比例 |
| 将核验质量与纠错成本纳入独立复核 | counterfactual | 若可行，可减少为额度制造问题 | 需记录、复核资源和申诉渠道；原文未记此制度 |

纠偏诏是永明八年的另一个决策阶段，不是建元二年已知的结果或选项。

## 结构化案例卡

```yaml
schema_version: "0.2"
case_id: case_qi_register_daily_quota
title: 南齐检籍：核验责任、查错日额与纠偏诏
status: reviewed
review:
  reviewed_by: "Astra 模板证据审阅；docs/history_case_batch_a_astra_recheck_20261001.md"
  reviewed_at: 2026-10-01
  notes: "HC-014；2026-10-01 Astra 通过模板证据审阅，保留 U-014；2026-10-06 有限本地登记，本次登记差异待收尾复核。仅指所列本地材料支持相应层级，非独立史实、现代因果或执行效果确证；原核读日期、核心事实与未知不变。"
scope:
  period: 南朝齐太祖、世祖时
  date_range: 建元二年诏议至永明八年纠偏；宋代弊端与齐初检定为前史
  date_precision: approximate
  event_boundary: 二年诏议与虞表、太祖采表另加查错日额、传文叙强退，至世祖颁复注与许还本诏
  people: [虞玩之, 齐太祖萧道成, 齐世祖萧赜, 傅坚意]
  organizations: [南齐朝廷, 州县, 板籍官及令史, 边疆戍役单位]
classification:
  primary_category: organization_people
  secondary_categories: [risk_uncertainty]
  tags: [incentives, accountability, information_quality, feedback_speed, downside]
  classification_note: 核心是审核目标被查错产量替代与跨帝纠偏；不能据一传推导全国行政因果。
sources:
  - source_id: src_nanqi34
    work_title: 南齐书
    author_or_compiler: 萧子显
    source_type: later_compilation
    chapter_or_volume: 卷三十四·列传第十五（虞玩之传）
    edition_or_translator: 用户本地 Markdown 转录；未在本轮核对应 DOCX、纸本或影印底本，具体版次未确认
    locator: source-md/7.南齐书.md:L5101–5117；核心 L5109–5113，从建元二年诏至世祖纠偏诏
    url: null
    accessed_on: "2026-10-01"
    verification: checked
    temporal_relation: 梁代编纂前朝齐事，距事件数十年；书中保存的表诏不是本轮取得的原件。
    dependence_on_other_sources: 单传内的诏、表及叙述属于同一材料组，未获独立执行评价或个案档案。
    limitations: 传记叙事可能压缩时间；户数来自虞表，日额后果与纠偏执行无独立量化记录。
claims:
  - claim_id: clm_01
    statement: 传文先记太祖即位后命虞玩之、傅坚意检定簿籍，再记建元二年诏问欺巧、刑德取舍与募役不足；不是二年才第一次开始检籍。
    claim_type: recorded_event
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5109｜及即位", "source-md/7.南齐书.md:L5109｜建元二年"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 前史与诏议可在同段区分，命令原件和起始细节未核。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_02
    statement: 虞表称泰始三年至元徽四年扬州等九郡四号黄籍共却七万一千余户，所正不足四万，并说于今十一年；不能视为全国户数、去重人口数或准确率。
    claim_type: attributed_speech
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5111｜共却七万一千余户"]
    support: supported
    historicity_confidence: low
    confidence_reason: 有明确范围的上表统计，原籍及计算口径未核；十一年不擅改成唯一精确累计期间。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_03
    statement: 虞表批评县不检合即送州、贿赂和退答拖延，提议县官先审、然后上州，虚昧州县同咎，一听首悔；也主张迷而不反依制必戮及落实募役。
    claim_type: attributed_speech
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5111｜使官长审自检校", "source-md/7.南齐书.md:L5111｜依制必戮"]
    support: supported
    historicity_confidence: low
    confidence_reason: 核到完整上表而非现代温和审计摘要；贿赂程度、责任制度的实效与原话未独立核实。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_04
    statement: 传文记太祖采纳虞表后另置板籍官、令史，并要求每人每日查得数巧；日额不是虞表所列提案，所核段未给统一确切数。
    claim_type: recorded_event
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5113｜限人一日得数巧"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 安排及主体在采表后的传文明确，具体命令、日额数量与覆盖范围未核。
    exact_quote: "限人一日得数巧"
    quote_checked: true
  - claim_id: clm_05
    statement: 同段记货赂因缘、籍注虽正仍强推却，以充程限；这里有正籍被强退的行为记载，不能概称所有退籍或谪戍都是冤案。
    claim_type: recorded_event
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5113｜籍注虽正"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 单传叙事明确记行为，未获具体名册、案件样本及频率数据。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_06
    statement: 传文把加日额的用意说成防懈怠，把强退与充程限相联系；是史书所呈的意图及因果解释，不是已经隔离旧贿赂等因素的效果研究。
    claim_type: source_commentary
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5113｜以防懈怠", "source-md/7.南齐书.md:L5113｜以充程限"]
    support: supported
    historicity_confidence: low
    confidence_reason: 文字关联清楚，但解释来自同一叙述者，无独立个案比较。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_07
    statement: 世祖永明八年诏以既往之愆不足追咎为理由，允许宋升明以前复注、谪役边疆者各还本，此后有犯仍严治；是跨帝且有时间界限的纠偏诏令。
    claim_type: attributed_speech
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5113｜至世祖永明八年", "source-md/7.南齐书.md:L5113｜自宋升明以前"]
    support: supported
    historicity_confidence: low
    confidence_reason: 本传保存诏令口径，原件与逐人施行未知；不能把有界限的旧案处理写成取消未来处罚。
    exact_quote: "各许还本"
    quote_checked: true
  - claim_id: clm_08
    statement: 传文记世祖颁纠偏诏；所核段落未记复注及返乡的完成名单、比例或日期，不能从许还推定全部实际返乡。
    claim_type: recorded_event
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5113｜世祖乃诏曰"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 颁诏有记载，执行效果属材料缺口而非被证实的否定。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_09
    statement: 至永明八年，传文叙谪巧者戍缘淮各十年；十年是所叙戍役期限，不是所有人此前都已服满十年，也不证每个戍者被错判。
    claim_type: recorded_event
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5113｜谪巧者戍缘淮各十年"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 处罚范围与期限有单传记载，缺逐案判处及实际服役记录。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_10
    statement: 作者以百姓怨望描述纠偏前的社会反应，接叙世祖颁诏；这不是独立投诉统计，也不足隔离民怨与纠偏的全部原因。
    claim_type: source_commentary
    source_refs: [src_nanqi34]
    source_locators: ["source-md/7.南齐书.md:L5113｜百姓怨望"]
    support: supported
    historicity_confidence: low
    confidence_reason: 社会心态与叙事关联由传记概括，投诉人数、报告渠道及政治原因未核。
    exact_quote: null
    quote_checked: false
source_assessment:
  conflicts: []
  single_source_limit: 核心来自虞玩之同一传。诏、表与史家后果叙述应分内容类型，不能计三份独立评价；无全国户籍审计或返乡执行册。
  later_embellishments: [不将查错日额归给虞玩之上表, 不将旧籍户数作全国准确率, 不写所有冤案由日额造成或纠偏后全已修复]
situation:
  summary: 朝廷希望处理簿籍欺巧和役源问题；虞表提出核验责任，太祖采表后另加每日查错要求，传文叙强退及民怨，世祖后来颁纠偏诏。
  claim_refs: [clm_01, clm_03, clm_04, clm_05, clm_07, clm_08, clm_09, clm_10]
  decision_maker: 太祖决定采表与日额安排；虞玩之提案；世祖作永明八年纠偏决定
  affected_parties: [编户及家属, 州县官吏, 板籍官和令史, 谪戍者, 征役机关]
  desired_outcome_at_the_time: 诏表表达求实籍、治欺巧及供役目标；后来的纠偏也保留身份区分和严治，不能改作现代权利改革。
  constraints: [既有贿赂与县州推诿, 募役不足与身份利益, 皇权下严刑和谪戍, 缺独立质量统计]
  information_available_then: [太祖可听虞表关于旧籍与推诿的报告，但非已核实全国事实, 日额的防懈怠意图由传文归属, 后来强退和民怨不能当作二年已知政策后果, 永明八年世祖面对的民怨程度仅有传记概括]
  decision_problem: 如何使检籍得到真实校正并落实责任，数量要求会否改变执行者行为；发现后果后如何限定纠偏？
options_available:
  - option: 建元二年按虞表核验责任与首悔提案治理
    availability_basis: 实际上表；独立于后来另加日额的原提案
    claim_refs: [clm_03]
    constraints: [含严刑及役法, 州县实际复核能力未知]
  - option: 太祖采表后另设板籍官和每日查错额
    availability_basis: 实际安排，不是原表同义转述
    claim_refs: [clm_04, clm_06]
    constraints: [不知确切额度, 可产生凑额与贿赂激励]
  - option: 永明八年颁有年代界限的复注与还本诏
    availability_basis: 世祖实际颁诏；属后一个信息阶段
    claim_refs: [clm_07, clm_08]
    constraints: [执行未知, 不取消未来处罚, 不足证明每个案件都错]
decision_taken:
  action: 太祖采纳虞表并另加日额，传文叙强退；世祖于永明八年颁旧案复注和谪役者许还本诏。
  claim_refs: [clm_04, clm_05, clm_07, clm_08]
counterfactual_options:
  - option: 以独立抽核、纠正记录及受影响者成本检验审核质量
    feasibility_assumptions: [可保留原籍与退籍理由, 有不受查错额度约束的复核者, 有可安全使用的申诉渠道]
    uncertainty: 属现代分析备选，所核原文未记这些程序，当时可行性未知。
key_variables:
  - variable_id: var_quota
    tag: incentives
    historical_observation: 日额要求与正籍强退充限被传文相连。
    claim_refs: [clm_04, clm_05, clm_06]
    modern_equivalent: 发现数量是否成为奖惩条件，影响真实核验
    observable_indicator: 查错额度与绩效规则、误退复核率、临近考核时的异常分布
  - variable_id: var_responsibility
    tag: accountability
    historical_observation: 虞表欲县审上州、虚昧同咎；后又增板籍官与令史。
    claim_refs: [clm_03, clm_04]
    modern_equivalent: 谁核验、谁复核、谁对错误负责
    observable_indicator: 职责与复核权限、错误追踪、申诉记录及处理时长
  - variable_id: var_harm
    tag: downside
    historical_observation: 传文叙强退、谪戍和民怨，后来许复注还本。
    claim_refs: [clm_05, clm_07, clm_08, clm_09, clm_10]
    modern_equivalent: 错误发现对被审核者造成的损害能否纠正
    observable_indicator: 错误处置的实际损失、恢复状态时间及补救完成证据
outcomes:
  - perspective: 被检籍者及行政真实性
    criterion: 是否发生为充限而强退正籍
    horizon: 加日额后至纠偏叙述
    observed_result: 同传记正籍被强退，民怨与边戍接在后文。
    claim_refs: [clm_05, clm_09, clm_10]
    assessment: failure
    uncertainty: 指传文所记错误行为，不是全国错误比例；不能断每个戍者都被错判。
  - perspective: 世祖与旧案受影响者
    criterion: 是否颁纠偏命令及完成恢复
    horizon: 永明八年诏与其后
    observed_result: 已记颁诏、许复注和还本，执行完成度所核段未记载。
    claim_refs: [clm_07, clm_08]
    assessment: ambiguous
    uncertainty: 命令存在，实际效果未知；不等于从未执行。
overall_assessment:
  label: mixed
  rationale: 传文呈现指标副作用及纠偏命令；未有资料证明全国净效果、全部错案恢复或财政收益。
causal_analysis:
  proposed_mechanisms:
    - mechanism: 把求真目标转为每日查错产量，可能诱使执行者制造退籍以满足额度。
      variable_refs: [var_quota, var_responsibility, var_harm]
      supporting_claim_refs: [clm_03, clm_04, clm_05, clm_06]
      inference_strength: plausible_contribution
      inference_reason: 传文明说以充程限且籍正仍退，机制有文本支撑；无独立样本隔离其他原因。
      competing_explanations: [旧有贿赂和责任推诿, 户籍身份争议本身, 州县执行能力不足, 传记以民怨及纠偏压缩长期过程]
      evidence_that_would_weaken_it: [独立案卷显示多数强退与额度无关或日额未产生实际奖惩, 更完整命令显示额度并非强制发现量]
  selection_and_outcome_bias: 不能由纠偏诏反推全部旧处置冤枉，也不能用这段失败叙事断定所有指标必然扭曲。
  unresolved_factors: [确切日额与覆盖机关, 强退频率, 原有欺巧比例, 各类处分与错误的对应, 纠偏执行]
warning_signs:
  - signal: 虞表报告退答迟滞、贿赂和县州推诿，提示现有记录质量不足。
    available_to_actor_then: true
    claim_refs: [clm_02, clm_03]
  - signal: 正籍被强退以充限，属于后来的反馈；谁在何时向太祖或世祖报告未知。
    available_to_actor_then: null
    claim_refs: [clm_05, clm_06]
transferable_mechanisms:
  - mechanism: 检查发现量考核是否诱使制造错误，并独立核实纠偏是否完成。
    conditions_required: [存在发现量与奖惩的实际关联, 可保留审核理由和复核样本, 被审核者有有效纠错途径]
    modern_evidence_needed: [数量与质量指标, 原案和复核结果, 错误处置成本, 恢复完成记录]
    what_not_to_infer: 不推出一切量化有害或现代机构与齐廷等同；纠偏公告不能代替已完成补救的证据。
analogy_limits:
  - historical_condition: 户籍决定贵贱、徭役与边戍，提案含死刑
    modern_difference: 现代审查须遵守平等、隐私、程序及适用法律，对人的后果不同。
    effect_on_recommendation: 只借指标与真实性冲突，不能搬用身份等级、严刑或谪戍作为管理手段。
  - historical_condition: 帝的纠偏诏缺独立执行反馈
    modern_difference: 现实机构可要求可核的恢复、申诉与问责记录。
    effect_on_recommendation: 建议应落实到实际恢复指标，不能止于上级发令。
modern_problem_examples: [审核团队被要求每天发现固定数量问题时如何判断误报？, 已公告纠正错误处罚后如何核实受影响者确已恢复？]
comparison_ids: []
missing_information: [古籍底本及原诏表, 全国与去重户数, 统一日额数字, 独立错案样本, 太祖知悉后果的时间, 复注和返乡执行记录, 净财政和役源结果]
decision_reconstruction:
  decision_stages:
    - stage: 齐初检定与建元二年询议
      evidence: clm_01
      interpretation: 政策有前史，诏议不是唯一开始节点。
    - stage: 虞表提出责任核验
      evidence: clm_02、clm_03
      interpretation: 旧籍数据是上表报告；提案含首悔、严刑与募役，不只是一项柔性审计。
    - stage: 太祖采表后加日额
      evidence: clm_04、clm_06
      interpretation: 执行考核发生实质改变，归属不能写成虞本人主张日额。
    - stage: 传文叙强退及世祖纠偏
      evidence: clm_05、clm_09、clm_10、clm_07、clm_08
      interpretation: 跨帝反馈与命令，不等于完成了全部补救。
  goal_hypotheses:
    - goal: 获得真实簿籍并充实役源
      evidence_level: source_attribution
      basis: clm_01、clm_03的诏表内容
      limit: 真实性与征役控制并存，不是现代公共利益指标。
    - goal: 通过日额防止审核者懈怠
      evidence_level: source_attribution
      basis: clm_06传文以防懈怠
      limit: 史家归属意图，非独立心理记录；不证手段能实现目标。
  option_tradeoffs:
    - option_id: opt_responsibility
      option: 建元二年按虞表落实县审上州、虚昧同咎与首悔
      availability: recorded_offer
      claim_refs: [clm_03]
      basis: 实际提案，与新增日额区分。
      expected_benefits: [可能减少推诿, 可能使原籍校正责任明确]
      expected_costs: [基层核验成本, 同咎可能引出责任转嫁, 严刑与役法损害风险]
      conditions: [官长能真实检校, 州复核可靠, 规则可执行]
      possible_reactions: [官吏可能遵从或掩饰错误，被审核者可能首悔或隐瞒；均不能预断]
      future_options: 真实记录或可支撑后续治理，错误责任设计也可能压缩纠错空间。
      uncertainty: 最终另加日额，原提案单独实施结果未知。
    - option_id: opt_quota
      option: 采表后增板籍官、令史与每日查错要求
      availability: recorded_action
      claim_refs: [clm_04, clm_06]
      basis: 太祖采表后的传文安排。
      expected_benefits: [按传文意图可能提升执行强度和可见产量]
      expected_costs: [凑额与贿赂风险, 真籍被误退的损失, 增官与复查成本]
      conditions: [可管理审核人员, 有可辨真假的材料, 查错产量与真实问题量有关系]
      possible_reactions: [传文记以充程限强退；这项后续不能当作太祖已预见]
      future_options: 被污染的记录可能损害以后判断，纠偏还需追溯原案。
      uncertainty: 无确切日额、考核处罚和覆盖范围，不能算误退增幅。
    - option_id: opt_quality
      option: 建元阶段以质量抽核和纠错记录替代固定发现量
      availability: counterfactual
      claim_refs: []
      basis: 现代分析备选，不是古人已提出或实施的路径。
      expected_benefits: [若有独立复核，可降低制造问题的激励]
      expected_costs: [复核需时间与可信人员, 可能降低可见处理速度]
      conditions: [有原籍及理由记录, 复核者不受同额约束, 可安全申诉]
      possible_reactions: [执行者可能支持、规避或反对，所核材料未记]
      future_options: 可能保留持续校正空间，不能保证当时制度容纳。
      uncertainty: 当时资源与程序可行性未知，不补写独立审计制度。
    - option_id: opt_correct
      option: 永明八年准旧案复注、谪役者还本并保留未来严治
      availability: recorded_action
      claim_refs: [clm_07, clm_08]
      basis: 世祖后一个阶段实际颁诏。
      expected_benefits: [可能减少旧案负担和民怨, 可能恢复部分身份与生活]
      expected_costs: [区分旧案与未来案件的执行成本, 可能恢复部分原本有问题的登记]
      conditions: [可识别年代与谪役者, 地方实际执行, 家属与迁返有接续安排]
      possible_reactions: [受影响者可能申请恢复；实际反应和完成名单未知]
      future_options: 若落实可修复部分关系，后续严治仍可能带来新争议。
      uncertainty: 不能把许还写成全已还，也不等于废除身份役法。
  motive_hypotheses:
    - hypothesis_id: hyp_diligence
      question: 太祖为何另加查错日额？
      explanation: 传文归因为防懈怠，可能想用可见产量督促执行。
      evidence_level: source_attribution
      claim_refs: [clm_06]
      support: 有明确意图用语，强于无据的个人心理推定。
      alternatives: [也可能受役源不足和治理压力影响]
      what_is_missing: 太祖决策讨论、额度设计和奖惩原令。
    - hypothesis_id: hyp_revenue_labor
      question: 太祖为何选择提高查错产量？
      explanation: 诏议关注募役缺口，资源压力可能使快速检出欺巧更有吸引力。
      evidence_level: plausible_inference
      claim_refs: [clm_01, clm_03, clm_04]
      support: 资源问题确在当时诏表中，直接推动日额仍属推断。
      alternatives: [单纯防懈怠, 便于监督新设人员]
      what_is_missing: 役源目标与日额的明确连接，不可写成已经证实的财政动机。
    - hypothesis_id: hyp_correction
      question: 世祖为何颁纠偏诏？
      explanation: 减少旧案负担和回应民怨是有情境依据的解释，政治安抚也可能参与。
      evidence_level: plausible_inference
      claim_refs: [clm_07, clm_08, clm_10]
      support: 传文先叙民怨，诏强调既往不足追咎。
      alternatives: [年代界限下的秩序重建, 传记突出新帝宽政]
      what_is_missing: 纠偏前报告、实际受益规模及各动机权重。
  implementation:
    recorded_steps: [clm_01检定与诏议, clm_03上表, clm_04另置官并加日额, clm_05传文叙强退, clm_08颁纠偏诏]
    necessary_questions: [何种查错算完成日额？, 谁复核强退理由？, 如何识别旧案并核实还本？]
    unknown_procedures: [日额标准及处罚, 个案申辩与复核, 从退籍到谪戍的逐案过程, 返乡及复注完成记录]
    do_not_invent: 不补造现代审计或申诉制度，不以纠偏诏替代执行簿，不把每个谪戍者都定义为误判。
  choice_explanation:
    best_supported: 虞提责任核验、太祖另加日额、世祖后颁纠偏；防懈怠是传文解释，资源压力可能贡献但未证。
    confidence: 安排与叙事后果有单传依据；整体错误比例、真实心理及纠偏效果更不确定。
    counterfactual_limit: 三条建元阶段路径中只有两条有史载提案或动作依据；质量复核为条件假设，不能凑成三种真实选项。
  life_course:
    short_term: 增设板籍审核及日额改变执行约束，传文叙正籍遭退；具体个人生活影响无名册。
    medium_term: 戍役和民怨被记至永明八年，诏给恢复机会，实际返乡未知。
    long_term: 不以虞玩之退休或后世评价判断制度整体收益，不延伸全国长期人口效果。
    values_limit: 朝廷征役目标与编户生活并非同一指标，不替受影响者接受其损害。
    modern_bridge: 在现实审核中先确认求真目标、错误成本与复核权限，再选产量指标；纠偏要核完成而非只核公告。
```
