# HC-034｜孙承宗查重关案：配置风险与有限处置

## 案例定位

候选编号 HC-034；稳定 ID 为 `case_sunchengzong_eight_li_fort_review`。本卡按 Astra 2026-10-01 模板证据审阅于 2026-10-06 有限登记为 reviewed；保留 U-034 及原证据限制。核心从天启二年广宁失后八里铺重关提案与属员反对，到孙承宗获准亲往、配置问答及劝说、返朝后王在晋改任与重关议止。后续筑宁远属于不同阶段，不能拿后来战果证明原案必败。

本轮实际回读《明史》卷二百五十 L37705–37725，补读卷二百五十九袁崇焕传 L38977–38985。见 [配置问答与选点](../../source-md/24.明史.md:37711)、[返朝处置](../../source-md/24.明史.md:37713)、[宁远后来筑城](../../source-md/24.明史.md:38983)。同书两传互参，不作独立双证；未取得王在晋自陈或工程账。

## 决策分析速览

| 路径 | 证据地位 | 预期收益 | 主要代价／缺口 |
|---|---|---|---|
| 八里铺筑重关、增设四万守兵 | recorded_offer | 主张者希望重关卫山海及京师 | 连旧四万合八万；新旧设施、败兵入口等有风险争论 |
| 关外主守中前所 | recorded_offer | 可能保留较近据点 | 完整守备、退路和预算未核，不能自动称折中最优 |
| 主守觉华岛 | recorded_offer | 可能利用海岛据点 | 本段未交代独立防御和陆岸协作全案 |
| 宁远与觉华呼应 | recorded_offer | 孙主张前推防御、保留疆土与难民安置空间 | 成本、互援和敌反应未获完整检验，非当时已建成 |

上述方案在争论中先后出现；主守某地不等于排除所有其他据点。下面另列接口演练及阶段审查为现代分析备选。

## 结构化案例卡

