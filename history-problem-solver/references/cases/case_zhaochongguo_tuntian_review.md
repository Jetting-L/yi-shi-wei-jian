# HC-004｜赵充国屯田提案：连续质询与组合政策

## 案例定位

候选编号 HC-004；稳定 ID 为 `case_zhaochongguo_tuntian_review`。本卡按 Astra 2026-10-01 模板证据审阅于 2026-10-06 有限登记为 reviewed；保留 U-004 及原证据限制。核心从神爵元年秋屯田奏到次年五月罢屯获准；六月／七月攻击对象之争为前史，次年秋降附为边界外尾注。

本轮实际回读《汉书》卷六十九本地转录 L9813–9888，完整读取秋季奏疏、帝的质询和答复、兼采出击与次年罢屯段。原文见 [秋季提案](../../source-md/2.汉书.md:9857)、[组合政策](../../source-md/2.汉书.md:9873)、[罢屯奏报](../../source-md/2.汉书.md:9875)。仅核本地文字，底本未确认。

## 决策分析速览

以下是分阶段的条件比较；不是某一日同时摆在皇帝面前的三选一，也不是成本实测。

| 路径 | 证据地位 | 预期收益 | 主要代价／缺口 |
|---|---|---|---|
| 秋季按进兵诏继续出击 | recorded_offer | 可能较快取得战果、减少等待 | 运输、伤亡及其他边防压力；战果不能预知 |
| 罢骑留步兵屯田，待敌敝 | recorded_offer | 按奏估可能降低粮运负担、保留守备 | 期限、袭田与联羌风险须回答；纯方案未被单独观察 |
| 留屯并令其他将领出击 | recorded_action | 同时保留军事压力和屯田安排 | 多策并行使结果难归因，不能称纯屯田胜利 |

## 结构化案例卡

