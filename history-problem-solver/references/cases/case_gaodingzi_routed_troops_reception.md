# HC-030｜高定子接纳溃卒：给犒、有限戒备与待遇边界

## 案例定位

候选编号 HC-030；稳定 ID 为 `case_gaodingzi_routed_troops_reception`。本卡按 Astra 2026-10-01 模板证据审阅于 2026-10-06 有限登记为 reviewed；保留 U-030 及原证据限制。张钺被捕为前史；核心是另一批受招而不释甲的军队到州、给犒与安置；后批和彦威部索同额、另给军饷与催还戍作为待遇边界检验。不是统一镇压／救济二择一，也不称复编成功。

本轮实际回读《宋史》卷四百九 L82999–83013，完整读取 L83009–83011；另读 L82987–82997 王霆传末，确认人物边界。见 [前史与首批接纳](../../source-md/20.宋史.md:83009)、[后批索饷](../../source-md/20.宋史.md:83011)。所核为本地转录，名册与财政账未取得。

## 决策分析速览

| 路径 | 证据地位 | 预期收益 | 主要代价／缺口 |
|---|---|---|---|
| 首批受招者给犒安置，并令帐下卒衷甲待命、毋轻动 | recorded_action | 若高的缺粮判断属实，可能缓和饥乏；克制戒备可能减少接触升级、保留防护 | 资源支出与武装接触风险；无逐人领取及长期纪律记录 |
| 后批按首批例索取同额钱米 | recorded_offer | 来军预期获得按人数的供给 | 会扩大原令对象；人数及是否适格未独立核实 |
| 高区分待遇对象，另给四十万缗并催还戍 | recorded_action | 可能兼顾急需与承诺边界 | 大额支出；催还不是已全部归戍 |

全面缴械后再给粮是下文的分析备选，未在所核段发现其作为当时提案。上述路径分两批出现，不能当成同一批人的同时三选一。

## 结构化案例卡