```yaml
schema_version: "0.2"
case_id: case_sunchengzong_eight_li_fort_review
title: 孙承宗查重关案：配置风险与有限处置
status: reviewed
review:
  reviewed_by: "Astra 模板证据审阅；docs/history_case_batch_a_astra_recheck_20261001.md"
  reviewed_at: 2026-10-01
  notes: "HC-034；2026-10-01 Astra 通过模板证据审阅，保留 U-034；2026-10-06 有限本地登记，本次登记差异待收尾复核。仅指所列本地材料支持相应层级，非独立史实、现代因果或执行效果确证；原核读日期、核心事实与未知不变。"
scope:
  period: 明熹宗天启二年
  date_range: 广宁失后至王在晋改任、八里筑城议止；不伪造具体日月
  date_precision: approximate
  event_boundary: 八里铺重关提案及属员反对、孙承宗获准亲往、配置问答与七昼夜劝说、返朝奏请，至调任和议止
  people: [孙承宗, 明熹宗, 王在晋, 王象乾, 袁崇焕, 沈棨, 孙元化, 叶向高, 阎鸣泰, 邢慎言, 张应吾]
  organizations: [明廷, 辽东经略机构, 山海关守军, 关外驻军及难民, 哈喇慎诸部]
classification:
  primary_category: risk_uncertainty
  secondary_categories: [organization_people]
  tags: [dependencies, resources, information_quality, downside, accountability, alternatives]
  classification_note: 核心是新增防御配置如何影响原设施、退路及其他防区；类别不是以填补库中缺额决定。
sources:
  - source_id: src_ming250
    work_title: 明史
    author_or_compiler: 张廷玉等
    source_type: later_compilation
    chapter_or_volume: 卷二百五十·列传第一百三十八（孙承宗传）
    edition_or_translator: 用户本地 Markdown 转录；底本、版次和校勘者未确认，本轮未核 DOCX 或影印本
    locator: source-md/24.明史.md:L37705–37725；核心 L37711–37713，从王在晋方案至八里筑城议止
    url: null
    accessed_on: "2026-10-01"
    verification: checked
    temporal_relation: 清代编纂明末事件，距事约百余年；非现场会议或工程记录。
    dependence_on_other_sources: 与卷259同书互参；具体早期底本承袭未考定，不按独立证据累加。
    limitations: 对孙的褒扬与对王等的贬评明显；对话、败兵风险是叙事和推演，缺双方完整技术文件、工程进度和支出。
  - source_id: src_ming259
    work_title: 明史
    author_or_compiler: 张廷玉等
    source_type: later_compilation
    chapter_or_volume: 卷二百五十九·列传第一百四十七（袁崇焕传）
    edition_or_translator: 同一本地 Markdown 转录；版本未确认
    locator: source-md/24.明史.md:L38977–38985；重关争论、关外选点和三年九月后宁远工段
    url: null
    accessed_on: "2026-10-01"
    verification: checked
    temporal_relation: 同为清代追述明末，非袁崇焕同期自陈。
    dependence_on_other_sources: 同书另传，重关争论文字接近；独立材料链未核，后续增文只帮助区分阶段。
    limitations: 不提供原重关若建成的结果；宁远工事规制与后续不能反证原案战效或净费用。
claims:
  - claim_id: clm_01
    statement: 传文记王在晋先谋用西部袭广宁，经王象乾劝重关卫山海而改请八里铺筑重关；不是王从头到尾只有一个静态方案。
    claim_type: recorded_event
    source_refs: [src_ming250]
    source_locators: ["source-md/24.明史.md:L37711｜在晋谋用西部袭广宁"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 提案改变见单传叙事；王自陈和双方通信未核。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_02
    statement: 原案用四万守新关；问答中王在晋否认移旧城四万人，称须更设兵，孙由此说八里内合八万。是新增四万、连旧四万合八万的拟配置，不是新增八万或兵已募足。
    claim_type: attributed_speech
    source_refs: [src_ming250]
    source_locators: ["source-md/24.明史.md:L37711｜如此，则八里内守兵八万矣"]
    support: supported
    historicity_confidence: low
    confidence_reason: 对话中算式可核，但兵额可用性和原话未获独立军册证明。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_03
    statement: 袁崇焕等属员反对重关并奏记叶向高；叶说不可臆度，孙请身往并获帝准，抵关询问王在晋。卷259也记袁争不得而奏记，不算第二份独立见证。
    claim_type: recorded_event
    source_refs: [src_ming250, src_ming259]
    source_locators: ["source-md/24.明史.md:L37711｜承宗请身往决之", "source-md/24.明史.md:L38979｜奏记首辅叶向高"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 同书两传有相近行动链，无独立现场记录，不能据重复叙事提高置信度。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_04
    statement: 孙在问答中质疑其他防区需兵、新城背靠旧城与旧坑雷、败兵入关或被弃、三道关及拟三寨可能让敌尾随；这些是配置问题和未实施风险推演，不是已发生的攻击结果。
    claim_type: attributed_speech
    source_refs: [src_ming250]
    source_locators: ["source-md/24.明史.md:L37711｜敌亦可尾之入"]
    support: supported
    historicity_confidence: low
    confidence_reason: 核到完整追问及王的回应，未获得地图、双方技术记录或敌方行动概率；在晋无以难是传文评价。
    exact_quote: "敌亦可尾之入"
    quote_checked: true
  - claim_id: clm_05
    statement: 同段记阎鸣泰主觉华岛、袁崇焕主宁远、王在晋主中前所；孙回朝主张宁远与觉华犄角。不能压成重关与宁远两案，也不能说主某地即只守该地。
    claim_type: attributed_speech
    source_refs: [src_ming250, src_ming259]
    source_locators: ["source-md/24.明史.md:L37711｜阎鸣泰主觉华岛", "source-md/24.明史.md:L37713｜与觉华相犄角", "source-md/24.明史.md:L38981｜阎鸣泰主觉华"]
    support: supported
    historicity_confidence: low
    confidence_reason: 选点提案及呼应方向可核，具体范围、兵饷与阶段安排不全，同书互参不独立。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_06
    statement: 传文记孙劝王七昼夜未应，回朝奏请并面奏王不足任；帝改王为南京兵部尚书，八里筑城之议遂止。
    claim_type: recorded_event
    source_refs: [src_ming250]
    source_locators: ["source-md/24.明史.md:L37713｜推心告语凡七昼夜", "source-md/24.明史.md:L37713｜八里筑城之议遂熄"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 有限处置有明确记载；时间与问答仍依单传，不证停议全部由技术论证导致。
    exact_quote: "八里筑城之议遂熄"
    quote_checked: true
  - claim_id: clm_07
    statement: 孙返朝奏语批评百万金钱浪掷版筑、倡以四万人当宁远冲并与觉华呼应，兼称不可把难民置外；金额是其议论，不是已核支出或节省总额。
    claim_type: attributed_speech
    source_refs: [src_ming250]
    source_locators: ["source-md/24.明史.md:L37713｜百万金钱浪掷", "source-md/24.明史.md:L37713｜杏山之难民"]
    support: supported
    historicity_confidence: low
    confidence_reason: 传中奏语可定位，预算原件、对比成本及动机权重未核。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_08
    statement: 孙传贬王象乾无他才、羁縻并冀以老解职；这是传记作者归因，不能作原案所有支持者只为谋私避祸的事实。
    claim_type: source_commentary
    source_refs: [src_ming250]
    source_locators: ["source-md/24.明史.md:L37711｜冀得以老解职而已"]
    support: supported
    historicity_confidence: low
    confidence_reason: 作者评价有文本依据，缺当事人独立目标记录；不以道德评语代工程判断。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_09
    statement: 孙传先记熹宗听其讲说而眷注特殷，重关评审又获准亲往；君臣信任是可能影响处置的既有背景，非独立证明技术结论。
    claim_type: source_commentary
    source_refs: [src_ming250]
    source_locators: ["source-md/24.明史.md:L37707｜故眷注特殷", "source-md/24.明史.md:L37711｜帝大喜"]
    support: supported
    historicity_confidence: low
    confidence_reason: 心理与关系由传书概括，可提示竞争解释而非量化政治原因。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_10
    statement: 袁传另记三年九月决守宁远、原城工仅十一且疏薄、袁改规制并翌年迄工；此后续另有决策和实施，不能写成天启二年一次现场追问已直接造成后来战果。
    claim_type: recorded_event
    source_refs: [src_ming259]
    source_locators: ["source-md/24.明史.md:L38983｜三年九月，承宗决守宁远"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 后续阶段在同书可区分；具体完成量十一不作现代精确进度计算，亦非原重关进度。
    exact_quote: null
    quote_checked: false
source_assessment:
  conflicts:
    - claim_refs: [clm_05, clm_10]
      source_refs: [src_ming250, src_ming259]
      disagreement: 袁传同次选点概括孙主袁议，孙传另叙宁远与觉华呼应；后续仍有选点复议和筑城调整。属于详略及阶段差别，不足判定当时已排除所有其他据点。
      handling: 保留多地点主张及组合方向，不合成当时已定、已建成的唯一完整防御方案。
  single_source_limit: 两传同属明史、重关文字接近，材料链未考定；缺王在晋自陈、工程账、兵册与独立评审记录。
  later_embellishments: [不把新增四万写成新增八万, 不称工程从未开工或全部预算获节省, 不用后来宁远战果证原案必败, 不以王等贬语替代配置审查]
situation:
  summary: 广宁失后王改提八里重关，属员反对；孙获准亲往，追问新旧防线和退兵路径，另议关外配置，返朝后王调任、议止。
  claim_refs: [clm_01, clm_02, clm_03, clm_04, clm_05, clm_06]
  decision_maker: 熹宗批准评审与人事处置；孙承宗评审及建议；王在晋主原案
  affected_parties: [新旧守军, 关外难民, 其他防区, 财政与征募负担者, 原案负责人及属员]
  desired_outcome_at_the_time: 王象乾所劝为卫山海以卫京师；孙奏主前推防御与难民不置外。不同主张有不同风险判断，不预设皆只谋私。
  constraints: [已发生败退与士气问题, 关外据点与诸部关系, 新旧兵力配置需求, 财政及征募负担, 技术争论与人事权相连]
  information_available_then: [王拟增守兵和三寨的答复供孙追问, 孙可看到形势并听属员主张，但现场调查流程与图册未知, 败兵敌尾随是风险预测非已发生事实, 原工程进度和实费未知, 三年九月及以后宁远结果不能前置为二年已知]
  decision_problem: 是否支持八里新关配置，新增设施会如何影响原防线、撤退通道和其他防区；如何比较关外多地点方案并作处置？
options_available:
  - option: 八里铺筑重关、增四万守兵
    availability_basis: 王在晋提案及问答
    claim_refs: [clm_01, clm_02]
    constraints: [合旧四万为八万拟额, 新旧设施接口与退兵问题, 成本和招募能力未核]
  - option: 关外主守中前所
    availability_basis: 王在晋在关外议论中的主张
    claim_refs: [clm_05]
    constraints: [主守范围不完整, 与八里原案不是同一表述, 地形和互援全案未核]
  - option: 主守觉华岛
    availability_basis: 阎鸣泰在同次选点讨论中的主张
    claim_refs: [clm_05]
    constraints: [不能擅称独守, 岛陆互援和供给条件未完整记载]
  - option: 主宁远并与觉华呼应
    availability_basis: 袁主宁远，孙返朝进一步提出与觉华犄角
    claim_refs: [clm_05, clm_07]
    constraints: [需关外兵饷与工事, 敌方反应及互援效能未证]
decision_taken:
  action: 孙获准亲往评审、追问并劝说，返朝提出替代部署及王不足任；帝调任王，八里重关议止。
  claim_refs: [clm_03, clm_04, clm_06, clm_07]
counterfactual_options:
  - option: 先对新旧设施、撤退和互援进行独立演练或阶段审查再批投入
    feasibility_assumptions: [能取得地形与兵饷资料, 有时间和独立技术人员, 有合法安全的演练条件, 评审结果能影响拨款]
    uncertainty: 现代分析备选，原文未记采用这套程序；不能以身往一语补出实际演练。
key_variables:
  - variable_id: var_interfaces
    tag: dependencies
    historical_observation: 孙追问旧城坑雷、退兵入口、三道关和拟寨对整体防御的影响。
    claim_refs: [clm_04]
    modern_equivalent: 新控制是否破坏原有接口并传播故障
    observable_indicator: 接口图、故障情景、恢复路径、跨系统相互影响记录
  - variable_id: var_allocation
    tag: resources
    historical_observation: 拟新增四万与旧四万合八万，孙质疑其他防区仍须兵。
    claim_refs: [clm_02, clm_04, clm_07]
    modern_equivalent: 局部防护占用资源及其机会成本
    observable_indicator: 可用资源与名额区别、总预算、替代方案成本和被挤出的任务
  - variable_id: var_review
    tag: information_quality
    historical_observation: 孙获准亲往并问答，但缺完整技术文件和原案支持方记录。
    claim_refs: [clm_03, clm_04]
    modern_equivalent: 方案审查能否核前提并取得双方可复核证据
    observable_indicator: 原方案、反对理由、现场记录、反驳与未确认条件
  - variable_id: var_authority
    tag: accountability
    historical_observation: 帝最后以负责人调任及议止回应，君臣信任可能影响采纳。
    claim_refs: [clm_06, clm_09]
    modern_equivalent: 技术评审、审批和人事决定的实际关系
    observable_indicator: 决策权限、批准理由、评审记录及利益冲突说明
outcomes:
  - perspective: 明廷与评审过程
    criterion: 原议是否停止、负责人是否调整
    horizon: 天启二年该次评审与返朝处置
    observed_result: 传文记王改任南京兵部尚书，八里筑城议止。
    claim_refs: [clm_06]
    assessment: success
    uncertainty: 只对孙所求的有限处置评价，不说明原案必败或停议净收益为正。
  - perspective: 军民与财政承担者
    criterion: 防御实效、生命风险及净资源节省
    horizon: 停议后及替代部署
    observed_result: 所核段未给原案已开工比例、实费与若建成战效；宁远后来另有工事与复议。
    claim_refs: [clm_07, clm_10]
    assessment: ambiguous
    uncertainty: 不把议止等同零开工、拆除完成、省下全部预算或后来战果单因。
overall_assessment:
  label: mixed
  rationale: 调任与议止可追溯，工程反事实、各案总成本及军民收益仍未知。
causal_analysis:
  proposed_mechanisms:
    - mechanism: 追问新增配置对旧系统、退路和其他资源的影响，可能揭出局部保护与整体目标的冲突并促成停止提案。
      variable_refs: [var_interfaces, var_allocation, var_review, var_authority]
      supporting_claim_refs: [clm_02, clm_03, clm_04, clm_05, clm_06]
      inference_strength: plausible_contribution
      inference_reason: 质询先于处置且问题具体，然而不是完整工程试验，技术贡献不能与政治、人事或战略偏好分离。
      competing_explanations: [熹宗对讲官孙的信任, 袁等此前反对, 前推关外防御偏好, 人事竞争与传记立场]
      evidence_that_would_weaken_it: [王自陈或完整图册能解决接口问题且改变评审判断, 决策记录显示调任早已因其他原因决定]
  selection_and_outcome_bias: 被否决方案缺可观察战效；胜者传记与后来宁远成果不能充作原案必败或替代方案必优的证明。
  unresolved_factors: [原案完整兵饷与工事设计, 开工及已支付成本, 敌方响应概率, 技术与人事因素权重, 各案长期军民代价]
warning_signs:
  - signal: 新关须另增兵，仍未回答旧城设施和败兵入口如何兼容。
    available_to_actor_then: true
    claim_refs: [clm_02, clm_04]
  - signal: 多名属员反对且方案支持者与评审者难达一致。
    available_to_actor_then: true
    claim_refs: [clm_03, clm_06]
transferable_mechanisms:
  - mechanism: 审查新增保护是否造成资源重复、接口冲突和故障传播，并核替代方案而非只问新增单元是否够强。
    conditions_required: [系统确有相互依赖, 可取得方案及故障情景, 评审者有权限要求解释, 替代方案也接受同样审查]
    modern_evidence_needed: [整体架构与资源口径, 失效与恢复演练, 替代成本, 双方论证和审批记录]
    what_not_to_infer: 不推出多一道保护必有害，也不证明安全系统、物理安防或任何重叠设计应被撤销。
analogy_limits:
  - historical_condition: 战争防线需处置败兵、敌军及难民，失败后果含生命损失
    modern_difference: 现代系统控制和一般项目不是同一武力环境，具体风险须由专业资料检验。
    effect_on_recommendation: 只能借用接口与整体配置检查；不能据古战场情节裁定具体网络或场所安防设计。
  - historical_condition: 技术争论与君主信任、人事调任相连，原案支持方材料缺失
    modern_difference: 现实评审应有可复核设计、完整成本与适当独立性。
    effect_on_recommendation: 强化双方证据与利益冲突核查，不能将负责人的调任当成技术判决已证。
modern_problem_examples: [新增一道系统保护会不会堵住恢复路径或消耗其他关键任务资源？, 方案被停止后怎样区分审批结果与尚未证实的净收益？]
comparison_ids: []
missing_information: [古籍底本和早期材料关系, 王在晋自陈及原方案图册, 重关开工比例和已付支出, 四万新兵可募集程度, 各案完整成本和互援条件, 未实施原案的战效, 帝及参与者完整心理]
decision_reconstruction:
  decision_stages:
    - stage: 败后改案与属员反对
      evidence: clm_01、clm_02、clm_03
      interpretation: 原案已有变化，属员异议在孙亲往之前。
    - stage: 亲往及配置问答
      evidence: clm_03、clm_04
      interpretation: 追问的是系统关联和风险，不是已发生的敌尾随。
    - stage: 多地点争论与劝王七昼夜
      evidence: clm_05、clm_06
      interpretation: 中前、觉华、宁远及呼应均有主张，不能重写成静态二选一。
    - stage: 返朝奏请、王调任、议止
      evidence: clm_06、clm_07
      interpretation: 这是可观察结果，原工程状态与反事实战效仍未知。
    - stage: 边界外宁远复议与筑城
      evidence: clm_10
      interpretation: 保留阶段差异，后事不用来证成二年所有批评。
  goal_hypotheses:
    - goal: 避免局部重关配置损害整体守御
      evidence_level: source_attribution
      basis: clm_04、clm_07中的追问及奏语
      limit: 公开论证不是完整真实心理，也不自动证技术正确。
    - goal: 前推防御并保留关外土地、难民安置空间
      evidence_level: source_attribution
      basis: clm_05、clm_07的宁远觉华及难民论述
      limit: 战略目标不保证实现，也不等于相关难民已获得安置。
  option_tradeoffs:
    - option_id: opt_fort
      option: 八里铺重关增四万守兵
      availability: recorded_offer
      claim_refs: [clm_01, clm_02, clm_04]
      basis: 王的提案和问答；不是已募足且建成。
      expected_benefits: [按主张者希望加一道近关屏障并卫京师]
      expected_costs: [新增兵饷和建设, 挤占其他防区, 退兵及旧设施接口风险]
      conditions: [新增守兵可用, 新旧防线可协同, 可处置撤退与敌随入]
      possible_reactions: [属员已反对，孙质疑；敌反应仅为预测]
      future_options: 或可加强近关守御，也可能加重资源绑定；未实施结果不可知。
      uncertainty: 缺完整设计和工程账，不能确定必败或零开工。
    - option_id: opt_zhongqian
      option: 关外主守中前所
      availability: recorded_offer
      claim_refs: [clm_05]
      basis: 王在关外选点中的主张，不擅合为先前重关原案。
      expected_benefits: [可能在较近据点保留关外部署]
      expected_costs: [仍需出关资源和防御, 对更远土地与居民的影响未知]
      conditions: [地形与补给适合, 与关门及其他据点能呼应]
      possible_reactions: [孙主宁远觉华，王持异议；其他人具体权衡未知]
      future_options: 可能保留进一步前推或退回空间，须核路径与成本。
      uncertainty: 原文没有完整方案，收益是分析假设，不能称天然折中最佳。
    - option_id: opt_juehua
      option: 主守觉华岛
      availability: recorded_offer
      claim_refs: [clm_05]
      basis: 阎鸣泰明确主张；不补为独守岛而弃陆。
      expected_benefits: [可能利用海岛据点形成支撑]
      expected_costs: [岛上供给与陆岸协同压力, 无完整代价记录]
      conditions: [运输可维持, 岛陆部署与其他防区匹配]
      possible_reactions: [袁另主宁远，孙进一步主两地呼应]
      future_options: 可能成为呼应部署一环，是否足够单独实现目标未知。
      uncertainty: 本段只存选点意见，无法比较独立守岛表现。
    - option_id: opt_ningyuan
      option: 主宁远并与觉华犄角
      availability: recorded_offer
      claim_refs: [clm_05, clm_07]
      basis: 袁主宁远，孙奏中详主宁远与觉华呼应，非当时已完成全部实施。
      expected_benefits: [可能前推防御, 保留疆土与难民空间, 分散敌对关门压力]
      expected_costs: [出关、建设及持续兵饷, 互援与敌反应不确定]
      conditions: [可出关部署, 工事和供给能维持, 两地确能协同]
      possible_reactions: [王等反对；后续复议表明意见并非一次消失]
      future_options: 可能打开前沿部署，也可能形成新的长期供给义务。
      uncertainty: 后续三年与筑城变化不能当二年已实现或准确预测。
    - option_id: opt_stage_review
      option: 先作接口演练及阶段投入审查
      availability: counterfactual
      claim_refs: []
      basis: 现代分析提出，亲往不等于已有该程序。
      expected_benefits: [若可行，可能及早发现互援与撤退问题]
      expected_costs: [时间与评审资源, 危机中可能延误必要防御]
      conditions: [可靠图册、兵饷资料与专业人员, 安全演练和审批权限]
      possible_reactions: [各方可能认可或拒绝，所核材料未记]
      future_options: 或可保留修订与分阶段投入，能否容纳取决于实际时限。
      uncertainty: 不假称孙曾设计现代风险测试或阶段拨款。
  motive_hypotheses:
    - hypothesis_id: hyp_system_risk
      question: 孙为何反对重关并亲往质询？
      explanation: 公开论证关注重复兵额、旧设施和退兵接口，可能认为其损害整体守御。
      evidence_level: source_attribution
      claim_refs: [clm_03, clm_04, clm_07]
      support: 具体追问与奏语比传记道德贬评更直接。
      alternatives: [原已有前推战略偏好, 人事及组织立场影响]
      what_is_missing: 完整双方设计、评审记录及真实心理权重。
    - hypothesis_id: hyp_forward
      question: 孙为何坚持关外方案而不止于修改近关设施？
      explanation: 他奏语重视前推和难民，可能认为只守关会失去屏障与恢复空间。
      evidence_level: source_attribution
      claim_refs: [clm_05, clm_07]
      support: 有明确战略论述，但不是社会收益或战效已经证明。
      alternatives: [与袁等的相近立场, 名望与人事竞争可能参与但未证]
      what_is_missing: 各目标相对权重、难民安排与替代方案完整评价。
    - hypothesis_id: hyp_wang_risk
      question: 王为何支持重关或较近部署？
      explanation: 王象乾的劝说认为广宁得而难守、可能获更大罪，王可能更看重可守程度及失败问责。
      evidence_level: plausible_inference
      claim_refs: [clm_01, clm_05, clm_08]
      support: 有提案改变和较近选点依据；冀解职仅是传记对王象乾的归因。
      alternatives: [有未被传文保存的技术依据, 其他资源约束]
      what_is_missing: 王在晋自陈和资源判断，不能将王象乾的心理直接移给王在晋或所有支持者。
  implementation:
    recorded_steps: [clm_03属员奏记与孙获准亲往, clm_04现场问答, clm_05讨论关外选点, clm_06七昼夜劝说后返朝面奏, clm_06帝调任王并止议]
    necessary_questions: [原案在何阶段、已付何费？, 新旧守兵多少可用？, 怎样验证撤退和互援假设？, 议止后责任与资源如何移交？]
    unknown_procedures: [原重关开工及停止执行比例, 现场图册和勘查方法, 王的完整答辩, 正式预算对照, 已付费用与人员转配]
    do_not_invent: 不补造零开工、拆除完成、全预算节省或现场演练；不将后来关上兵名七万用来抹平原案拟八万。
  choice_explanation:
    best_supported: 孙以整体配置风险和前推战略主张反对原议，帝最后调任止议；对君臣信任和人事因素的竞争解释仍须保留。
    confidence: 有限行动链有同书依据，完整技术正确性、心理与反事实战效更不确定。
    counterfactual_limit: 四条史载主张可比较，但不是同时静态菜单，且主守范围不完整；不据后来战果选择必优方案。
  life_course:
    short_term: 王改任南京兵部尚书，原议止；军民安全和费用的即时变化未详。
    medium_term: 袁传后续另有宁远复议、改规制与筑城，属于新阶段，不是此卡的已完成替代结果。
    long_term: 不以两位人物后来功过及结局评价本次配置审查的全部人生价值。
    values_limit: 京师安全、边地居民、军人风险和财政负担并非同一目标；不能只按掌权者收益判断。
    modern_bridge: 现实中先定保护对象、依赖和资源，再核双方设计和故障情景；方案获否决与净风险改善分别验收。
```