```yaml
schema_version: "0.2"
case_id: case_zhaochongguo_tuntian_review
title: 赵充国屯田提案：连续质询与组合政策
status: reviewed
review:
  reviewed_by: "Astra 模板证据审阅；docs/history_case_batch_a_astra_recheck_20261001.md"
  reviewed_at: 2026-10-01
  notes: "HC-004；2026-10-01 Astra 通过模板证据审阅，保留 U-004；2026-10-06 有限本地登记，本次登记差异待收尾复核。仅指所列本地材料支持相应层级，非独立史实、现代因果或执行效果确证；原核读日期、核心事实与未知不变。"
scope:
  period: 西汉宣帝时
  date_range: 神爵元年秋至次年五月；六月／七月争论为前史，次年秋降附为尾注
  date_precision: approximate
  event_boundary: 秋季罢骑屯田提案、往复质询与兼采出击，至次年五月请罢屯兵获准并还军
  people: [赵充国, 汉宣帝, 辛武贤, 许延寿, 赵卬, 魏相, 浩星赐]
  organizations: [汉廷, 赵充国所部, 破羌将军所部, 强弩将军所部, 先零羌, 罕羌, 开羌]
classification:
  primary_category: organization_people
  secondary_categories: [risk_uncertainty, timing]
  tags: [information_quality, resources, accountability, dependencies, uncertainty, time_window]
  classification_note: 核心是军事政策如何提交估计、回应质询并获修订批准；不以等待本身或最终降附归类。
sources:
  - source_id: src_hanshu69
    work_title: 汉书
    author_or_compiler: 班固等
    source_type: later_compilation
    chapter_or_volume: 卷六十九·赵充国辛庆忌传第三十九（赵充国传）
    edition_or_translator: 用户本地 Markdown 转录；对应 DOCX 及古籍底本未在本轮重核，版次与校勘者未确认
    locator: source-md/2.汉书.md:L9813–9888；核心 L9857–9877，从其秋充国病至还军后的归功争论
    url: null
    accessed_on: "2026-10-01"
    verification: checked
    temporal_relation: 东汉编纂西汉事件，相距约百余年；传中奏疏可能保存较早材料，原件未核。
    dependence_on_other_sources: 核心仅此一传；奏、诏、叙述与浩星赐之言是同一传所存内容，未证明独立，DOCX 与转录不算两源。
    limitations: 无独立军粮账或人口战果册；传记选材、奏报立场、数字口径和对话原貌均有限制。
claims:
  - claim_id: clm_01
    statement: 传文记赵充国请求先至金城再报方略，随后渡河、遣骑侦察并取得俘虏言语；具体情报是否准确未获独立核验。
    claim_type: recorded_event
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9825｜臣愿驰至金城", "source-md/2.汉书.md:L9827｜遣骑候四望狭中"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 有动作和前后情境的单传记载；非独立现场情报档案。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_02
    statement: 较早阶段辛武贤主攻罕、开，赵充国主先击先零并分化其他羌种；六月戊申奏、七月甲寅报从充国计，是攻击对象决定而非秋季屯田批准。
    claim_type: recorded_event
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9833｜合击罕、开", "source-md/2.汉书.md:L9853｜六月戊申奏"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 奏议与批复在同传有清楚次序，独立军令原件未核。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_03
    statement: 秋季帝诏令按时机击先零，病剧可留屯遣他将；赵充国欲罢骑屯田，赵卬遣客以触怒皇帝的风险劝阻，充国仍上奏。
    claim_type: recorded_event
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9857｜作奏未上"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 选择与劝阻有文本依据，转述话语及政治风险的精确程度不明。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_04
    statement: 屯田奏称当时所部吏士马牛月用粮谷199630斛，拟留10281人、月谷27363斛；还估可田二千顷以上、现到谷足万人一年。均为充国奏报及方案估计，不是实施后的成本审计。
    claim_type: attributed_speech
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9859｜月用粮谷十九万九千六百三十斛", "source-md/2.汉书.md:L9861｜合凡万二百八十一人"]
    support: supported
    historicity_confidence: low
    confidence_reason: 数字可核到奏文；两组人员构成及马牛耗费不同，无独立实耗账，不能推出实证节费比例。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_05
    statement: 传中帝先问何时兵决，再追问期月是何时、敌袭屯田与道路、罕开联先零等风险；充国答以预计来春、联屯守备和敌方衰弱，同时承认小寇时杀人民未可骤禁。
    claim_type: attributed_speech
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9863｜虏当何时伏诛", "source-md/2.汉书.md:L9869｜将何以止之", "source-md/2.汉书.md:L9871｜其原未可卒禁"]
    support: supported
    historicity_confidence: low
    confidence_reason: 核到完整问答而非摘句；预测、防御可靠性及原话均未由独立记录证实。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_06
    statement: 传文先概括支持充国者由什三至什五再至什八，再记帝诘前言不便者、皆顿首服；帝接受屯田方向后仍因他将主攻及担心屯田离散而兼令两将与赵卬出击，后罢其他兵，留充国屯田。
    claim_type: recorded_event
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9873｜有诏诘前言不便者", "source-md/2.汉书.md:L9873｜于是两从其计"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 组合政策与部署后续明确；支持比例是传文概括，非表决名册，顿首服是所记公开表态，不证私人判断已改变；帝理由仍为史书归属。
    exact_quote: "于是两从其计"
    quote_checked: true
  - claim_id: clm_07
    statement: 次年五月充国奏报羌军原约五万、斩7600、降31200、溺死饥死五六千、遗脱不逾四千，并请罢屯。人数是奏报约数及不同类别，不能视为互斥精确总账；批准与还军另见clm_08。
    claim_type: attributed_speech
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9875｜羌本可五万人军"]
    support: supported
    historicity_confidence: low
    confidence_reason: 仅确认奏报内容；战果、死因与分类重叠无独立统计，不能硬凑总数。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_08
    statement: 传文记五月请罢屯获准，赵充国还军；这是本卡的核心结束节点。
    claim_type: recorded_event
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9875｜奏可。充国振旅而还"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 批准与还军见单传，屯田全部作业及撤收细节未载。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_09
    statement: 浩星赐在还军后转述有识者认为不出兵亦必自服，并劝归功二将；充国不肯这样答帝。该反事实判断不是已观察的纯屯田结果。
    claim_type: attributed_speech
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9877｜兵虽不出，必自服矣"]
    support: supported
    historicity_confidence: low
    confidence_reason: 史书内嵌的转述与归功争论，不能独立验证未实施方案。
    exact_quote: null
    quote_checked: false
  - claim_id: clm_10
    statement: 次年秋余部约四千余降附在传文中晚于五月还军；只作后续尾注，不并入罢屯时已知结果。
    claim_type: recorded_event
    source_refs: [src_hanshu69]
    source_locators: ["source-md/2.汉书.md:L9879｜其秋"]
    support: supported
    historicity_confidence: medium
    confidence_reason: 时序可核，降附规模同为传文所记，未获独立名册。
    exact_quote: null
    quote_checked: false
source_assessment:
  conflicts: []
  single_source_limit: 全例依卷69同传；奏报、帝问答和他人归功各有立场，未获得独立粮食、工程、人口或战果记录。传内存在归因竞争，不当作多源冲突或多数确证。
  later_embellishments: [不采用纯屯田不战获胜的概括, 不把奏报差额写成实际净节费或最优成本, 不把什三什五什八写成可核投票结果]
situation:
  summary: 前史已有军事分化与进攻，秋季赵充国在继续出击压力下提出罢骑留屯；帝问期限和守备，后来兼用出击与屯田。
  claim_refs: [clm_01, clm_02, clm_03, clm_04, clm_05, clm_06]
  decision_maker: 汉宣帝批准与修订，赵充国提案并执行；其他将领承担出击
  affected_parties: [汉军及供给者, 边地居民, 各羌种及家属, 其他边防部队]
  desired_outcome_at_the_time: 奏文以安边、省费、保留应付其他边患资源为目标；非已证实全部人的共同利益。
  constraints: [粮运与役使负担, 匈奴及其他边患需备, 屯田可能被袭, 皇帝可处罚将领, 羌众生计与人身承受严重损害]
  information_available_then: [充国当时可用侦察及俘虏转述, 奏文内耗费与敌况估计而非独立事实, 皇帝能收到连续奏报和不同将领意见, 次年五月与秋季降数不能提前作为秋奏时已知]
  decision_problem: 在秋季继续出击的要求下，能否以有守备的留屯减轻耗费，如何回答期限与被袭风险并安排其他军队？
options_available:
  - option: 秋季依进兵诏出击先零
    availability_basis: 秋季帝诏；病剧可留屯遣他将，具体带兵者不同
    claim_refs: [clm_03]
    constraints: [马况与粮运, 其他边防资源, 战果与死伤不确定]
  - option: 秋季提出罢骑留步兵屯田待敝
    availability_basis: 充国实际上奏，未单独按纯方案观察结局
    claim_refs: [clm_04, clm_05]
    constraints: [需帝批准, 留屯守备与农作条件, 期限未保证]
  - option: 批准屯田方向后兼令其他将领出击
    availability_basis: 帝后续实际部署，不是秋季最初已定折中
    claim_refs: [clm_06]
    constraints: [同时供给多军, 协同与结果归因困难]
decision_taken:
  action: 充国坚持提案、回应质询；帝接受留屯方向并兼令他军出击，后留充国屯田，次年五月批准罢屯还军。
  claim_refs: [clm_03, clm_05, clm_06, clm_08]
counterfactual_options: []
key_variables:
  - variable_id: var_estimates
    tag: information_quality
    historical_observation: 两组月耗与留屯数由奏文提出，帝继续问前提、期限和风险。
    claim_refs: [clm_04, clm_05]
    modern_equivalent: 方案估计是否可追踪、口径是否一致
    observable_indicator: 估计基线、人员构成、费用范围、误差和实际反馈记录
  - variable_id: var_resources
    tag: resources
    historical_observation: 奏文把军粮、役使和其他边防资源相连。
    claim_refs: [clm_04, clm_05]
    modern_equivalent: 单项投入对整体储备和其他任务的影响
    observable_indicator: 总预算、已承诺支出、可支撑时长及他项任务需求
  - variable_id: var_mix
    tag: dependencies
    historical_observation: 帝兼用他军出击，不能分离屯田与作战贡献。
    claim_refs: [clm_06, clm_07, clm_09]
    modern_equivalent: 同期多措施的协作与归因边界
    observable_indicator: 各措施实施时间、影响链和可区分的结果指标
outcomes:
  - perspective: 汉廷与赵充国
    criterion: 提案是否获修订采纳并到罢屯节点
    horizon: 神爵元年秋至次年五月
    observed_result: 传文记接受留屯方向、兼出击、后留屯，五月奏可还军。
    claim_refs: [clm_06, clm_08]
    assessment: success
    uncertainty: 只评价有限行动链，不证纯屯田必胜、最省费或全部工程按计划完成。
  - perspective: 汉军、供给民众与羌众
    criterion: 净费用、伤亡与生活损害
    horizon: 同期政策及其后
    observed_result: 奏报有斩降和溺死饥死数量，缺可比较的完整成本和居民负担账。
    claim_refs: [clm_04, clm_07]
    assessment: ambiguous
    uncertainty: 军事阶段结束不能等于各方福祉改善；数字不能按精确分类合计。
overall_assessment:
  label: mixed
  rationale: 修订采纳及还军有记载；军事成果来源、净费用和多方损害无法据同传求出。
causal_analysis:
  proposed_mechanisms:
    - mechanism: 明确估计并回应反对意见，可能促使提案被逐步采纳和调整。
      variable_refs: [var_estimates, var_resources]
      supporting_claim_refs: [clm_04, clm_05, clm_06]
      inference_strength: plausible_contribution
      inference_reason: 有连续提案、质询和修订的行动次序；不能证支持转变全由数据造成。
      competing_explanations: [皇权质诘可能影响公开表态但不证私人判断转变，且质诘记在比例概括之后，不能倒推其造成前三轮比例上升, 魏相对充国的信任, 羌众既已分化且困敝, 他将出击, 皇帝平衡各方军事主张, 传记突出老将远见]
      evidence_that_would_weaken_it: [可靠材料显示批准主要先由其他交易决定或奏估未影响选择]
    - mechanism: 留屯可能维持压力并减轻部分运输需求，但不能单独解释全部降附。
      variable_refs: [var_resources, var_mix]
      supporting_claim_refs: [clm_04, clm_06, clm_07, clm_09]
      inference_strength: hypothesis
      inference_reason: 奏文预测与组合后续相接，缺独立实耗和分项贡献观察。
      competing_explanations: [他军直接作战, 羌种互攻及先前分化, 失地饥冻, 降附叙事的选择性]
      evidence_that_would_weaken_it: [独立记录显示降附主要由其他作战决定或屯田实际负担并未下降]
  selection_and_outcome_bias: 名将传记及有利结局不能证方案事前最优；未观察纯屯田，更不能用浩星赐转述补出其结果。
  unresolved_factors: [各措施边际作用, 屯田实施成本, 奏报分类重叠, 供给者及羌众负担]
warning_signs:
  - signal: 帝质询目标期限、袭田和其他羌种联结，方案关键前提仍须解释。
    available_to_actor_then: true
    claim_refs: [clm_05]
  - signal: 赵卬所遣客提醒违逆上意的风险，讨论不在现代自由审议环境中。
    available_to_actor_then: true
    claim_refs: [clm_03]
transferable_mechanisms:
  - mechanism: 将方案数字与假设一同提交质询，记录修订，并分开估计与执行结果。
    conditions_required: [有实际决策权限与反馈渠道, 能核对估计口径, 允许讨论反例与剩余风险]
    modern_evidence_needed: [预算基线与预测误差, 决策记录, 同期措施及结果口径, 受影响者成本]
    what_not_to_infer: 不推出屯田或等待必胜、节费比例已证或每次坚持意见都正确；也不是已验证的现代实验制度。
analogy_limits:
  - historical_condition: 军事占地、夺取生计、悬赏杀戮及迫降
    modern_difference: 现代项目与个人决策须保障权利、合法性和第三方利益。
    effect_on_recommendation: 只迁移估计质询与整体资源检查，排除暴力、断生计和迫降手段。
  - historical_condition: 君主可处罚持异议的将领，传中批准并非程序独立审计
    modern_difference: 现实组织应核实正式权限、专业复核与不报复的异议渠道。
    effect_on_recommendation: 不能把冒死进谏作为常规要求，先查安全沟通和证据条件。
modern_problem_examples: [项目要降低高成本投入时如何核对替代方案的期限与风险？, 多项措施同时改善指标时怎样避免把成果全归给一种方法？]
comparison_ids: []
missing_information: [古籍底本与奏诏原件, 独立军粮和战果记录, 纯屯田的未实施结果, 各军行动贡献, 土地与居民代价, 赵充国和宣帝的完整目标权重]
decision_reconstruction:
  decision_stages:
    - stage: 必要前史：六月／七月攻击对象之争
      evidence: clm_01、clm_02
      interpretation: 现场了解与羌种分化在屯田奏以前，不能将第一次批复当作屯田批准。
    - stage: 秋季进兵诏与留屯提案
      evidence: clm_03、clm_04
      interpretation: 充国以预测耗费和守备方案挑战继续出击方向。
    - stage: 质询、答复与组合修订
      evidence: clm_05、clm_06
      interpretation: 帝接受留屯却仍兼出击，原提案与最终政策不等同。
    - stage: 次年五月罢屯；边界外归功争论与秋降
      evidence: clm_07、clm_08；clm_09、clm_10为尾注
      interpretation: 结束节点是批准和还军，后来的反事实评论不作为成效。
  goal_hypotheses:
    - goal: 安边、省费并留资源应付其他边患
      evidence_level: source_attribution
      basis: clm_04、clm_05中的充国奏文
      limit: 是传世奏文的目标表达，不说明各方共享，也不证实际净收益。
    - goal: 皇帝希望尽快结束军事负担并控制留屯风险
      evidence_level: plausible_inference
      basis: clm_03、clm_05的进兵诏及期限、袭田问答
      limit: 帝完整权衡与意见改变原因不明。
  option_tradeoffs:
    - option_id: opt_attack
      option: 秋季继续出击
      availability: recorded_offer
      claim_refs: [clm_03, clm_05]
      basis: 帝诏允许病剧由他将出击；不等于充国已实施同一方案。
      expected_benefits: [可能较快削弱敌军, 可能缩短驻军时期]
      expected_costs: [运输与伤亡, 分化目标可能受扰, 占用其他边防资源]
      conditions: [兵马后勤可用, 情报与线路可靠, 对手可被有效打击]
      possible_reactions: [对手可能避战或联合，充国奏文有此担忧]
      future_options: 速胜或可早撤，失利或深入则可能压缩后续资源。
      uncertainty: 无法由后续胜局确定该纯方案最优或必败。
    - option_id: opt_tuntian
      option: 罢骑留步兵屯田待敝
      availability: recorded_offer
      claim_refs: [clm_04, clm_05]
      basis: 充国秋奏与答复；其收益是预测。
      expected_benefits: [可能降低粮运需求, 保留守备并积谷, 留资源应付其他边患]
      expected_costs: [留屯仍耗粮役使, 被袭与期限风险, 占地断生计损害羌众]
      conditions: [土地农时和守备可行, 帝批准, 其他边防与补给维持]
      possible_reactions: [帝继续追问, 羌众可能袭田或分化，均未保证]
      future_options: 可能保留以后出击与撤屯空间，前提是局势允许。
      uncertainty: 最终另有出击，不能单独检验纯屯田效果。
    - option_id: opt_mix
      option: 留屯并令他军出击
      availability: recorded_action
      claim_refs: [clm_06]
      basis: 接受屯田方向后实际组合，不是最初同时可知的固定第三案。
      expected_benefits: [可能保留军事压力, 回应屯田离散的风险担忧]
      expected_costs: [多军供给与协同, 出击伤亡, 难辨各策贡献]
      conditions: [各军能分工行动, 物资承受并行支出, 留屯有守备]
      possible_reactions: [他将可按诏出击，羌众反应仍受多重条件影响]
      future_options: 在传文中随后罢他军、独留屯，再罢屯；不是所有过程预先保证。
      uncertainty: 不能因组合后达到结束节点断定每项措施必要。
  motive_hypotheses:
    - hypothesis_id: hyp_overall_resources
      question: 充国为何坚持屯田而不依诏远击？
      explanation: 传世奏文将长期转运与其他边患相连，强调全取胜和不冒无把握之险。
      evidence_level: source_attribution
      claim_refs: [clm_04, clm_05]
      support: 有连续的利益与风险说明，不只是后见赞誉。
      alternatives: [对敌军已困敝的判断, 个体经历与风险偏好]
      what_is_missing: 奏文修辞与真实目标的权重，以及对其他方案的完整评估。
    - hypothesis_id: hyp_mixed_risk
      question: 帝为何接受留屯却仍遣他军出击？
      explanation: 传文把兼采解释为其他将领主攻及帝担忧留屯离散遭袭。
      evidence_level: source_attribution
      claim_refs: [clm_06]
      support: 同段明确列出理由，较无依据的争功解释更受支持。
      alternatives: [平衡不同将领与廷臣, 对期限缺乏信心]
      what_is_missing: 帝同期内廷记录及各理由权重，不能假定完整政治交易。
  implementation:
    recorded_steps: [clm_03秋上奏, clm_04列耗费和器用簿, clm_05往复答诏, clm_06兼用出击后独留屯, clm_08次年请罢获准还军]
    necessary_questions: [粮运与农作如何实际记账？, 联屯守备如何落实？, 各军与受影响居民承担何种成本？]
    unknown_procedures: [田亩与桥路计划实际完成比例, 连屯警报效能, 逐月费用, 撤屯交接细节]
    do_not_invent: 奏文中的器用簿与计划不等于全部执行；不补造独立审计、现代试验或精确节费结果。
  choice_explanation:
    best_supported: 提案在反复质询中获部分采纳并形成组合政策；支持的是修改与批准链，而非纯屯田单因胜利。
    confidence: 行动时序有单源文本依据；奏估、人物原话和各策因果贡献更不确定。
    counterfactual_limit: 三条核心路径足够比较，但分阶段出现；未观察的纯方案不能凭浩星赐之言填出结果。
  life_course:
    short_term: 充国继续承担留屯与答诏责任，帝仍配置他军出击；本人病情和政治压力见传文。
    medium_term: 次年五月罢屯还军是观察节点，秋季余部降附只作尾注。
    long_term: 不以日后褒扬或家族经历评价本次政策的整体人生收益。
    values_limit: 汉廷安边与军费目标不能抹去羌众和居民代价；不替当事人确定全部生活价值。
    modern_bridge: 对现实已明确的目标，核估计、资源和守备条件，再记修订与停止节点；不让成功故事替代实际反馈。
```