```yaml
schema_version: "0.2"
case_id: case_gaodingzi_routed_troops_reception
title: 高定子接纳溃卒：给犒、有限戒备与待遇边界
status: reviewed
review:
  reviewed_by: "Astra 模板证据审阅；docs/history_case_batch_a_astra_recheck_20261001.md"
  reviewed_at: 2026-10-01
  notes: "HC-030；2026-10-01 Astra 通过模板证据审阅，保留 U-030；2026-10-06 有限本地登记，本次登记差异待收尾复核。仅指所列本地材料支持相应层级，非独立史实、现代因果或执行效果确证；原核读日期、核心事实与未知不变。"
scope:
  period: 南宋高定子知绵州时，蒙古军入蜀背景
  date_range: 绵州任内首批招纳及亡几何后的后批索饷；所读核心段未给确切年月
  date_precision: unknown
  event_boundary: 受招诸军不释甲、到州接触、给犒安置，至和彦威部索同额、另给军饷与催还戍
  people: [高定子, 陈训, 张钺, 黄伯固, 和彦威, 陈邦佐, 曹篪, 张涓, 姚承祖]
  organizations: [绵州官府, 高定子帐下卒, 首批受招溃军, 和彦威所部, 制置司, 诸司]
classification:
  primary_category: cooperation_trust
  secondary_categories: [organization_people, risk_uncertainty]
  tags: [incentives, boundaries, resources, accountability, information_quality, power_balance]
  classification_note: 低信任接触中如何兑现有限承诺并约束升级、界定资格；不将归顺表态等同长期信任。
sources:
  - source_id: src_song409
    work_title: 宋史
    author_or_compiler: 脱脱等
    source_type: later_compilation
    chapter_or_volume: 卷四百九·列传第一百六十八（高定子传）
    edition_or_translator: 用户本地 Markdown 转录；古籍底本、版次未确认，未在本轮重核 DOCX 或影印本
    locator: source-md/20.宋史.md:L82999–83013；核心 L83009–83011，差知绵州至仍趣其还戍
    url: null
    accessed_on: "2026-10-01"
    verification: checked
    temporal_relation: 元代编纂南宋事件，相距约百年；本段早期材料来源未考定。
    dependence_on_other_sources: 单一高定子传；钱粮令、问答和赞誉出自同传，未获得独立名册、账簿或归戍军令执行记录。
    limitations: 传记突出守臣担当，对话和悦服描写可能有褒扬；受招人数、资金实付和长期纪律未能量化。
claims:
  - claim_id: clm_01
    statement: 传文记张钺溃入文州、杀守臣并欲趋绵窥成都，高定子奉相关任命部署扼青塘岭而捕获张钺；这是后来受招诸军到州以前的前史。
    claim_type: recorded_event
    source_refs: [src_song409]
    source_locators: ["source-md/20.宋史.md:L83009｜钺就擒"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 行动与对象有单传依据，不与随后另一批来军混合；独立战报未核。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_02
    statement: 高在传中向僚吏与群胥表示守州、发州藏及截诸司纲运以供给，且以杀戮威胁约束逃亡；这是宣言和归属言论，不是已核逐笔资源调拨账。
    claim_type: attributed_speech
    source_refs: [src_song409]
    source_locators: ["source-md/20.宋史.md:L83009｜吾将尽发吾州之藏"]
    support: supported
    historicity_confidence: low
    confidence_reason: 同传归属的言语，具体金额、权限和全数执行未明；不将威胁美化为管理示范。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_03
    statement: 传文记下令招溃卒，每人缗钱五十、米一石，命都监陈训专任接纳；这是首批受招者的令与职掌，不证所有溃军均用同一待遇。
    claim_type: recorded_event
    source_refs: [src_song409]
    source_locators: ["source-md/20.宋史.md:L83009｜命都监陈训专任接纳"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 对象、数额与负责人明确；命令不等于逐人足额领取。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_04
    statement: 陈训报告受招诸军不肯释甲；高令帐下卒衷甲于两庑待命、戒毋轻动，继而坐堂接触来军。传文不等于完全无防备，也未记强制缴械成功。
    claim_type: recorded_event
    source_refs: [src_song409]
    source_locators: ["source-md/20.宋史.md:L83009｜戒毋轻动"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 有报告、安排和接触次序，无独立现场记录或完整升级权限。
    exact_quote: "戒毋轻动"
    quote_checked: true
  - claim_id: clm_05
    statement: 传中高劝诸军还本部候犒，来将称制置使存亡未知、诸军无主；高以暂移治、已遣人访所在安抚，将来军至此解释为无粮，并称州府承担供给、劝敌至协力。无粮是高的判断，暂移治是他的安抚说法，不证需求已独立核实或他当时确知上级位置。
    claim_type: attributed_speech
    source_refs: [src_song409]
    source_locators: ["source-md/20.宋史.md:L83009｜制置使未知存亡，诸军无主", "source-md/20.宋史.md:L83009｜大帅不过暂移治尔", "source-md/20.宋史.md:L83009｜且诸军至此以无粮故"]
    support: supported
    historicity_confidence: low
    confidence_reason: 问答与安抚话语可定位；上级消息不明及无主为来将自报，无粮与暂移治为高的判断或安抚说法，需求实情及军心状态未独立核验。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_06
    statement: 传文记众悦而去，随后遣吏给犒如令，辟寺观祠宇安置；支持发放和住宿安排，未提供逐人名册、完成比例、制度性复编或长期战力结果。
    claim_type: recorded_event
    source_refs: [src_song409]
    source_locators: ["source-md/20.宋史.md:L83009｜给犒如令"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 比单一许诺有更强的执行记载，但悦服为传记描写，缺完整行政和军事后续。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_07
    statement: 后批和彦威等部被传文称败将、剽掠；陈邦佐口称麾下兵且二万余，高随后提出入境须受其节制、各守纪律才给钱粮，继而和彦威符移称所部不下二万人并索同例钱米。高说原令针对就招免罪溃军、都统所部非溃，是待遇分类论证，不证后批全然有序；其纪律条件不等于对方已接受或遵守。
    claim_type: attributed_speech
    source_refs: [src_song409]
    source_locators: ["source-md/20.宋史.md:L83011｜麾下兵且二万余", "source-md/20.宋史.md:L83011｜惟各守纪律，则给以钱粮", "source-md/20.宋史.md:L83011｜今所部不下二万人", "source-md/20.宋史.md:L83011｜都统所部非溃也"]
    support: supported
    historicity_confidence: low
    confidence_reason: 二万余与不下二万人分别为陈邦佐口述和和彦威符移口径，可相容但不能互换，不据此推兵员变化或谎报；节制纪律条件与资格为高的论证，实数、身份及纪律执行未独立核实。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_08
    statement: 传文记和彦威改乞别给军饷，高另捐四十万缗并催还戍；所核段未证全部按期到戍所，另给金额不按二万人倒算作每人实领。
    claim_type: recorded_event
    source_refs: [src_song409]
    source_locators: ["source-md/20.宋史.md:L83011｜四十万缗", "source-md/20.宋史.md:L83011｜仍趣其还戍"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 另给和催促有单传依据，独立财账与归戍执行未核。
    exact_quote: "仍趣其还戍"
    quote_checked: true
source_assessment:
  conflicts:
    - claim_refs: [clm_07]
      source_refs: [src_song409]
      disagreement: 同段叙后批为败将且剽掠，高却在待遇论证中称其所部非溃；这是叙述称谓与资格论证的张力，非已核定军事身份的两份冲突记录。
      handling: 保留双方话语层级；不据非溃一语消去剽掠，不将所有批次合并成同一种受招者。
  single_source_limit: 两批来军、指令、拨给与悦服均来自一传，不按多段计独立佐证；缺人员、领饷与归戍记录。
  later_embellishments: [不采用徒手无戒备赢得所有溃军信任的概括, 不把还本部或催还戍写成成功复编, 不称同一待遇惠及全部来军]
situation:
  summary: 张钺被捕后，另一批受招军队持械来州；高在资源与秩序压力下安抚、克制戒备并给犒安置；后批借首令索饷，高界定对象而另给。
  claim_refs: [clm_01, clm_03, clm_04, clm_05, clm_06, clm_07, clm_08]
  decision_maker: 高定子；陈训负责接纳并报告疑惧，未见独立更改待遇或动武授权
  affected_parties: [受招军人, 后批部队, 绵州居民与吏士, 寺观祠宇及使用者, 财政供给机关]
  desired_outcome_at_the_time: 传中高表达守州、供给、使军队为国效力的目标；长期信任与纪律恢复不是已证实的成果。
  constraints: [此前已有杀守兵变, 来军不释甲, 来将自报上级存亡不明和无主，缺粮为高的判断而非已核需求, 州藏及诸司物资不是无限资源, 武装和权力不对等, 强制威胁影响合作表态]
  information_available_then: [陈训明确报告不释甲, 来将自称制置使存亡未知、诸军无主，高将来军至此解释为无粮并称州府承担供给, 高表示已派人访上级，不能将暂移治当已证事实, 后批人数与威权由其代表声称，未核名册, 未来敌至和归戍结果不可前置]
  decision_problem: 首批武装来军受招但仍有风险，如何接触并兑现供给；后批要求套用待遇时如何界定承诺而继续处置资源需求？
options_available:
  - option: 首批接纳、给犒安置并保持克制戒备
    availability_basis: 高实际下令与实施，陈训执行接纳
    claim_refs: [clm_03, clm_04, clm_06]
    constraints: [给付资源, 接触仍有武装风险, 未知未来纪律]
  - option: 后批按首令每人钱米同额给付
    availability_basis: 和彦威符移明确索取；不是高已承诺此范围
    claim_refs: [clm_07]
    constraints: [适格范围有争议, 所部人数未独立核实, 扩大承诺需资源与权限]
  - option: 后批区分对象、另给军饷并催归戍
    availability_basis: 高实际回应，和彦威改乞别给后获四十万缗
    claim_refs: [clm_07, clm_08]
    constraints: [大额支出, 催归戍未证执行]
decision_taken:
  action: 首批接触时保持衷甲待命而不轻动，安抚后给犒住宿；后批明确首令资格，另给军饷并催还戍。
  claim_refs: [clm_04, clm_05, clm_06, clm_07, clm_08]
counterfactual_options:
  - option: 首批先全面缴械再提供钱粮
    feasibility_assumptions: [具有合法且足够的控制能力, 来军愿接受条件, 能避免断粮或接触升级造成更大损害]
    uncertainty: 现代分析提出的条件比较，所核原文未记此项提案或可行性，不能写高曾认真考虑。
key_variables:
  - variable_id: var_delivery
    tag: incentives
    historical_observation: 招令给钱米，后来记遣吏给犒和住宿安排。
    claim_refs: [clm_03, clm_06]
    modern_equivalent: 危机中有限承诺是否真实执行
    observable_indicator: 对象名单、承诺内容、实付凭证、资源缺口和投诉反馈
  - variable_id: var_escalation
    tag: accountability
    historical_observation: 陈训报告持械，高让帐下待命并戒毋轻动。
    claim_refs: [clm_04]
    modern_equivalent: 由谁报告风险、由谁决定升级响应
    observable_indicator: 明确升级权限、工作人员报告与接触处置记录
  - variable_id: var_eligibility
    tag: boundaries
    historical_observation: 高用就招免罪资格区分首批与后批，随后另给军饷。
    claim_refs: [clm_07, clm_08]
    modern_equivalent: 一个承诺是否被扩张到未约定群体
    observable_indicator: 原政策适格条件、例外授权、新增受益人数与成本
  - variable_id: var_information
    tag: information_quality
    historical_observation: 上级存亡、移治与后批人数由不同人物陈述，没有完整核实记录。
    claim_refs: [clm_05, clm_07]
    modern_equivalent: 安抚话语与已核信息的区分
    observable_indicator: 原始报告、核实时间、未确认事项及后续更新
outcomes:
  - perspective: 首批受招军人及绵州官府
    criterion: 是否完成记载中的接触、给犒与安置
    horizon: 不释甲报告后至遣吏给犒和住宿安排
    observed_result: 传文记来军拜、悦而去，随后按令给犒、辟场所住宿。
    claim_refs: [clm_04, clm_05, clm_06]
    assessment: success
    uncertainty: 限短期行动；未获逐人足额证明，所核段未记交战不等于证明整个过程从无冲突。
  - perspective: 后批部队与地方财政
    criterion: 是否界定同额对象并处理新索饷、是否实际归戍
    horizon: 后批交涉至另给与催还戍
    observed_result: 传文记改乞别给、四十万缗给付和催还戍。
    claim_refs: [clm_07, clm_08]
    assessment: mixed
    uncertainty: 处置动作有记载，归戍执行、支出来源与财政负担未知。
  - perspective: 居民、财政供给者与军队长期运行
    criterion: 剽掠、纪律、战力及生活损害是否持续改善
    horizon: 后续较长期
    observed_result: 所核段未提供持续观察、独立纪律或战斗记录。
    claim_refs: []
    assessment: ambiguous
    uncertainty: 不以传记悦服或官职奖励填补长期效果。
overall_assessment:
  label: mixed
  rationale: 首批有限接纳与安置、后批另给有记载；长期纪律、战力、全部归戍和总体民众代价未知。
causal_analysis:
  proposed_mechanisms:
    - mechanism: 给付可执行的供给并约束即时升级，可能让低信任接触得以继续。
      variable_refs: [var_delivery, var_escalation, var_information]
      supporting_claim_refs: [clm_03, clm_04, clm_05, clm_06]
      inference_strength: plausible_contribution
      inference_reason: 宣令、克制戒备、安抚和执行相继记载，不能隔离哪一项促成悦服。
      competing_explanations: [若高的缺粮判断属实，供给压力可能使来军接受，但需求及合作理由未独立证实, 地方军力与高的职位威慑, 来军另有不得不合作的约束, 传记褒扬守臣的选择性叙述]
      evidence_that_would_weaken_it: [独立军令显示来军原已决定服从或主要由其他力量控制, 执行账显示供给未实际到位]
    - mechanism: 界定原令对象并另行处置新需求，可能避免把承诺机械扩张。
      variable_refs: [var_eligibility, var_delivery]
      supporting_claim_refs: [clm_07, clm_08]
      inference_strength: hypothesis
      inference_reason: 对象论证与改乞别给有次序，未证明实际支出更少或双方认可统一资格制度。
      competing_explanations: [高先提出受其节制、守纪律才给钱粮，权威与纪律条件可能影响交涉，但接受及执行未知, 四十万缗本身缓和需求, 威慑或面子退让, 后批另有军令压力]
      evidence_that_would_weaken_it: [可靠原令显示本来覆盖后批, 后续记录显示仍按同额追加或资格论证未影响请求]
  selection_and_outcome_bias: 守臣传记的悦服和褒奖不能证长期信任，更不能以有限接纳倒推所有溃军同样适用。
  unresolved_factors: [每批人数与领取, 资源权限及来源, 各措施相对贡献, 强制因素对表态的影响, 后批实际归戍]
warning_signs:
  - signal: 受招后仍不释甲，陈训已报告接触风险。
    available_to_actor_then: true
    claim_refs: [clm_04]
  - signal: 后批以未核人数要求复制首令同额待遇。
    available_to_actor_then: true
    claim_refs: [clm_07]
transferable_mechanisms:
  - mechanism: 危机接触中把供给承诺、风险报告和升级权限写清，并核兑现；新群体要求同待遇时复核原承诺范围。
    conditions_required: [合法安全的接触条件, 有可兑现且被授权的资源, 适格条件明确且可公平复核, 不靠威胁迫使表态]
    modern_evidence_needed: [实际需求与对象名单, 执行凭证, 接触及升级记录, 政策例外权限和总支出]
    what_not_to_infer: 不推出钱粮必换信任、武装风险已消失或长期复编；资格界定也不能作为任意剥夺应有待遇的借口。
analogy_limits:
  - historical_condition: 武装溃军、地方军事权与杀戮威胁
    modern_difference: 现代工作人员、救助对象与合作方有法律权利及专业处置要求，不具有同样强制环境。
    effect_on_recommendation: 不把员工比作溃军，不复制隐蔽武力或斩首威胁；严重威胁需按现实专业程序处理。
  - historical_condition: 高宣称发州藏和截诸司纲运，缺逐笔授权及账项
    modern_difference: 现实机构使用公共或他方资源须有合法权限、预算与审计。
    effect_on_recommendation: 先核权限和实际可用资源，不能将个人担当当作挪用资源的理由。
modern_problem_examples: [危机期间向一批合作方承诺临时支持后另一批要求同待遇，应核查哪些资格和资源？, 接触对象仍有风险时如何同时明确承诺兑现与升级权限？]
comparison_ids: []
missing_information: [确切年月及各批总人数, 底本与早期材料链, 逐人领钱米名册, 寺观安置的成本与使用者影响, 截诸司纲运的权限和实账, 后批实际归戍, 长期纪律和战力, 当事人真实心理]
decision_reconstruction:
  decision_stages:
    - stage: 前史：捕获张钺
      evidence: clm_01
      interpretation: 高此前已有强制应对，不能概称对所有来军只用救济。
    - stage: 首批招令与未释甲报告
      evidence: clm_03、clm_04
      interpretation: 接纳已开始，风险仍在；陈训报告不能补成独立动武授权。
    - stage: 克制戒备、安抚与给犒住宿
      evidence: clm_04、clm_05、clm_06
      interpretation: 有有限实施后续，表态不能替代长期信任证据。
    - stage: 后批索同例、另给与催还戍
      evidence: clm_07、clm_08
      interpretation: 待遇边界被检验，催促不是完成归戍。
  goal_hypotheses:
    - goal: 守州并将来军需求引向供给与协力防敌
      evidence_level: source_attribution
      basis: clm_02、clm_05的守臣宣言和问答
      limit: 传世言论含强制威胁，非完整目标和可验证军心记录。
    - goal: 在回应后批需求时守住原令对象边界
      evidence_level: plausible_inference
      basis: clm_07、clm_08的身份区分及另给
      limit: 不能证其完整财政规划或以减少支出为唯一动机。
  option_tradeoffs:
    - option_id: opt_receive
      option: 首批给犒安置并克制戒备
      availability: recorded_action
      claim_refs: [clm_03, clm_04, clm_05, clm_06]
      basis: 首批实际招令、待命与后续发放。
      expected_benefits: [若高对缺粮的判断属实，供给可能缓和饥乏；对来将自报的无主状态仍需核实后续统属, 保留协作机会并维持防护]
      expected_costs: [公共资源支出, 武装接触及住宿影响, 后续期待可能扩大]
      conditions: [供给可兑现, 接纳负责人能报告, 戒备不自行升级]
      possible_reactions: [传文记拜与悦服；真实信任、全部成员态度仍未知]
      future_options: 可能保留安置和协作，长期统属仍需另证。
      uncertainty: 无独立资料分离钱粮、说服和威慑作用。
    - option_id: opt_same_pay
      option: 后批要求复制首令按人钱米
      availability: recorded_offer
      claim_refs: [clm_07]
      basis: 和彦威符移提出的请求；不等于高曾保证或认可。
      expected_benefits: [若适格且能给，可能满足来军期待]
      expected_costs: [扩大财政负担, 不核人数及资格可能损害一致性]
      conditions: [人数可靠, 原令适用或另有授权, 钱米资源足够]
      possible_reactions: [高实际以所部非溃抗辩；其他人反应未知]
      future_options: 或可缓和眼前争议，也可能形成更大追索期待。
      uncertainty: 不将陈邦佐的二万余或符移的不下二万人当名册实数，不统一两口径，不倒算准确总额及人均实收。
    - option_id: opt_separate
      option: 后批另给四十万缗、催还戍
      availability: recorded_action
      claim_refs: [clm_07, clm_08]
      basis: 高先提出节制纪律条件，后以资格抗辩，对方改乞别给后获另给与催戍；属于后一阶段，不证给款附有已落实的正式协议。
      expected_benefits: [可能同时回应补给需求与资格边界, 可能推动军队返回职责]
      expected_costs: [大额支出, 收饷仍可能不归戍, 居民和其他机关承担机会成本]
      conditions: [资金可给且有权给, 有归戍目的地和执行条件]
      possible_reactions: [传文记改乞别给；惭是作者赋予的心理，不独立确认]
      future_options: 若实际归戍可减地方驻留压力，未有完成证据。
      uncertainty: 不是已经证明比同额更省或更公平的方案；对方是否接受节制、遵守纪律及实际归戍未知。
    - option_id: opt_disarm
      option: 首批先全面缴械再给粮
      availability: counterfactual
      claim_refs: []
      basis: 为比较接触条件而提出，原文未记。
      expected_benefits: [若可合法安全执行，可能降低武装接触风险]
      expected_costs: [可能升级冲突, 延误必要供给, 需额外控制能力]
      conditions: [合法权限与足够能力, 避免更大伤害, 来军接受]
      possible_reactions: [接受或抵抗均未知，不能把后来的悦服反推当时必可缴械]
      future_options: 可能改变接触条件，也可能关闭合作空间。
      uncertainty: 没有证据显示高采用、提出或具备实施条件。
  motive_hypotheses:
    - hypothesis_id: hyp_duty
      question: 高为何留州接纳而非随危局离去？
      explanation: 传中自述守臣职责与为朝廷捍蔽全蜀，可能以守土责任组织行动。
      evidence_level: source_attribution
      claim_refs: [clm_02, clm_05]
      support: 有归属言论及相连行动，但不能当完整私人心理。
      alternatives: [职位责任与惩罚压力, 传记塑造担当形象]
      what_is_missing: 个人记录、实际退出条件及风险权衡。
    - hypothesis_id: hyp_needs_order
      question: 高为何以钱粮和安抚配合戒备？
      explanation: 高将来军至此解释为无粮，可能以供给回应其所判断的需求，并以安抚回应来将自报的上级存亡不明、无主，配合戒备避免接触升级。
      evidence_level: plausible_inference
      claim_refs: [clm_03, clm_04, clm_05, clm_06]
      support: 高的需求判断、来将的指挥信息报告、毋轻动及给犒相接，条件性解释有动作依据；不证需求已核实或供给已恢复统属。
      alternatives: [依赖武力和官位威慑, 来军本就缺少替代出路]
      what_is_missing: 高对各种措施的主观权重及来军独立的合作理由。
    - hypothesis_id: hyp_boundary
      question: 高为何拒套首令却仍另给钱？
      explanation: 可能想维持承诺范围又满足实际军需；不等于拒绝所有后批支持。
      evidence_level: plausible_inference
      claim_refs: [clm_07, clm_08]
      support: 分类抗辩后实际另给，较单纯节省说更合文本。
      alternatives: [临时议价, 高明示受其节制并守纪律才给钱粮，可能意在维护州府节制权，但接受及执行未知, 对后批威权的应对]
      what_is_missing: 原令全文、资格名册及拨给决策记录。
  implementation:
    recorded_steps: [clm_03命陈训接纳并定给犒额, clm_04受报后令帐下待命毋轻动, clm_05安抚与劝还本部, clm_06遣吏给犒及辟住宿, clm_08另给军饷并催还戍]
    necessary_questions: [谁核首批身份和人数？, 钱米如何实际领取？, 住宿如何安排及补偿？, 谁核后批归戍？]
    unknown_procedures: [逐人登记和发付, 其他升级权限, 正式编制与统属恢复, 军粮调拨授权及实账, 归戍验收]
    do_not_invent: 不补写全面缴械、编制整顿、长期信任、人人足额或全部到戍；不将陈训职掌扩成独立军事授权。
  choice_explanation:
    best_supported: 高在首批持械条件下配合供给与克制戒备，后批则按承诺对象另行给饷；文本未证明复编或长期秩序恢复。
    confidence: 对命令与有限执行有单传依据，对对方心理、长期信任和归戍完成的把握较低。
    counterfactual_limit: 首批有据的接触路径只有一条，不足三条，供给与戒备是配套动作而非另外两案；后批另有同额请求与另给处置。全卡可分阶段比较，不能凑成首批同时三选一；缴械备选的可行性未知。
  life_course:
    short_term: 首批有钱米给犒和住宿安排，州府承担接触与支出；实际覆盖度未知。
    medium_term: 后批另获军饷并被催还戍，归戍与纪律尚不能确认。
    long_term: 不用高后来升官或吏民赞誉证明军队长期战力、地方财政和居民福祉。
    values_limit: 守土、军需与居民安全有不同代价；传中强制之下的表态不能代当事人选择。
    modern_bridge: 在现实已授权的支持中核需求、对象、兑现和升级权限；不把武装溃军等同普通合作或现代员工。
```
